# Comparing `tmp/alia-0.2.7.tar.gz` & `tmp/alia-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.2.7.tar", last modified: Mon Jul 24 16:38:59 2023, max compression
+gzip compressed data, was "alia-0.2.8.tar", last modified: Mon Jul 24 16:43:08 2023, max compression
```

## Comparing `alia-0.2.7.tar` & `alia-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-24 16:38:59.598482 alia-0.2.7/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.7/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-24 16:38:59.597796 alia-0.2.7/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      529 2023-04-20 21:02:49.000000 alia-0.2.7/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-24 16:38:59.592817 alia-0.2.7/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.7/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.7/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.7/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    30041 2023-07-24 16:37:22.000000 alia-0.2.7/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-24 16:38:59.597010 alia-0.2.7/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-24 16:38:59.000000 alia-0.2.7/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-07-24 16:38:59.000000 alia-0.2.7/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-07-24 16:38:59.000000 alia-0.2.7/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-07-24 16:38:59.000000 alia-0.2.7/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-07-24 16:38:59.000000 alia-0.2.7/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-07-24 16:38:59.598635 alia-0.2.7/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-07-24 16:38:17.000000 alia-0.2.7/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-24 16:43:08.887862 alia-0.2.8/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.8/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-24 16:43:08.887287 alia-0.2.8/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      529 2023-04-20 21:02:49.000000 alia-0.2.8/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-24 16:43:08.884832 alia-0.2.8/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.8/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.8/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.8/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    30013 2023-07-24 16:42:21.000000 alia-0.2.8/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-24 16:43:08.886786 alia-0.2.8/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-24 16:43:08.000000 alia-0.2.8/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-07-24 16:43:08.000000 alia-0.2.8/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-07-24 16:43:08.000000 alia-0.2.8/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-07-24 16:43:08.000000 alia-0.2.8/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-07-24 16:43:08.000000 alia-0.2.8/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-07-24 16:43:08.887989 alia-0.2.8/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-07-24 16:42:26.000000 alia-0.2.8/setup.py
```

### Comparing `alia-0.2.7/LICENSE` & `alia-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.2.7/PKG-INFO` & `alia-0.2.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.7
+Version: 0.2.8
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.7/README.md` & `alia-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alia-0.2.7/alia/colors.py` & `alia-0.2.8/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.7/alia/df_tools.py` & `alia-0.2.8/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.7/alia/tools.py` & `alia-0.2.8/alia/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,74 @@
 import pyperclip
 from cryptography.fernet import Fernet
 from dateutil.parser import parse
 
 from .colors import *
 
 
+def clipboard(string):
+    """Copies text to clipboard so it can be pasted anywhere.
+
+    Args:
+        string (str): String to copy
+
+    Returns:
+        Nothing."""
+    pyperclip.copy(string)
+    green("Copied to clipboard", ts=False)
+
+
+def save_obj(obj, filename, mode="wb"):
+    """Saves an object to a file by pickling it.
+
+    Args:
+        obj (any type): Object to save
+        filename (str): Filename to save the object as
+        mode (str): Which file mode to use ('wb' by default, 'ab' to append)
+
+    Returns:
+        Nothing."""
+    if ".pkl" not in filename:
+        filename = f"{filename.strip()}.pkl"
+
+    with open(filename, mode) as f:
+        pickle.dump(obj, f)
+
+    green(f"Object saved as {filename}", ts=False)
+
+
+def load_obj(filename):
+    """Loads a saved pickled object.
+
+    Args:
+        filename (str): Filename of the pickled object
+
+    Returns:
+        An un-pickled object."""
+    with open(filename, "rb") as f:
+        obj = pickle.load(f)
+
+    return obj
+
+
+def read_csv(file_path):
+    """Reads a CSV file.
+
+    Args:
+        file_path (str): Path to the CSV file to read
+
+    Returns:
+        A list of dictionaries where each dictionary represents a row of the CSV."""
+    with open(file_path, "r", newline="") as file:
+        reader = csv.DictReader(file)
+        rows = [{k: v.strip() for k, v in row.items()} for row in reader]
+
+    return rows
+
+
 def b64encode(obj, encoding="utf-8"):
     """Encodes an object using the base64 library.
 
     Args:
         obj (any type): Object to encode
         encoding (str): Encoding to use (utf-8 by default)
 
@@ -25,26 +85,139 @@
         An encoded string representing the given object."""
     if isinstance(obj, str):
         return base64.b64encode(bytes(obj, encoding)).decode(encoding)
     else:
         return base64.b64encode(obj).decode(encoding)
 
 
-def blanknull(string):
-    """Converts any null values to a blank string.
+def encrypt(string):
+    """Uses Fernet 128-bit encryption to encrypt the passed string
 
     Args:
-        string (str): String to check
+        string (str): String to encrypt
 
     Returns:
