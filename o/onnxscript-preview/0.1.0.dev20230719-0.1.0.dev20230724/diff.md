# Comparing `tmp/onnxscript-preview-0.1.0.dev20230719.tar.gz` & `tmp/onnxscript-preview-0.1.0.dev20230724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-preview-0.1.0.dev20230719.tar", last modified: Wed Jul 19 00:10:08 2023, max compression
+gzip compressed data, was "onnxscript-preview-0.1.0.dev20230724.tar", last modified: Mon Jul 24 00:09:06 2023, max compression
```

## Comparing `onnxscript-preview-0.1.0.dev20230719.tar` & `onnxscript-preview-0.1.0.dev20230724.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.694314 onnxscript-preview-0.1.0.dev20230719/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-19 00:10:08.694314 onnxscript-preview-0.1.0.dev20230719/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.674313 onnxscript-preview-0.1.0.dev20230719/onnxscript/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.674313 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/feature_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/param_manipulation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/analysis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/autocast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.674313 onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    59507 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/converter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.670313 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.674313 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.682313 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/evaluator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.670313 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.670313 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.682313 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.682313 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27667 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/graph_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/graph_building_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.682313 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   223119 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    72897 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/tensor_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/irbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.682313 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.686313 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.690314 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.690314 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/common/onnx_script_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/eager_mode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/eager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/external_tensor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.670313 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.690314 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    69314 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.690314 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/attr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/gemmgelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/gemmgelu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/onnxfns1A_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/onnxfns2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/onnxfns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/ort_custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/loop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.694314 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/attrref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/cast_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/different_opset.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/eager_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/eg1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/graph_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/if_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/loops_break.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/loops_while.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/m1.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/onnxfns1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/onnxfns1A.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/onnxfns2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/opt_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/opt_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/renaming.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/signal_dft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/subfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/type_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/onnx_types_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/operator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/type_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/type_annotation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript/values_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:10:08.694314 onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-19 00:10:08.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-19 00:10:08.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 00:10:08.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 00:10:08.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 00:10:08.000000 onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-19 00:10:01.000000 onnxscript-preview-0.1.0.dev20230719/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 00:10:08.694314 onnxscript-preview-0.1.0.dev20230719/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-19 00:09:58.000000 onnxscript-preview-0.1.0.dev20230719/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.129945 onnxscript-preview-0.1.0.dev20230724/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-24 00:09:06.129945 onnxscript-preview-0.1.0.dev20230724/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.093945 onnxscript-preview-0.1.0.dev20230724/onnxscript/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.093945 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/feature_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/autocast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.097945 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/converter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.097945 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   225758 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75574 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/tensor_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/irbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.113945 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.117945 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.117945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.117945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/onnx_script_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_mode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/external_tensor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.121945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71562 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.121945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/attr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns1A_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/ort_custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/loop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.125945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/attrref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/cast_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/different_opset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eager_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eg1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/graph_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/if_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_while.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/m1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1A.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/renaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/signal_dft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/subfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/type_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/onnx_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/operator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/values_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.125945 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-24 00:08:56.000000 onnxscript-preview-0.1.0.dev20230724/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:09:06.129945 onnxscript-preview-0.1.0.dev20230724/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/setup.py
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/LICENSE` & `onnxscript-preview-0.1.0.dev20230724/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230724/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230719
+Version: 0.1.0.dev20230724
 Summary: Authoring ONNX functions in Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/README.md` & `onnxscript-preview-0.1.0.dev20230724/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/__init__.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/ast_utils.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/param_manipulation.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/param_manipulation_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/runtime_typing.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/_internal/version_utils.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/analysis.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/analysis_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/autocast.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/autocast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 
 from __future__ import annotations
 
-from typing import Any, Callable, Optional
+from typing import TYPE_CHECKING, Any, Callable, Optional, Sequence
 
 import numpy as np
 import onnx
 from onnx import helper, numpy_helper
 from onnx.defs import OpSchema
 
-from onnxscript import tensor, values
+from onnxscript import tensor
+
+if TYPE_CHECKING:
+    from onnxscript import converter
 
 # Conversions from python values to ONNX are used by both the script converter as well
 # as the eager-mode runtime and both need to be consistent. The script converter converts
 # python values into ONNX TensorProto, while the runtime converts python values into
 # ONNXScript runtime's value-representation (based on Tensor).
 
 
@@ -169,28 +172,37 @@
 
     def get_type_info(x):
         return x.dtype if isinstance(x, tensor.Tensor) else None
 
     return cast_inputs(get_type_info, cast_pyvalue_to_os_tensor, op_schema, args)
 
 
-def static_cast_inputs(converter, op_schema: Optional[OpSchema], args) -> tuple[str, ...]:
-    """Used for autocast during script-translation."""
-
-    def get_type_info(x):
-        return x if not x.is_const() else None
+def static_cast_inputs(
+    converter_: converter.Converter,
+    op_schema: Optional[OpSchema],
+    args: Sequence[Optional[converter.Variable]],
+) -> tuple[str, ...]:
+    """Used for autocast during script-translation.
+    This is meant to transform expressions like "Add(X, 1)" to "Add(X, CastLike(1, X))"
+    Polymorphic constants (like 0 and 1) are cast to the type of other operands as needed.
+    """
 
-    def cast(x, typeinfo) -> str:
-        if x.is_const() and typeinfo is not None:
-            # Scalar values are promoted to tensors of a type chosen as below:
-
-            tmp = converter.generate_unique_name(f"{x.name}_cast")
-            converter.emit(
-                [tmp],
-                values.Op(converter.default_opset, "CastLike"),
-                [x.name, typeinfo],
-                [],
-            )
-            return tmp
+    def get_type_info(x: Optional[converter.Variable]) -> Optional[converter.Variable]:
+        """Returns x back if x can serve as the target-type for a cast (as the second
+        argument of CastLike) and None otherwise. In the expression "Add(X, 1), 1 is
+        castable, while X can serve as the target-type.
+        """
+        return None if x is None or x.is_castable else x
+
+    def cast_like(
+        x: Optional[converter.Variable], y: Optional[converter.Variable]
+    ) -> Optional[str]:
+        if x is None:
+            return None
+        if x.is_castable and y is not None:
+            # Polymorphic constant x is cast to the type of y:
+            x_cast = converter_.generate_unique_name(f"{x.name}_cast")
+            converter_.emit([x_cast], "CastLike", [x.name, y.name])
+            return x_cast
         return x.name
 
-    return cast_inputs(get_type_info, cast, op_schema, args)
+    return cast_inputs(get_type_info, cast_like, op_schema, args)
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_backend.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_backend_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_export.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/backend/onnx_export_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/converter.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from __future__ import annotations
 
 import ast
 import logging
-from enum import IntEnum
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     NoReturn,
     Optional,
@@ -83,29 +82,35 @@
     ast.Or: "Or",
     ast.Pow: "Pow",
     ast.Sub: "Sub",
     ast.USub: "Neg",
 }
 
 
-class ConverterExpressionKind(IntEnum):
-    ANY = 0
-    CONST = 1
+class Variable:
+    """Represents an ONNX variable.
 
+    TODO(rama): Consider merging this with IRVar. However, "castable" is specific to this
+    converter.
+    """
 
-class ConverterExpression:
-    def __init__(self, name: Optional[Union[str, List[str]]], kind: ConverterExpressionKind):
-        self.name = name
-        self.kind = kind
+    def __init__(self, name: str, castable: bool = False):
+        """Initialize the instance.
 
-    def is_const(self):
-        return self.kind == ConverterExpressionKind.CONST
+        Args:
+           name: Name of the ONNX variable
+           castable: Whether this variable is castable to a desired target type.
+              Used for ONNX variables representing constants created from python values
+              like 0 or 1 or 0.5 which are treated as polymorphic values castable to other
+              types as needed.
+        """
+        self.name = name
+        self.is_castable = castable
 
     def __str__(self) -> str:
