# Comparing `tmp/fuzzyset-0.0.9.tar.gz` & `tmp/fuzzyset-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuzzyset-0.0.9.tar", last modified: Fri Jun  8 22:13:43 2012, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

