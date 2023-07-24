# Comparing `tmp/rlottie-python-1.1.1.tar.gz` & `tmp/rlottie_python-1.1.2-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlottie-python-1.1.1.tar", last modified: Thu Mar  9 15:41:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