-        '' if the passed string is null otherwise the string is returned."""
-    if nullstr(string) or not string:
-        return ""
+        encrypted_str (bytes): Encrypted string
+        key (bytes): Associated encryption key (keep private!)"""
+    key = Fernet.generate_key()
+    f = Fernet(key)
+    encrypted_str = f.encrypt(string.encode())
+
+    return encrypted_str, key
+
+
+def decrypt(encrypted_str, key):
+    """Decrypts an encrypted bytes string using Fernet.
+
+    Args:
+        encrypted_str (bytes): Encrypted bytes string to decrypt
+        key (bytes): Associated encryption key
+
+    Returns:
+        A decrypted string."""
+    f = Fernet(key)
+    return f.decrypt(encrypted_str).decode()
+
+
+def tformat(date_obj, style=None):
+    """Formats a date or datetime object as a string with the given style.
+    When style=None default datetime format is %Y-%m-%d %H:%M:%S and default date format is %Y-%m-%d.
+
+    Args:
+        date_obj (date, datetime): Date or datetime object to format
+        style (str): Desired datetime format (i.e. %Y-%m-%d)
+
+    Returns:
+        A string representation of the passed date_obj in the given style."""
+    if type(date_obj) not in [datetime, date]:
+        if ":" in date_obj:
+            date_obj = todt(date_obj)
+        else:
+            date_obj = todt(date_obj, as_date=True)
+    if style is None:
+        if type(date_obj) == datetime:
+            style = "%Y-%m-%d %H:%M:%S"
+        elif type(date_obj) == date:
+            style = "%Y-%m-%d"
+    return date_obj.strftime(style)
+
+
+def todt(dt_str=None, as_date=False):
+    """Takes a datetime string and converts it to an actual datetime object.
+    When as_date=True a date object is returned instead of a datetime object.
+
+    Args:
+        dt_str (str): Date or datetime string
+        as_date (bool): Whether or not to return the value as a date not datetime object
+
+    Returns:
+        A date or datetime objects of the passed string.
+    """
+    if dt_str is None:
+        dt_str = now()
+    elif "_" in dt_str:
+        dt_str = dt_str.replace("_", "-")
+
+    if as_date:
+        return parse(dt_str).date()
     else:
-        return string
+        return parse(dt_str)
+
+
+def now(style="%Y-%m-%d %H:%M:%S", dt=False):
+    """Returns the current date and time.
+
+    Args:
+        style (str): Datetime format to use (default is %Y-%m-%d %H:%M:%S)
+        dt (bool): If True a datetime object is returned instead of a string
+
+    Returns:
+        Either a string or datetime object of the current date and time"""
+    if dt:
+        return datetime.now()
+    else:
+        return datetime.now().strftime(style)
+
+
+def monthdays(month, year=todt(now()).year):
+    """Returns the total number of days in a given month.
+
+    Args:
+        month (int): Integer representation of a given month
+        year (int): Year to reference
+
+    Returns:
+        A integer representing the number of days in a given month.
+    """
+    if type(month) == str:
+        if len(month) == 4:
+            try:
+                out = calendar.monthrange(
+                    year, datetime.strptime(month[:3], "%b").month
+                )
+            except:
+                red(
+                    "If passing a month abbreviation, it must be a <b>3 letter</b> abbreviation",
+                    ts=False,
+                )
+                return None
+        elif len(month) == 3:
+            out = calendar.monthrange(year, datetime.strptime(month, "%b").month)
+        elif len(month) > 4:
+            try:
+                out = calendar.monthrange(year, datetime.strptime(month, "%B").month)
+            except:
+                red(
+                    "Can't parse passed month string; try passing month as an integer",
+                    ts=False,
+                )
+                return None
+    elif type(month) == int:
+        out = calendar.monthrange(year, month)
+    return out[1]
 
 
 def bomonth(month=todt(now()).month, year=todt(now()).year, offset=0, style="%Y-%m-%d"):
     """Returns the 1st of the given month (current month is default).
 
     Args:
         month (int): Month to reference
@@ -81,152 +254,51 @@
             year = todt(dt_int(-60)).year
         else:
             month = month + offset
     rawdate = todt(f"{year}-{month}-01")
     return tformat(rawdate, style=style)
 
 
-def chunkify(input_list, num):
-    """Divides a list into a given number of chunks.
-
-        Args:
-            input_list (list): A list to divide
-            num (int): The number of items each chunk should contain
-
-        Returns:
-            A list of lists where each list contains the passed number of items from the given list."""
-    return [input_list[i: i + num] for i in range(0, len(input_list), num)]
-
-
-def clipboard(string):
-    """Copies text to clipboard so it can be pasted anywhere.
-
-    Args:
-        string (str): String to copy
-
-    Returns:
-        Nothing."""
-    pyperclip.copy(string)
-    green("Copied to clipboard", ts=False)
-
-
-def comma_and(input_list, sep=", ", last_sep="and"):
-    """Joins a list of strings together joined by the given separators.
-    e.g. comma_and(['dog', 'cat', 'rat'], sep=', ', last_sep='&') would return 'dog, cat & rat'
-    
-    Args:
-        input_list (list): A list of strings to join and parse
-        sep (str): The separator to be used to join the strings in the list (', ' by default)
-        last_sep (str): The separator for the last string in the list ('and' by default)
-
-    Returns:
-        A string of the passed list joined by the given separators."""
-    if type(input_list) == str:
-        input_list = [i.strip() for i in input_list.split(",")]
-
-    if len(input_list) >= 3:
-        return sep.join(input_list[:-1]) + f" {last_sep} " + input_list[-1]
-    elif len(input_list) == 2:
-        return f" {last_sep} ".join(input_list)
-    else:
-        return "".join(input_list)
-
-
-def contains(ref, checklist, exact=True, show_all=True):
-    """Iterates through passed items and checks if they exist in a given list.
-    
-    Args:
-        ref (list): List of reference items to check
-        checklist (list): List of things to look for in ref
-        exact (bool): If False checklist is lowercased to find matches regardless of captilization/trailing spaces
-        show_all (bool): If False only the first matching item is returned, otherwise everything is
-
-    Returns:
-        A list of items from checklist that exist in ref."""
-    if not isinstance(checklist, list) and not isinstance(checklist, str):
-        # account for Series and whatnot
-        checklist = list(checklist)
-
-    if not exact:
-        checklist = [str(i).lower().strip() for i in checklist]
-
-    if isinstance(ref, str):
-        if "," in ref and ref.strip() != ",":
-            ref = [i.strip() for i in ref.split(",")]
-        else:
-            ref = [ref]
-    
-    dd = []
-    if exact:
-        for i in ref:
-            if i in checklist:
-                dd.append(i)
-    else:
-        for i in ref:
-            if str(i).lower().strip() in checklist:
-                dd.append(i)
-    
-    if len(dd) == 0:
-        pink("None of the items passed were found in given list",ts=False)
-    else:
-        if show_all or len(dd) == 1:
-            out = dd
-        else:
-            out = [dd[0]]
-        return out
-
-
-def daydiff(start, stop=None):
-    """Calculates the number of days between two dates.
-
-    Args:
-        start (date, datetime, str): Date to subtract from
-        stop (None, date, datetime, str): Date to subtract (default is the current day)
-
-    Returns:
-        A integer representing the number of days in between the given dates"""
-    start = todt(str(start))
-    if stop is None:
-        stop = todt(now())
-    else:
-        stop = todt(str(stop))
-    return (stop - start).days
-
-
-def decrypt(encrypted_str, key):
-    """Decrypts an encrypted bytes string using Fernet.
-
-    Args:
-        encrypted_str (bytes): Encrypted bytes string to decrypt
-        key (bytes): Associated encryption key
-
-    Returns:
-        A decrypted string."""
-    f = Fernet(key)
-    return f.decrypt(encrypted_str).decode()
-
-
-def dget(dict_obj, key, val=None):
-    """More secure version of dict.get(key, val). This accounts for edge cases where a key exists and the
-    value is a blank string and returns None (or whatever you pass as val) instead of the blank string.
+def eomonth(month=todt(now()).month, year=todt(now()).year, offset=0, style="%Y-%m-%d"):
+    """Returns the last date of the given month (current month is default).
 
     Args:
-        dict_obj (dict): Dictionary to reference
-        key (str): Target key to grab from the dictionary
-        val (str, None): Default value to return if the target key isn't in the dictionary
+        month (int): Month to reference
+        year (int): Year to reference
+        offset (int): Number of months to offset by
+        style (str): Desired datetime format
 
     Returns:
-        The value of the key of the passed dictionary (or the value of val if the key doesn't exist)."""
-    if key in dict_obj:
-        if not dict_obj[key] or (
-            isinstance(dict_obj[key], str) and nullstr(dict_obj[key])
-        ):
-            return val
-
-    return dict_obj.get(key, val)
+        A date string of the last date of the given month."""
+    if type(month) == str:
+        if len(month) == 4:
+            try:
+                month = datetime.strptime(month[:3], "%b").month
+            except:
+                red(
+                    "If passing a month abbreviation, it must be a <b>3 letter</b> abbreviation",
+                    ts=False,
+                )
+                return None
+        elif len(month) == 3:
+            month = datetime.strptime(month, "%b").month
+        elif len(month) > 4:
+            try:
+                month = datetime.strptime(month, "%B").month
+            except:
+                red(
+                    "Can't parse passed month string; try passing month as an integer",
+                    ts=False,
+                )
+                return None
+    if offset != 0:
+        month = month + offset
+    last_day = monthdays(month)
+    rawdate = todt(f"{year}-{month}-{last_day}")
+    return tformat(rawdate, style=style)
 
 
 def dt_int(num, start=None, metric="days", style="%Y-%m-%d", dt=True):
     """Adds/subtracts days, minutes or hours from a given date or datetime.
 
     Args:
         num (int): Number to offset by