-        assert isinstance(self.name, str), "`name` is not a string. This is likely a bug."
         return self.name
 
 
 if TYPE_CHECKING:
     # The type-alias LocalSymValue represents the types of values that local names in a
     # script-function may be bound to during translation, (ONNX IR values).
     # TODO(rama): Rationalize this and values.SymbolValue
@@ -122,21 +127,20 @@
 
     # The type-alias SymValue denotes values that an identifier may be bound to during
     # translation. A local name will be bound to a LocalSymValue, while a global name
     # will be bound to a PyValue.
 
     SymValue = Union[LocalSymValue, PyValue]
 
-    # PreferredName is a type used to represent the preferred name(s) used in the
-    # generated ONNX for the (one or more) values returned by an expression.
-    # If none specified, the names are generated automatically. Even if names
-    # are specified, the converter will modify them (with a suffix) to ensure
-    # they are unique (to ensure ONNX's SSA requirement).
+    # PreferredName is a type-alias used to represent the preferred name used in the generated
+    # ONNX for a value returned by an expression. There is no guarantee that the specified
+    # name will be used exactly. The converter will modify the name (with a suffix),
+    # if necesssary, to ensure that it is unique (to ensure ONNX's SSA requirement).
 
-    PreferredName = Optional[Union[str, List[str]]]
+    PreferredName = str
 
     # The type-alias OnnxVar indicates variable names used in the generated ONNX.
     OnnxVarName = str
 
 
 class Converter:
     """Main class to translate python code into ONNX operators.
@@ -161,45 +165,45 @@
         logger.setLevel(logging.DEBUG)
         console = logging.StreamHandler()
         logger.addHandler(console)
     """
 
     def __init__(
         self,
-        ir_builder=None,
-        opset=None,
-        global_names=None,
-        source=None,
-        default_opset=None,
+        ir_builder: Optional[irbuilder.IRBuilder] = None,
+        opset: Optional[values.Opset] = None,
+        global_names: Optional[dict[str, Any]] = None,
+        source: Optional[str] = None,
+        default_opset: Optional[values.Opset] = None,
     ):
         self.ir_builder = ir_builder or irbuilder.IRBuilder()
         self.source = source
         if global_names is not None:
             # We make a copy in case function eval modifies it.
             self.globals = global_names.copy()
         self.this_module = opset
         self.default_opset_ = default_opset
 
         # States initialized by `init_function_translation`
-        self._outer = []
-        self._current_fn = None
-        self._nextvar = 0
-        self._used_vars = set()
+        self._outer: List[irbuilder.IRFunction] = []
+        self._current_fn: irbuilder.IRFunction = None
+        self._nextvar: int = 0
+        self._used_vars: set[str] = set()
         self._locals: List[Dict[str, LocalSymValue]] = [{}]
 
     @property
-    def default_opset(self):
+    def default_opset(self) -> values.Opset:
         if self.default_opset_ is None:
             raise RuntimeError(
                 "default_opset must be specified in script for functions "
                 "that do not contain any use of an ONNX opset."
             )
         return self.default_opset_
 
-    def set_default_opset(self, opset, node):
+    def set_default_opset(self, opset: values.Opset, node: ast.AST) -> None:
         if opset.domain != "":
             return
         if self.default_opset_ is not None:
             if (
                 opset.domain != self.default_opset_.domain
                 or opset.version != self.default_opset_.version
             ):
@@ -222,15 +226,15 @@
                             return opset
         for child in ast.iter_child_nodes(node):
             res = self.find_onnx_opset(child)
             if res is not None:
                 return res
         return None
 
-    def init_function_translation(self):
+    def init_function_translation(self) -> None:
         """Initialize self for translating a new (top-level) function."""
         self._outer = []
         self._current_fn: Optional[irbuilder.IRFunction] = None
         self._nextvar = 0
         self._used_vars = set()
         self._locals: List[Dict[str, LocalSymValue]] = [{}]
 
@@ -319,15 +323,15 @@
         return self.ir_builder.make_attr_ref(attrname, val.value, pytype)
 
     def to_onnx_var(
         self,
         val: values.SymbolValue | PyValue,
         target: Optional[PreferredName] = None,
         info: Optional[sourceinfo.SourceInfo] = None,
-    ) -> ConverterExpression:
+    ) -> Variable:
         if isinstance(val, values.AttrRef):
             # promote attribute to value
             result = self.generate_unique_name(target or "tmp")
             attr = self.to_onnx_attr_ref(val, info)
             self.emit([result], values.Op(self.default_opset, "Constant"), [], [attr])
             if ta.base_type_is_bool(val.typeinfo):
                 # ONNX attributes use an int-encoding for bools, but ONNX tensor types
@@ -337,26 +341,24 @@
                 cast_attr = self.ir_builder.make_attr("to", onnx_types.BOOL.dtype)
                 self.emit(
                     [result_as_bool],
                     values.Op(self.default_opset, "Cast"),
                     [result],
                     [cast_attr],
                 )
-                return ConverterExpression(result_as_bool, ConverterExpressionKind.CONST)
-            return ConverterExpression(result, ConverterExpressionKind.CONST)
+                return Variable(result_as_bool, True)
+            return Variable(result, True)
         if isinstance(val, values.Dynamic):
-            return ConverterExpression(val.value, ConverterExpressionKind.ANY)
+            return Variable(val.value)
         # Assume value is a python-value convertible to a tensor
         # TODO: check if value is convertible to a TensorProto, so that we can
         # produce a better error message otherwise
         return self.emit_const(val, target or "tmp", info)
 
-    def py_var_to_onnx_var(
-        self, py_var: str, info: sourceinfo.SourceInfo
-    ) -> ConverterExpression:
+    def py_var_to_onnx_var(self, py_var: str, info: sourceinfo.SourceInfo) -> Variable:
         return self.to_onnx_var(self.lookup(py_var, info), target=py_var, info=info)
 
     def emit_docstring(self, docstring: str) -> None:
         self.ir_builder.add_docstring(self._current_fn, docstring)
 
     def emit(
         self,
@@ -378,16 +380,19 @@
             callee,
             inputs,
             attrs,
             sub_functions,
         )
 
     def emit_const(
-        self, pyvalue: PyValue, suggested_name: PreferredName, info: sourceinfo.SourceInfo
-    ) -> ConverterExpression:
+        self,
+        pyvalue: PyValue,
+        suggested_name: Optional[PreferredName],
+        info: sourceinfo.SourceInfo,
+    ) -> Variable:
         if suggested_name is None:
             if isinstance(pyvalue, int):
                 if pyvalue >= 0:
                     suggested_name = f"int64_{pyvalue}"
                 else:
                     suggested_name = f"int64_m{abs(pyvalue)}"
             elif (
@@ -402,20 +407,20 @@
         ovar = self.generate_unique_name(suggested_name)
         try:
             tensor = autocast.pyvalue_to_onnx_tensor(ovar, pyvalue)
         except ValueError as e:
             fail(info.msg(str(e)))
         attr = self.ir_builder.make_attr("value", tensor)
         self.emit([ovar], values.Op(self.default_opset, "Constant"), [], [attr])
-        return ConverterExpression(ovar, ConverterExpressionKind.CONST)
+        return Variable(ovar, True)
 
     def emit_copy(self, original_var: str, suggested_name: str) -> str:
         """Emits a copy statement, using the ONNX Identity operator."""
         new_var = self.generate_unique_name(suggested_name)
-        self.emit([new_var], values.Op(self.default_opset, "Identity"), [original_var], [])
+        self.emit([new_var], "Identity", [original_var])
         return new_var
 
     def is_constant_expr(self, node: ast.AST) -> None:
         if isinstance(node, ast.UnaryOp):
             if self.is_constant_expr(node.operand):
                 return True
             return False
@@ -512,63 +517,57 @@
             return self.emit_docstring(node.value.value)
         raise TypeError(
             f"Unexpected type {type(node)!r} for node. Unsupoorted version of python."
         )
 
     def translate_expr(
         self, node: ast.AST, target: Optional[PreferredName] = None
-    ) -> ConverterExpression:
+    ) -> Variable:
         """Expression-translation generates "IR statements/nodes" that compute the value of
         the expression into a target-variable, and returns the variable that is
         assigned this value.
         """
         if isinstance(node, ast.Call):
             r = self.translate_call_expr(node)
         elif isinstance(node, (ast.BinOp, ast.BitAnd, ast.BitOr)):
             r = self.translate_bin_op_expr(node)
