# Comparing `tmp/nvidia-dali-tf-plugin-cuda110-1.27.0.tar.gz` & `tmp/nvidia-dali-tf-plugin-cuda110-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-cuda110-1.27.0.tar", last modified: Tue Jun 13 09:35:47 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-cuda110-1.28.0.tar", last modified: Mon Jul 10 16:31:49 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0.tar` & `nvidia-dali-tf-plugin-cuda110-1.28.0.tar`

### file list

```diff
@@ -1,131 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    43001 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_dataset_op.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.486541 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/
--rw-r--r--   0 root         (0) root         (0)     5169 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_dataset.h
--rw-r--r--   0 root         (0) root         (0)     7079 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_helper.h
--rw-r--r--   0 root         (0) root         (0)    17344 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_install_tool.py
--rw-r--r--   0 root         (0) root         (0)     6207 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_utils.py
--rw-r--r--   0 root         (0) root         (0)    17543 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/daliop.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.482541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.486541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/
--rw-r--r--   0 root         (0) root         (0)    27259 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/c_api.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.490541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/
--rw-r--r--   0 root         (0) root         (0)     5686 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/access_order.h
--rw-r--r--   0 root         (0) root         (0)    10320 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/any.h
--rw-r--r--   0 root         (0) root         (0)     1461 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/api_helper.h
--rw-r--r--   0 root         (0) root         (0)     2207 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/backend_tags.h
--rw-r--r--   0 root         (0) root         (0)     7777 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/bitmask.h
--rw-r--r--   0 root         (0) root         (0)     7937 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/boundary.h
--rw-r--r--   0 root         (0) root         (0)     3297 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/byte_io.h
--rw-r--r--   0 root         (0) root         (0)     1281 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/call_at_exit.h
--rw-r--r--   0 root         (0) root         (0)     5354 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/common.h
--rw-r--r--   0 root         (0) root         (0)    17542 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/convert.h
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/copy_vector_helper.h
--rw-r--r--   0 root         (0) root         (0)     5249 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_error.h
--rw-r--r--   0 root         (0) root         (0)     1895 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event.h
--rw-r--r--   0 root         (0) root         (0)     3154 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event_pool.h
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_rt_utils.h
--rw-r--r--   0 root         (0) root         (0)     2059 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream.h
--rw-r--r--   0 root         (0) root         (0)     7050 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream_pool.h
--rw-r--r--   0 root         (0) root         (0)     2179 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_utils.h
--rw-r--r--   0 root         (0) root         (0)     5012 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_array.h
--rw-r--r--   0 root         (0) root         (0)     5315 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_buffer.h
--rw-r--r--   0 root         (0) root         (0)     6438 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_string.h
--rw-r--r--   0 root         (0) root         (0)     1381 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/device_guard.h
--rw-r--r--   0 root         (0) root         (0)      815 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cuda.h
--rw-r--r--   0 root         (0) root         (0)     5034 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cufile.h
--rw-r--r--   0 root         (0) root         (0)     6146 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/endian_util.h
--rw-r--r--   0 root         (0) root         (0)    10891 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/error_handling.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.490541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/exec/
--rw-r--r--   0 root         (0) root         (0)     2115 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/exec/engine.h
--rw-r--r--   0 root         (0) root         (0)     4648 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/expand_dims.h
--rw-r--r--   0 root         (0) root         (0)     6831 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/fast_div.h
--rw-r--r--   0 root         (0) root         (0)    14461 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/float16.h
--rw-r--r--   0 root         (0) root         (0)      977 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/force_inline.h
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/format.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/box.h
--rw-r--r--   0 root         (0) root         (0)     1706 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/geom_utils.h
--rw-r--r--   0 root         (0) root         (0)    17992 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/mat.h
--rw-r--r--   0 root         (0) root         (0)     4521 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/transform.h
--rw-r--r--   0 root         (0) root         (0)    21114 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/vec.h
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/host_dev.h
--rw-r--r--   0 root         (0) root         (0)     2267 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/int_literals.h
--rw-r--r--   0 root         (0) root         (0)     5889 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/math_util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/
--rw-r--r--   0 root         (0) root         (0)    22129 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/async_pool.h
--rw-r--r--   0 root         (0) root         (0)     7562 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/binning_resource.h
--rw-r--r--   0 root         (0) root         (0)     5291 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/composite_resource.h
--rw-r--r--   0 root         (0) root         (0)     9018 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cu_vm.h
--rw-r--r--   0 root         (0) root         (0)    34893 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cuda_vm_resource.h
--rw-r--r--   0 root         (0) root         (0)     5267 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/default_resources.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/
--rw-r--r--   0 root         (0) root         (0)     3850 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/align.h
--rw-r--r--   0 root         (0) root         (0)     6541 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_alloc.h
--rw-r--r--   0 root         (0) root         (0)     1426 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_collections.h
--rw-r--r--   0 root         (0) root         (0)    25585 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/free_list.h
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/util.h
--rw-r--r--   0 root         (0) root         (0)     2934 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/fixed_order_resource.h
--rw-r--r--   0 root         (0) root         (0)     6580 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/malloc_resource.h
--rw-r--r--   0 root         (0) root         (0)    22782 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory.h
--rw-r--r--   0 root         (0) root         (0)     2057 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_kind.h
--rw-r--r--   0 root         (0) root         (0)     2278 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_resource.h
--rw-r--r--   0 root         (0) root         (0)     9348 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/monotonic_resource.h
--rw-r--r--   0 root         (0) root         (0)    11682 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource.h
--rw-r--r--   0 root         (0) root         (0)     1084 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource_base.h
--rw-r--r--   0 root         (0) root         (0)      998 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/with_upstream.h
--rw-r--r--   0 root         (0) root         (0)     3169 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/nvtx.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/os/
--rw-r--r--   0 root         (0) root         (0)     5420 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/os/shared_mem.h
--rw-r--r--   0 root         (0) root         (0)     4677 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/partition.h
--rw-r--r--   0 root         (0) root         (0)    10461 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/per_stream_pool.h
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/permute.h
--rw-r--r--   0 root         (0) root         (0)     2337 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/python_util.h
--rw-r--r--   0 root         (0) root         (0)     3283 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/random.h
--rw-r--r--   0 root         (0) root         (0)    19482 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/small_vector.h
--rw-r--r--   0 root         (0) root         (0)     9394 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/span.h
--rw-r--r--   0 root         (0) root         (0)     1902 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/spinlock.h
--rw-r--r--   0 root         (0) root         (0)     5372 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_map.h
--rw-r--r--   0 root         (0) root         (0)     6547 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_switch.h
--rw-r--r--   0 root         (0) root         (0)     5872 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/stream.h
--rw-r--r--   0 root         (0) root         (0)    18748 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_layout.h
--rw-r--r--   0 root         (0) root         (0)    54963 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape.h
--rw-r--r--   0 root         (0) root         (0)     1617 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape_print.h
--rw-r--r--   0 root         (0) root         (0)    33471 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_view.h
--rw-r--r--   0 root         (0) root         (0)     2403 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/traits.h
--rw-r--r--   0 root         (0) root         (0)     8062 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tuple_helpers.h
--rw-r--r--   0 root         (0) root         (0)     5479 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/unique_handle.h
--rw-r--r--   0 root         (0) root         (0)    13956 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/util.h
--rw-r--r--   0 root         (0) root         (0)     1655 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/version_util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/
--rw-r--r--   0 root         (0) root         (0)     5734 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/decode_results.h
--rw-r--r--   0 root         (0) root         (0)     8884 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder.h
--rw-r--r--   0 root         (0) root         (0)     8845 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder_interfaces.h
--rw-r--r--   0 root         (0) root         (0)     4098 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_format.h
--rw-r--r--   0 root         (0) root         (0)     1542 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_orientation.h
--rw-r--r--   0 root         (0) root         (0)     5546 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_source.h
--rw-r--r--   0 root         (0) root         (0)     1992 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/operators.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.482541 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/
--rw-r--r--   0 root         (0) root         (0)   256667 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/Acknowledgements.txt
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/COPYRIGHT
--rw-r--r--   0 root         (0) root         (0)    10142 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      690 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/dali_tf_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4027 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/
--rw-r--r--   0 root         (0) root         (0)   206632 2023-06-13 09:35:40.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_11.so
--rw-r--r--   0 root         (0) root         (0)   206896 2023-06-13 09:35:40.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_12.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/stub/
--rw-r--r--   0 root         (0) root         (0)    13800 2023-06-13 09:35:40.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/stub/libdali.so
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4409 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/stubgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.523388 nvidia-dali-tf-plugin-cuda110-1.28.0/
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-07-10 16:31:49.523388 nvidia-dali-tf-plugin-cuda110-1.28.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    43001 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/dali_dataset_op.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.511388 nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin/
+-rw-r--r--   0 root         (0) root         (0)     5169 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin/dali_dataset.h
+-rw-r--r--   0 root         (0) root         (0)     7079 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin/dali_helper.h
+-rw-r--r--   0 root         (0) root         (0)    17344 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin_install_tool.py
+-rw-r--r--   0 root         (0) root         (0)     6207 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17543 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/daliop.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.507388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.511388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/
+-rw-r--r--   0 root         (0) root         (0)    27259 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/c_api.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.515388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/
+-rw-r--r--   0 root         (0) root         (0)     5686 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/access_order.h
+-rw-r--r--   0 root         (0) root         (0)    10320 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/any.h
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/api_helper.h
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-07-10 15:14:41.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/backend_tags.h
+-rw-r--r--   0 root         (0) root         (0)     7777 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/bitmask.h
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/boundary.h
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/byte_io.h
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/call_at_exit.h
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/common.h
+-rw-r--r--   0 root         (0) root         (0)    17542 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/convert.h
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/copy_vector_helper.h
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_error.h
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_event.h
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_event_pool.h
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_rt_utils.h
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_stream.h
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_stream_pool.h
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_utils.h
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dev_array.h
+-rw-r--r--   0 root         (0) root         (0)     5315 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dev_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dev_string.h
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/device_guard.h
+-rw-r--r--   0 root         (0) root         (0)      815 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dynlink_cuda.h
+-rw-r--r--   0 root         (0) root         (0)     5034 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dynlink_cufile.h
+-rw-r--r--   0 root         (0) root         (0)     6146 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/endian_util.h
+-rw-r--r--   0 root         (0) root         (0)    10891 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/error_handling.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.515388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/exec/
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/exec/engine.h
+-rw-r--r--   0 root         (0) root         (0)     4648 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/expand_dims.h
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/fast_div.h
+-rw-r--r--   0 root         (0) root         (0)    14461 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/float16.h
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/force_inline.h
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/format.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.519388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/box.h
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/geom_utils.h
+-rw-r--r--   0 root         (0) root         (0)    17992 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/mat.h
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/transform.h
+-rw-r--r--   0 root         (0) root         (0)    21114 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/vec.h
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/host_dev.h
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/int_literals.h
+-rw-r--r--   0 root         (0) root         (0)     5889 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/math_util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.519388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/
+-rw-r--r--   0 root         (0) root         (0)    22129 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/async_pool.h
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/binning_resource.h
+-rw-r--r--   0 root         (0) root         (0)     5291 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/composite_resource.h
+-rw-r--r--   0 root         (0) root         (0)     9018 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/cu_vm.h
+-rw-r--r--   0 root         (0) root         (0)    37732 2023-07-10 15:14:41.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/cuda_memory_resource.h
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-07-10 15:14:41.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/cuda_stream_view.h
+-rw-r--r--   0 root         (0) root         (0)    34893 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/cuda_vm_resource.h
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/default_resources.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.519388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/align.h
+-rw-r--r--   0 root         (0) root         (0)     6541 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/aux_alloc.h
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/aux_collections.h
+-rw-r--r--   0 root         (0) root         (0)    25585 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/free_list.h
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/util.h
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/fixed_order_resource.h
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/malloc_resource.h
+-rw-r--r--   0 root         (0) root         (0)    22782 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/memory.h
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/memory_kind.h
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-07-10 15:14:41.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/memory_resource.h
+-rw-r--r--   0 root         (0) root         (0)     9348 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/monotonic_resource.h
+-rw-r--r--   0 root         (0) root         (0)    11682 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/pool_resource.h
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/pool_resource_base.h
+-rw-r--r--   0 root         (0) root         (0)      998 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/with_upstream.h
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/nvtx.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.519388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/os/
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/os/shared_mem.h
+-rw-r--r--   0 root         (0) root         (0)     4677 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/partition.h
+-rw-r--r--   0 root         (0) root         (0)    10461 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/per_stream_pool.h
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/permute.h
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/python_util.h
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/random.h
+-rw-r--r--   0 root         (0) root         (0)    19482 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/small_vector.h
+-rw-r--r--   0 root         (0) root         (0)     9394 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/span.h
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/spinlock.h
+-rw-r--r--   0 root         (0) root         (0)     5372 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/static_map.h
+-rw-r--r--   0 root         (0) root         (0)     6547 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/static_switch.h
+-rw-r--r--   0 root         (0) root         (0)     5872 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/stream.h
+-rw-r--r--   0 root         (0) root         (0)    18748 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_layout.h
+-rw-r--r--   0 root         (0) root         (0)    54963 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_shape.h
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_shape_print.h
+-rw-r--r--   0 root         (0) root         (0)    33471 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_view.h
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/traits.h
+-rw-r--r--   0 root         (0) root         (0)     8062 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tuple_helpers.h
+-rw-r--r--   0 root         (0) root         (0)     5454 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/unique_handle.h
+-rw-r--r--   0 root         (0) root         (0)    13956 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/util.h
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/version_util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.519388 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/decode_results.h
+-rw-r--r--   0 root         (0) root         (0)     8884 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_decoder.h
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_decoder_interfaces.h
+-rw-r--r--   0 root         (0) root         (0)     4098 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_format.h
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_orientation.h
+-rw-r--r--   0 root         (0) root         (0)     5546 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_source.h
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/operators.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.507388 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.523388 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/
+-rw-r--r--   0 root         (0) root         (0)   256667 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/Acknowledgements.txt
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/COPYRIGHT
+-rw-r--r--   0 root         (0) root         (0)    10142 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      690 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 09:30:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/dali_tf_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.523388 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.523388 nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/
+-rw-r--r--   0 root         (0) root         (0)   206632 2023-07-10 16:31:45.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/libdali_tf_2_11.so
+-rw-r--r--   0 root         (0) root         (0)   206896 2023-07-10 16:31:45.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/libdali_tf_2_12.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:49.523388 nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/stub/
+-rw-r--r--   0 root         (0) root         (0)    13800 2023-07-10 16:31:45.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/stub/libdali.so
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 16:31:49.523388 nvidia-dali-tf-plugin-cuda110-1.28.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4410 2023-07-10 16:31:49.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-07-10 09:30:50.000000 nvidia-dali-tf-plugin-cuda110-1.28.0/stubgen.py
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/PKG-INFO` & `nvidia-dali-tf-plugin-cuda110-1.28.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-cuda110
-Version: 1.27.0
-Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 4cc38a6b48a74cc06fe8594b6e5c18ae090dc045
+Version: 1.28.0
+Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 7268fe15c50db664b4df5226b66cb46e717f46be
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Description: TensorFlow plugin for NVIDIA DALI
         =================================
         
         The TensorFlow plugin enables usage of DALI with TensorFlow.
@@ -38,14 +38,14 @@
             :align: center
             :alt: DALI Diagram
         
         .. |release-doc| replace:: latest DALI Documentation
         .. _release-doc: https://docs.nvidia.com/deeplearning/dali/user-guide/docs/index.html
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/x-rst
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_dataset_op.cc` & `nvidia-dali-tf-plugin-cuda110-1.28.0/dali_dataset_op.cc`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_dataset.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin/dali_dataset.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin/dali_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_install_tool.py` & `nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin_install_tool.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_utils.py` & `nvidia-dali-tf-plugin-cuda110-1.28.0/dali_tf_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/daliop.cc` & `nvidia-dali-tf-plugin-cuda110-1.28.0/daliop.cc`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/c_api.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/c_api.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/access_order.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/access_order.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/any.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/any.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/api_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/api_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/backend_tags.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/backend_tags.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2018-2021, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+// Copyright (c) 2018-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -12,15 +12,15 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef DALI_CORE_BACKEND_TAGS_H_
 #define DALI_CORE_BACKEND_TAGS_H_
 
 #include <type_traits>
-#include <cuda/memory_resource>
+#include "dali/core/mm/cuda_memory_resource.h"
 
 namespace dali {
 
 struct StorageGPU {};
 struct StorageCPU {};
 struct StorageUnified {};
 
@@ -55,30 +55,30 @@
 template<class ComputeBackend>
 using compute_to_storage_t = typename compute_to_storage<ComputeBackend>::type;
 
 template <typename MemoryKind>
 struct kind2storage;
 
 template <>
-struct kind2storage<cuda::memory_kind::host> {
+struct kind2storage<cuda_for_dali::memory_kind::host> {
   using type = StorageCPU;
 };
 
 template <>
-struct kind2storage<cuda::memory_kind::pinned> {
+struct kind2storage<cuda_for_dali::memory_kind::pinned> {
   using type = StorageCPU;
 };
 
 template <>
-struct kind2storage<cuda::memory_kind::device> {
+struct kind2storage<cuda_for_dali::memory_kind::device> {
   using type = StorageGPU;
 };
 
 template <>
-struct kind2storage<cuda::memory_kind::managed> {
+struct kind2storage<cuda_for_dali::memory_kind::managed> {
   using type = StorageUnified;
 };
 
 template <typename MemoryKind>
 using kind2storage_t = typename kind2storage<MemoryKind>::type;
 
 }  // namespace dali
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/bitmask.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/bitmask.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/boundary.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/boundary.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/byte_io.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/byte_io.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/call_at_exit.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/call_at_exit.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/common.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/common.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/convert.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/convert.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/copy_vector_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/copy_vector_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_error.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_error.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_event.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020, NVIDIA CORPORATION. All rights reserved.
+// Copyright (c) 2020, 2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -14,14 +14,15 @@
 
 #ifndef DALI_CORE_CUDA_EVENT_H_
 #define DALI_CORE_CUDA_EVENT_H_
 
 #include <driver_types.h>
 #include <utility>
 #include "dali/core/unique_handle.h"
+#include "dali/core/api_helper.h"
 
 namespace dali {
 
 /**
  * @brief A wrapper class for CUDA event handle (cudaEvent_t),
  *
  * The purpose of this class is to provide safe ownership and lifecycle management
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_event_pool.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020, NVIDIA CORPORATION. All rights reserved.
+// Copyright (c) 2020, 2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -15,14 +15,15 @@
 #ifndef DALI_CORE_CUDA_EVENT_POOL_H_
 #define DALI_CORE_CUDA_EVENT_POOL_H_
 
 #include <vector>
 #include <utility>
 #include "dali/core/cuda_event.h"
 #include "dali/core/spinlock.h"
+#include "dali/core/api_helper.h"
 
 namespace dali {
 
 class DLL_PUBLIC CUDAEventPool {
  public:
   ~CUDAEventPool();
   explicit CUDAEventPool(unsigned event_flags = cudaEventDisableTiming);
@@ -76,15 +77,15 @@
     : event(std::move(event)), next(next) {}
     CUDAEvent event;
     EventEntry *next = nullptr;
   };
 
   EventEntry *unused_ = nullptr;
 
-  vector<EventEntry *> dev_events_;
+  std::vector<EventEntry *> dev_events_;
   spinlock lock_;
 
   static EventEntry *Pop(EventEntry *&head) {
     auto *e = head;
     if (e)
       head = head->next;
     return e;
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_rt_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_rt_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_stream.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2021, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+// Copyright (c) 2020-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -14,14 +14,15 @@
 
 #ifndef DALI_CORE_CUDA_STREAM_H_
 #define DALI_CORE_CUDA_STREAM_H_
 
 #include <driver_types.h>
 #include <utility>
 #include "dali/core/unique_handle.h"
+#include "dali/core/api_helper.h"
 
 namespace dali {
 
 DLL_PUBLIC int DeviceFromStream(cudaStream_t s);
 
 /**
  * @brief A wrapper class for CUDA stream handle (cudaStream_t),
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_stream_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2021-2022, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+// Copyright (c) 2021-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -87,15 +87,15 @@
     CUDAStream stream;
     StreamEntry *next = nullptr;
   };
 
   StreamEntry *unused_ = nullptr;
   std::atomic_int lease_count_{0};
 
-  vector<StreamEntry *> dev_streams_;
+  std::vector<StreamEntry *> dev_streams_;
   spinlock lock_;
 
   static StreamEntry *Pop(StreamEntry *&head) {
     auto *e = head;
     if (e)
       head = head->next;
     return e;
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_array.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dev_array.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_buffer.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dev_buffer.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_string.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dev_string.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/device_guard.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/device_guard.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cuda.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dynlink_cuda.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cufile.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/dynlink_cufile.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/endian_util.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/endian_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/error_handling.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/error_handling.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/exec/engine.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/exec/engine.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/expand_dims.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/expand_dims.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/fast_div.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/fast_div.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/float16.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/float16.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/force_inline.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/force_inline.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/format.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/format.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/box.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/box.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/geom_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/geom_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/mat.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/mat.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/transform.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/transform.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/vec.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/geom/vec.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/host_dev.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/host_dev.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/int_literals.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/int_literals.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/math_util.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/math_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/async_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/async_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/binning_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/binning_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/composite_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/composite_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cu_vm.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/cu_vm.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cuda_vm_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/cuda_vm_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/default_resources.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/default_resources.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/align.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/align.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_alloc.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/aux_alloc.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_collections.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/aux_collections.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/free_list.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/free_list.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/util.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/detail/util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/fixed_order_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/fixed_order_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/malloc_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/malloc_resource.h`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #ifndef DALI_CORE_MM_MALLOC_RESOURCE_H_
 #define DALI_CORE_MM_MALLOC_RESOURCE_H_
 
 #include <stdlib.h>
 #include <malloc.h>
 #include "dali/core/mm/memory_resource.h"
 #include "dali/core/cuda_error.h"
