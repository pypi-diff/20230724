# Comparing `tmp/peviitor_pyscraper-0.0.3.tar.gz` & `tmp/peviitor_pyscraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peviitor_pyscraper-0.0.3.tar", last modified: Sun Jul 23 20:04:17 2023, max compression
+gzip compressed data, was "peviitor_pyscraper-0.0.4.tar", last modified: Sun Jul 23 23:27:26 2023, max compression
```

## Comparing `peviitor_pyscraper-0.0.3.tar` & `peviitor_pyscraper-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 20:04:17.311333 peviitor_pyscraper-0.0.3/
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)     1080 2023-07-23 09:51:34.000000 peviitor_pyscraper-0.0.3/LICENSE
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      259 2023-07-23 20:04:17.311109 peviitor_pyscraper-0.0.3/PKG-INFO
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)       64 2023-07-23 09:51:34.000000 peviitor_pyscraper-0.0.3/README.md
-drwxr-xr-x   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 20:04:17.309789 peviitor_pyscraper-0.0.3/peviitor_pyscraper.egg-info/
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      259 2023-07-23 20:04:17.000000 peviitor_pyscraper-0.0.3/peviitor_pyscraper.egg-info/PKG-INFO
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      274 2023-07-23 20:04:17.000000 peviitor_pyscraper-0.0.3/peviitor_pyscraper.egg-info/SOURCES.txt
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)        1 2023-07-23 20:04:17.000000 peviitor_pyscraper-0.0.3/peviitor_pyscraper.egg-info/dependency_links.txt
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      138 2023-07-23 20:04:17.000000 peviitor_pyscraper-0.0.3/peviitor_pyscraper.egg-info/requires.txt
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)        8 2023-07-23 20:04:17.000000 peviitor_pyscraper-0.0.3/peviitor_pyscraper.egg-info/top_level.txt
-drwxr-xr-x   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 20:04:17.310717 peviitor_pyscraper-0.0.3/scraper/
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)     3849 2023-07-23 19:35:21.000000 peviitor_pyscraper-0.0.3/scraper/Scraper.py
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 19:42:41.000000 peviitor_pyscraper-0.0.3/scraper/__init__.py
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)       38 2023-07-23 20:04:17.311788 peviitor_pyscraper-0.0.3/setup.cfg
--rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      586 2023-07-23 20:03:57.000000 peviitor_pyscraper-0.0.3/setup.py
+drwxr-xr-x   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 23:27:26.113531 peviitor_pyscraper-0.0.4/
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)     1080 2023-07-23 09:51:34.000000 peviitor_pyscraper-0.0.4/LICENSE
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)     4962 2023-07-23 23:27:26.113343 peviitor_pyscraper-0.0.4/PKG-INFO
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)     4626 2023-07-23 23:17:03.000000 peviitor_pyscraper-0.0.4/README.md
+drwxr-xr-x   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 23:27:26.112415 peviitor_pyscraper-0.0.4/peviitor_pyscraper.egg-info/
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)     4962 2023-07-23 23:27:26.000000 peviitor_pyscraper-0.0.4/peviitor_pyscraper.egg-info/PKG-INFO
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      274 2023-07-23 23:27:26.000000 peviitor_pyscraper-0.0.4/peviitor_pyscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)        1 2023-07-23 23:27:26.000000 peviitor_pyscraper-0.0.4/peviitor_pyscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      138 2023-07-23 23:27:26.000000 peviitor_pyscraper-0.0.4/peviitor_pyscraper.egg-info/requires.txt
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)        8 2023-07-23 23:27:26.000000 peviitor_pyscraper-0.0.4/peviitor_pyscraper.egg-info/top_level.txt
+drwxr-xr-x   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 23:27:26.113115 peviitor_pyscraper-0.0.4/scraper/
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)     3692 2023-07-23 20:10:29.000000 peviitor_pyscraper-0.0.4/scraper/Scraper.py
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)        0 2023-07-23 19:42:41.000000 peviitor_pyscraper-0.0.4/scraper/__init__.py
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)       38 2023-07-23 23:27:26.113593 peviitor_pyscraper-0.0.4/setup.cfg
+-rw-r--r--   0 laurentiumarianbaluta   (501) staff       (20)      791 2023-07-23 23:26:56.000000 peviitor_pyscraper-0.0.4/setup.py
```

### Comparing `peviitor_pyscraper-0.0.3/LICENSE` & `peviitor_pyscraper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `peviitor_pyscraper-0.0.3/scraper/Scraper.py` & `peviitor_pyscraper-0.0.4/scraper/Scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,11 +119,7 @@
         process = subprocess.run(["node", "-e", js], input=file.read(), capture_output=True)
         if process.returncode != 0:
             raise Exception("Failed to render page, make sure you have node and peviitor_jsscraper installed")
         
         self.markup = process.stdout.decode("utf-8")
         self.__init__(self.markup, 'html.parser')
         return self.markup
-
-test = Scraper()
-test.render_page("https://careers.celestica.com/search/?createNewAlert=false&q=&locationsearch=Romania&startrow=10")
-print(test.prettify())
```