-        elif isinstance(node, ast.BoolOp):
-            r = self.translate_bool_op_expr(node)
         elif isinstance(node, ast.UnaryOp):
             r = self.translate_unary_op_expr(node)
         elif isinstance(node, ast.Compare):
             r = self.translate_compare_expr(node)
         elif isinstance(node, ast.Name):
             r = self.translate_name_expr(node)
         elif isinstance(node, ast.Subscript):
             r = self.translate_subscript_expr(node, target)
         elif self.is_constant_expr(node):
             r = self.emit_const(self.eval_constant_expr(node), target, self.source_of(node))
         else:
             raise ValueError(
                 self.message(node, f"Unsupported expression type {type(node)!r}.")
             )
-        if isinstance(r, ConverterExpression):
+        if isinstance(r, Variable):
             return r
-        if isinstance(r, tuple):
-            callee, args, attrs = r
-            target = "tmp" if target is None else target
-            if isinstance(target, str):
-                result = self.generate_unique_name(target)
-                self.emit([result], callee, args, attrs)
-                return ConverterExpression(result, ConverterExpressionKind.ANY)
-            results = [self.generate_unique_name(x) for x in target]
-            self.emit(results, callee, args, attrs)
-            return ConverterExpression(results, ConverterExpressionKind.ANY)
-        return ConverterExpression(r, ConverterExpressionKind.ANY)
-
-    def translate_opt_expr(self, node: ast.expr) -> ConverterExpression:
-        """Translation of an expression where "None" is permitted.
-        (eg., for an optional argument)
+        callee, args, attrs = r
+        target = "tmp" if target is None else target
+        assert isinstance(target, str)
+        result = self.generate_unique_name(target)
+        self.emit([result], callee, args, attrs)
+        return Variable(result)
+
+    def translate_opt_expr(self, node: ast.expr) -> Optional[Variable]:
+        """Translation of an expression where "None" is permitted (eg., for an optional argument).
         None is represented as a NameConstant in Python 3.7 and Constant in Python 3.9.
         """
         if isinstance(node, (ast.NameConstant, ast.Constant)) and (node.value is None):
-            return ConverterExpression(None, ConverterExpressionKind.ANY)
+            return None
         return self.translate_expr(node)
 
-    def translate_subscript_expr(self, node: ast.Subscript, target: PreferredName):
+    def translate_subscript_expr(
+        self, node: ast.Subscript, target: Optional[PreferredName]
+    ) -> Variable:
         """List of supported syntaxes is below.
         `A` is a tensor or an expression equivalent to a tensor.
 
         ::
 
             A[:, 1]
             A[:2, 0]
@@ -693,15 +692,15 @@
             elif self.is_constant_expr(elt) and isinstance(self.eval_constant_expr(elt), int):
                 scalar_indices.append((axis, elt))
             else:
                 non_scalar_indices.append((axis, elt))
         if not (sliced_indices or scalar_indices or non_scalar_indices):
             # Edge case: no index specified. Eg. A[:, :]
             self.emit([target], "Identity", [var_name])
-            return target
+            return Variable(target)
         if sliced_indices or len(scalar_indices) > 1:
             # We emit a Slice operation if we have any indices like 1:5:2 or if the number of
             # scalar indices (like 2) is more than 1.
             starts = []
             ends = []
             axes = []
             steps = []
@@ -784,15 +783,15 @@
             if axis != last_axis:  # use temporary to store result of Gather
                 gathered = self.generate_unique_name(f"{var_name}_axis_{axis}")
             else:  # store result of Gather in final target
                 gathered = target
             self.emit([gathered], "Gather", [str(result), index_value], [axis_attr])
             result = gathered
 
-        return result
+        return Variable(result)
 
     def translate_call_expr(self, node: ast.Call):
         """Translates a call-expression."""
         callee = self.translate_callee_expr(node.func)
         param_schemas = callee.param_schemas()
         # If the callee's schema is available, we use it to determine the inputs and attributes.
         # Otherwise, we map named arguments to attributes and positional arguments to inputs.
@@ -814,32 +813,14 @@
         attrs = [attr for attr in attrs if attr is not None]
         return callee, args, attrs
 
     def _cast_like_binary_expression(self, op, left, right):
         schema = op.op_schema
         return autocast.static_cast_inputs(self, schema, (left, right))
 
-    def translate_bool_op_expr(self, node: ast.BoolOp) -> ConverterExpression:
-        if isinstance(node.op, ast.And):
-            op = values.Op(self.default_opset, "And")
-        elif isinstance(node.op, ast.Or):
-            op = values.Op(self.default_opset, "Or")
-        else:
-            raise ValueError(self.message(node, f"Unsupported operator {node.op!r}."))
-
-        expr = self.translate_expr(node.values[0])
-        for operand in node.values[1:]:
-            left, right = self._cast_like_binary_expression(
-                op, expr, self.translate_expr(operand)
-            )
-            ovar = self.generate_unique_name()
-            self.emit([ovar], op, [left, right], [])
-            expr = ConverterExpression(ovar, ConverterExpressionKind.ANY)
-        return expr
-
     def translate_bin_op_expr(self, node: ast.BinOp):
         op = type(node.op)
         if op not in primop_map:
             raise ValueError(self.message(node, f"Unsupported operator {op!r}."))
 
         attr = []
         if isinstance(node.op, ast.Mod) and self.is_constant_expr(node.right):
@@ -895,21 +876,21 @@
 
         # NotEqual is not a standard ONNX op, and needs to be translated into
         # an Equal op/node followed by a Not op/node.
         op = values.Op(self.default_opset, opname if opname != "NotEqual" else "Equal")
         left, right = self._cast_like_binary_expression(op, left, right)
         if opname == "NotEqual":
             tmp = self.generate_unique_name()
-            self.emit([tmp], op, [left, right], [])
+            self.emit([tmp], op, [left, right])
             not_op = values.Op(self.default_opset, "Not")
             return not_op, [tmp], []
 
         return op, [left, right], []
 
-    def translate_name_expr(self, node: ast.Name) -> ConverterExpression:
+    def translate_name_expr(self, node: ast.Name) -> Variable:
         return self.py_var_to_onnx_var(node.id, self.source_of(node))
 
     # pylint: disable=inconsistent-return-statements
     def translate_opset_expr(self, node: ast.Attribute) -> values.Opset:
         """Return an Opset"""
         if isinstance(node, ast.Name):
             val = self.lookup(node.id, self.source_of(node), raise_exception=False)