@@ -286,14 +358,31 @@
             return todt(out)
         else:
             return todt(out, as_date=True)
     else:
         return out
 
 
+def daydiff(start, stop=None):
+    """Calculates the number of days between two dates.
+
+    Args:
+        start (date, datetime, str): Date to subtract from
+        stop (None, date, datetime, str): Date to subtract (default is the current day)
+
+    Returns:
+        A integer representing the number of days in between the given dates"""
+    start = todt(str(start))
+    if stop is None:
+        stop = todt(now())
+    else:
+        stop = todt(str(stop))
+    return (stop - start).days
+
+
 def elapsed(start, stop=None, metric="minutes", full=False):
     """Pass a datetime.datetime object and return elapsed time from then to now. Metric opts:
     seconds, minutes, hours. When full=True elapsed time is returned as H:M:S.
 
     Args:
         start (datetime, str): The datetime value to subtract from
         stop (None, datetime, str): The datetime value to subtract with (current day by default)
@@ -342,118 +431,14 @@
             return seconds
         elif metric == "minutes":
             return minutes
         elif metric == "hours":
             return hours
 
 
-def encrypt(string):
-    """Uses Fernet 128-bit encryption to encrypt the passed string
-
-    Args:
-        string (str): String to encrypt
-
-    Returns:
-        encrypted_str (bytes): Encrypted string
-        key (bytes): Associated encryption key (keep private!)"""
-    key = Fernet.generate_key()
-    f = Fernet(key)
-    encrypted_str = f.encrypt(string.encode())
-
-    return encrypted_str, key
-
-
-def eomonth(month=todt(now()).month, year=todt(now()).year, offset=0, style="%Y-%m-%d"):
-    """Returns the last date of the given month (current month is default).
-
-    Args:
-        month (int): Month to reference
-        year (int): Year to reference
-        offset (int): Number of months to offset by
-        style (str): Desired datetime format
-
-    Returns:
-        A date string of the last date of the given month."""
-    if type(month) == str:
-        if len(month) == 4:
-            try:
-                month = datetime.strptime(month[:3], "%b").month
-            except:
-                red(
-                    "If passing a month abbreviation, it must be a <b>3 letter</b> abbreviation",
-                    ts=False,
-                )
-                return None
-        elif len(month) == 3:
-            month = datetime.strptime(month, "%b").month
-        elif len(month) > 4:
-            try:
-                month = datetime.strptime(month, "%B").month
-            except:
-                red(
-                    "Can't parse passed month string; try passing month as an integer",
-                    ts=False,
-                )
-                return None
-    if offset != 0:
-        month = month + offset
-    last_day = monthdays(month)
-    rawdate = todt(f"{year}-{month}-{last_day}")
-    return tformat(rawdate, style=style)
-
-
-def filelist(dirpath, ext=None, prefix=None, raise_err=False, keep_ext=True):
-    """Lists the filenames in the passed directory.
-
-    Args:
-        dirpath (str): Directory path to reference
-        ext (str): Extension of the files to target
-        prefix (str): Target files that start with this prefix
-        raise_err (bool): If False FileNotFoundErrors will fail silently
-        keep_ext (bool): If Flase base filenames without their extensions are returned
-
-    Returns:
-        A list containing all the filenames in the given directory."""
-    if ext and "." not in ext:
-        ext = f".{ext.strip()}"
-    blacklist = [".DS_Store"]
-
-    try:
-        if keep_ext:
-            if ext and prefix:
-                return [
-                    i for i in os.listdir(dirpath)
-                    if i.startswith(prefix) and i.endswith(ext)
-                ]
-            elif ext:
-                return [i for i in os.listdir(dirpath) if i.endswith(ext)]
-            elif prefix:
-                return [i for i in os.listdir(dirpath) if i.startswith(prefix)]
-            else:
-                return [i for i in os.listdir(dirpath) if i not in blacklist]
-        else:
-            if ext and prefix:
-                return [
-                    i.rsplit(".", 1)[0] for i in os.listdir(dirpath)
-                    if i.startswith(prefix) and i.endswith(ext)
-                ]
-            elif ext:
-                return [i.rsplit(".", 1)[0] for i in os.listdir(dirpath) if i.endswith(ext)]
-            elif prefix:
-                return [i.rsplit(".", 1)[0] for i in os.listdir(dirpath) if i.startswith(prefix)]
-            else:
-                return [i.rsplit(".", 1)[0] for i in os.listdir(dirpath) if i not in blacklist]
-    except FileNotFoundError:
-        if raise_err:
-            raise FileNotFoundError
-        else:
-            red("<b>Can't locate directory</b>")
-            return None
-
-
 def filldates(start, end=None, as_str=False, weekends=True):
     """Calculates the dates in between two dates.
 
     Args:
         start (date, str): Start of the desired date range
         end (None, date, str): End of the desired date range (current day by default)
         as_str (bool): If True dates are returned as strings instead of date objects
