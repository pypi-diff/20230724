# Comparing `tmp/fasttextsearch-0.6.tar.gz` & `tmp/fasttextsearch-0.61-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttextsearch-0.6.tar", last modified: Sun Jul 23 09:59:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