@@ -973,56 +954,71 @@
                 if hasattr(node.value, "value") and isinstance(node.value.value, str):
                     # python 3.8+
                     return self.translate_docstring(node)
         if isinstance(node, ast.FunctionDef):
             return self.translate_nested_function_def(node)
         if ast_utils.is_print_call(node):
             return None
-        raise ValueError(self.message(node, f"Unsupported statement type {type(node)!r}."))
+        raise ValueError(self.message(node, f"Unsupported statement type '{type(node)!r}'."))
 
     def translate_assign_stmt(self, stmt: Union[ast.Assign, ast.AnnAssign]) -> None:
-        def assign(lhs, rhs):
-            info = self.source_of(lhs)
+        def assign(lhs: ast.AST, rhs: ast.AST) -> None:
             if isinstance(lhs, ast.Name):
+                # Assignments of the form "x = SomeExpression"
+                info = self.source_of(lhs)
                 lhs = lhs.id
                 t = self.translate_expr(rhs, lhs).name
                 if isinstance(stmt, ast.AnnAssign):
-                    var = values.Dynamic(
-                        t,
-                        values.DynamicKind.Intermediate,
-                        info,
-                        typeinfo=self.eval_constant_expr(stmt.annotation),
-                    )
+                    typeinfo = self.eval_constant_expr(stmt.annotation)
                 else:
-                    var = values.Dynamic(t, values.DynamicKind.Intermediate, info)
+                    typeinfo = None
+                var = values.Dynamic(t, values.DynamicKind.Intermediate, info, typeinfo)
                 self.bind(lhs, var)
             elif isinstance(lhs, ast.Tuple):
+                # Assignments of the form "x, y, z = op.SomeOp(...)"
+                if not isinstance(rhs, ast.Call):
+                    self.fail(
+                        rhs,
+                        f"RHS must be a Call expression for unpacking, found: '{type(rhs)!r}'",
+                    )
+                callee, inputs, attrs = self.translate_call_expr(rhs)
+
+                def generate_onnx_name(x: ast.AST):
+                    if not isinstance(x, ast.Name):
+                        self.fail(x, f"LHS must be a Name for unpacking, found: '{type(x)!r}'")
+                    onnx_name = self.generate_unique_name(x.id)
+                    self.bind(
+                        x.id,
+                        values.Dynamic(
+                            onnx_name, values.DynamicKind.Intermediate, self.source_of(x)
+                        ),
+                    )
+                    return onnx_name
 
-                def id(x):
-                    assert isinstance(x, ast.Name)
-                    return x.id
-
-                ids = [id(x) for x in lhs.elts]
-                onnxids = self.translate_expr(rhs, ids).name
-                for x, y in zip(ids, onnxids):
-                    self.bind(x, values.Dynamic(y, values.DynamicKind.Intermediate, info))
+                outputs = [generate_onnx_name(x) for x in lhs.elts]
+                self.emit(outputs, callee, inputs, attrs)
             else:
-                fail("Unsupported construct in LHS of assignment.")
+                self.fail(lhs, f"Unsupported construct in LHS of assignment: '{type(lhs)!r}'")
 
         if isinstance(stmt, ast.Assign):
             targets = stmt.targets
         else:
             targets = [stmt.target]
         if len(targets) != 1:
+            # Assignments of the form "x = y = SomeExpression"
             self.fail(stmt, "Multi-assignment not supported.")
         lhs = targets[0]
         rhs = stmt.value
         if isinstance(rhs, ast.Tuple):
+            # Assignments of the form "... = Expression1, Expression2"
             if not isinstance(lhs, ast.Tuple):
-                self.fail(lhs, f"Left term must be a tuple not {type(lhs)!r}.")
+                # Assignments of the form "single_var = Expression1, Expression2".
+                # We do not support tuple-typed variables.
+                self.fail(lhs, f"Left term must be a tuple not '{type(lhs)!r}'.")
+            # Parallel assignments of the form "x, y = Expression1, Expression2"
             if len(lhs.elts) != len(rhs.elts):
                 self.fail(
                     stmt, "Expected same number of elements on lhs and rhs of assignments."
                 )
             for p, r in zip(lhs.elts, rhs.elts):
                 assign(p, r)
         else:
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/converter_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/converter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
                 value=onnx.helper.make_tensor("zero", onnx.TensorProto.INT64, [1], [0])
             )
             index = zero, zero + 1
             r = A[index]
             return r
 
         ast_name = "_ast" if sys.version_info[:2] < (3, 9) else "ast"
-        self.check_failure(f1, f"Left term must be a tuple not <class '{ast_name}.Name'>")
+        self.check_failure(f1, f"Left term must be a tuple not '<class '{ast_name}.Name'>'")
 
     def check_run(self, onnxfn, inputs, expected_output):
         # Test by converting to model and running with ORT
         model = onnxfn.to_model_proto()
         session = ort.InferenceSession(model.SerializeToString())
         input_names = [x.name for x in model.graph.input]
         input_dict = dict(zip(input_names, inputs))
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/context.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/diagnostics/infra/utils.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/evaluator.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/evaluator_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,22 +62,26 @@
     None,
 ]
 
 # TODO(justinchuby): Build a context manager to handle source information.
 
 
 def _rename_intermediate_value(name: str) -> str:
-    if name.isdigit():
-        return f"_val_{name}"
-    return name
+    """Prepend `_val_` to a numeric tensor name make it valid in ONNX.
 
+    The TorchScript graph creates numeric value names by default. e.g. `0`, `1`.
+    These are not legal ONNX tensor names, since ONNX requires the names to be valid
+    C variable names.
 
-def _rename_intermediate_constant(name: str) -> str:
+    It also improves readability by making the names less likely to be confused
+    with shape values.
+    """
     if name.isdigit():
-        return f"_const_{name}"
+        # Prefix with `_` to avoid name collision
+        return f"_val_{name}"
     return name
 
 
 class TorchScriptTensor(onnxscript_tensor.Tensor):
     """A onnxscript tensor that wraps a torchscript Value."""
 
     def __init__(self, value: torch.Value):
@@ -454,15 +458,15 @@
 
     def _add_constant_to_graph(self, constant) -> torch.Value:
         if constant is None:
             value = _create_op_call_in_torch_graph(
                 self._torch_graph, "prim::Constant", inputs=(), attributes={}
             )[0]
             value.setType(torch.OptionalType.ofTensor())
-            value.setDebugName(_rename_intermediate_constant(value.debugName()))
+            value.setDebugName(_rename_intermediate_value(value.debugName()))
             return value
 
         if isinstance(constant, bool):
             # Be sure to put bool before int, because bool is a subclass of int
             constant_tensor = torch.tensor(constant, dtype=torch.bool)
         elif isinstance(constant, float):
             constant_tensor = torch.tensor(constant, dtype=torch.float)
@@ -482,15 +486,15 @@
             )
         value = _create_op_call_in_torch_graph(
             self._torch_graph,
             "onnx::Constant",
             inputs=(),
             attributes=dict(value=constant_tensor),
         )[0]