@@ -483,89 +468,40 @@
         except:
             red("Problem formatting as strings, returning dates as-is", False)
             return dd
     else:
         return dd
 
 
-def find_common(list1, list2):
-    """Finds common values between two lists.
-    
-    Args:
-        list1 (Series, list): List to check against
-        list2 (Series, list): List to check
-    
-    Returns:
-        A list of items that appear in both list1 and list2."""
-    if isinstance(list1, pd.Series):
-        list1 = list(list1)
-    if isinstance(list1, str):
-        list1 = [t.strip() for t in list1.split(",")]
-    
-    if isinstance(list2, pd.Series):
-        list2 = list(list2)
-    if isinstance(list2, str):
-        list2 = [t.strip() for t in list2.split(",")]
-
-    items = set(list1) & set(list2)
-    # keep original order of list1
-    return sorted(items, key=lambda x: list1.index(x))
-
-
-def find_uncommon(list1, list2):
-    """Compares two lists and finds values that appear in the first list but not the second.
+def nullstr(string):
+    """More robust way of checking if a string is null even in cases where things like '#N/A'
+    are present.
 
     Args:
-        list1 (Series, list): List to check against
-        list2 (Series, list): List to check
+        string (str): String to check
 
     Returns:
-        A list of items that appear in list1 that don't appear in list2."""
-    if isinstance(list1, pd.Series):
-        list1 = list(list1)
-    if isinstance(list1, str):
-        list1 = [t.strip() for t in list1.split(",")]
-
-    if isinstance(list2, pd.Series):
-        list2 = list(list2)
-    if isinstance(list2, str):
-        list2 = [t.strip() for t in list2.split(",")]
-
-    items = set(list1) - set(list2)
-    # keep original order of list1
-    return sorted(items, key=lambda x: list1.index(x))
+        A boolean dictating whether or not the passed string is truly null."""
+    return bool(
+        pd.isnull(string) or string in ["", None, "nan", "NaN", "None", "NONE", "N/A", "#N/A"]
+    )
 
 
-def is_empty(obj):
-    """Checks if a given obj is either null, blank or len(obj) == 0.
+def blanknull(string):
+    """Converts any null values to a blank string.
 
     Args:
-        obj (DataFrame, Series, list, dict, str): Object to check
+        string (str): String to check
 
     Returns:
-        True if the object is empty, False if not."""
-    if obj is None:
-        return True
-    elif type(obj) in (pd.DataFrame, pd.Series):
-        if len(list(obj.columns)) > 1:
-            return bool(
-                len(obj) == 0
-                or (
-                    obj[list(obj.columns)[0]].values[0] == ""
-                    and obj[list(obj.columns)[1]].values[0] == ""
-                )
-            )
-        else:
-            return bool(len(obj) == 0 or obj[list(obj.columns)[0]].values[0] == "")
-    elif isinstance(obj, list):
-        return bool(obj == [])
-    elif isinstance(obj, str):
-        return bool(obj == "")
-    elif isinstance(obj, dict):
-        return bool(len(obj.keys()) == 0)
+        '' if the passed string is null otherwise the string is returned."""
+    if nullstr(string) or not string:
+        return ""
+    else:
+        return string
 
 
 def is_float(string):
     """Checks if a string is meant to be a float.
 
     Args:
         string (str): String to check
