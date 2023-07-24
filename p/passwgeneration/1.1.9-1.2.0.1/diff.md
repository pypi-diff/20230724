# Comparing `tmp/passwgeneration-1.1.9.tar.gz` & `tmp/passwgeneration-1.2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwgeneration-1.1.9.tar", last modified: Mon Jul 24 09:56:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