+#include "dali/core/cuda_stream_pool.h"
 #include "dali/core/mm/detail/align.h"
 #include "dali/core/device_guard.h"
 
 namespace dali {
 namespace mm {
 
 /**
@@ -197,12 +198,39 @@
  public:
   static managed_malloc_memory_resource &instance() {
     static managed_malloc_memory_resource inst;
     return inst;
   }
 };
 
+#if CUDA_VERSION >= 11020
+
+class DLL_PUBLIC cuda_malloc_async_memory_resource
+: public mm::async_memory_resource<mm::memory_kind::device> {
+ public:
+  cuda_malloc_async_memory_resource() : cuda_malloc_async_memory_resource(-1) {}
+
+  explicit cuda_malloc_async_memory_resource(int device_id);
+
+  static bool is_supported(int device_id = -1);
+
+  int device_id() const noexcept { return device_id_; }
+
+ private:
+  void *do_allocate(size_t size, size_t alignment) override;
+
+  void do_deallocate(void *ptr, size_t size, size_t alignment) override;
+
+  void *do_allocate_async(size_t size, size_t alignment, stream_view stream) override;
+
+  void do_deallocate_async(void *ptr, size_t size, size_t alignment, stream_view stream) override;
+
+  int device_id_;
+  CUDAStreamLease dummy_host_stream_;
+};
+
+#endif
+
 }  // namespace mm
 }  // namespace dali
 
-
 #endif  // DALI_CORE_MM_MALLOC_RESOURCE_H_
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/memory.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_kind.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/memory_kind.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/memory_resource.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2021, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+// Copyright (c) 2021-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -14,15 +14,15 @@
 
 #ifndef DALI_CORE_MM_MEMORY_RESOURCE_H_
 #define DALI_CORE_MM_MEMORY_RESOURCE_H_
 
 #include <cuda_runtime.h>
 #include <cstddef>
 
-#include <cuda/memory_resource>
+#include "dali/core/mm/cuda_memory_resource.h"
 
 namespace dali {
 
 /**
  * @brief Memory Manager
  *
  * This namespace contains classes and function for memory managment.
@@ -32,39 +32,40 @@
  *
  * Some of the memory resources are composable, accepting an upstream memory resource.
  * Such composite resources can be used to quickly build an application-specific memory resource,
  * tailored to specific needs.
  */
 namespace mm {
 
-namespace memory_kind = cuda::memory_kind;
+namespace memory_kind = cuda_for_dali::memory_kind;
 
-using cuda::memory_resource;
-using cuda::resource_view;
-using cuda::stream_ordered_resource_view;
+using cuda_for_dali::memory_resource;
+using cuda_for_dali::resource_view;
+using cuda_for_dali::stream_ordered_resource_view;
 
 using host_memory_resource = memory_resource<memory_kind::host>;
 using pinned_memory_resource = memory_resource<memory_kind::pinned>;
-using cuda::stream_view;
+using cuda_for_dali::stream_view;
 
 template <typename Kind>
-using async_memory_resource = cuda::stream_ordered_memory_resource<Kind>;
+using async_memory_resource = cuda_for_dali::stream_ordered_memory_resource<Kind>;
 
 using device_async_resource = async_memory_resource<memory_kind::device>;
 using pinned_async_resource = async_memory_resource<memory_kind::pinned>;
 using managed_async_resource = async_memory_resource<memory_kind::managed>;
 
 struct stream_context {
   stream_view stream;
 };
 
 namespace detail {
 
 template <typename Kind>
-constexpr bool is_host_accessible = cuda::kind_has_property<Kind, cuda::memory_access::host>::value;
+constexpr bool is_host_accessible =
+    cuda_for_dali::kind_has_property<Kind, cuda_for_dali::memory_access::host>::value;
 
 }  // namespace detail
 
 }  // namespace mm
 }  // namespace dali
 
 #endif  // DALI_CORE_MM_MEMORY_RESOURCE_H_
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/monotonic_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/monotonic_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/pool_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource_base.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/pool_resource_base.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/with_upstream.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/mm/with_upstream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/nvtx.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/nvtx.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/os/shared_mem.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/os/shared_mem.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/partition.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/partition.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/per_stream_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/per_stream_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/permute.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/permute.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/python_util.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/python_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/random.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/random.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/small_vector.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/small_vector.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/span.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/span.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/spinlock.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/spinlock.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_map.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/static_map.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_switch.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/static_switch.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/stream.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/stream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_layout.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_layout.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_shape.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape_print.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_shape_print.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_view.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tensor_view.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/traits.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/traits.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tuple_helpers.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/tuple_helpers.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/unique_handle.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/unique_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020, 2022, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+// Copyright (c) 2020, 2022-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -12,15 +12,14 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef DALI_CORE_UNIQUE_HANDLE_H_
 #define DALI_CORE_UNIQUE_HANDLE_H_
 
 #include <utility>
-#include "dali/core/common.h"
 
 namespace dali {
 
 /**
  * @brief This class is an analogue of `unique_ptr` for non-memory resource handles.
  *
  * UniqueHandle is a base class for implementing managed resources (files, OS handles, etc).
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/util.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/version_util.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/core/version_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/decode_results.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/decode_results.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_decoder.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder_interfaces.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_decoder_interfaces.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_format.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_format.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_orientation.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_orientation.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_source.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/imgcodec/image_source.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/operators.h` & `nvidia-dali-tf-plugin-cuda110-1.28.0/include/dali/operators.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/Acknowledgements.txt` & `nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/Acknowledgements.txt`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/COPYRIGHT` & `nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/LICENSE` & `nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/LICENSE`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/__init__.py` & `nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.27.0'
-__git_sha__ = '4cc38a6b48a74cc06fe8594b6e5c18ae090dc045'
+__version__ = '1.28.0'
+__git_sha__ = '7268fe15c50db664b4df5226b66cb46e717f46be'
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/dali_tf_plugin.py` & `nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia/dali_tf_plugin/dali_tf_plugin.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-cuda110
-Version: 1.27.0
-Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 4cc38a6b48a74cc06fe8594b6e5c18ae090dc045
+Version: 1.28.0
+Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 7268fe15c50db664b4df5226b66cb46e717f46be
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Description: TensorFlow plugin for NVIDIA DALI
         =================================
         
         The TensorFlow plugin enables usage of DALI with TensorFlow.
@@ -38,14 +38,14 @@
             :align: center
             :alt: DALI Diagram
         
         .. |release-doc| replace:: latest DALI Documentation
         .. _release-doc: https://docs.nvidia.com/deeplearning/dali/user-guide/docs/index.html
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/x-rst
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt` & `nvidia-dali-tf-plugin-cuda110-1.28.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 ./include/dali/core/geom/mat.h
 ./include/dali/core/geom/transform.h
 ./include/dali/core/geom/vec.h
 ./include/dali/core/mm/async_pool.h
 ./include/dali/core/mm/binning_resource.h
 ./include/dali/core/mm/composite_resource.h
 ./include/dali/core/mm/cu_vm.h
+./include/dali/core/mm/cuda_memory_resource.h
+./include/dali/core/mm/cuda_stream_view.h
 ./include/dali/core/mm/cuda_vm_resource.h
 ./include/dali/core/mm/default_resources.h
 ./include/dali/core/mm/fixed_order_resource.h
 ./include/dali/core/mm/malloc_resource.h
 ./include/dali/core/mm/memory.h
 ./include/dali/core/mm/memory_kind.h
 ./include/dali/core/mm/memory_resource.h
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_11.so` & `nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/libdali_tf_2_11.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_12.so` & `nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/libdali_tf_2_12.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/stub/libdali.so` & `nvidia-dali-tf-plugin-cuda110-1.28.0/prebuilt/stub/libdali.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/setup.py` & `nvidia-dali-tf-plugin-cuda110-1.28.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         # It doesn't matter what we write here, because we are overriding the
         # build_ext step altogether.
         # By filling this ext_modules we are signaling that this package needs
         # to be built for different platforms
         self.ext_modules = [Extension('nvidia.dali_tf_plugin', [])]
 
 setup(name='nvidia-dali-tf-plugin-cuda110',
-      description='NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 4cc38a6b48a74cc06fe8594b6e5c18ae090dc045',
+      description='NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 7268fe15c50db664b4df5226b66cb46e717f46be',
       long_description='''TensorFlow plugin for NVIDIA DALI
 =================================
 
 The TensorFlow plugin enables usage of DALI with TensorFlow.
 
 The NVIDIA Data Loading Library (DALI) is a library for data loading and
 pre-processing to accelerate deep learning applications. It provides a
@@ -70,30 +70,30 @@
     :alt: DALI Diagram
 
 .. |release-doc| replace:: latest DALI Documentation
 .. _release-doc: https://docs.nvidia.com/deeplearning/dali/user-guide/docs/index.html
 ''',
       long_description_content_type="text/x-rst",
       url='https://github.com/NVIDIA/dali',
-      version='1.27.0',
+      version='1.28.0',
       author='NVIDIA Corporation',
       license='Apache License 2.0',
       packages=find_namespace_packages(include=['nvidia.*']),
       include_package_data=True,
       zip_safe=False,
-      python_requires='>=3.6, <3.11',
+      python_requires='>=3.7, <3.12',
       classifiers=[
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           ],
       install_requires = [
-          'nvidia-dali-cuda110==1.27.0'
+          'nvidia-dali-cuda110==1.28.0'
           ],
 
       cmdclass={
           'build_ext': CustomBuildExt,
       },
       distclass=CustomDistribution
      )
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.27.0/stubgen.py` & `nvidia-dali-tf-plugin-cuda110-1.28.0/stubgen.py`

 * *Files identical despite different names*