@@ -574,281 +510,336 @@
         True if the string is a float, False if not."""
     if str(string).replace(".", "").isnumeric():
         return True
     else:
         return False
 
 
-def is_jupyter():
-    """Checks if the script is currently running in a Jupyter notebook.
+def isodd(num):
+    """Checks if a given number is odd.
+
+    Args:
+        num (int): Number to check
 
     Returns:
-        True or False."""
-    try:
-        from IPython import get_ipython
-        config_file = get_ipython().config.IPKernelApp.connection_file
-        if isinstance(config_file, str):
-            if "jupyter" in config_file.lower() or "ipykernel" in config_file.lower():
-                return True
-            else:
-                return False
-        else:
-            return False
-    except ImportError:
-        return False
+        True if the given number is odd, False if it's even."""
+    if not isinstance(num, int):
+        num = int(num.replace(",", ""))
+    return (num % 2) != 0
+
+
 def iseven(num):
     """Checks if a given number is even.
 
     Args:
         num (int): Number to check
 
     Returns:
         True if the given number is even, False if it's odd."""
     if not isinstance(num, int):
         num = int(num.replace(",", ""))
     return (num % 2) == 0
 
 
-def isodd(num):
-    """Checks if a given number is odd.
+def regex(string, pattern, ignore_case=False):
+    """Performs a regex extraction of a given string.
 
     Args:
-        num (int): Number to check
+        string (str, re.compile): String or compiled re object to reference
+        pattern (str): Regex pattern to search the string with
+        ignore_case (bool): Whether or not to use re.IGNORECASE
 
     Returns:
-        True if the given number is odd, False if it's even."""
-    if not isinstance(num, int):
-        num = int(num.replace(",", ""))
-    return (num % 2) != 0
+        A string of the output of the passed regex."""
+    try:
+        if isinstance(pattern, str):
+            if ignore_case:
+                return re.search(pattern, string, re.IGNORECASE).group(1)
+            else:
+                return re.search(pattern, string).group(1)
+        elif ignore_case:
+            return pattern.search(string, re.IGNORECASE).group(1)
+        else:
+            return pattern.search(string).group(1)
+    except AttributeError:
+        print("Nothing matches the given regex pattern in the given string")
 
 
-def keepkeys(mydict, keys):
-    """Creates a dictionary from the passed dictionary containing only the given keys.
+def str_dedupe(txt):
+    """Removes duplicate substrings from a string.
 
     Args:
-        mydict (dict): Dictionary to filter
-        keys (list): List of keys you want to keep from the passed dictionary
+        txt (str): String to dedupe
 
     Returns:
-        The passed dictionary containing only the desired keys."""
-    if isinstance(keys, str):
-        if "," in keys:
-            keys = [i.strip() for i in keys.split(",")]
-        else:
-            keys = [keys]
+        A string with unique substrings."""
+    words = txt.strip().split()
+    unique_words = []
+    for word in words:
+        if word not in unique_words:
+            unique_words.append(word)
 
-    return {k: v for k, v in mydict.items() if k in keys}
+    return " ".join(unique_words)
 
 
-def load_obj(filename):
-    """Loads a saved pickled object.
+def str_remove(txt, rplc_strs):
+    """Removes passed strings from a string.
 
     Args:
-        filename (str): Filename of the pickled object
+        txt (str): String to clean
+        rplc_strs (list): Strings to remove from the passed txt string
 
     Returns:
-        An un-pickled object."""
-    with open(filename, "rb") as f:
-        obj = pickle.load(f)
-
-    return obj
+        The passed string with the strings passed in rplc_strs removed from it."""
+    if not isinstance(rplc_strs, list):
+        rplc_strs = [r.strip() for r in rplc_strs.split(",")]
+    ntxt = txt
+    for i in rplc_strs:
+        ntxt = ntxt.replace(i, "")
+    return ntxt
 
 
-def monthdays(month, year=todt(now()).year):
-    """Returns the total number of days in a given month.
+def str_replace(txt, **rplc_map):
+    """Replaces things in a string.
 
     Args:
-        month (int): Integer representation of a given month
-        year (int): Year to reference
+        txt (str): String to clean
+        rplc_map (dict): Dict where the keys are what to replace and the values are what to replace it with
 
     Returns:
-        A integer representing the number of days in a given month.
-    """
-    if type(month) == str:
-        if len(month) == 4:
-            try:
-                out = calendar.monthrange(
-                    year, datetime.strptime(month[:3], "%b").month
-                )
-            except:
-                red(
-                    "If passing a month abbreviation, it must be a <b>3 letter</b> abbreviation",
-                    ts=False,
-                )
-                return None
-        elif len(month) == 3:
-            out = calendar.monthrange(year, datetime.strptime(month, "%b").month)
-        elif len(month) > 4:
-            try:
-                out = calendar.monthrange(year, datetime.strptime(month, "%B").month)
-            except:
-                red(
-                    "Can't parse passed month string; try passing month as an integer",
-                    ts=False,
-                )
-                return None
-    elif type(month) == int:
-        out = calendar.monthrange(year, month)
-    return out[1]
+        The passed string with the desired replacements."""
+    out = txt
+    for k, v in rplc_map.items():
+        out = out.replace(k, v)
+    return out
 
 
-def now(style="%Y-%m-%d %H:%M:%S", dt=False):
-    """Returns the current date and time.
+def contains(ref, checklist, exact=True, show_all=True):
+    """Iterates through passed items and checks if they exist in a given list.
 
     Args:
-        style (str): Datetime format to use (default is %Y-%m-%d %H:%M:%S)
-        dt (bool): If True a datetime object is returned instead of a string
+        ref (list): List of reference items to check
+        checklist (list): List of things to look for in ref
+        exact (bool): If False checklist is lowercased to find matches regardless of captilization/trailing spaces
+        show_all (bool): If False only the first matching item is returned, otherwise everything is
 
     Returns:
-        Either a string or datetime object of the current date and time"""
-    if dt:
-        return datetime.now()
+        A list of items from checklist that exist in ref."""
+    if not isinstance(checklist, list) and not isinstance(checklist, str):
+        # account for Series and whatnot
+        checklist = list(checklist)
+
+    if not exact:
+        checklist = [str(i).lower().strip() for i in checklist]
+
+    if isinstance(ref, str):
+        if "," in ref and ref.strip() != ",":
+            ref = [i.strip() for i in ref.split(",")]
+        else:
+            ref = [ref]
+
+    dd = []
+    if exact:
+        for i in ref:
+            if i in checklist:
+                dd.append(i)
     else:
-        return datetime.now().strftime(style)
+        for i in ref:
+            if str(i).lower().strip() in checklist:
+                dd.append(i)
 
+    if len(dd) == 0:
+        pink("None of the items passed were found in given list",ts=False)
+    else:
+        if show_all or len(dd) == 1:
+            out = dd
+        else:
+            out = [dd[0]]
+        return out
 
-def nullstr(string):
-    """More robust way of checking if a string is null even in cases where things like '#N/A'
-    are present.
+
+def is_empty(obj):
+    """Checks if a given obj is either null, blank or len(obj) == 0.
 
     Args:
-        string (str): String to check
+        obj (DataFrame, Series, list, dict, str): Object to check
 
     Returns:
-        A boolean dictating whether or not the passed string is truly null."""
-    return bool(
-        pd.isnull(string) or string in ["", None, "nan", "NaN", "None", "NONE", "N/A", "#N/A"]
-    )
+        True if the object is empty, False if not."""
+    if obj is None:
+        return True
+    elif type(obj) in (pd.DataFrame, pd.Series):
+        if len(list(obj.columns)) > 1:
+            return bool(
+                len(obj) == 0
+                or (
+                    obj[list(obj.columns)[0]].values[0] == ""
+                    and obj[list(obj.columns)[1]].values[0] == ""
+                )
+            )
+        else:
+            return bool(len(obj) == 0 or obj[list(obj.columns)[0]].values[0] == "")
+    elif isinstance(obj, list):
+        return bool(obj == [])
+    elif isinstance(obj, str):
+        return bool(obj == "")
+    elif isinstance(obj, dict):
+        return bool(len(obj.keys()) == 0)
 
 
 def numdict(input_list):
     """Creates a dictionary from a list where the keys are an item's index and the values are the list's items.
 
     Args:
         input_list (list): List of items
 
     Returns:
         A dictionary where the keys are the index of each item in a given list and the values are the lists's items."""
     input_list = list(filter(None, input_list))
     return dict(zip(range(1, len(input_list) + 1), input_list))
 
 
