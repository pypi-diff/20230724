# Comparing `tmp/construct-editor-0.1.4.tar.gz` & `tmp/construct-editor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-editor-0.1.4.tar", last modified: Wed Jun 28 10:02:44 2023, max compression
+gzip compressed data, was "construct-editor-0.1.5.tar", last modified: Mon Jul 24 09:22:53 2023, max compression
```

## Comparing `construct-editor-0.1.4.tar` & `construct-editor-0.1.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:44.734607 construct-editor-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-28 10:02:35.000000 construct-editor-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-28 10:02:44.734607 construct-editor-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-28 10:02:35.000000 construct-editor-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:44.718607 construct-editor-0.1.4/construct_editor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:44.722607 construct-editor-0.1.4/construct_editor/core/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/construct_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/context_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    63127 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/core/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:44.730607 construct-editor-0.1.4/construct_editor/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/example_cmd_resp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27072 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/example_ipstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/example_pe32coff.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_aligned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_bits_swapped_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_bytes_greedybytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_compressed.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_computed.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_const.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_dataclass_bit_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_dataclass_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_fixedsized.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_flagsenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_focusedseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_greedyrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_ifthenelse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_ifthenelse_nested_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_nullstripped.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_nullterminated.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_padded.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_padded_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_pointer_peek_seek_tell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_renamed.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_select_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_stringencodded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_switch_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_tenum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_tflagsenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/gallery/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:44.734607 construct-editor-0.1.4/construct_editor/wx_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25380 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/wx_construct_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/wx_construct_hex_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/wx_context_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/wx_exception_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/wx_hex_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/wx_obj_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-06-28 10:02:35.000000 construct-editor-0.1.4/construct_editor/wx_widgets/wx_python_code_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:02:44.718607 construct-editor-0.1.4/construct_editor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-28 10:02:44.000000 construct-editor-0.1.4/construct_editor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-28 10:02:44.000000 construct-editor-0.1.4/construct_editor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:02:44.000000 construct-editor-0.1.4/construct_editor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-28 10:02:44.000000 construct-editor-0.1.4/construct_editor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-28 10:02:44.000000 construct-editor-0.1.4/construct_editor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 10:02:44.000000 construct-editor-0.1.4/construct_editor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 10:02:44.734607 construct-editor-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-28 10:02:35.000000 construct-editor-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:53.502920 construct-editor-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 09:22:40.000000 construct-editor-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-24 09:22:53.502920 construct-editor-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-24 09:22:40.000000 construct-editor-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:53.498920 construct-editor-0.1.5/construct_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:53.498920 construct-editor-0.1.5/construct_editor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/construct_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/context_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63127 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/core/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:53.502920 construct-editor-0.1.5/construct_editor/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/example_cmd_resp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27072 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/example_ipstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/example_pe32coff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_aligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_bits_swapped_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_bytes_greedybytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_compressed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_computed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_dataclass_bit_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_dataclass_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_fixedsized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_flagsenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_focusedseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_greedyrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_ifthenelse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_ifthenelse_nested_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_nullstripped.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_nullterminated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_padded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_padded_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_pointer_peek_seek_tell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_renamed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_select_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_stringencodded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_switch_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_tenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_tflagsenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/gallery/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:53.502920 construct-editor-0.1.5/construct_editor/wx_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25380 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/wx_construct_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/wx_construct_hex_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/wx_context_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/wx_exception_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/wx_hex_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/wx_obj_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-07-24 09:22:40.000000 construct-editor-0.1.5/construct_editor/wx_widgets/wx_python_code_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:22:53.498920 construct-editor-0.1.5/construct_editor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-24 09:22:53.000000 construct-editor-0.1.5/construct_editor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-24 09:22:53.000000 construct-editor-0.1.5/construct_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:22:53.000000 construct-editor-0.1.5/construct_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 09:22:53.000000 construct-editor-0.1.5/construct_editor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 09:22:53.000000 construct-editor-0.1.5/construct_editor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 09:22:53.000000 construct-editor-0.1.5/construct_editor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:22:53.502920 construct-editor-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-24 09:22:40.000000 construct-editor-0.1.5/setup.py
```

### Comparing `construct-editor-0.1.4/LICENSE` & `construct-editor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/PKG-INFO` & `construct-editor-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-editor
-Version: 0.1.4
+Version: 0.1.5
 Summary: GUI (based on wxPython) for 'construct', which is a powerful declarative and symmetrical parser and builder for binary data.
 Home-page: https://github.com/timrid/construct-editor
 Author: Tim Riddermann
 License: MIT
 Keywords: gui,wx,wxpython,widget,binary,editorconstruct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,bitstruct
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `construct-editor-0.1.4/README.md` & `construct-editor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/callbacks.py` & `construct-editor-0.1.5/construct_editor/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/commands.py` & `construct-editor-0.1.5/construct_editor/core/commands.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/construct_editor.py` & `construct-editor-0.1.5/construct_editor/core/construct_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/context_menu.py` & `construct-editor-0.1.5/construct_editor/core/context_menu.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/custom.py` & `construct-editor-0.1.5/construct_editor/core/custom.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/entries.py` & `construct-editor-0.1.5/construct_editor/core/entries.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/model.py` & `construct-editor-0.1.5/construct_editor/core/model.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/core/preprocessor.py` & `construct-editor-0.1.5/construct_editor/core/preprocessor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/example_cmd_resp.py` & `construct-editor-0.1.5/construct_editor/gallery/example_cmd_resp.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/example_ipstack.py` & `construct-editor-0.1.5/construct_editor/gallery/example_ipstack.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/example_pe32coff.py` & `construct-editor-0.1.5/construct_editor/gallery/example_pe32coff.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_array.py` & `construct-editor-0.1.5/construct_editor/gallery/test_array.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_checksum.py` & `construct-editor-0.1.5/construct_editor/gallery/test_checksum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_compressed.py` & `construct-editor-0.1.5/construct_editor/gallery/test_compressed.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_computed.py` & `construct-editor-0.1.5/construct_editor/gallery/test_computed.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_const.py` & `construct-editor-0.1.5/construct_editor/gallery/test_const.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_dataclass_bit_struct.py` & `construct-editor-0.1.5/construct_editor/gallery/test_dataclass_bit_struct.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_dataclass_struct.py` & `construct-editor-0.1.5/construct_editor/gallery/test_dataclass_struct.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_enum.py` & `construct-editor-0.1.5/construct_editor/gallery/test_enum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_fixedsized.py` & `construct-editor-0.1.5/construct_editor/gallery/test_fixedsized.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_flagsenum.py` & `construct-editor-0.1.5/construct_editor/gallery/test_flagsenum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_focusedseq.py` & `construct-editor-0.1.5/construct_editor/gallery/test_focusedseq.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_greedyrange.py` & `construct-editor-0.1.5/construct_editor/gallery/test_greedyrange.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_ifthenelse.py` & `construct-editor-0.1.5/construct_editor/gallery/test_ifthenelse.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_ifthenelse_nested_switch.py` & `construct-editor-0.1.5/construct_editor/gallery/test_ifthenelse_nested_switch.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_pointer_peek_seek_tell.py` & `construct-editor-0.1.5/construct_editor/gallery/test_pointer_peek_seek_tell.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_renamed.py` & `construct-editor-0.1.5/construct_editor/gallery/test_renamed.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_select.py` & `construct-editor-0.1.5/construct_editor/gallery/test_select.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_select_complex.py` & `construct-editor-0.1.5/construct_editor/gallery/test_select_complex.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_stringencodded.py` & `construct-editor-0.1.5/construct_editor/gallery/test_stringencodded.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_switch.py` & `construct-editor-0.1.5/construct_editor/gallery/test_switch.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_switch_dataclass.py` & `construct-editor-0.1.5/construct_editor/gallery/test_switch_dataclass.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_tenum.py` & `construct-editor-0.1.5/construct_editor/gallery/test_tenum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_tflagsenum.py` & `construct-editor-0.1.5/construct_editor/gallery/test_tflagsenum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/gallery/test_timestamp.py` & `construct-editor-0.1.5/construct_editor/gallery/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/main.py` & `construct-editor-0.1.5/construct_editor/main.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/wx_widgets/wx_construct_editor.py` & `construct-editor-0.1.5/construct_editor/wx_widgets/wx_construct_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/wx_widgets/wx_construct_hex_editor.py` & `construct-editor-0.1.5/construct_editor/wx_widgets/wx_construct_hex_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/wx_widgets/wx_context_menu.py` & `construct-editor-0.1.5/construct_editor/wx_widgets/wx_context_menu.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/wx_widgets/wx_exception_dialog.py` & `construct-editor-0.1.5/construct_editor/wx_widgets/wx_exception_dialog.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/wx_widgets/wx_hex_editor.py` & `construct-editor-0.1.5/construct_editor/wx_widgets/wx_hex_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/wx_widgets/wx_obj_view.py` & `construct-editor-0.1.5/construct_editor/wx_widgets/wx_obj_view.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor/wx_widgets/wx_python_code_editor.py` & `construct-editor-0.1.5/construct_editor/wx_widgets/wx_python_code_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/construct_editor.egg-info/PKG-INFO` & `construct-editor-0.1.5/construct_editor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-editor
-Version: 0.1.4
+Version: 0.1.5
 Summary: GUI (based on wxPython) for 'construct', which is a powerful declarative and symmetrical parser and builder for binary data.
 Home-page: https://github.com/timrid/construct-editor
 Author: Tim Riddermann
 License: MIT
 Keywords: gui,wx,wxpython,widget,binary,editorconstruct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,bitstruct
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `construct-editor-0.1.4/construct_editor.egg-info/SOURCES.txt` & `construct-editor-0.1.5/construct_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.4/setup.py` & `construct-editor-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     long_description_content_type="text/markdown",
     platforms=["Windows"],
     url="https://github.com/timrid/construct-editor",
     author="Tim Riddermann",
     python_requires=">=3.8",
     install_requires=[
         "construct==2.10.68",
-        "construct-typing==0.5.6",
+        "construct-typing==0.6.*",
         "wxPython>=4.1.1",
         "arrow>=1.0.0",
         "wrapt>=1.14.0",
         "typing-extensions>=4.4.0"
     ],
     keywords=[
         "gui",
```

