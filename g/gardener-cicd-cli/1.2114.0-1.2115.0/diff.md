# Comparing `tmp/gardener-cicd-cli-1.2114.0.tar.gz` & `tmp/gardener_cicd_cli-1.2115.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2114.0.tar", last modified: Fri Jul 21 12:31:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