-def ordinal(n):
-    """Converts a number into its ordinal representation (e.g. 1st, 2nd, etc).
+def reverse_dict(mydict, vals_as_list=False):
+    """Reverses a dictionary by swapping its keys with its values. In cases where this causes duplicate keys,
+    rather than overwriting the values all values of duplicate keys are merged into lists.
 
     Args:
-        n (int, str): The string or integer to convert
+        mydict (dict): Dictionary to reverse
+        vals_as_list (bool): If True all values are returned as lists, not just values of duplicate keys
 
     Returns:
-        An ordinal string representation of the given number."""
-    n = int(str(n))
-    suffix = ["th", "st", "nd", "rd", "th"][min(n % 10, 4)]
+        A reversed dictionary."""
+    reversed_dict = {}
+    for key, val in mydict.items():
+        reversed_dict.setdefault(val, [])
+        reversed_dict[val].append(key)
 
-    if 11 <= (n % 100) <= 13:
-        suffix = "th"
+    if not vals_as_list:
+        # all values will be lists, otherwise only
+        # duplicate values are lists
+        for key, val in reversed_dict.items():
+            if len(val) == 1:
+                reversed_dict[key] = val[0]
 
-    return f"{n}{suffix}"
+    return reversed_dict
 
 
-def quotify(input_list, single=True):
-    """Joins a list of strings together commas and places each string inside quotes.
+def keepkeys(mydict, keys):
+    """Creates a dictionary from the passed dictionary containing only the given keys.
 
     Args:
-        input_list (list): A list of strings to join and parse
-        single (bool): If True single quotes are used otherwise double quotes are used
+        mydict (dict): Dictionary to filter
+        keys (list): List of keys you want to keep from the passed dictionary
 
     Returns:
-        A string of the passed list joined together by commas with each string inside quotes."""
-    if single:
-        return ", ".join([f"'{i}'" for i in input_list])
-    else:
-        return ", ".join([f'"{i}"' for i in input_list])
+        The passed dictionary containing only the desired keys."""
+    if isinstance(keys, str):
+        if "," in keys:
+            keys = [i.strip() for i in keys.split(",")]
+        else:
+            keys = [keys]
 
+    return {k: v for k, v in mydict.items() if k in keys}
 
-def read_csv(file_path):
-    """Reads a CSV file.
+
+def find_common(list1, list2):
+    """Finds common values between two lists.
 
     Args:
-        file_path (str): Path to the CSV file to read
+        list1 (Series, list): List to check against
+        list2 (Series, list): List to check
 
     Returns:
-        A list of dictionaries where each dictionary represents a row of the CSV."""
-    with open(file_path, "r", newline="") as file:
-        reader = csv.DictReader(file)
-        rows = [{k: v.strip() for k, v in row.items()} for row in reader]
+        A list of items that appear in both list1 and list2."""
+    if isinstance(list1, pd.Series):
+        list1 = list(list1)
+    if isinstance(list1, str):
+        list1 = [t.strip() for t in list1.split(",")]
 
