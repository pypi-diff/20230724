# Comparing `tmp/bec_scihub-0.14.0.tar.gz` & `tmp/bec_scihub-0.14.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-0.14.0.tar", last modified: Fri Jul 21 20:43:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