-        value.setDebugName(_rename_intermediate_constant(value.debugName()))
+        value.setDebugName(_rename_intermediate_value(value.debugName()))
         return value
 
     @runtime_typing.checked
     def _add_torchscript_op_call(
         self,
         name: str,
         onnx_inputs: Sequence[ValidInputType],
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/graph_building_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -808,27 +808,14 @@
     if rank <= 1:
         self = op.Reshape(self, op.Constant(value_ints=[1, -1, 1]))
     elif rank == 2:
         self = op.Unsqueeze(self, op.Constant(value_ints=[-1]))
     return self
 
 
-def aten_avg_pool1d(
-    self: TensorType,
-    kernel_size: Sequence[int],
-    stride: Optional[Sequence[int]] = None,
-    padding: Sequence[int] = (0,),
-    ceil_mode: bool = False,
-    count_include_pad: bool = True,
-) -> TensorType:
-    """avg_pool1d(Tensor self, int[1] kernel_size, int[1] stride=[], int[1] padding=0, bool ceil_mode=False, bool count_include_pad=True) -> Tensor"""
-
-    raise NotImplementedError()
-
-
 @torch_op("aten::baddbmm")
 def aten_baddbmm(
     self: TRealOrUInt8,
     batch1: TRealUnlessInt16OrInt8,
     batch2: TRealUnlessInt16OrInt8,
     beta: float = 1.0,
     alpha: float = 1.0,
@@ -1016,58 +1003,77 @@
     count: TensorType, prob: TensorType, generator: Optional[str] = None
 ) -> TensorType:
     """binomial(Tensor count, Tensor prob, Generator? generator=None) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::bitwise_and")
+@torch_op(
+    (
+        "aten::bitwise_and",
+        "aten::bitwise_and.Tensor",
+        "aten::bitwise_and.Scalar",
+        "aten::bitwise_and.Scalar_Tensor",
+    )
+)
 def aten_bitwise_and(self: TInt, other: TInt) -> TInt:
     """bitwise_and.Tensor(Tensor self, Tensor other) -> Tensor"""
+    # logical_and implements the BOOL variant
 
     return op.BitwiseAnd(self, other)
 
 
 @torch_op("aten::bitwise_left_shift")
 def aten_bitwise_left_shift(self: TInt, other: TInt) -> TInt:
     """bitwise_left_shift.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     return op.BitShift(self, other, direction="LEFT")
 
 
 @torch_op("aten::bitwise_not")
 def aten_bitwise_not(self: TInt) -> TInt:
     """bitwise_not(Tensor self) -> Tensor"""
+    # logical_not implements the BOOL variant
 
     return op.BitwiseNot(self)
 
 
-@torch_op("aten::bitwise_not")
-def aten_bitwise_not_bool(self: BOOL) -> BOOL:
-    """bitwise_not(Tensor self) -> Tensor"""
-    return op.Not(self)
-
-
-@torch_op("aten::bitwise_or")
+@torch_op(
+    (
+        "aten::bitwise_or",
+        "aten::bitwise_or.Tensor",
+        "aten::bitwise_or.Scalar",
+        "aten::bitwise_or.Scalar_Tensor",
+    )
+)
 def aten_bitwise_or(self: TInt, other: TInt) -> TInt:
     """bitwise_or.Tensor(Tensor self, Tensor other) -> Tensor"""
+    # logical_or implements the BOOL variant
 
     return op.BitwiseOr(self, other)
 
 
 @torch_op("aten::bitwise_right_shift")
 def aten_bitwise_right_shift(self: TInt, other: TInt) -> TInt:
     """bitwise_right_shift.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     return op.BitShift(self, other, direction="RIGHT")
 
 
-@torch_op("aten::bitwise_xor")
+@torch_op(
+    (
+        "aten::bitwise_xor",
+        "aten::bitwise_xor.Tensor",
+        "aten::bitwise_xor.Scalar",
+        "aten::bitwise_xor.Scalar_Tensor",
+    )
+)
 def aten_bitwise_xor(self: TInt, other: TInt) -> TInt:
     """bitwise_xor.Tensor(Tensor self, Tensor other) -> Tensor"""
+    # logical_xor implements the BOOL variant
 
     return op.BitwiseXor(self, other)
 
 
 def aten_blackman_window(window_length: int) -> TensorType:
     """blackman_window(int window_length, *, ScalarType? dtype=None, Layout? layout=None, Device? device=None, bool? pin_memory=None) -> Tensor"""
 
@@ -3743,36 +3749,60 @@
 @torch_op("aten::logdet")
 def aten_logdet(self: TFloat) -> TFloat:
     """logdet(Tensor self) -> Tensor"""
 
     return op.Log(op.Det(self))
 
 
-@torch_op("aten::logical_and")
+@torch_op(
+    (
+        "aten::logical_and",
+        "aten::bitwise_and",
+        "aten::bitwise_and.Tensor",
+        "aten::bitwise_and.Scalar",
+        "aten::bitwise_and.Scalar_Tensor",
+    )
+)
 def aten_logical_and(self: BOOL, other: BOOL) -> BOOL:
     """logical_and(Tensor self, Tensor other) -> Tensor"""
 
     return op.And(self, other)
 
 
-@torch_op("aten::logical_not")
+@torch_op(("aten::logical_not", "aten::bitwise_not"))
 def aten_logical_not(self: BOOL) -> BOOL:
     """logical_not(Tensor self) -> Tensor"""
 
     return op.Not(self)
 
 
-@torch_op("aten::logical_or")
+@torch_op(
+    (
+        "aten::logical_or",
+        "aten::bitwise_or",
+        "aten::bitwise_or.Tensor",
+        "aten::bitwise_or.Scalar",
+        "aten::bitwise_or.Scalar_Tensor",
+    )
+)
 def aten_logical_or(self: BOOL, other: BOOL) -> BOOL:
     """logical_or(Tensor self, Tensor other) -> Tensor"""
 
     return op.Or(self, other)
 
 
-@torch_op("aten::logical_xor")
+@torch_op(
+    (
+        "aten::logical_xor",
+        "aten::bitwise_xor",
+        "aten::bitwise_xor.Tensor",
+        "aten::bitwise_xor.Scalar",
+        "aten::bitwise_xor.Scalar_Tensor",
+    )
+)
 def aten_logical_xor(self: BOOL, other: BOOL) -> BOOL:
     """logical_xor(Tensor self, Tensor other) -> Tensor"""
 
     return op.Xor(self, other)
 
 
 @torch_op("aten::logit", private=True)
@@ -5836,18 +5866,24 @@
     grad_output: TensorType, input_sizes: INT64, dim: int, index: int
 ) -> TensorType:
     """select_backward(Tensor grad_output, SymInt[] input_sizes, int dim, int index) -> Tensor"""
 
     raise NotImplementedError()
 
 
+@torch_op("aten::select_scatter")
 def aten_select_scatter(self: TensorType, src: TensorType, dim: int, index: int) -> TensorType:
     """select_scatter(Tensor self, Tensor src, int dim, int index) -> Tensor"""
 
-    raise NotImplementedError()
+    # Change src rank to self rank according to dim
+    # e.g. if self is [2,3,4], src is [2,4], dim=1, then update is [2,1,4]
+    update = op.Unsqueeze(src, axes=dim)
+    # Change index rank to the same as 'update' [2,1,4]
+    indices = op.Expand(index, op.Shape(update))
+    return op.ScatterElements(self, indices, update, axis=dim, reduction="none")
 
 
 @torch_op("aten::selu")
 def aten_selu(self: TFloat) -> TFloat:
     """selu(Tensor self) -> Tensor"""
 
     return op.Selu(self)
@@ -6721,18 +6757,55 @@
     tail_part_rank = op.Slice(self_size, tail_start_idx, tail_end_idx)
 
     final_shape = op.Concat(head_part_rank, sizes, tail_part_rank, axis=0)
 
     return op.Reshape(self, final_shape)
 
 
-def aten_unfold(self: TensorType, dimension: int, size: int, step: int) -> TensorType:
+@torch_op("aten::unfold", trace_only=True)
+def aten_unfold(self: TTensor, dimension: int, size: int, step: int) -> TTensor:
     """unfold(Tensor(a) self, int dimension, int size, int step) -> Tensor(a)"""
 
-    raise NotImplementedError()
+    self_rank = len(self.shape)
+    if self_rank == 0:
+        result = op.Unsqueeze(self, 0)
+    else:
+        dim_size = self.shape[dimension]
+        target_end = (dim_size - size) // step + 1
+        if target_end > 1:  # the rank of final reuslt will be self_rank + 1
+            self_rank = self_rank + 1
+        # perm need to be list[int], so have to be generated in trace_only mode
+        perm = list(range(self_rank))
+        # from [0,1,2,3,4] -> [0,1,3,4,2] when dimension=1
+        perm.append(perm.pop(dimension + 1))
+        result = _aten_unfold_onnx(self, dimension, size, step, target_end, perm)
+    return result
+
+
+@torch_op("aten::unfold", private=True)
+def _aten_unfold_onnx(
+    self: TTensor, dim: int, size: int, step: int, target_end: int, perm: Sequence[int]
+) -> TTensor:
+    dims = op.Reshape(op.Constant(value_int=dim), op.Constant(value_ints=[-1]))
+    # FIXME: the dtype for this function cannot work, default to float
+    seq_result = op.SequenceEmpty()
+    i = op.Constant(value_ints=[0])
+    cond = i < target_end
+    while cond:  # because for loop cannot work here, so use while loop
+        starts = i * step  # starts is [0, step, step*2, step*3, ...]
+        ends = starts + size  # ends is [0+size, step+size, step*2+size, step*3+size, ...]
+        slice_result = op.Slice(self, starts, ends, dims)
+        # sequence only support float32
+        slice_result_float32 = op.Cast(slice_result, to=FLOAT.dtype)
+        seq_result = op.SequenceInsert(seq_result, slice_result_float32)
+        i = i + 1
+        cond = i < target_end
+    concat_result = op.ConcatFromSequence(seq_result, axis=dim, new_axis=1)
+    result = op.Transpose(concat_result, perm=perm)
+    return op.CastLike(result, self)
 
 
 def aten_unfold_backward(
     grad_in: TensorType, input_sizes: INT64, dim: int, size: int, step: int
 ) -> TensorType:
     """unfold_backward(Tensor grad_in, SymInt[] input_sizes, int dim, int size, int step) -> Tensor"""
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,78 @@
     grad_output: TensorType, self: TensorType, indices: TensorType
 ) -> TensorType:
     """adaptive_max_pool3d_backward(Tensor grad_output, Tensor self, Tensor indices) -> Tensor"""
 
     raise NotImplementedError()
 
 
+def _adjust_attributes_of_avg_pool(
+    expand_size: int,
+    kernel_size: Sequence[int],
+    stride: Sequence[int],
+    padding: Sequence[int],
+) -> Tuple[Sequence[int], Sequence[int], Sequence[int]]:
+    """Adjust attributes of avg_pool to match ONNX specification."""
+
+    if isinstance(kernel_size, int):
+        kernel_shape = [kernel_size] * expand_size
+    else:
+        kernel_shape = kernel_size
+
+    if isinstance(padding, int):
+        pads = [padding] * expand_size * 2
+    elif len(padding) == 1:
+        pads = padding * expand_size * 2
+    elif len(padding) == 2:
+        pads = padding * expand_size
+    else:
+        pads = padding * 2
+
+    if isinstance(stride, int):
+        strides = [stride] * expand_size
+    elif not stride:
+        strides = kernel_shape
+    else:
+        strides = stride
+
+    return (kernel_shape, strides, pads)
+
+
+@torch_op("aten::avg_pool1d", trace_only=True)
+def aten_avg_pool1d(
+    self: TFloat,
+    kernel_size: Sequence[int],
+    stride: Sequence[int] = (),
+    padding: Sequence[int] = (0,),
+    ceil_mode: bool = False,
+    count_include_pad: bool = True,
+) -> TFloat:
+    """avg_pool1d(Tensor self, int[1] kernel_size, int[1] stride=[], int[1] padding=0, bool ceil_mode=False, bool count_include_pad=True) -> Tensor"""
+
+    # Torch prefer to use single number x for kerne,stride,pad,dilation on both side implicitly
+    # But ONNX needs pair number [x,y] to specify on each side explicitly
+    # For pool3d, this number should be 3
+    expand_size = 1
+
+    kernel_shape, strides, pads = _adjust_attributes_of_avg_pool(
+        expand_size, kernel_size, stride, padding
+    )
+
+    result = op.AveragePool(
+        self,
+        ceil_mode=ceil_mode,
+        count_include_pad=count_include_pad,
+        kernel_shape=kernel_shape,
+        pads=pads,
+        strides=strides,
+    )
+
+    return result
+
+
 @torch_op("aten::avg_pool2d", trace_only=True)
 def aten_avg_pool2d(
     self: TFloat,
     kernel_size: Sequence[int],
     stride: Sequence[int] = (),
     padding: Sequence[int] = (0, 0),
     ceil_mode: bool = False,
@@ -140,38 +204,17 @@
     """avg_pool2d(Tensor self, int[2] kernel_size, int[2] stride=[], int[2] padding=0, bool ceil_mode=False, bool count_include_pad=True, int? divisor_override=None) -> Tensor"""
 
     # Torch prefer to use single number x for kerne,stride,pad,dilation on both side implicitly
     # But ONNX needs pair number [x,y] to specify on each side explicitly
     # For pool3d, this number should be 3
     expand_size = 2
 
-    # The kernel_shape should be [x, y]
-    if isinstance(kernel_size, int):  # x -> [x, x]
-        kernel_shape = [kernel_size] * expand_size
-    else:  # assert(len(kernel_size)==2), already [x, y]
-        kernel_shape = kernel_size
-
-    # The pads should be [w, x, y, z]
-    if isinstance(padding, int):  # w -> [w, w, w, w]
-        pads = [padding] * expand_size * 2
-    elif len(padding) == 1:  # [w] -> [w, w, w, w]
-        pads = padding * 4
-    elif len(padding) == 2:  # [w, x] -> [w, x, w, x]
-        pads = padding * 2
-    else:  # assert len(padding) == 4, already [w, x, y, z]
-        pads = padding
-
-    # The strides should be [x, y]
-    if isinstance(stride, int):  # x -> [x, x]
-        strides = [stride] * expand_size
-    elif not stride:
-        # stride is empty
-        strides = kernel_shape
-    else:
-        strides = stride
+    kernel_shape, strides, pads = _adjust_attributes_of_avg_pool(
+        expand_size, kernel_size, stride, padding
+    )
 
     result = op.AveragePool(
         self,
         ceil_mode=ceil_mode,
         count_include_pad=count_include_pad,
         kernel_shape=kernel_shape,
         pads=pads,
@@ -205,26 +248,58 @@
     divisor_override: Optional[int],
 ) -> TensorType:
     """avg_pool2d_backward(Tensor grad_output, Tensor self, int[2] kernel_size, int[2] stride, int[2] padding, bool ceil_mode, bool count_include_pad, int? divisor_override) -> Tensor"""
 
     raise NotImplementedError()
 
 
+@torch_op("aten::avg_pool3d", trace_only=True)
 def aten_avg_pool3d(
-    self: TensorType,
+    self: TFloat,
     kernel_size: Sequence[int],
-    stride: Optional[Sequence[int]] = None,
+    stride: Sequence[int] = (),
     padding: Sequence[int] = (0, 0, 0),
     ceil_mode: bool = False,
     count_include_pad: bool = True,
-    divisor_override: Optional[int] = None,
-) -> TensorType:
+    divisor_override: Optional[int] = None,  # pylint: disable=unused-argument
+) -> TFloat:
     """avg_pool3d(Tensor self, int[3] kernel_size, int[3] stride=[], int[3] padding=0, bool ceil_mode=False, bool count_include_pad=True, int? divisor_override=None) -> Tensor"""
 
-    raise NotImplementedError()
+    # Torch prefer to use single number x for kerne,stride,pad,dilation on both side implicitly
+    # But ONNX needs pair number [x,y] to specify on each side explicitly
+    # For pool3d, this number should be 3
+    expand_size = 3
+
+    kernel_shape, strides, pads = _adjust_attributes_of_avg_pool(
+        expand_size, kernel_size, stride, padding
+    )
+
+    result = op.AveragePool(
+        self,
+        kernel_shape=kernel_shape,
+        strides=strides,
+        pads=pads,
+        count_include_pad=count_include_pad,
+        ceil_mode=ceil_mode,
+    )
+
+    # TODO: if want to support divisor_override argument, need to op.Mul(result, mask)
+    # mask = [
+    #    1, 2, 3, S,..3, 2, 1
+    #    2, 4, 6, 2S, 6, 4, 2
+    #    3, 6, 9, 3S, 9, 6, 3
+    #    S, 2S,3S,SS,3S,2S, S
+    #    3, 6, 9, 3S, 9, 6, 3
+    #    2, 4, 6, 2S, 6, 4, 2
+    #    1, 2, 3, S,..3, 2, 1
+    # ]
+    # S is stride size, in this case S=4,
+    # S may dup lot of times according to the image size
+
+    return result
 
 
 def aten_avg_pool3d_backward(
     grad_output: TensorType,
     self: TensorType,
     kernel_size: Sequence[int],
     stride: Sequence[int],
@@ -595,25 +670,35 @@
     grad_output: TensorType, self: TensorType, negative_slope: float, self_is_result: bool
 ) -> TensorType:
     """leaky_relu_backward(Tensor grad_output, Tensor self, Scalar negative_slope, bool self_is_result) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::linear", trace_only=True)
-def aten_linear(input: TFloat, weight: TFloat, bias: Optional[TFloat] = None) -> TFloat:
+@torch_op("aten::linear")
+def aten_linear(input: TFloat, weight: TFloat) -> TFloat:
     """linear(Tensor input, Tensor weight, Tensor? bias=None) -> Tensor"""
 
     # NOTE: The symbolic function in torch.onnx also uses Gemm in certain cases
     # Optimizers may consider this path and replace it with Gemm
+    # We do not use Gemm here because input can have batch dimensions, which Gemm does not support
     weight_transposed = op.Transpose(weight, perm=[1, 0])
-    result = op.MatMul(input, weight_transposed)
-    if bias is not None:
-        result = op.Add(result, bias)
-    return result
+    return op.MatMul(input, weight_transposed)
+
+
+@torch_op("aten::linear")
+def aten_linear_bias(input: TFloat, weight: TFloat, bias: TFloat) -> TFloat:
+    """linear(Tensor input, Tensor weight, Tensor? bias=None) -> Tensor"""
+
+    # NOTE: The symbolic function in torch.onnx also uses Gemm in certain cases
+    # Optimizers may consider this path and replace it with Gemm
+    # We do not use Gemm here because input can have batch dimensions, which Gemm does not support
+    weight_transposed = op.Transpose(weight, perm=[1, 0])
+    mul = op.MatMul(input, weight_transposed)
+    return op.Add(mul, bias)
 
 
 @torch_op("aten::log_sigmoid")
 def aten_log_sigmoid(self: TFloatOrBFloat16) -> TFloatOrBFloat16:
     """log_sigmoid(Tensor self) -> Tensor"""
 
     return op.Log(op.Sigmoid(self))
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/irbuilder.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/main.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/__init__.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/onnx_types.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/sourceinfo.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tensor.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tensor_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/testing.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/testing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/common/onnx_script_test_case.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/onnx_script_test_case.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/eager_mode_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_mode_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/eager_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/external_tensor_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/external_tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/ops_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/ops_test_common.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/function_libs/torch_lib/ops_test_data.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         kwargs["dim"] = np.array([], dtype=np.int64)
     else:
         # Convert dim to a numpy array
         kwargs["dim"] = np.array(kwargs["dim"], dtype=np.int64).reshape((-1,))
     return args, kwargs
 
 
-def _avg_pool2d_input_wrangler(
+def _avg_pool_input_wrangler(
     args: list[Any], kwargs: dict[str, Any]
 ) -> tuple[list[Any], dict[str, Any]]:
     if "dim" not in kwargs:
         if len(args) > 6:
             kwargs["divisor_override"] = args.pop(6)
         if len(args) > 5:
             kwargs["count_include_pad"] = args.pop(5)
@@ -193,18 +193,19 @@
             kwargs["ceil_mode"] = args.pop(4)
         if len(args) > 3:
             padding = args.pop(3)
             if isinstance(padding, np.ndarray):
                 # Cannot using list(padding) here, because the element will be numpy.int64 instead of int
                 padding = padding.tolist()
             kwargs["padding"] = padding
-        stride = args.pop(2)
-        if isinstance(stride, np.ndarray):
-            stride = stride.tolist()
-        kwargs["stride"] = stride
+        if len(args) > 2:
+            stride = args.pop(2)
+            if isinstance(stride, np.ndarray):
+                stride = stride.tolist()
+            kwargs["stride"] = stride
         kernel_size = args.pop(1)
         if isinstance(kernel_size, np.ndarray):
             kernel_size = kernel_size.tolist()
         kwargs["kernel_size"] = kernel_size
     return args, kwargs
 
 
@@ -425,15 +426,15 @@
         reason="this Aten overload only support one tensor as input by design",
     ),
     TorchLibOpInfo("abs", core_ops.aten_abs),
     TorchLibOpInfo("abs", core_ops.aten_abs_complex, complex=True),
     TorchLibOpInfo("acos", core_ops.aten_acos),
     TorchLibOpInfo("acosh", core_ops.aten_acosh),
     TorchLibOpInfo("add", core_ops.aten_add, tolerance={torch.float16: (1e-3, 1e-3)}),
-    TorchLibOpInfo("addbmm", core_ops.aten_addbmm),
+    TorchLibOpInfo("addbmm", core_ops.aten_addbmm, tolerance={torch.float32: (2e-5, 2e-5)}),
     TorchLibOpInfo("addcdiv", core_ops.aten_addcdiv),
     TorchLibOpInfo("addcmul", core_ops.aten_addcmul, tolerance={torch.float16: (4e-3, 3e-3)}),
     TorchLibOpInfo("addmm", core_ops.aten_addmm),
     TorchLibOpInfo("addmv", core_ops.aten_addmv),
     TorchLibOpInfo(
         "addr",
         core_ops.aten_addr,
@@ -1058,14 +1059,15 @@
         reason="fixme: Rank(0) input will lead ORT failed due to different rank(result) in if-else branch",
     )
     .xfail(
         dtypes=[torch.float16],
         reason="fixme: ORT failed",
     ),
     TorchLibOpInfo("select", core_ops.aten_select),
+    TorchLibOpInfo("select_scatter", core_ops.aten_select_scatter),
     TorchLibOpInfo("sigmoid", core_ops.aten_sigmoid),
     TorchLibOpInfo("sign", core_ops.aten_sign),
     TorchLibOpInfo("sin", core_ops.aten_sin),
     TorchLibOpInfo("sinh", core_ops.aten_sinh),
     TorchLibOpInfo(
         "softmax",
         special_ops.aten_special_softmax,
@@ -1160,14 +1162,15 @@
         reason="fixme: ORT fails with invalid model: 'INVALID_ARGUMENT : Failed to load model with error: vector::_M_range_check: __n (which is 1) >= this->size() (which is 1)'",
         test_class_name="TestOutputConsistencyFullGraph",
     )
     .xfail(
         matcher=lambda sample: any(dim == 0 for dim in sample.input.shape),
         reason="fixme: Logic not implemented for size 0 inputs in op.Reshape",
     ),
+    TorchLibOpInfo("unfold", core_ops.aten_unfold, trace_only=True),
     TorchLibOpInfo("unsqueeze", core_ops.aten_unsqueeze),
     TorchLibOpInfo("view", core_ops.aten_view),
     TorchLibOpInfo("view_as", core_ops.aten_view_as),
     TorchLibOpInfo("view_as_complex", core_ops.aten_view_as_complex),
     TorchLibOpInfo("view_as_complex_copy", core_ops.aten_view_as_complex_copy),
     TorchLibOpInfo("view_as_real", core_ops.aten_view_as_real, complex=True),
     TorchLibOpInfo("view_as_real_copy", core_ops.aten_view_as_real_copy, complex=True),
@@ -1390,23 +1393,60 @@
     TorchLibOpInfo(
         "native_layer_norm",
         core_ops.aten_native_layer_norm,
         trace_only=True,
         tolerance={torch.float32: (3.7e-5, 1.8e-4)},
     ),
     TorchLibOpInfo(
+        "nn.functional.avg_pool1d",
+        nn_ops.aten_avg_pool1d,
+        input_wrangler=_avg_pool_input_wrangler,
+        trace_only=True,
+    )
+    .xfail(
+        matcher=lambda sample: (len(sample.args) > 5 and sample.args[5] is not None)
+        or (sample.kwargs.get("divisor_override") is not None),
+        reason="ONNX doesn't support divisor_override argument",
+    )
+    .xfail(
+        matcher=lambda sample: (sample.kwargs.get("ceil_mode") is True)
+        and (
+            sample.kwargs.get("count_include_pad") is True
+            or sample.input.shape[2]
+            % (sample.args[0][0] if isinstance(sample.args[0], tuple) else sample.args[0])
+            != 0
+        ),
+        reason="fixme: ORT doesn't match PyTorch when ceil_mode=True until opset 19",
+    ),
+    TorchLibOpInfo(
         "nn.functional.avg_pool2d",
         nn_ops.aten_avg_pool2d,
-        input_wrangler=_avg_pool2d_input_wrangler,
+        input_wrangler=_avg_pool_input_wrangler,
         trace_only=True,
     ).xfail(
-        matcher=lambda sample: len(sample.args) > 5 and sample.args[5] is not None,
+        matcher=lambda sample: (len(sample.args) > 5 and sample.args[5] is not None)
+        or (sample.kwargs.get("divisor_override") is not None),
         reason="ONNX doesn't support divisor_override argument",
     ),
     TorchLibOpInfo(
+        "nn.functional.avg_pool3d",
+        nn_ops.aten_avg_pool3d,
+        input_wrangler=_avg_pool_input_wrangler,
+        trace_only=True,
+    )
+    .xfail(
+        matcher=lambda sample: (len(sample.args) > 5 and sample.args[5] is not None)
+        or (sample.kwargs.get("divisor_override") is not None),
+        reason="ONNX doesn't support divisor_override argument",
+    )
+    .xfail(
+        matcher=lambda sample: sample.kwargs.get("ceil_mode") is True,
+        reason="fixme: ORT doesn't match PyTorch when ceil_mode=True until opset 19",
+    ),
+    TorchLibOpInfo(
         "nn.functional.conv1d",
         core_ops.aten_conv1d,
         trace_only=True,
     ).xfail(
         matcher=lambda sample: isinstance(sample.kwargs.get("padding"), str),
         reason="String padding is not accepted by aten::conv1d",
     ),
@@ -1429,15 +1469,24 @@
         "nn.functional.gelu",
         nn_ops.aten_gelu,
         trace_only=True,
     ).xfail(
         dtypes=[torch.float16],
         reason="fixme: ONNX Runtime aborted",
     ),