-    return rows
+    if isinstance(list2, pd.Series):
+        list2 = list(list2)
+    if isinstance(list2, str):
+        list2 = [t.strip() for t in list2.split(",")]
+
+    items = set(list1) & set(list2)
+    # keep original order of list1
+    return sorted(items, key=lambda x: list1.index(x))
 
 
-def regex(string, pattern, ignore_case=False):
-    """Performs a regex extraction of a given string.
+def find_uncommon(list1, list2):
+    """Compares two lists and finds values that appear in the first list but not the second.
 
     Args:
-        string (str, re.compile): String or compiled re object to reference
-        pattern (str): Regex pattern to search the string with
-        ignore_case (bool): Whether or not to use re.IGNORECASE
+        list1 (Series, list): List to check against
+        list2 (Series, list): List to check
 
     Returns:
-        A string of the output of the passed regex."""
-    try:
-        if isinstance(pattern, str):
-            if ignore_case:
-                return re.search(pattern, string, re.IGNORECASE).group(1)
-            else:
-                return re.search(pattern, string).group(1)
-        elif ignore_case:
-            return pattern.search(string, re.IGNORECASE).group(1)
-        else:
-            return pattern.search(string).group(1)
-    except AttributeError:
-        print("Nothing matches the given regex pattern in the given string")
+        A list of items that appear in list1 that don't appear in list2."""
+    if isinstance(list1, pd.Series):
+        list1 = list(list1)
+    if isinstance(list1, str):
+        list1 = [t.strip() for t in list1.split(",")]
 
+    if isinstance(list2, pd.Series):
+        list2 = list(list2)
+    if isinstance(list2, str):
+        list2 = [t.strip() for t in list2.split(",")]
 
-def reverse_dict(mydict, vals_as_list=False):
-    """Reverses a dictionary by swapping its keys with its values. In cases where this causes duplicate keys,
-    rather than overwriting the values all values of duplicate keys are merged into lists.
+    items = set(list1) - set(list2)
+    # keep original order of list1
+    return sorted(items, key=lambda x: list1.index(x))
+
+
+def comma_and(input_list, sep=", ", last_sep="and"):
+    """Joins a list of strings together joined by the given separators.
+    e.g. comma_and(['dog', 'cat', 'rat'], sep=', ', last_sep='&') would return 'dog, cat & rat'
 
     Args:
-        mydict (dict): Dictionary to reverse
-        vals_as_list (bool): If True all values are returned as lists, not just values of duplicate keys
+        input_list (list): A list of strings to join and parse
+        sep (str): The separator to be used to join the strings in the list (', ' by default)
+        last_sep (str): The separator for the last string in the list ('and' by default)
 
     Returns:
-        A reversed dictionary."""
-    reversed_dict = {}
-    for key, val in mydict.items():
-        reversed_dict.setdefault(val, [])
-        reversed_dict[val].append(key)
-
-    if not vals_as_list:
-        # all values will be lists, otherwise only
-        # duplicate values are lists
-        for key, val in reversed_dict.items():
-            if len(val) == 1:
-                reversed_dict[key] = val[0]
+        A string of the passed list joined by the given separators."""
+    if type(input_list) == str:
+        input_list = [i.strip() for i in input_list.split(",")]
 
-    return reversed_dict
+    if len(input_list) >= 3:
+        return sep.join(input_list[:-1]) + f" {last_sep} " + input_list[-1]
+    elif len(input_list) == 2:
+        return f" {last_sep} ".join(input_list)
+    else:
+        return "".join(input_list)
 
 
-def save_obj(obj, filename, mode="wb"):
-    """Saves an object to a file by pickling it.
+def quotify(input_list, single=True):
+    """Joins a list of strings together commas and places each string inside quotes.
 
     Args:
-        obj (any type): Object to save
-        filename (str): Filename to save the object as
-        mode (str): Which file mode to use ('wb' by default, 'ab' to append)
+        input_list (list): A list of strings to join and parse
+        single (bool): If True single quotes are used otherwise double quotes are used
 
     Returns:
-        Nothing."""
-    if ".pkl" not in filename:
-        filename = f"{filename.strip()}.pkl"
+        A string of the passed list joined together by commas with each string inside quotes."""
+    if single:
+        return ", ".join([f"'{i}'" for i in input_list])
+    else:
+        return ", ".join([f'"{i}"' for i in input_list])
 
-    with open(filename, mode) as f:
-        pickle.dump(obj, f)
 
-    green(f"Object saved as {filename}", ts=False)
+def chunkify(input_list, num):
+    """Divides a list into a given number of chunks.
+
+        Args:
+            input_list (list): A list to divide
+            num (int): The number of items each chunk should contain
+
+        Returns:
+            A list of lists where each list contains the passed number of items from the given list."""
+    return [input_list[i: i + num] for i in range(0, len(input_list), num)]
 
 
 def split_data(data, ratio):
     """Splits data into two chunks based on a given ratio.
 
         Args:
             data (list): The data to be split
@@ -857,101 +848,110 @@
         Returns:
             A tuple of 2 lists, the first containing the first 'ratio' proportion of the data,
             the second containing the rest."""
     split_index = int(len(data) * ratio)
     return data[:split_index], data[split_index:]
 
 
-def str_dedupe(txt):
-    """Removes duplicate substrings from a string.
+def ordinal(n):
+    """Converts a number into its ordinal representation (e.g. 1st, 2nd, etc).
 
     Args:
-        txt (str): String to dedupe
+        n (int, str): The string or integer to convert
 
     Returns:
