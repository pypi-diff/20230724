# Comparing `tmp/dbt_extractor-0.4.1.tar.gz` & `tmp/dbt_extractor-0.5.0-cp38-abi3-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