-    TorchLibOpInfo("nn.functional.linear", nn_ops.aten_linear, trace_only=True),
+    TorchLibOpInfo("nn.functional.linear", nn_ops.aten_linear).skip(
+        # input: input, args: weight, bias; so len(args) == 2 means bias is provided
+        matcher=lambda sample: len(sample.args) != 1,
+        reason="this overload is implemented for bias=None",
+    ),
+    TorchLibOpInfo("nn.functional.linear_bias", nn_ops.aten_linear_bias).skip(
+        # input: input, args: weight, bias; so len(args) == 2 means bias is provided
+        matcher=lambda sample: len(sample.args) != 2,
+        reason="this overload is implemented for bias!=None",
+    ),
     TorchLibOpInfo(
         "nn.functional.max_pool1d",
         nn_ops.aten_max_pool1d,
         input_wrangler=_max_pool_input_wrangler,
         trace_only=True,
     ).skip(
         matcher=lambda sample: sample.kwargs.get("return_indices") is True,
@@ -1679,14 +1728,17 @@
 ops_test_common.duplicate_opinfo(OPS_DB, "min", ("min_dim",))
 ops_test_common.duplicate_opinfo(OPS_DB, "new_empty", ("new_empty_dtype",))
 ops_test_common.duplicate_opinfo(OPS_DB, "new_empty_strided", ("new_empty_strided_dtype",))
 ops_test_common.duplicate_opinfo(OPS_DB, "new_full", ("new_full_dtype",))
 ops_test_common.duplicate_opinfo(OPS_DB, "new_ones", ("new_ones_dtype",))
 ops_test_common.duplicate_opinfo(OPS_DB, "new_zeros", ("new_zeros_dtype",))
 ops_test_common.duplicate_opinfo(
+    OPS_DB, "nn.functional.linear", ("nn.functional.linear_bias",)
+)
+ops_test_common.duplicate_opinfo(
     OPS_DB, "nn.functional.nll_loss", ("nn.functional.nll_loss_weight",)
 )
 ops_test_common.duplicate_opinfo(
     OPS_DB,
     "nn.functional.pad",
     (
         "nn.functional.reflection_pad2d",
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/attr_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/attr_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/gemmgelu.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/gemmgelu_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/if_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/onnxfns1A_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns1A_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/onnxfns2_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns2_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/onnxfns_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/functions/ort_custom_ops.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/ort_custom_ops.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/if_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/loop_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/loop_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/attrref.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/attrref.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/cast_like.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/cast_like.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/different_opset.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/different_opset.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/dropout.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/dropout.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/eager_op.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eager_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/eg1.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eg1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/getitem.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/getitem.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/graph_attr.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/graph_attr.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/identity.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/identity.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/if_statement.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/if_statement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/loops_break.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_break.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/loops_while.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_while.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/onnxfns1.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/onnxfns1A.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1A.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/onnxfns2.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/opt_input.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_input.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/opt_output.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_output.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/renaming.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/renaming.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/sequences.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/sequences.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/signal_dft.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/signal_dft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/subfunction.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/subfunction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/models/type_double.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/type_double.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/tests/onnx_types_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/onnx_types_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/type_annotation.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/type_annotation_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/utils.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/values.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript/values_test.py` & `onnxscript-preview-0.1.0.dev20230724/onnxscript/values_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230719
+Version: 0.1.0.dev20230724
 Summary: Authoring ONNX functions in Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-preview-0.1.0.dev20230719/onnxscript_preview.egg-info/SOURCES.txt` & `onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/pyproject.toml` & `onnxscript-preview-0.1.0.dev20230724/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230719/setup.py` & `onnxscript-preview-0.1.0.dev20230724/setup.py`

 * *Files identical despite different names*

