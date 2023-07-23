# Comparing `tmp/pyvalidata-0.1.0.tar.gz` & `tmp/pyvalidata-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvalidata-0.1.0.tar", last modified: Sun Jul 23 07:11:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

