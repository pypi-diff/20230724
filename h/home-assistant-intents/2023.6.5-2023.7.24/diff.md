# Comparing `tmp/home-assistant-intents-2023.6.5.tar.gz` & `tmp/home_assistant_intents-2023.7.24-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.6.5.tar", last modified: Mon Jun  5 15:46:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

