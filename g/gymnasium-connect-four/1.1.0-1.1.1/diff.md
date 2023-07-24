# Comparing `tmp/gymnasium_connect_four-1.1.0.tar.gz` & `tmp/gymnasium_connect_four-1.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.1.0.tar", last modified: Mon Jul 24 10:54:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