-        A string with unique substrings."""
-    words = txt.strip().split()
-    unique_words = []
-    for word in words:
-        if word not in unique_words:
-            unique_words.append(word)
-
-    return " ".join(unique_words)
-
-
-def str_remove(txt, rplc_strs):
-    """Removes passed strings from a string.
+        An ordinal string representation of the given number."""
+    n = int(str(n))
+    suffix = ["th", "st", "nd", "rd", "th"][min(n % 10, 4)]
 
-    Args:
-        txt (str): String to clean
-        rplc_strs (list): Strings to remove from the passed txt string
+    if 11 <= (n % 100) <= 13:
+        suffix = "th"
 
-    Returns:
-        The passed string with the strings passed in rplc_strs removed from it."""
-    if not isinstance(rplc_strs, list):
-        rplc_strs = [r.strip() for r in rplc_strs.split(",")]
-    ntxt = txt
-    for i in rplc_strs:
-        ntxt = ntxt.replace(i, "")
-    return ntxt
+    return f"{n}{suffix}"
 
 
-def str_replace(txt, **rplc_map):
-    """Replaces things in a string.
+def dget(dict_obj, key, val=None):
+    """More secure version of dict.get(key, val). This accounts for edge cases where a key exists and the
+    value is a blank string and returns None (or whatever you pass as val) instead of the blank string.
 
     Args:
-        txt (str): String to clean
-        rplc_map (dict): Dict where the keys are what to replace and the values are what to replace it with
+        dict_obj (dict): Dictionary to reference
+        key (str): Target key to grab from the dictionary
+        val (str, None): Default value to return if the target key isn't in the dictionary
 
     Returns:
-        The passed string with the desired replacements."""
-    out = txt
-    for k, v in rplc_map.items():
-        out = out.replace(k, v)
-    return out
+        The value of the key of the passed dictionary (or the value of val if the key doesn't exist)."""
+    if key in dict_obj:
+        if not dict_obj[key] or (
+            isinstance(dict_obj[key], str) and nullstr(dict_obj[key])
+        ):
+            return val
 
+    return dict_obj.get(key, val)
 
-def tformat(date_obj, style=None):
-    """Formats a date or datetime object as a string with the given style.
-    When style=None default datetime format is %Y-%m-%d %H:%M:%S and default date format is %Y-%m-%d.
+
+def filelist(dirpath, ext=None, prefix=None, raise_err=False, keep_ext=True):
+    """Lists the filenames in the passed directory.
 
     Args:
-        date_obj (date, datetime): Date or datetime object to format
-        style (str): Desired datetime format (i.e. %Y-%m-%d)
+        dirpath (str): Directory path to reference
+        ext (str): Extension of the files to target
+        prefix (str): Target files that start with this prefix
+        raise_err (bool): If False FileNotFoundErrors will fail silently
+        keep_ext (bool): If Flase base filenames without their extensions are returned
 
     Returns:
-        A string representation of the passed date_obj in the given style."""
-    if type(date_obj) not in [datetime, date]:
-        if ":" in date_obj:
-            date_obj = todt(date_obj)
-        else:
-            date_obj = todt(date_obj, as_date=True)
-    if style is None:
-        if type(date_obj) == datetime:
-            style = "%Y-%m-%d %H:%M:%S"
-        elif type(date_obj) == date:
-            style = "%Y-%m-%d"
-    return date_obj.strftime(style)
+        A list containing all the filenames in the given directory."""
+    if ext and "." not in ext:
+        ext = f".{ext.strip()}"
+    blacklist = [".DS_Store"]
 
+    try:
+        if keep_ext:
+            if ext and prefix:
+                return [
+                    i for i in os.listdir(dirpath)
+                    if i.startswith(prefix) and i.endswith(ext)
+                ]
+            elif ext:
+                return [i for i in os.listdir(dirpath) if i.endswith(ext)]
+            elif prefix:
+                return [i for i in os.listdir(dirpath) if i.startswith(prefix)]
+            else:
+                return [i for i in os.listdir(dirpath) if i not in blacklist]
+        else:
+            if ext and prefix:
+                return [
+                    i.rsplit(".", 1)[0] for i in os.listdir(dirpath)
+                    if i.startswith(prefix) and i.endswith(ext)
+                ]
+            elif ext:
+                return [i.rsplit(".", 1)[0] for i in os.listdir(dirpath) if i.endswith(ext)]
+            elif prefix:
+                return [i.rsplit(".", 1)[0] for i in os.listdir(dirpath) if i.startswith(prefix)]
+            else:
+                return [i.rsplit(".", 1)[0] for i in os.listdir(dirpath) if i not in blacklist]
+    except FileNotFoundError:
+        if raise_err:
+            raise FileNotFoundError
+        else:
+            red("<b>Can't locate directory</b>")
+            return None
 
-def todt(dt_str=None, as_date=False):
-    """Takes a datetime string and converts it to an actual datetime object.
-    When as_date=True a date object is returned instead of a datetime object.
 
-    Args:
-        dt_str (str): Date or datetime string
-        as_date (bool): Whether or not to return the value as a date not datetime object
+def is_jupyter():
+    """Checks if the script is currently running in a Jupyter notebook.
 
     Returns:
-        A date or datetime objects of the passed string.
-    """
-    if dt_str is None:
-        dt_str = now()
-    elif "_" in dt_str:
-        dt_str = dt_str.replace("_", "-")
-
-    if as_date:
-        return parse(dt_str).date()
-    else:
-        return parse(dt_str)
-
-
+        True or False."""
+    try:
+        from IPython import get_ipython
+        config_file = get_ipython().config.IPKernelApp.connection_file
+        if isinstance(config_file, str):
+            if "jupyter" in config_file.lower() or "ipykernel" in config_file.lower():
+                return True
+            else:
+                return False
+        else:
+            return False
+    except ImportError:
+        return False
```

### Comparing `alia-0.2.7/alia.egg-info/PKG-INFO` & `alia-0.2.8/alia.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.7
+Version: 0.2.8
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.7/setup.py` & `alia-0.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.2.7",
+    version="0.2.8",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
```

