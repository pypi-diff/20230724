# Comparing `tmp/roughpy-0.0.4.tar.gz` & `tmp/roughpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roughpy-0.0.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "roughpy-0.0.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `roughpy-0.0.4.tar` & `roughpy-0.0.5.tar`

### file list

```diff
@@ -1,728 +1,737 @@
--rw-r--r--   0        0        0     2345 2022-11-09 12:37:21.000000 roughpy-0.0.4/.clang-format
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     3994 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/workflows/manage_version.yml
--rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0     5667 2022-11-09 12:37:21.000000 roughpy-0.0.4/.gitignore
--rw-r--r--   0        0        0      433 2022-11-09 12:37:21.000000 roughpy-0.0.4/.gitmodules
--rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 roughpy-0.0.4/CHANGELOG
--rw-r--r--   0        0        0     9736 2022-11-09 12:37:21.000000 roughpy-0.0.4/CMakeLists.txt
--rw-r--r--   0        0        0     1489 2022-11-09 12:37:21.000000 roughpy-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     4108 2022-11-09 12:37:21.000000 roughpy-0.0.4/README.md
--rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 roughpy-0.0.4/THANKS.txt
--rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 roughpy-0.0.4/VERSION.txt
--rw-r--r--   0        0        0     3262 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/CMakeLists.txt
--rw-r--r--   0        0        0    16233 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base.h
--rw-r--r--   0        0        0    23529 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base_impl.h
--rw-r--r--   0        0        0     8100 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle.h
--rw-r--r--   0        0        0    13572 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h
--rw-r--r--   0        0        0    26323 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_impl.h
--rw-r--r--   0        0        0     2737 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_fwd.h
--rw-r--r--   0        0        0    31744 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_impl.h
--rw-r--r--   0        0        0     3829 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_info.h
--rw-r--r--   0        0        0     7137 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator.h
--rw-r--r--   0        0        0     3740 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator_impl.h
--rw-r--r--   0        0        0     9250 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/basis.h
--rw-r--r--   0        0        0     6672 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/basis_impl.h
--rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/basis_info.h
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/bundle_info.h
--rw-r--r--   0        0        0     9538 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/context.h
--rw-r--r--   0        0        0     4148 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/context_fwd.h
--rw-r--r--   0        0        0     1881 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/fallback_operations.h
--rw-r--r--   0        0        0     2707 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor.h
--rw-r--r--   0        0        0     3750 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_fwd.h
--rw-r--r--   0        0        0     6431 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_impl.h
--rw-r--r--   0        0        0     2730 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/lie.h
--rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/lie_basis.h
--rw-r--r--   0        0        0     1852 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/lie_fwd.h
--rw-r--r--   0        0        0     2633 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/linear_operator.h
--rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor.h
--rw-r--r--   0        0        0     1858 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h
--rw-r--r--   0        0        0     2192 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/tensor_basis.h
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/ContextFixture.cpp
--rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/ContextFixture.h
--rw-r--r--   0        0        0     3000 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/algebra_base.cpp
--rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/algebra_iterator.cpp
--rw-r--r--   0        0        0     1747 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/basis.cpp
--rw-r--r--   0        0        0     9768 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/context.cpp
--rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/double_lite_context.cpp
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/float_lite_context.cpp
--rw-r--r--   0        0        0     4084 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/free_tensor.cpp
--rw-r--r--   0        0        0     4248 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/hall_set_size.cpp
--rw-r--r--   0        0        0     2569 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/hall_set_size.h
--rw-r--r--   0        0        0     3031 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h
--rw-r--r--   0        0        0     4222 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/free_tensor_info.h
--rw-r--r--   0        0        0     6669 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_basis_info.h
--rw-r--r--   0        0        0     4191 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_info.h
--rw-r--r--   0        0        0     3099 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lite_vector_selector.h
--rw-r--r--   0        0        0     4223 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h
--rw-r--r--   0        0        0     5973 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h
--rw-r--r--   0        0        0     2450 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h
--rw-r--r--   0        0        0     6642 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/tensor_basis_info.h
--rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/vector_type_helper.h
--rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lie.cpp
--rw-r--r--   0        0        0     1821 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lie_basis.cpp
--rw-r--r--   0        0        0     4732 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lite_context.cpp
--rw-r--r--   0        0        0    28170 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lite_context.h
--rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/rational_lite_context.cpp
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/rational_poly_lite_context.cpp
--rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/shuffle_tensor.cpp
--rw-r--r--   0        0        0     1883 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/tensor_basis.cpp
--rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/test_lie.cpp
--rw-r--r--   0        0        0     1631 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/testing/mock_context.cpp
--rw-r--r--   0        0        0     2139 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/testing/mock_context.h
--rw-r--r--   0        0        0   106087 2022-11-09 12:37:21.000000 roughpy-0.0.4/branding/logo/logo_square_white.jpg
--rw-r--r--   0        0        0      509 2022-11-09 12:37:21.000000 roughpy-0.0.4/cmake/Modules/FindPCGRandom.cmake
--rw-r--r--   0        0        0    20238 2022-11-09 12:37:21.000000 roughpy-0.0.4/cmake/roughpy_helpers.cmake
--rw-r--r--   0        0        0      355 2022-11-09 12:37:21.000000 roughpy-0.0.4/cmake/version.py.in
--rw-r--r--   0        0        0      495 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/CMakeLists.txt
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/alloc.h
--rw-r--r--   0        0        0     3627 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/helpers.h
--rw-r--r--   0        0        0    10918 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/macros.h
--rw-r--r--   0        0        0     4701 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/slice.h
--rw-r--r--   0        0        0     5000 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/traits.h
--rw-r--r--   0        0        0     2628 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/types.h
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/CMakeLists.txt
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/CMakeLists.txt
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/CudaDeviceContext.cu
--rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/CudaDeviceContext.cuh
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/CMakeLists.txt
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/src/CUDAFloatType.cu
--rw-r--r--   0        0        0     2005 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/src/CUDAFloatType.cuh
--rw-r--r--   0        0        0     8605 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/src/CUDA_standard_scalar.cuh
--rw-r--r--   0        0        0      868 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/include/roughpy/device/core.h
--rw-r--r--   0        0        0    18540 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/include/roughpy/device/device_algebra_base.h
--rw-r--r--   0        0        0     4377 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/include/roughpy/device/device_context.h
--rw-r--r--   0        0        0     2348 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/binary_kernel.cuh
--rw-r--r--   0        0        0     3972 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/functors.h
--rw-r--r--   0        0        0     1712 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/tmp.cu
--rw-r--r--   0        0        0     2304 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/unary_kernel.cuh
--rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_algebra_base.cpp
--rw-r--r--   0        0        0     1728 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_context.cpp
--rw-r--r--   0        0        0     2854 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_free_tensor.cpp
--rw-r--r--   0        0        0     2912 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_free_tensor.h
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 roughpy-0.0.4/docs/make.bat
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 roughpy-0.0.4/docs/source/conf.py
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 roughpy-0.0.4/docs/source/index.rst
--rw-r--r--   0        0        0     3589 2022-11-09 12:37:21.000000 roughpy-0.0.4/examples/lie_to_tensor_formulae.py
--rw-r--r--   0        0        0     1956 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/.clang-format
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/.git
--rw-r--r--   0        0        0     5992 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/.gitignore
--rw-r--r--   0        0        0     7502 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/CMakeLists.txt
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/Dockerfile
--rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/Dockerfile.remote-cpp-env
--rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/LibalgebraConfig.cmake.in
--rw-r--r--   0        0        0     2706 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/README.md
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/CMakeLists.txt
--rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/antipode/CMakeLists.txt
--rw-r--r--   0        0        0     5078 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/antipode/antipode_bm.cpp
--rw-r--r--   0        0        0     1941 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/CMakeLists.txt
--rw-r--r--   0        0        0    14501 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp
--rw-r--r--   0        0        0     2363 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp
--rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/Modules/FindBignum.cmake
--rw-r--r--   0        0        0     3540 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP.cmake
--rw-r--r--   0        0        0     4012 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake
--rw-r--r--   0        0        0     1602 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/libalgebra_test_helper.cmake
--rw-r--r--   0        0        0    19400 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/_tensor_basis.h
--rw-r--r--   0        0        0     5123 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/alg_types.h
--rw-r--r--   0        0        0    33383 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/algebra.h
--rw-r--r--   0        0        0     4069 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/alternative_multiplications.h
--rw-r--r--   0        0        0     2188 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_basis.h
--rw-r--r--   0        0        0    10008 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_multiplication.h
--rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/base_basis.h
--rw-r--r--   0        0        0     2600 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/base_vector.h
--rw-r--r--   0        0        0     3202 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/basis.h
--rw-r--r--   0        0        0    12663 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/coefficients/gmp_ser.h
--rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/coefficients.h
--rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/complex.h
--rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/composition_operator.h
--rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/constlog2.h
--rw-r--r--   0        0        0     2065 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/constpower.h
--rw-r--r--   0        0        0    25576 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/dense_storage.h
--rw-r--r--   0        0        0    32612 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/dense_vector.h
--rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/caching_tags.h
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/function_extension_cache_base.h
--rw-r--r--   0        0        0     4044 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/integer_maths.h
--rw-r--r--   0        0        0     1536 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/level_walkers.h
--rw-r--r--   0        0        0     3387 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/meta.h
--rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/order_trait.h
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/platform.h
--rw-r--r--   0        0        0     3762 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/reversing_permutation.h
--rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/smallest_int_type.h
--rw-r--r--   0        0        0     6839 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/dot_product_implementations.h
--rw-r--r--   0        0        0     2824 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/free_extension.h
--rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/functionals.h
--rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h
--rw-r--r--   0        0        0    10154 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h
--rw-r--r--   0        0        0    21063 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/hall_set.h
--rw-r--r--   0        0        0    40389 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/hybrid_vector.h
--rw-r--r--   0        0        0     2519 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/implementation_types.h
--rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/iterators.h
--rw-r--r--   0        0        0     4414 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/key_iterators.h
--rw-r--r--   0        0        0     6487 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/libalgebra.h
--rw-r--r--   0        0        0     6024 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/lie.h
--rw-r--r--   0        0        0    17479 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/lie_basis.h
--rw-r--r--   0        0        0     3791 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/lie_inner_product.h
--rw-r--r--   0        0        0     7234 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/monomial_basis.h
--rw-r--r--   0        0        0      886 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/mpfloat_coefficients.h
--rw-r--r--   0        0        0     1033 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/multi_linear_operators.h
--rw-r--r--   0        0        0     5991 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/multi_polynomial.h
--rw-r--r--   0        0        0     1693 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/multiplication_helpers.h
--rw-r--r--   0        0        0     9179 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/operators.h
--rw-r--r--   0        0        0     5565 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/poly_basis.h
--rw-r--r--   0        0        0     6082 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie.h
--rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie_basis.h
--rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/polynomial_coefficients.h
--rw-r--r--   0        0        0     6720 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/polynomials.h
--rw-r--r--   0        0        0      779 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/rational_coefficients.h
--rw-r--r--   0        0        0     5880 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/reconfigure_operator.h
--rw-r--r--   0        0        0     8186 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/scalar_bundle.h
--rw-r--r--   0        0        0      982 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/scalar_multiply_operator.h
--rw-r--r--   0        0        0    41789 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/sparse_vector.h
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/sum_operator.h
--rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tags.h
--rw-r--r--   0        0        0   144218 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tensor.h
--rw-r--r--   0        0        0    19208 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tensor_basis.h
--rw-r--r--   0        0        0     1724 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tensor_operator.h
--rw-r--r--   0        0        0    11862 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/utils.h
--rw-r--r--   0        0        0    24861 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/vector.h
--rw-r--r--   0        0        0    31254 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/vector_bundle.h
--rw-r--r--   0        0        0     1309 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/vectors.h
--rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/CMakeLists.txt
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/README.md
--rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/CMakeLists.txt
--rw-r--r--   0        0        0     1872 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/SHOW.h
--rw-r--r--   0        0        0     2676 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/compat.h
--rw-r--r--   0        0        0     1058 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/helpers.h
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/memfile.cpp
--rw-r--r--   0        0        0     3236 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/memfile.h
--rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/multi_test.h
--rw-r--r--   0        0        0     1554 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/random_coeffs.h
--rw-r--r--   0        0        0     2483 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/random_vector_generator.h
--rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/reporter.cpp
--rw-r--r--   0        0        0      670 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/reporter.h
--rw-r--r--   0        0        0     1711 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/rng.h
--rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/run_tests.cpp
--rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/simple_basis.h
--rw-r--r--   0        0        0     2372 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/time_and_details.h
--rw-r--r--   0        0        0     3181 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp
--rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/CMakeLists.txt
--rw-r--r--   0        0        0     5679 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/HallSetTests.cpp
--rw-r--r--   0        0        0     4658 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/LatticePathTests.cpp
--rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/LibAlgebraUnitTests.cpp
--rw-r--r--   0        0        0    43337 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm
--rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp
--rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/SigHelpers.h
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/TreeBufferHelper.cpp
--rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/TreeBufferHelper.h
--rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/alg_framework.h
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/brown_path_increments.h
--rw-r--r--   0        0        0     2936 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/categorical_path.h
--rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/log2ceil.h
--rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/makebm.cpp
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/makebm.h
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/CMakeLists.txt
--rw-r--r--   0        0        0    17054 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins
--rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins
--rw-r--r--   0        0        0     1579 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins
--rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins
--rw-r--r--   0        0        0     1224 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h
--rw-r--r--   0        0        0     2240 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h
--rw-r--r--   0        0        0     1580 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/run_tests.cpp
--rw-r--r--   0        0        0    20566 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp
--rw-r--r--   0        0        0    11406 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp
--rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/speed_tests.cpp
--rw-r--r--   0        0        0    12166 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp
--rw-r--r--   0        0        0     6213 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp
--rw-r--r--   0        0        0     1590 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/x64sigs.cpp
--rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/CMakeLists.txt
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/adjoint/CMakeLists.txt
--rw-r--r--   0        0        0     7719 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp
--rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt
--rw-r--r--   0        0        0     2223 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h
--rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h
--rw-r--r--   0        0        0      696 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/antipode/CMakeLists.txt
--rw-r--r--   0        0        0     7994 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp
--rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/CMakeLists.txt
--rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h
--rw-r--r--   0        0        0     3917 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp
--rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp
--rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_tensor_basis_iteration.cpp
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/CMakeLists.txt
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp
--rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h
--rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_double_field.cpp
--rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_float_field.cpp
--rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp
--rw-r--r--   0        0        0      441 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_field.cpp
--rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp
--rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_rational_field.cpp
--rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h
--rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/CMakeLists.txt
--rw-r--r--   0        0        0    19137 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h
--rw-r--r--   0        0        0     8440 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp
--rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/hall_set/CMakeLists.txt
--rw-r--r--   0        0        0     8138 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp
--rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/CMakeLists.txt
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/run_tests.cpp
--rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_basis.cpp
--rw-r--r--   0        0        0     2083 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp
--rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp
--rw-r--r--   0        0        0     5505 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp
--rw-r--r--   0        0        0     1663 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/multipoly/CMakeLists.txt
--rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/multipoly/test_multipoly_prod.cpp
--rw-r--r--   0        0        0      387 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/CMakeLists.txt
--rw-r--r--   0        0        0     2816 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp
--rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp
--rw-r--r--   0        0        0     2406 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp
--rw-r--r--   0        0        0     1548 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp
--rw-r--r--   0        0        0     1791 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp
--rw-r--r--   0        0        0     1203 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp
--rw-r--r--   0        0        0     4353 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp
--rw-r--r--   0        0        0     2553 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp
--rw-r--r--   0        0        0     1785 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp
--rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt
--rw-r--r--   0        0        0     3057 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp
--rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/fixture.cpp
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/fixture.h
--rw-r--r--   0        0        0     4014 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp
--rw-r--r--   0        0        0     7910 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp
--rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp
--rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/temporary_directory.h
--rw-r--r--   0        0        0     2991 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp
--rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp
--rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/CMakeLists.txt
--rw-r--r--   0        0        0    43877 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp
--rw-r--r--   0        0        0      753 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt
--rw-r--r--   0        0        0    20887 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp
--rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/test_tangents.h
--rw-r--r--   0        0        0      983 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/run_tests.cpp
--rw-r--r--   0        0        0     3985 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h
--rw-r--r--   0        0        0     1797 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h
--rw-r--r--   0        0        0     4055 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h
--rw-r--r--   0        0        0     3037 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h
--rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp
--rw-r--r--   0        0        0     2509 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp
--rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp
--rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp
--rw-r--r--   0        0        0     5037 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp
--rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp
--rw-r--r--   0        0        0     2535 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp
--rw-r--r--   0        0        0     4900 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp
--rw-r--r--   0        0        0     3291 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp
--rw-r--r--   0        0        0    38059 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp
--rw-r--r--   0        0        0     2419 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/CMakeLists.txt
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/run_tests.cpp
--rw-r--r--   0        0        0     2678 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/CMakeLists.txt
--rw-r--r--   0        0        0     3599 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/framework_fixture.h
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/run_tests.cpp
--rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense.cpp
--rw-r--r--   0        0        0    13508 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp
--rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp
--rw-r--r--   0        0        0    12957 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h
--rw-r--r--   0        0        0    11707 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h
--rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h
--rw-r--r--   0        0        0     7086 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h
--rw-r--r--   0        0        0     1907 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h
--rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/CMakeLists.txt
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/types.cpp
--rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1.h
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1_lie.cpp
--rw-r--r--   0        0        0     4024 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/.git
--rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/CMakeLists.txt
--rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/README.md
--rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/Libalgebra_liteConfig.cmake.in
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/config.h.in
--rw-r--r--   0        0        0     2787 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/lalhelpers.cmake
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/rationals.h.in
--rw-r--r--   0        0        0    31148 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/algebra.h
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/basis.h
--rw-r--r--   0        0        0     3322 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h
--rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/coefficients.h
--rw-r--r--   0        0        0    13187 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h
--rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/integer_maths.h
--rw-r--r--   0        0        0     2875 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/macros.h
--rw-r--r--   0        0        0     1370 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h
--rw-r--r--   0        0        0     2796 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/traits.h
--rw-r--r--   0        0        0    29648 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h
--rw-r--r--   0        0        0     6649 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/hall_set.h
--rw-r--r--   0        0        0     1242 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h
--rw-r--r--   0        0        0     4878 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/index_key.h
--rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/key_range.h
--rw-r--r--   0        0        0     1890 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/lie.h
--rw-r--r--   0        0        0     7253 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/maps.h
--rw-r--r--   0        0        0     6637 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/operators.h
--rw-r--r--   0        0        0     7010 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h
--rw-r--r--   0        0        0     3643 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial.h
--rw-r--r--   0        0        0     4088 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h
--rw-r--r--   0        0        0     2604 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/registry.h
--rw-r--r--   0        0        0    14411 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h
--rw-r--r--   0        0        0    14014 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h
--rw-r--r--   0        0        0     3125 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/tensor_basis.h
--rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h
--rw-r--r--   0        0        0    21879 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector.h
--rw-r--r--   0        0        0     1216 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_base.h
--rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h
--rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp
--rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp
--rw-r--r--   0        0        0     1618 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/lie_multiplier.cpp
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial.cpp
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp
--rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial_ring.cpp
--rw-r--r--   0        0        0      812 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp
--rw-r--r--   0        0        0     6227 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/hall_set.cpp
--rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/monomial.cpp
--rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/polynomial_basis.cpp
--rw-r--r--   0        0        0     2294 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/tensor_basis.cpp
--rw-r--r--   0        0        0     5600 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp
--rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/coefficients/floating_fields.cpp
--rw-r--r--   0        0        0      166 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/coefficients/rational_field.cpp
--rw-r--r--   0        0        0     2895 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/maps.cpp
--rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/CMakeLists.txt
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/common/main.cpp
--rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/CMakeLists.txt
--rw-r--r--   0        0        0     2542 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/hall_basis.cpp
--rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_fixture.h
--rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_multiplier.cpp
--rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/maps/CMakeLists.txt
--rw-r--r--   0        0        0     3200 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps.cpp
--rw-r--r--   0        0        0     4683 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps_fixture.h
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/CMakeLists.txt
--rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp
--rw-r--r--   0        0        0      618 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h
--rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/CMakeLists.txt
--rw-r--r--   0        0        0     9809 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/dense_tensor.cpp
--rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp
--rw-r--r--   0        0        0     2020 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp
--rw-r--r--   0        0        0     9850 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp
--rw-r--r--   0        0        0     2548 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_basis.cpp
--rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_fixture.h
--rw-r--r--   0        0        0     4677 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp
--rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/utilities/CMakeLists.txt
--rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/utilities/packed_integer.cpp
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/vector.cpp
--rw-r--r--   0        0        0      679 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/vcpkg.json
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/.git
--rw-r--r--   0        0        0     2176 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/CMakeLists.txt
--rw-r--r--   0        0        0     1428 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/LICENSE.txt
--rw-r--r--   0        0        0     4666 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/README.md
--rw-r--r--   0        0        0     8441 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/CMakeLists.txt
--rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/BufferConstructor.h
--rw-r--r--   0        0        0     3270 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/Compare.cpp
--rw-r--r--   0        0        0     7934 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp
--rw-r--r--   0        0        0     2313 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h
--rw-r--r--   0        0        0    13604 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/RdToPowers.cpp
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/RdToPowers.h
--rw-r--r--   0        0        0   230430 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/SafeInt3.hpp
--rw-r--r--   0        0        0     1299 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.cpp
--rw-r--r--   0        0        0      931 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.h
--rw-r--r--   0        0        0     9792 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/aligned_allocator.h
--rw-r--r--   0        0        0     6660 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/lapack_defns.h
--rw-r--r--   0        0        0     3027 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/lapack_fortran_definitions.h
--rw-r--r--   0        0        0    14477 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/recombine.cpp
--rw-r--r--   0        0        0     4293 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/recombine.h
--rw-r--r--   0        0        0     7967 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/reweight.h
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/stdafx.h
--rw-r--r--   0        0        0     2538 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/tjlUtilities.h
--rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine.pc.in
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/CMakeLists.txt
--rw-r--r--   0        0        0     4086 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h
--rw-r--r--   0        0        0     1186 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h
--rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp
--rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.h
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/stdafx.h
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/targetver.h
--rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/utils.h
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/set_env_test_recombine.sh
--rw-r--r--   0        0        0     5597 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/test_recombine.cpp
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/test_recombine.h
--rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/CMakeLists.txt
--rw-r--r--   0        0        0     3939 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic.h
--rw-r--r--   0        0        0     4961 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic_interval.h
--rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/interval.h
--rw-r--r--   0        0        0     1394 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/partition.h
--rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/real_interval.h
--rw-r--r--   0        0        0     2131 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/segmentation.h
--rw-r--r--   0        0        0     5705 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic.cpp
--rw-r--r--   0        0        0     8134 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic_interval.cpp
--rw-r--r--   0        0        0     9339 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic_searcher.cpp
--rw-r--r--   0        0        0     3525 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic_searcher.h
--rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/interval.cpp
--rw-r--r--   0        0        0     9360 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/partition.cpp
--rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/real_interval.cpp
--rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/scaled_predicate.cpp
--rw-r--r--   0        0        0     2286 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/scaled_predicate.h
--rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/segmentation.cpp
--rw-r--r--   0        0        0     2322 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_dyadic.cpp
--rw-r--r--   0        0        0    12091 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_dyadic_intervals.cpp
--rw-r--r--   0        0        0     7851 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_partition.cpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_real_interval.cpp
--rw-r--r--   0        0        0     1101 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/CMakeLists.txt
--rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/free_tensor_info.h
--rw-r--r--   0        0        0     6553 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/lie_basis_info.h
--rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/lie_info.h
--rw-r--r--   0        0        0     2650 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/shuffle_tensor_info.h
--rw-r--r--   0        0        0     6925 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/tensor_basis_info.h
--rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/vector_iterator.h
--rw-r--r--   0        0        0     2428 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_helper.h
--rw-r--r--   0        0        0     3263 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_selector.h
--rw-r--r--   0        0        0    23080 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context.h
--rw-r--r--   0        0        0     1780 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/src/la_context.cpp
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/CMakeLists.txt
--rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/configuration.h
--rw-r--r--   0        0        0     1302 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/filesystem.h
--rw-r--r--   0        0        0     9674 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/serialization.h
--rw-r--r--   0        0        0     4130 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/serialization_instantiations.inl
--rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform.h
--rw-r--r--   0        0        0     2022 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/src/configuration.cpp
--rw-r--r--   0        0        0     3411 2022-11-09 12:37:21.000000 roughpy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5427 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/CMakeLists.txt
--rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/__init__.py
--rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/__init__.pyi
--rw-r--r--   0        0        0    19063 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/_roughpy.pyi
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/py.typed
--rw-r--r--   0        0        0     2339 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra.cpp
--rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra.h
--rw-r--r--   0        0        0     2673 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.cpp
--rw-r--r--   0        0        0     1903 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.h
--rw-r--r--   0        0        0     2865 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/basis.cpp
--rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/basis.h
--rw-r--r--   0        0        0    16086 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/context.cpp
--rw-r--r--   0        0        0     2243 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/context.h
--rw-r--r--   0        0        0     6914 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/free_tensor.cpp
--rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/free_tensor.h
--rw-r--r--   0        0        0     3804 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie.cpp
--rw-r--r--   0        0        0     1795 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie.h
--rw-r--r--   0        0        0    13067 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key.cpp
--rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key.h
--rw-r--r--   0        0        0     3581 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.cpp
--rw-r--r--   0        0        0     2250 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.h
--rw-r--r--   0        0        0     1749 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_letter.cpp
--rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_letter.h
--rw-r--r--   0        0        0     8011 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/setup_algebra_type.h
--rw-r--r--   0        0        0     4924 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.cpp
--rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.h
--rw-r--r--   0        0        0     5731 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key.cpp
--rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key.h
--rw-r--r--   0        0        0     3243 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.cpp
--rw-r--r--   0        0        0     2228 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.h
--rw-r--r--   0        0        0     4269 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/convert_timestamp.cpp
--rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/convert_timestamp.h
--rw-r--r--   0        0        0     8155 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.cpp
--rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.h
--rw-r--r--   0        0        0     3178 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.cpp
--rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.h
--rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/numpy.cpp
--rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/numpy.h
--rw-r--r--   0        0        0    14003 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/parse_schema.cpp
--rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/parse_schema.h
--rw-r--r--   0        0        0    10164 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/dlpack.h
--rw-r--r--   0        0        0    11345 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/dlpack_LICENSE
--rw-r--r--   0        0        0     1367 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/date_time_interval.cpp
--rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/date_time_interval.h
--rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic.cpp
--rw-r--r--   0        0        0     1813 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic.h
--rw-r--r--   0        0        0     3976 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.cpp
--rw-r--r--   0        0        0     1849 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.h
--rw-r--r--   0        0        0     4391 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/interval.cpp
--rw-r--r--   0        0        0     2387 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/interval.h
--rw-r--r--   0        0        0     2248 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/intervals.cpp
--rw-r--r--   0        0        0     1825 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/intervals.h
--rw-r--r--   0        0        0     2978 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/partition.cpp
--rw-r--r--   0        0        0     1913 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/partition.h
--rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/real_interval.cpp
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/real_interval.h
--rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/segmentation.cpp
--rw-r--r--   0        0        0     1837 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/segmentation.h
--rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/recombine.cpp
--rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/recombine.h
--rw-r--r--   0        0        0     2234 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/roughpy_module.cpp
--rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/roughpy_module.h
--rw-r--r--   0        0        0    53300 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.cpp
--rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.h
--rw-r--r--   0        0        0    14251 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalar_type.cpp
--rw-r--r--   0        0        0     5932 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalar_type.h
--rw-r--r--   0        0        0    20017 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalars.cpp
--rw-r--r--   0        0        0     3487 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalars.h
--rw-r--r--   0        0        0     3871 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/BaseStream.cpp
--rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/BaseStream.h
--rw-r--r--   0        0        0     3427 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/brownian_stream.cpp
--rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/brownian_stream.h
--rw-r--r--   0        0        0     2768 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/externally_sourced_stream.cpp
--rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/externally_sourced_stream.h
--rw-r--r--   0        0        0     4425 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/function_stream.cpp
--rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/function_stream.h
--rw-r--r--   0        0        0     7325 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.cpp
--rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.h
--rw-r--r--   0        0        0     3510 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.cpp
--rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.h
--rw-r--r--   0        0        0     1270 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/py_schema_context.cpp
--rw-r--r--   0        0        0     2540 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/py_schema_context.h
--rw-r--r--   0        0        0     5107 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.cpp
--rw-r--r--   0        0        0     3919 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.h
--rw-r--r--   0        0        0     6517 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/schema.cpp
--rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/schema.h
--rw-r--r--   0        0        0    23321 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/stream.cpp
--rw-r--r--   0        0        0     2024 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/stream.h
--rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/streams.cpp
--rw-r--r--   0        0        0     1811 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/streams.h
--rw-r--r--   0        0        0    15603 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/tick_stream.cpp
--rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/tick_stream.h
--rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/streams/__init__.py
--rw-r--r--   0        0        0     6198 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/streams/tick_stream.py
--rw-r--r--   0        0        0     3228 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/CMakeLists.txt
--rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/conversion.h
--rw-r--r--   0        0        0     4783 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/key_scalar_array.h
--rw-r--r--   0        0        0     2725 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/owned_scalar_array.h
--rw-r--r--   0        0        0     2776 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/random.h
--rw-r--r--   0        0        0     8620 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar.h
--rw-r--r--   0        0        0     3474 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_array.h
--rw-r--r--   0        0        0     3142 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_blas.h
--rw-r--r--   0        0        0     3004 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_interface.h
--rw-r--r--   0        0        0     4213 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_matrix.h
--rw-r--r--   0        0        0    13459 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_pointer.h
--rw-r--r--   0        0        0     3012 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_stream.h
--rw-r--r--   0        0        0     3109 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_traits.h
--rw-r--r--   0        0        0    16541 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_type.h
--rw-r--r--   0        0        0     6594 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalars_fwd.h
--rw-r--r--   0        0        0     2035 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars.h
--rw-r--r--   0        0        0     1477 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/scalar_blas_defs.h.in
--rw-r--r--   0        0        0    17500 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/RationalType.cpp
--rw-r--r--   0        0        0     5477 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/RationalType.h
--rw-r--r--   0        0        0     2117 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/ScalarTests.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/b_float_16_type.cpp
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/b_float_16_type.h
--rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/bfloat16_random_generator.cpp
--rw-r--r--   0        0        0     6106 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/bfloat16_random_generator.h
--rw-r--r--   0        0        0     1736 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/double_type.cpp
--rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/double_type.h
--rw-r--r--   0        0        0    17637 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_blas.cpp
--rw-r--r--   0        0        0     3803 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_blas.h
--rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_type.cpp
--rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_type.h
--rw-r--r--   0        0        0     1836 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_random_generator.cpp
--rw-r--r--   0        0        0     5999 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_random_generator.h
--rw-r--r--   0        0        0     1790 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_type.cpp
--rw-r--r--   0        0        0     1955 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_type.h
--rw-r--r--   0        0        0     6399 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/key_scalar_array.cpp
--rw-r--r--   0        0        0     4579 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/owned_scalar_array.cpp
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/random_impl.cpp
--rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/random_impl.h
--rw-r--r--   0        0        0    14466 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/rational_poly_scalar_type.cpp
--rw-r--r--   0        0        0     5089 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/rational_poly_scalar_type.h
--rw-r--r--   0        0        0    11521 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar.cpp
--rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_array.cpp
--rw-r--r--   0        0        0     4835 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_blas.cpp
--rw-r--r--   0        0        0     6889 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_blas_impl.h
--rw-r--r--   0        0        0     1942 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_interface.cpp
--rw-r--r--   0        0        0     8248 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_matrix.cpp
--rw-r--r--   0        0        0     5961 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_pointer.cpp
--rw-r--r--   0        0        0     4525 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_stream.cpp
--rw-r--r--   0        0        0    16127 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_type.cpp
--rw-r--r--   0        0        0     1991 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/standard_random_generator.cpp
--rw-r--r--   0        0        0     6903 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/standard_random_generator.h
--rw-r--r--   0        0        0    21578 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/standard_scalar_type.h
--rw-r--r--   0        0        0     2731 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_float_blas.cpp
--rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_key_scalar_array.cpp
--rw-r--r--   0        0        0     2518 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_pcg_standard_random.cpp
--rw-r--r--   0        0        0     6701 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar.cpp
--rw-r--r--   0        0        0     2590 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar_array.cpp
--rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar_matrix.cpp
--rw-r--r--   0        0        0     5404 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar_type.cpp
--rw-r--r--   0        0        0     4201 2022-11-09 12:37:21.000000 roughpy-0.0.4/setup.py
--rw-r--r--   0        0        0     1932 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/CMakeLists.txt
--rw-r--r--   0        0        0     4501 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/brownian_stream.h
--rw-r--r--   0        0        0     9020 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/channels.h
--rw-r--r--   0        0        0     3945 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/dyadic_caching_layer.h
--rw-r--r--   0        0        0     8489 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/dynamically_constructed_stream.h
--rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/external_data_stream.h
--rw-r--r--   0        0        0     3758 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/lie_increment_stream.h
--rw-r--r--   0        0        0     4018 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/piecewise_abelian_stream.h
--rw-r--r--   0        0        0     8084 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/schema.h
--rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/schema_context.h
--rw-r--r--   0        0        0     6232 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/stream.h
--rw-r--r--   0        0        0     7645 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/stream_base.h
--rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/stream_construction_helper.h
--rw-r--r--   0        0        0     6020 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/tick_stream.h
--rw-r--r--   0        0        0     3595 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/brownian_stream.cpp
--rw-r--r--   0        0        0    15358 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/channels.cpp
--rw-r--r--   0        0        0     4949 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/dyadic_caching_layer.cpp
--rw-r--r--   0        0        0    14792 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/dynamically_constructed_stream.cpp
--rw-r--r--   0        0        0     1823 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.cpp
--rw-r--r--   0        0        0     2273 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.h
--rw-r--r--   0        0        0    10976 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.cpp
--rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.h
--rw-r--r--   0        0        0     7343 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_stream.cpp
--rw-r--r--   0        0        0     5126 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/lie_increment_stream.cpp
--rw-r--r--   0        0        0     7701 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/piecewise_abelian_stream.cpp
--rw-r--r--   0        0        0     9413 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/schema.cpp
--rw-r--r--   0        0        0     1981 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/schema_context.cpp
--rw-r--r--   0        0        0    10523 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/stream.cpp
--rw-r--r--   0        0        0     4131 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/stream_base.cpp
--rw-r--r--   0        0        0     4749 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/stream_construction_helper.cpp
--rw-r--r--   0        0        0     3902 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/test_brownian_stream.cpp
--rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/test_lie_increment_stream.cpp
--rw-r--r--   0        0        0     8105 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/test_schema.cpp
--rw-r--r--   0        0        0    10348 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/tick_stream.cpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/__init__.py
--rw-r--r--   0        0        0     3303 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_alg_poly_coeffs.py
--rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_algebra_context.py
--rw-r--r--   0        0        0    11886 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_free_tensor.py
--rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_lie.py
--rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_lie_keys.py
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_tensor_iterator.py
--rw-r--r--   0        0        0     2039 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_tensor_keys.py
--rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/intervals/__init__.py
--rw-r--r--   0        0        0      458 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/intervals/test_dyadic.py
--rw-r--r--   0        0        0     2507 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/intervals/test_intervals.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/scalars/__init__.py
--rw-r--r--   0        0        0     1396 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/scalars/test_monomial.py
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/scalars/test_polynomial.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/__init__.py
--rw-r--r--   0        0        0   187338 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/audio/test.flac
--rw-r--r--   0        0        0    44146 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/audio/test.mp3
--rw-r--r--   0        0        0   311172 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/audio/test.wav
--rw-r--r--   0        0        0     2291 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_brownian_stream.py
--rw-r--r--   0        0        0     4341 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_function_path.py
--rw-r--r--   0        0        0     7804 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_lie_increment_path.py
--rw-r--r--   0        0        0     1482 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_piecewise_lie_path.py
--rw-r--r--   0        0        0     6231 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_schema.py
--rw-r--r--   0        0        0     2397 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_sound_path.py
--rw-r--r--   0        0        0     4142 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_tick_stream.py
--rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/before-all-common.sh
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/arm-uwp.cmake
--rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/arm64-windows.cmake
--rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/common.cmake
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-linux.cmake
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-osx.cmake
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-uwp.cmake
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-windows-static.cmake
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-windows.cmake
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x86-windows.cmake
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra/portfile.cmake
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra/vcpkg.json
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra-lite/portfile.cmake
--rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra-lite/vcpkg.json
--rw-r--r--   0        0        0     4396 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/python-get-binary-obj-path.py
--rw-r--r--   0        0        0     2511 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/version_from_file.py
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.4/vcpkg.json
--rw-r--r--   0        0        0     6248 2022-11-09 12:37:21.000000 roughpy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2345 2022-11-09 12:37:21.000000 roughpy-0.0.5/.clang-format
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 roughpy-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 roughpy-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     3994 2022-11-09 12:37:21.000000 roughpy-0.0.5/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0      931 2022-11-09 12:37:21.000000 roughpy-0.0.5/.github/workflows/manage_version.yml
+-rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 roughpy-0.0.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     5667 2022-11-09 12:37:21.000000 roughpy-0.0.5/.gitignore
+-rw-r--r--   0        0        0      433 2022-11-09 12:37:21.000000 roughpy-0.0.5/.gitmodules
+-rw-r--r--   0        0        0     1720 2022-11-09 12:37:21.000000 roughpy-0.0.5/CHANGELOG
+-rw-r--r--   0        0        0    10822 2022-11-09 12:37:21.000000 roughpy-0.0.5/CMakeLists.txt
+-rw-r--r--   0        0        0     1489 2022-11-09 12:37:21.000000 roughpy-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     4708 2022-11-09 12:37:21.000000 roughpy-0.0.5/README.md
+-rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 roughpy-0.0.5/THANKS.txt
+-rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 roughpy-0.0.5/VERSION.txt
+-rw-r--r--   0        0        0     3508 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/CMakeLists.txt
+-rw-r--r--   0        0        0    16848 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_base.h
+-rw-r--r--   0        0        0    23554 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_base_impl.h
+-rw-r--r--   0        0        0     8100 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_bundle.h
+-rw-r--r--   0        0        0    13572 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h
+-rw-r--r--   0        0        0    26328 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_bundle_impl.h
+-rw-r--r--   0        0        0     2912 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_fwd.h
+-rw-r--r--   0        0        0    31758 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_impl.h
+-rw-r--r--   0        0        0     3829 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_info.h
+-rw-r--r--   0        0        0     7146 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_iterator.h
+-rw-r--r--   0        0        0     3740 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_iterator_impl.h
+-rw-r--r--   0        0        0     9250 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/basis.h
+-rw-r--r--   0        0        0     6672 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/basis_impl.h
+-rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/basis_info.h
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/bundle_info.h
+-rw-r--r--   0        0        0    10237 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/context.h
+-rw-r--r--   0        0        0     4968 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/context_fwd.h
+-rw-r--r--   0        0        0     1881 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/fallback_operations.h
+-rw-r--r--   0        0        0     2707 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/free_tensor.h
+-rw-r--r--   0        0        0     3750 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/free_tensor_fwd.h
+-rw-r--r--   0        0        0     6431 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/free_tensor_impl.h
+-rw-r--r--   0        0        0     2730 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/lie.h
+-rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/lie_basis.h
+-rw-r--r--   0        0        0     1852 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/lie_fwd.h
+-rw-r--r--   0        0        0     2633 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/linear_operator.h
+-rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/shuffle_tensor.h
+-rw-r--r--   0        0        0     1858 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h
+-rw-r--r--   0        0        0     2192 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/include/roughpy/algebra/tensor_basis.h
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/ContextFixture.cpp
+-rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/ContextFixture.h
+-rw-r--r--   0        0        0     3068 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/algebra_base.cpp
+-rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/algebra_iterator.cpp
+-rw-r--r--   0        0        0     1747 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/basis.cpp
+-rw-r--r--   0        0        0    11042 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/context.cpp
+-rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/double_lite_context.cpp
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/float_lite_context.cpp
+-rw-r--r--   0        0        0     4084 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/free_tensor.cpp
+-rw-r--r--   0        0        0     4248 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/hall_set_size.cpp
+-rw-r--r--   0        0        0     2569 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/hall_set_size.h
+-rw-r--r--   0        0        0     3546 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/algebra_type_caster.h
+-rw-r--r--   0        0        0     2301 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/algebra_type_helper.h
+-rw-r--r--   0        0        0     3031 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h
+-rw-r--r--   0        0        0     4222 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/free_tensor_info.h
+-rw-r--r--   0        0        0     6725 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/lie_basis_info.h
+-rw-r--r--   0        0        0     4191 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/lie_info.h
+-rw-r--r--   0        0        0     3099 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/lite_vector_selector.h
+-rw-r--r--   0        0        0     4223 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h
+-rw-r--r--   0        0        0     5982 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h
+-rw-r--r--   0        0        0     2450 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h
+-rw-r--r--   0        0        0     6642 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/tensor_basis_info.h
+-rw-r--r--   0        0        0     7510 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/unspecified_algebra_binary_op.h
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/vector_storage_type.h
+-rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/libalgebra_lite_internal/vector_type_helper.h
+-rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/lie.cpp
+-rw-r--r--   0        0        0     1821 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/lie_basis.cpp
+-rw-r--r--   0        0        0     4732 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/lite_context.cpp
+-rw-r--r--   0        0        0    34854 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/lite_context.h
+-rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/rational_lite_context.cpp
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/rational_poly_lite_context.cpp
+-rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/shuffle_tensor.cpp
+-rw-r--r--   0        0        0     1883 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/tensor_basis.cpp
+-rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/test_lie.cpp
+-rw-r--r--   0        0        0     1631 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/testing/mock_context.cpp
+-rw-r--r--   0        0        0     2139 2022-11-09 12:37:21.000000 roughpy-0.0.5/algebra/src/testing/mock_context.h
+-rw-r--r--   0        0        0   106087 2022-11-09 12:37:21.000000 roughpy-0.0.5/branding/logo/logo_square_white.jpg
+-rw-r--r--   0        0        0      509 2022-11-09 12:37:21.000000 roughpy-0.0.5/cmake/Modules/FindPCGRandom.cmake
+-rw-r--r--   0        0        0    21567 2022-11-09 12:37:21.000000 roughpy-0.0.5/cmake/roughpy_helpers.cmake
+-rw-r--r--   0        0        0      355 2022-11-09 12:37:21.000000 roughpy-0.0.5/cmake/version.py.in
+-rw-r--r--   0        0        0      495 2022-11-09 12:37:21.000000 roughpy-0.0.5/core/CMakeLists.txt
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 roughpy-0.0.5/core/include/roughpy/core/alloc.h
+-rw-r--r--   0        0        0     3627 2022-11-09 12:37:21.000000 roughpy-0.0.5/core/include/roughpy/core/helpers.h
+-rw-r--r--   0        0        0    12443 2022-11-09 12:37:21.000000 roughpy-0.0.5/core/include/roughpy/core/macros.h
+-rw-r--r--   0        0        0     4701 2022-11-09 12:37:21.000000 roughpy-0.0.5/core/include/roughpy/core/slice.h
+-rw-r--r--   0        0        0     5168 2022-11-09 12:37:21.000000 roughpy-0.0.5/core/include/roughpy/core/traits.h
+-rw-r--r--   0        0        0     2628 2022-11-09 12:37:21.000000 roughpy-0.0.5/core/include/roughpy/core/types.h
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/cuda/CMakeLists.txt
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/cuda/CudaDeviceContext.cu
+-rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/cuda/CudaDeviceContext.cuh
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/cuda/scalars/CMakeLists.txt
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/cuda/scalars/src/CUDAFloatType.cu
+-rw-r--r--   0        0        0     2005 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/cuda/scalars/src/CUDAFloatType.cuh
+-rw-r--r--   0        0        0     8615 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/cuda/scalars/src/CUDA_standard_scalar.cuh
+-rw-r--r--   0        0        0      868 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/include/roughpy/device/core.h
+-rw-r--r--   0        0        0    18540 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/include/roughpy/device/device_algebra_base.h
+-rw-r--r--   0        0        0     4377 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/include/roughpy/device/device_context.h
+-rw-r--r--   0        0        0     2348 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/kernels/binary_kernel.cuh
+-rw-r--r--   0        0        0     3972 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/kernels/functors.h
+-rw-r--r--   0        0        0     1712 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/kernels/tmp.cu
+-rw-r--r--   0        0        0     2304 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/kernels/unary_kernel.cuh
+-rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/src/device_algebra_base.cpp
+-rw-r--r--   0        0        0     1728 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/src/device_context.cpp
+-rw-r--r--   0        0        0     2854 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/src/device_free_tensor.cpp
+-rw-r--r--   0        0        0     2912 2022-11-09 12:37:21.000000 roughpy-0.0.5/device/src/device_free_tensor.h
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 roughpy-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 roughpy-0.0.5/docs/source/conf.py
+-rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 roughpy-0.0.5/docs/source/index.rst
+-rw-r--r--   0        0        0     3589 2022-11-09 12:37:21.000000 roughpy-0.0.5/examples/lie_to_tensor_formulae.py
+-rw-r--r--   0        0        0      972 2022-11-09 12:37:21.000000 roughpy-0.0.5/examples/list_basis_keys.py
+-rw-r--r--   0        0        0     1956 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/.clang-format
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/.git
+-rw-r--r--   0        0        0     5992 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/.gitignore
+-rw-r--r--   0        0        0     7502 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/CMakeLists.txt
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/Dockerfile
+-rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/Dockerfile.remote-cpp-env
+-rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/LibalgebraConfig.cmake.in
+-rw-r--r--   0        0        0     2706 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/README.md
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/benchmarks/CMakeLists.txt
+-rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/benchmarks/antipode/CMakeLists.txt
+-rw-r--r--   0        0        0     5078 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/benchmarks/antipode/antipode_bm.cpp
+-rw-r--r--   0        0        0     1941 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/benchmarks/multiplication/CMakeLists.txt
+-rw-r--r--   0        0        0    14501 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp
+-rw-r--r--   0        0        0     2363 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp
+-rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/cmake/Modules/FindBignum.cmake
+-rw-r--r--   0        0        0     3540 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/cmake/Modules/UnitTestPP.cmake
+-rw-r--r--   0        0        0     4012 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake
+-rw-r--r--   0        0        0     1602 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/cmake/libalgebra_test_helper.cmake
+-rw-r--r--   0        0        0    19397 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/_tensor_basis.h
+-rw-r--r--   0        0        0     5123 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/alg_types.h
+-rw-r--r--   0        0        0    33380 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/algebra.h
+-rw-r--r--   0        0        0     4069 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/alternative_multiplications.h
+-rw-r--r--   0        0        0     2188 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/area_tensor_basis.h
+-rw-r--r--   0        0        0    10008 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/area_tensor_multiplication.h
+-rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/base_basis.h
+-rw-r--r--   0        0        0     2597 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/base_vector.h
+-rw-r--r--   0        0        0     3199 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/basis.h
+-rw-r--r--   0        0        0    12660 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/coefficients/gmp_ser.h
+-rw-r--r--   0        0        0     5978 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/coefficients.h
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/complex.h
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/composition_operator.h
+-rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/constlog2.h
+-rw-r--r--   0        0        0     2062 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/constpower.h
+-rw-r--r--   0        0        0    25573 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/dense_storage.h
+-rw-r--r--   0        0        0    32609 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/dense_vector.h
+-rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/caching_tags.h
+-rw-r--r--   0        0        0      957 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/function_extension_cache_base.h
+-rw-r--r--   0        0        0     4041 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/integer_maths.h
+-rw-r--r--   0        0        0     1536 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/level_walkers.h
+-rw-r--r--   0        0        0     3384 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/meta.h
+-rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/order_trait.h
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/platform.h
+-rw-r--r--   0        0        0     3762 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/reversing_permutation.h
+-rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/smallest_int_type.h
+-rw-r--r--   0        0        0     6839 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/dot_product_implementations.h
+-rw-r--r--   0        0        0     2821 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/free_extension.h
+-rw-r--r--   0        0        0     1300 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/functionals.h
+-rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h
+-rw-r--r--   0        0        0    10151 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h
+-rw-r--r--   0        0        0    21060 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/hall_set.h
+-rw-r--r--   0        0        0    40386 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/hybrid_vector.h
+-rw-r--r--   0        0        0     2516 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/implementation_types.h
+-rw-r--r--   0        0        0     3357 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/iterators.h
+-rw-r--r--   0        0        0     4411 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/key_iterators.h
+-rw-r--r--   0        0        0     6680 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/libalgebra.h
+-rw-r--r--   0        0        0     6021 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/lie.h
+-rw-r--r--   0        0        0    17479 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/lie_basis.h
+-rw-r--r--   0        0        0     3788 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/lie_inner_product.h
+-rw-r--r--   0        0        0     7231 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/monomial_basis.h
+-rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/mpfloat_coefficients.h
+-rw-r--r--   0        0        0     1030 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/multi_linear_operators.h
+-rw-r--r--   0        0        0     5988 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/multi_polynomial.h
+-rw-r--r--   0        0        0     1690 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/multiplication_helpers.h
+-rw-r--r--   0        0        0     9196 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/operators.h
+-rw-r--r--   0        0        0     5562 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/poly_basis.h
+-rw-r--r--   0        0        0     6079 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/poly_lie.h
+-rw-r--r--   0        0        0     3447 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/poly_lie_basis.h
+-rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/polynomial_coefficients.h
+-rw-r--r--   0        0        0     6717 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/polynomials.h
+-rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/rational_coefficients.h
+-rw-r--r--   0        0        0     6046 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/reconfigure_operator.h
+-rw-r--r--   0        0        0     8186 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/scalar_bundle.h
+-rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/scalar_multiply_operator.h
+-rw-r--r--   0        0        0    41786 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/sparse_vector.h
+-rw-r--r--   0        0        0      618 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/sum_operator.h
+-rw-r--r--   0        0        0     1472 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/tags.h
+-rw-r--r--   0        0        0   144591 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/tensor.h
+-rw-r--r--   0        0        0    19205 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/tensor_basis.h
+-rw-r--r--   0        0        0     1721 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/tensor_operator.h
+-rw-r--r--   0        0        0    11859 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/utils.h
+-rw-r--r--   0        0        0    24858 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/vector.h
+-rw-r--r--   0        0        0    31254 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/vector_bundle.h
+-rw-r--r--   0        0        0     1306 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/libalgebra/vectors.h
+-rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/README.md
+-rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/CMakeLists.txt
+-rw-r--r--   0        0        0     1872 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/SHOW.h
+-rw-r--r--   0        0        0     2676 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/compat.h
+-rw-r--r--   0        0        0     1058 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/helpers.h
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/memfile.cpp
+-rw-r--r--   0        0        0     3236 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/memfile.h
+-rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/multi_test.h
+-rw-r--r--   0        0        0     1554 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/random_coeffs.h
+-rw-r--r--   0        0        0     2483 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/random_vector_generator.h
+-rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/reporter.cpp
+-rw-r--r--   0        0        0      670 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/reporter.h
+-rw-r--r--   0        0        0     1711 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/rng.h
+-rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/run_tests.cpp
+-rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/simple_basis.h
+-rw-r--r--   0        0        0     2372 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/common/time_and_details.h
+-rw-r--r--   0        0        0     3181 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp
+-rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/CMakeLists.txt
+-rw-r--r--   0        0        0     5679 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/HallSetTests.cpp
+-rw-r--r--   0        0        0     4658 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/LatticePathTests.cpp
+-rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/LibAlgebraUnitTests.cpp
+-rw-r--r--   0        0        0    43337 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm
+-rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp
+-rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/SigHelpers.h
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/TreeBufferHelper.cpp
+-rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/TreeBufferHelper.h
+-rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/alg_framework.h
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/brown_path_increments.h
+-rw-r--r--   0        0        0     2936 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/categorical_path.h
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/log2ceil.h
+-rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/makebm.cpp
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/makebm.h
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/CMakeLists.txt
+-rw-r--r--   0        0        0    17054 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins
+-rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins
+-rw-r--r--   0        0        0     1579 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins
+-rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins
+-rw-r--r--   0        0        0     1224 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h
+-rw-r--r--   0        0        0     2240 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h
+-rw-r--r--   0        0        0     1580 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/run_tests.cpp
+-rw-r--r--   0        0        0    20566 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp
+-rw-r--r--   0        0        0    11406 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp
+-rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/speed_tests.cpp
+-rw-r--r--   0        0        0    12166 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp
+-rw-r--r--   0        0        0     6213 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp
+-rw-r--r--   0        0        0     1590 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/integration_tests/x64sigs.cpp
+-rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/CMakeLists.txt
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/adjoint/CMakeLists.txt
+-rw-r--r--   0        0        0     8834 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp
+-rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt
+-rw-r--r--   0        0        0     2223 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h
+-rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h
+-rw-r--r--   0        0        0      696 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/antipode/CMakeLists.txt
+-rw-r--r--   0        0        0     7994 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/CMakeLists.txt
+-rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h
+-rw-r--r--   0        0        0     3917 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp
+-rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/test_tensor_basis_iteration.cpp
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/CMakeLists.txt
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp
+-rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h
+-rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_double_field.cpp
+-rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_float_field.cpp
+-rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp
+-rw-r--r--   0        0        0      441 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_field.cpp
+-rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp
+-rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_rational_field.cpp
+-rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/half-shuffle-tests/CMakeLists.txt
+-rw-r--r--   0        0        0    19137 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h
+-rw-r--r--   0        0        0     8440 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp
+-rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/hall_set/CMakeLists.txt
+-rw-r--r--   0        0        0     8138 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp
+-rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/CMakeLists.txt
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/run_tests.cpp
+-rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_basis.cpp
+-rw-r--r--   0        0        0     2083 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp
+-rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp
+-rw-r--r--   0        0        0     5505 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp
+-rw-r--r--   0        0        0     1663 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/multipoly/CMakeLists.txt
+-rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/multipoly/test_multipoly_prod.cpp
+-rw-r--r--   0        0        0      387 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/CMakeLists.txt
+-rw-r--r--   0        0        0     2816 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp
+-rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp
+-rw-r--r--   0        0        0     2406 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp
+-rw-r--r--   0        0        0     1548 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp
+-rw-r--r--   0        0        0     1791 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp
+-rw-r--r--   0        0        0     1203 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp
+-rw-r--r--   0        0        0     4353 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp
+-rw-r--r--   0        0        0     2553 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp
+-rw-r--r--   0        0        0     1785 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp
+-rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt
+-rw-r--r--   0        0        0     3057 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp
+-rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/fixture.cpp
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/fixture.h
+-rw-r--r--   0        0        0     4014 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp
+-rw-r--r--   0        0        0     7910 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp
+-rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp
+-rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/temporary_directory.h
+-rw-r--r--   0        0        0     2991 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp
+-rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp
+-rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp
+-rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/CMakeLists.txt
+-rw-r--r--   0        0        0    43877 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp
+-rw-r--r--   0        0        0      753 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt
+-rw-r--r--   0        0        0    20887 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp
+-rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tangents/test_tangents.h
+-rw-r--r--   0        0        0      983 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/run_tests.cpp
+-rw-r--r--   0        0        0     3985 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h
+-rw-r--r--   0        0        0     1797 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h
+-rw-r--r--   0        0        0     4055 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h
+-rw-r--r--   0        0        0     3037 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h
+-rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp
+-rw-r--r--   0        0        0     2509 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp
+-rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp
+-rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp
+-rw-r--r--   0        0        0     5037 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp
+-rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp
+-rw-r--r--   0        0        0     2535 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp
+-rw-r--r--   0        0        0     4900 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp
+-rw-r--r--   0        0        0     3291 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp
+-rw-r--r--   0        0        0    38059 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp
+-rw-r--r--   0        0        0     2419 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/utils/CMakeLists.txt
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/utils/run_tests.cpp
+-rw-r--r--   0        0        0     2678 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/CMakeLists.txt
+-rw-r--r--   0        0        0     3599 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/framework_fixture.h
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/run_tests.cpp
+-rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_dense.cpp
+-rw-r--r--   0        0        0    13508 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp
+-rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp
+-rw-r--r--   0        0        0    12957 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h
+-rw-r--r--   0        0        0    11707 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h
+-rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h
+-rw-r--r--   0        0        0     7086 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h
+-rw-r--r--   0        0        0     1907 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h
+-rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/width1_tests/CMakeLists.txt
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/width1_tests/types.cpp
+-rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/width1_tests/width1.h
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/width1_tests/width1_lie.cpp
+-rw-r--r--   0        0        0     4024 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/.git
+-rw-r--r--   0        0        0     5393 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/CMakeLists.txt
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/README.md
+-rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/cmake/Libalgebra_liteConfig.cmake.in
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/cmake/config.h.in
+-rw-r--r--   0        0        0     2787 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/cmake/lalhelpers.cmake
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/cmake/rationals.h.in
+-rw-r--r--   0        0        0    30639 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/algebra.h
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/basis.h
+-rw-r--r--   0        0        0     3322 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h
+-rw-r--r--   0        0        0    10804 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/coefficients.h
+-rw-r--r--   0        0        0    13257 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h
+-rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/detail/integer_maths.h
+-rw-r--r--   0        0        0     2875 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/detail/macros.h
+-rw-r--r--   0        0        0     1370 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h
+-rw-r--r--   0        0        0     2796 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/detail/traits.h
+-rw-r--r--   0        0        0    36320 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h
+-rw-r--r--   0        0        0     6649 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/hall_set.h
+-rw-r--r--   0        0        0     1242 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h
+-rw-r--r--   0        0        0     4878 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/index_key.h
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/key_range.h
+-rw-r--r--   0        0        0     2100 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/lie.h
+-rw-r--r--   0        0        0     7730 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/maps.h
+-rw-r--r--   0        0        0     6637 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/operators.h
+-rw-r--r--   0        0        0     7010 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h
+-rw-r--r--   0        0        0     4506 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/polynomial.h
+-rw-r--r--   0        0        0     4088 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h
+-rw-r--r--   0        0        0     2604 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/registry.h
+-rw-r--r--   0        0        0    15548 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h
+-rw-r--r--   0        0        0    14627 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h
+-rw-r--r--   0        0        0     3511 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/tensor_basis.h
+-rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h
+-rw-r--r--   0        0        0    22029 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector.h
+-rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector_base.h
+-rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h
+-rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp
+-rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp
+-rw-r--r--   0        0        0     1657 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/algebra/lie_multiplier.cpp
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/algebra/polynomial.cpp
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp
+-rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/algebra/polynomial_ring.cpp
+-rw-r--r--   0        0        0      812 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp
+-rw-r--r--   0        0        0     6259 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/basis/hall_set.cpp
+-rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/basis/monomial.cpp
+-rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/basis/polynomial_basis.cpp
+-rw-r--r--   0        0        0     2294 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/basis/tensor_basis.cpp
+-rw-r--r--   0        0        0     5600 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/coefficients/floating_fields.cpp
+-rw-r--r--   0        0        0      166 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/coefficients/rational_field.cpp
+-rw-r--r--   0        0        0     2895 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/src/maps.cpp
+-rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/CMakeLists.txt
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/common/main.cpp
+-rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/lie/CMakeLists.txt
+-rw-r--r--   0        0        0     2542 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/lie/hall_basis.cpp
+-rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/lie/lie_fixture.h
+-rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/lie/lie_multiplier.cpp
+-rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/maps/CMakeLists.txt
+-rw-r--r--   0        0        0     3200 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/maps/maps.cpp
+-rw-r--r--   0        0        0     4683 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/maps/maps_fixture.h
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/polynomial/CMakeLists.txt
+-rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp
+-rw-r--r--   0        0        0      618 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h
+-rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/CMakeLists.txt
+-rw-r--r--   0        0        0     9809 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/dense_tensor.cpp
+-rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp
+-rw-r--r--   0        0        0     2020 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp
+-rw-r--r--   0        0        0     9850 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp
+-rw-r--r--   0        0        0     2548 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/tensor_basis.cpp
+-rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/tensor_fixture.h
+-rw-r--r--   0        0        0     4677 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp
+-rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/utilities/CMakeLists.txt
+-rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/utilities/packed_integer.cpp
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/tests/vector.cpp
+-rw-r--r--   0        0        0      679 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/libalgebra_lite/vcpkg.json
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/.git
+-rw-r--r--   0        0        0     2176 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/CMakeLists.txt
+-rw-r--r--   0        0        0     1428 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/LICENSE.txt
+-rw-r--r--   0        0        0     4666 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/README.md
+-rw-r--r--   0        0        0     8441 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/CMakeLists.txt
+-rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/BufferConstructor.h
+-rw-r--r--   0        0        0     3270 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/Compare.cpp
+-rw-r--r--   0        0        0     7934 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp
+-rw-r--r--   0        0        0     2313 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h
+-rw-r--r--   0        0        0    13604 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/RdToPowers.cpp
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/RdToPowers.h
+-rw-r--r--   0        0        0   230430 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/SafeInt3.hpp
+-rw-r--r--   0        0        0     1299 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/TreeBufferHelper.cpp
+-rw-r--r--   0        0        0      931 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/TreeBufferHelper.h
+-rw-r--r--   0        0        0     9792 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/aligned_allocator.h
+-rw-r--r--   0        0        0     6660 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/lapack_defns.h
+-rw-r--r--   0        0        0     3027 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/lapack_fortran_definitions.h
+-rw-r--r--   0        0        0    14477 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/recombine.cpp
+-rw-r--r--   0        0        0     4293 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/recombine.h
+-rw-r--r--   0        0        0     7967 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/reweight.h
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/stdafx.h
+-rw-r--r--   0        0        0     2538 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine/tjlUtilities.h
+-rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/recombine/recombine.pc.in
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/CMakeLists.txt
+-rw-r--r--   0        0        0     4086 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h
+-rw-r--r--   0        0        0     1186 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h
+-rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.h
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/TestVec/stdafx.h
+-rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/TestVec/targetver.h
+-rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/TestVec/utils.h
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/set_env_test_recombine.sh
+-rw-r--r--   0        0        0     5597 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/test_recombine.cpp
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 roughpy-0.0.5/external/recombine/test_recombine/test_recombine.h
+-rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/CMakeLists.txt
+-rw-r--r--   0        0        0     3939 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/include/roughpy/intervals/dyadic.h
+-rw-r--r--   0        0        0     4961 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/include/roughpy/intervals/dyadic_interval.h
+-rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/include/roughpy/intervals/interval.h
+-rw-r--r--   0        0        0     1394 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/include/roughpy/intervals/partition.h
+-rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/include/roughpy/intervals/real_interval.h
+-rw-r--r--   0        0        0     2131 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/include/roughpy/intervals/segmentation.h
+-rw-r--r--   0        0        0     5705 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/dyadic.cpp
+-rw-r--r--   0        0        0     8134 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/dyadic_interval.cpp
+-rw-r--r--   0        0        0     9339 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/dyadic_searcher.cpp
+-rw-r--r--   0        0        0     3525 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/dyadic_searcher.h
+-rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/interval.cpp
+-rw-r--r--   0        0        0     9364 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/partition.cpp
+-rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/real_interval.cpp
+-rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/scaled_predicate.cpp
+-rw-r--r--   0        0        0     2286 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/scaled_predicate.h
+-rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/segmentation.cpp
+-rw-r--r--   0        0        0     2322 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/test_dyadic.cpp
+-rw-r--r--   0        0        0    12091 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/test_dyadic_intervals.cpp
+-rw-r--r--   0        0        0     7851 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/test_partition.cpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 roughpy-0.0.5/intervals/src/test_real_interval.cpp
+-rw-r--r--   0        0        0     1101 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/CMakeLists.txt
+-rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/free_tensor_info.h
+-rw-r--r--   0        0        0     6553 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/lie_basis_info.h
+-rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/lie_info.h
+-rw-r--r--   0        0        0     2650 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/shuffle_tensor_info.h
+-rw-r--r--   0        0        0     6925 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/tensor_basis_info.h
+-rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/vector_iterator.h
+-rw-r--r--   0        0        0     2428 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/vector_type_helper.h
+-rw-r--r--   0        0        0     3263 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context/vector_type_selector.h
+-rw-r--r--   0        0        0    23088 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/include/roughpy/la_context.h
+-rw-r--r--   0        0        0     1780 2022-11-09 12:37:21.000000 roughpy-0.0.5/la_context/src/la_context.cpp
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 roughpy-0.0.5/platform/CMakeLists.txt
+-rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 roughpy-0.0.5/platform/include/roughpy/platform/configuration.h
+-rw-r--r--   0        0        0     1302 2022-11-09 12:37:21.000000 roughpy-0.0.5/platform/include/roughpy/platform/filesystem.h
+-rw-r--r--   0        0        0     9674 2022-11-09 12:37:21.000000 roughpy-0.0.5/platform/include/roughpy/platform/serialization.h
+-rw-r--r--   0        0        0     4130 2022-11-09 12:37:21.000000 roughpy-0.0.5/platform/include/roughpy/platform/serialization_instantiations.inl
+-rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 roughpy-0.0.5/platform/include/roughpy/platform.h
+-rw-r--r--   0        0        0     2022 2022-11-09 12:37:21.000000 roughpy-0.0.5/platform/src/configuration.cpp
+-rw-r--r--   0        0        0     3411 2022-11-09 12:37:21.000000 roughpy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5513 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/CMakeLists.txt
+-rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/__init__.py
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/__init__.pyi
+-rw-r--r--   0        0        0    19063 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/_roughpy.pyi
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/py.typed
+-rw-r--r--   0        0        0     2445 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/algebra.cpp
+-rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/algebra.h
+-rw-r--r--   0        0        0     2673 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/algebra_iterator.cpp
+-rw-r--r--   0        0        0     1903 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/algebra_iterator.h
+-rw-r--r--   0        0        0     3233 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/basis.cpp
+-rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/basis.h
+-rw-r--r--   0        0        0    16086 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/context.cpp
+-rw-r--r--   0        0        0     2243 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/context.h
+-rw-r--r--   0        0        0    10173 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/free_multiply_funcs.cpp
+-rw-r--r--   0        0        0      354 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/free_multiply_funcs.h
+-rw-r--r--   0        0        0     6923 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/free_tensor.cpp
+-rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/free_tensor.h
+-rw-r--r--   0        0        0     3812 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie.cpp
+-rw-r--r--   0        0        0     1795 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie.h
+-rw-r--r--   0        0        0    13106 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie_key.cpp
+-rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie_key.h
+-rw-r--r--   0        0        0     3810 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie_key_iterator.cpp
+-rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie_key_iterator.h
+-rw-r--r--   0        0        0     1749 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie_letter.cpp
+-rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/lie_letter.h
+-rw-r--r--   0        0        0     8011 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/setup_algebra_type.h
+-rw-r--r--   0        0        0     4933 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/shuffle_tensor.cpp
+-rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/shuffle_tensor.h
+-rw-r--r--   0        0        0     6896 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/tensor_key.cpp
+-rw-r--r--   0        0        0     3025 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/tensor_key.h
+-rw-r--r--   0        0        0     3270 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/tensor_key_iterator.cpp
+-rw-r--r--   0        0        0     2226 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/algebra/tensor_key_iterator.h
+-rw-r--r--   0        0        0     4283 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/convert_timestamp.cpp
+-rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/convert_timestamp.h
+-rw-r--r--   0        0        0     8160 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/kwargs_to_path_metadata.cpp
+-rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/kwargs_to_path_metadata.h
+-rw-r--r--   0        0        0     3178 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/kwargs_to_vector_construction.cpp
+-rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/kwargs_to_vector_construction.h
+-rw-r--r--   0        0        0     4257 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/numpy.cpp
+-rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/numpy.h
+-rw-r--r--   0        0        0    14061 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/parse_schema.cpp
+-rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/args/parse_schema.h
+-rw-r--r--   0        0        0    10164 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/dlpack.h
+-rw-r--r--   0        0        0    11345 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/dlpack_LICENSE
+-rw-r--r--   0        0        0     1375 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/date_time_interval.cpp
+-rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/date_time_interval.h
+-rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/dyadic.cpp
+-rw-r--r--   0        0        0     1813 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/dyadic.h
+-rw-r--r--   0        0        0     3976 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/dyadic_interval.cpp
+-rw-r--r--   0        0        0     1849 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/dyadic_interval.h
+-rw-r--r--   0        0        0     4391 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/interval.cpp
+-rw-r--r--   0        0        0     2387 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/interval.h
+-rw-r--r--   0        0        0     2248 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/intervals.cpp
+-rw-r--r--   0        0        0     1825 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/intervals.h
+-rw-r--r--   0        0        0     2978 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/partition.cpp
+-rw-r--r--   0        0        0     1913 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/partition.h
+-rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/real_interval.cpp
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/real_interval.h
+-rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/segmentation.cpp
+-rw-r--r--   0        0        0     1837 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/intervals/segmentation.h
+-rw-r--r--   0        0        0     3936 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/recombine.cpp
+-rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/recombine.h
+-rw-r--r--   0        0        0     2234 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/roughpy_module.cpp
+-rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/roughpy_module.h
+-rw-r--r--   0        0        0    53305 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/scalars/r_py_polynomial.cpp
+-rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/scalars/r_py_polynomial.h
+-rw-r--r--   0        0        0    14327 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/scalars/scalar_type.cpp
+-rw-r--r--   0        0        0     5937 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/scalars/scalar_type.h
+-rw-r--r--   0        0        0    20123 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/scalars/scalars.cpp
+-rw-r--r--   0        0        0     3487 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/scalars/scalars.h
+-rw-r--r--   0        0        0     3871 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/BaseStream.cpp
+-rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/BaseStream.h
+-rw-r--r--   0        0        0     3432 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/brownian_stream.cpp
+-rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/brownian_stream.h
+-rw-r--r--   0        0        0     2777 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/externally_sourced_stream.cpp
+-rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/externally_sourced_stream.h
+-rw-r--r--   0        0        0     4425 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/function_stream.cpp
+-rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/function_stream.h
+-rw-r--r--   0        0        0     7352 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/lie_increment_stream.cpp
+-rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/lie_increment_stream.h
+-rw-r--r--   0        0        0     3515 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/piecewise_abelian_stream.cpp
+-rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/piecewise_abelian_stream.h
+-rw-r--r--   0        0        0     1270 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/py_schema_context.cpp
+-rw-r--r--   0        0        0     2540 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/py_schema_context.h
+-rw-r--r--   0        0        0     5117 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/r_py_tick_construction_helper.cpp
+-rw-r--r--   0        0        0     3919 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/r_py_tick_construction_helper.h
+-rw-r--r--   0        0        0     6517 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/schema.cpp
+-rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/schema.h
+-rw-r--r--   0        0        0    23321 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/stream.cpp
+-rw-r--r--   0        0        0     2024 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/stream.h
+-rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/streams.cpp
+-rw-r--r--   0        0        0     1811 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/streams.h
+-rw-r--r--   0        0        0    15715 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/tick_stream.cpp
+-rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/src/streams/tick_stream.h
+-rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/streams/__init__.py
+-rw-r--r--   0        0        0     6198 2022-11-09 12:37:21.000000 roughpy-0.0.5/roughpy/streams/tick_stream.py
+-rw-r--r--   0        0        0     3228 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/CMakeLists.txt
+-rw-r--r--   0        0        0     1006 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/conversion.h
+-rw-r--r--   0        0        0     4783 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/key_scalar_array.h
+-rw-r--r--   0        0        0     2725 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/owned_scalar_array.h
+-rw-r--r--   0        0        0     2776 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/random.h
+-rw-r--r--   0        0        0     8624 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar.h
+-rw-r--r--   0        0        0     3474 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_array.h
+-rw-r--r--   0        0        0     3142 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_blas.h
+-rw-r--r--   0        0        0     3004 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_interface.h
+-rw-r--r--   0        0        0     4213 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_matrix.h
+-rw-r--r--   0        0        0    13463 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_pointer.h
+-rw-r--r--   0        0        0     3012 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_stream.h
+-rw-r--r--   0        0        0     3109 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_traits.h
+-rw-r--r--   0        0        0    16541 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_type.h
+-rw-r--r--   0        0        0     6594 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars/scalars_fwd.h
+-rw-r--r--   0        0        0     2035 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/include/roughpy/scalars.h
+-rw-r--r--   0        0        0     1477 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/scalar_blas_defs.h.in
+-rw-r--r--   0        0        0    17575 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/RationalType.cpp
+-rw-r--r--   0        0        0     5477 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/RationalType.h
+-rw-r--r--   0        0        0     2117 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/ScalarTests.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/b_float_16_type.cpp
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/b_float_16_type.h
+-rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/bfloat16_random_generator.cpp
+-rw-r--r--   0        0        0     6106 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/bfloat16_random_generator.h
+-rw-r--r--   0        0        0     1736 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/double_type.cpp
+-rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/double_type.h
+-rw-r--r--   0        0        0    17673 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/float_blas.cpp
+-rw-r--r--   0        0        0     3803 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/float_blas.h
+-rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/float_type.cpp
+-rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/float_type.h
+-rw-r--r--   0        0        0     1836 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/half_random_generator.cpp
+-rw-r--r--   0        0        0     5999 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/half_random_generator.h
+-rw-r--r--   0        0        0     1790 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/half_type.cpp
+-rw-r--r--   0        0        0     1955 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/half_type.h
+-rw-r--r--   0        0        0     6404 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/key_scalar_array.cpp
+-rw-r--r--   0        0        0     4589 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/owned_scalar_array.cpp
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/random_impl.cpp
+-rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/random_impl.h
+-rw-r--r--   0        0        0    14531 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/rational_poly_scalar_type.cpp
+-rw-r--r--   0        0        0     5089 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/rational_poly_scalar_type.h
+-rw-r--r--   0        0        0    11559 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar.cpp
+-rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_array.cpp
+-rw-r--r--   0        0        0     4835 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_blas.cpp
+-rw-r--r--   0        0        0     6889 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_blas_impl.h
+-rw-r--r--   0        0        0     1942 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_interface.cpp
+-rw-r--r--   0        0        0     8253 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_matrix.cpp
+-rw-r--r--   0        0        0     5969 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_pointer.cpp
+-rw-r--r--   0        0        0     4535 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_stream.cpp
+-rw-r--r--   0        0        0    16192 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/scalar_type.cpp
+-rw-r--r--   0        0        0     1991 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/standard_random_generator.cpp
+-rw-r--r--   0        0        0     6907 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/standard_random_generator.h
+-rw-r--r--   0        0        0    21652 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/standard_scalar_type.h
+-rw-r--r--   0        0        0     2731 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/test_float_blas.cpp
+-rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/test_key_scalar_array.cpp
+-rw-r--r--   0        0        0     2518 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/test_pcg_standard_random.cpp
+-rw-r--r--   0        0        0     6701 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/test_scalar.cpp
+-rw-r--r--   0        0        0     2590 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/test_scalar_array.cpp
+-rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/test_scalar_matrix.cpp
+-rw-r--r--   0        0        0     5404 2022-11-09 12:37:21.000000 roughpy-0.0.5/scalars/src/test_scalar_type.cpp
+-rw-r--r--   0        0        0     4201 2022-11-09 12:37:21.000000 roughpy-0.0.5/setup.py
+-rw-r--r--   0        0        0     1932 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/CMakeLists.txt
+-rw-r--r--   0        0        0     4501 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/brownian_stream.h
+-rw-r--r--   0        0        0     9020 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/channels.h
+-rw-r--r--   0        0        0     3945 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/dyadic_caching_layer.h
+-rw-r--r--   0        0        0     8489 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/dynamically_constructed_stream.h
+-rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/external_data_stream.h
+-rw-r--r--   0        0        0     3758 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/lie_increment_stream.h
+-rw-r--r--   0        0        0     4018 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/piecewise_abelian_stream.h
+-rw-r--r--   0        0        0     8252 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/schema.h
+-rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/schema_context.h
+-rw-r--r--   0        0        0     6232 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/stream.h
+-rw-r--r--   0        0        0     7645 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/stream_base.h
+-rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/stream_construction_helper.h
+-rw-r--r--   0        0        0     6020 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/include/roughpy/streams/tick_stream.h
+-rw-r--r--   0        0        0     3595 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/brownian_stream.cpp
+-rw-r--r--   0        0        0    15374 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/channels.cpp
+-rw-r--r--   0        0        0     4949 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/dyadic_caching_layer.cpp
+-rw-r--r--   0        0        0    14792 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/dynamically_constructed_stream.cpp
+-rw-r--r--   0        0        0     1823 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/external_data_sources/csv_data_source.cpp
+-rw-r--r--   0        0        0     2273 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/external_data_sources/csv_data_source.h
+-rw-r--r--   0        0        0    10989 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/external_data_sources/sound_file_data_source.cpp
+-rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/external_data_sources/sound_file_data_source.h
+-rw-r--r--   0        0        0     7343 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/external_data_stream.cpp
+-rw-r--r--   0        0        0     5126 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/lie_increment_stream.cpp
+-rw-r--r--   0        0        0     7701 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/piecewise_abelian_stream.cpp
+-rw-r--r--   0        0        0     9463 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/schema.cpp
+-rw-r--r--   0        0        0     1981 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/schema_context.cpp
+-rw-r--r--   0        0        0    10528 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/stream.cpp
+-rw-r--r--   0        0        0     4131 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/stream_base.cpp
+-rw-r--r--   0        0        0     4749 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/stream_construction_helper.cpp
+-rw-r--r--   0        0        0     3902 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/test_brownian_stream.cpp
+-rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/test_lie_increment_stream.cpp
+-rw-r--r--   0        0        0     8105 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/test_schema.cpp
+-rw-r--r--   0        0        0    10348 2022-11-09 12:37:21.000000 roughpy-0.0.5/streams/src/tick_stream.cpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/__init__.py
+-rw-r--r--   0        0        0     3303 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_alg_poly_coeffs.py
+-rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_algebra_context.py
+-rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_free_multiply_functions.py
+-rw-r--r--   0        0        0    11886 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_free_tensor.py
+-rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_lie.py
+-rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_lie_basis.py
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_lie_keys.py
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_tensor_iterator.py
+-rw-r--r--   0        0        0     2039 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/algebra/test_tensor_keys.py
+-rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/intervals/__init__.py
+-rw-r--r--   0        0        0      458 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/intervals/test_dyadic.py
+-rw-r--r--   0        0        0     2507 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/intervals/test_intervals.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/scalars/__init__.py
+-rw-r--r--   0        0        0     1396 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/scalars/test_monomial.py
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/scalars/test_polynomial.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/__init__.py
+-rw-r--r--   0        0        0   187338 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/audio/test.flac
+-rw-r--r--   0        0        0    44146 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/audio/test.mp3
+-rw-r--r--   0        0        0   311172 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/audio/test.wav
+-rw-r--r--   0        0        0     2291 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/test_brownian_stream.py
+-rw-r--r--   0        0        0     4341 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/test_function_path.py
+-rw-r--r--   0        0        0     7804 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/test_lie_increment_path.py
+-rw-r--r--   0        0        0     1482 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/test_piecewise_lie_path.py
+-rw-r--r--   0        0        0     6231 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/test_schema.py
+-rw-r--r--   0        0        0     2397 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/test_sound_path.py
+-rw-r--r--   0        0        0     4142 2022-11-09 12:37:21.000000 roughpy-0.0.5/tests/streams/test_tick_stream.py
+-rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/before-all-common.sh
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/arm-uwp.cmake
+-rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/arm64-windows.cmake
+-rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/common.cmake
+-rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/x64-linux.cmake
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/x64-osx.cmake
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/x64-uwp.cmake
+-rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/x64-windows-static.cmake
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/x64-windows.cmake
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ci/triplets/x86-windows.cmake
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ports/libalgebra/portfile.cmake
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ports/libalgebra/vcpkg.json
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ports/libalgebra-lite/portfile.cmake
+-rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/ports/libalgebra-lite/vcpkg.json
+-rw-r--r--   0        0        0     4396 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/python-get-binary-obj-path.py
+-rw-r--r--   0        0        0     2511 2022-11-09 12:37:21.000000 roughpy-0.0.5/tools/version_from_file.py
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.5/vcpkg.json
+-rw-r--r--   0        0        0     7305 2022-11-09 12:37:21.000000 roughpy-0.0.5/PKG-INFO
```

### Comparing `roughpy-0.0.4/.clang-format` & `roughpy-0.0.5/.clang-format`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `roughpy-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `roughpy-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/.github/workflows/build_wheels.yml` & `roughpy-0.0.5/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/.github/workflows/manage_version.yml` & `roughpy-0.0.5/.github/workflows/manage_version.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 name: Manage version file
 
 
 on:
   pull_request:
     branches:
-      - release/v[0-9]+.[0-9]+.[0-9]+**
+      - main
     types:
       - opened
 
 
 
 jobs:
   update_version:
     runs-on: ubuntu-latest
-    if: github.base_ref == 'refs/heads/main'
+    if: startsWith(github.ref_name, 'refs/heads/main')
     steps:
       - uses: actions/checkout@v3
       - name: Write version file
         shell: bash
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
```

### Comparing `roughpy-0.0.4/.github/workflows/tests.yml` & `roughpy-0.0.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/.gitignore` & `roughpy-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/CHANGELOG` & `roughpy-0.0.5/CHANGELOG`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Version 0.0.5:
+  - Added free functions for performing free-tensor, shuffle, half-shuffle
+  multiplication between pairs of tensors (of either kind).
+  - Added free function for applying the adjoint of left free tensor
+  multiplication to arbitrary tensors.
+  - Improved exception usage, messages now include filename, lineno, and
+  function name to help locate c++ exceptions passed through to Python.
+  - Basis objects in Python are now iterable.
+  - Added `split_n` and `to_index` methods to Tensor key.
+
 Version 0.0.4:
   - Overhauled the RPY_CHECK macro so it now gives much better contextual
   information.
   - Readme updated to reflect PyPI installation with wheels.
   - Antipode is now implemented in libalgebra_lite, and exposed to Python for
   Free tensors.
   - Streams now carry a support interval, outside of which the signature will be
```

### Comparing `roughpy-0.0.4/CMakeLists.txt` & `roughpy-0.0.5/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cmake_minimum_required(VERSION 3.21)
+cmake_minimum_required(VERSION 3.22)
 
 message(STATUS "Toolchain file: ${CMAKE_TOOLCHAIN_FILE}")
 list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_LIST_DIR}/cmake/Modules)
 #list(APPEND VCPKG_INSTALL_OPTIONS "--no-print-usage")
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
 if (EXISTS "VERSION.txt")
@@ -11,122 +11,134 @@
     string(REGEX MATCH "[0-9]+\\.[0-9]+\\.[0-9]+" _rpy_version "${_rpy_version}")
 else ()
     set(_rpy_version 0.0.1)
 endif ()
 
 project(RoughPy VERSION ${_rpy_version})
 
-set_property(GLOBAL PROPERTY USE_FOLDERS ON)
-
-set(CMAKE_INSTALL_LIBDIR "roughpy" CACHE STRING "install library dir")
-set(CMAKE_INSTALL_BINDIR "roughpy" CACHE STRING "install binary dir")
-
-set(CMAKE_CXX_STANDARD 17)
-set(CMAKE_CXX_STANDARD_REQUIRED ON)
-if (LINUX)
-    set(CMAKE_INSTALL_RPATH "$ORIGIN")
-elseif (APPLE)
-    execute_process(COMMAND "brew" "--prefix"
-            RESULT_VARIABLE _brew_prefix_found
-            OUTPUT_VARIABLE _brew_prefix
-            OUTPUT_STRIP_TRAILING_WHITESPACE
-            )
-    message(STATUS "Adding brew prefix: ${_brew_prefix}")
-    if (_brew_prefix_found)
-        list(APPEND CMAKE_PREFIX_PATH "${_brew_prefix}")
-    endif ()
-
-
-    #    set(CMAKE_BUILD_WITH_INSTALL_RPATH ON)
-    set(CMAKE_MACOSX_RPATH ON)
-    #    set(CMAKE_INSTALL_RPATH_USE_LINK_PATH ON)
-    #    set(CMAKE_INSTALL_RPATH @loader_path)
-    #    set(CMAKE_INSTALL_NAME_DIR @rpath)
-endif ()
+include(CMakeDependentOption)
 
 option(ROUGHPY_BUILD_LA_CONTEXTS "Build the collection of libalgebra contexts" OFF)
 option(ROUGHPY_BUILD_TESTS "Build C++ tests for RoughPy" ON)
 option(ROUGHPY_BUILD_PYMODULE_INPLACE "Buildg the pymodule in the project roughpy directory" OFF)
+option(ROUGHPY_LINK_NUMPY "Link with Numpy library for array handling" ON)
+option(ROUGHPY_GENERATE_DEVICE_CODE "Generate code for objects on devices" OFF)
+cmake_dependent_option(ROUGHPY_PREFER_ACCELERATE
+        "Prefer Accelerate framework on MacOS always" OFF APPLE OFF)
 
-if (MSVC)
-    #    add_compile_options(/permissive-)
-endif ()
-
-find_package(GTest CONFIG QUIET)
-if (ROUGHPY_BUILD_TESTS AND GTest_FOUND)
+# If testing is enabled, find GTest to make sure the tests can be
+# successfully built.
+if (ROUGHPY_BUILD_TESTS)
     find_package(GTest CONFIG REQUIRED)
 
     if (NOT TARGET GTest::gtest)
         message(FATAL_ERROR "GTest::gtest target not defined")
     endif ()
 
     enable_testing()
-else ()
-    set(ROUGHPY_BUILD_TESTS OFF CACHE INTERNAL "")
-endif ()
 
-include(cmake/roughpy_helpers.cmake)
+    # If we are building roughpy tests and gtest is available then we also
+    # to build the libalgebra_lite tests.
+    set(LIBALGEBRA_LITE_BUILD_TESTS ON CACHE INTERNAL "")
+endif ()
+
+# If we're building with SKBUILD, we need to define install locations for
+# all the components using their special directory variables. Otherwise,
+# use the GNUInstall dirs
+if (SKBUILD)
+
+    # This is all the variables set by GNUInstallDirs, minus LIBDIR and BINDIR
+    set(_ignore_dirs
+            SBINDIR
+            LIBEXECDIR
+            SYSCONFIGDIR
+            SHAREDSTATEDIR
+            LOCALSTATEDIR
+            RUNSTATEDIR
+            INCLUDEDIR
+            OLDINCLUDEDIR
+            DATAROOTDIR
+            DATADIR
+            INFODIR
+            LOCALEDIR
+            MANDIR
+            DOCDIR
+            )
 
+    if (WIN32)
+        # On Windows, DLLs are put in BINDIR
+        list(APPEND _ignore_dirs LIBDIR)
+        set(CMAKE_INSTALL_BINDIR ${SKBUILD_PLATLIB_DIR}/roughpy CACHE STRING
+                "Overwritten install for BINDIR")
+    else()
+        # On not Windows, Shared Objects go in LIBDIR
+        list(APPEND _ignore_dirs BINDIR)
+        set(CMAKE_INSTALL_LIBDIR ${SKBUILD_PLATLIB_DIR}/roughpy CACHE STRING
+                "Overwritten install for LIBDIR")
+
+        list(APPEND _ignore_dirs BINDIR)
+    endif()
+
+    foreach(_dir ${_ignore_dirs})
+        set(CMAKE_INSTALL_${_dir} ${SKBUILD_NULL_DIR} CACHE STRING
+                "Overwritten install for ${_dir}")
+    endforeach()
+
+else()
+    include(GNUInstallDirs)
+endif()
 
-option(ROUGHPY_LINK_NUMPY "Link with Numpy library for array handling" ON)
-option(ROUGHPY_GENERATE_DEVICE_CODE "Generate code for objects on devices" OFF)
 
+# Load the helper functions
+include(cmake/roughpy_helpers.cmake)
 
+# We need to provide some help to make sure we find the correct version of
+# Python. Ideally, if we're using Scikit-Build-Core to build the library (via
+# pip) and the Python executable is provided via the PYTHON_EXECUTABLE cache
+# variable. In this case, make sure that this is the version of Python that gets
+# found.
 set(PYBIND11_FINDPYTHON ON)
 if (NOT PYTHON_FOUND AND SKBUILD)
     cmake_path(GET PYTHON_EXECUTABLE PARENT_PATH _sk_env_dir)
     message(STATUS "SKBuild environment: ${_sk_env_dir}")
 
     # Some variables that are set might cause issues in the FindPython module,
     # so unset those
     unset(Python_LIBRARY CACHE)
     unset(PYTHON_LIBRARY CACHE)
     unset(Python3_LIBRARY CACHE)
 
     # clean up temporary
     unset(_sk_env_dir)
 else ()
+    # If we're not using Scikit-Build-Core (i.e. a pure CMake build) then try
+    # looking for a Python virtual environment first.
     set(Python_FIND_VIRTUALENV FIRST)
+
+    # In particular, if ENV{VIRTUAL_ENV} is set then add this to the cmake
+    # prefix path so FindPython is more likely to find this environemnt.
+    if (DEFINED ENV{VIRTUAL_ENV})
+        # Put venv/lib on the prefix path so we can find
+        # a pip installed MKL
+        message(STATUS "Adding python virtual environment to path")
+        list(PREPEND CMAKE_PREFIX_PATH "$ENV{VIRTUAL_ENV}")
+    endif ()
 endif ()
 
+
+# At minimum we need Interpreter and Development.Module in order to build a
+# Python extension module.
+set(PYTHON_COMPONENTS_NEEDED Interpreter Development.Module)
 if (ROUGHPY_LINK_NUMPY)
-    find_package(Python 3.8 REQUIRED COMPONENTS Interpreter Development.Module NumPy)
-else ()
-    find_package(Python 3.8 REQUIRED COMPONENTS Interpreter Development.Module)
+    list(APPEND PYTHON_COMPONENTS_NEEDED NumPy)
 endif ()
 
-if (DEFINED ENV{VIRTUAL_ENV})
-    # Put venv/lib on the prefix path so we can find
-    # a pip installed MKL
-    message(STATUS "Adding python virtual environment to path")
-    list(PREPEND CMAKE_PREFIX_PATH "$ENV{VIRTUAL_ENV}/lib")
-endif ()
-
-# Before we get too far, let's make use of Python's import
-# system to make sure MKL can be found if it was pip installed
-execute_process(COMMAND ${Python_EXECUTABLE}
-        "${CMAKE_CURRENT_LIST_DIR}/tools/python-get-binary-obj-path.py"
-        "--directory" "mkl-devel" "cmake/mkl/MKLConfig.cmake"
-        RESULT_VARIABLE _python_mkl_dir_found
-        OUTPUT_VARIABLE _python_mkl_dir
-        OUTPUT_STRIP_TRAILING_WHITESPACE
-        ERROR_QUIET
-        )
-
-if (NOT _python_mkl_dir_found AND EXISTS "${_python_mkl_dir}")
-    cmake_path(GET _python_mkl_dir PARENT_PATH _python_mkl_dir)
-    message(STATUS "Adding MKL dir from pip-installed mkl: ${_python_mkl_dir}")
-    list(APPEND CMAKE_PREFIX_PATH "${_python_mkl_dir}")
-    if (NOT MKL_ROOT)
-        set(MKL_ROOT "${_python_mkl_dir}")
-    endif ()
-    set(MKL_DIR "${_python_mkl_dir}")
+find_package(Python 3.8 REQUIRED COMPONENTS ${PYTHON_COMPONENTS_NEEDED})
 
 
-endif ()
 
 if (NOT DEFINED pybind11_ROOT)
     execute_process(COMMAND
             "${Python_EXECUTABLE}" "-m" "pybind11" "--cmakedir"
             COMMAND_ECHO STDOUT
             RESULT_VARIABLE _python_pybind11_dir_found
             OUTPUT_VARIABLE _python_pybind11_dir
@@ -149,15 +161,43 @@
 find_package(Eigen3 CONFIG REQUIRED)
 find_package(SndFile CONFIG REQUIRED)
 
 # This package is c++17 so cannot be used if changing to a lower standard
 find_package(tomlplusplus CONFIG REQUIRED)
 
 message(STATUS "Target architecture ${RPY_ARCH}")
-if (RPY_ARCH MATCHES "[xX](86(_64)?|64)|[aA][mM][dD]64")
+if (RPY_ARCH MATCHES "[xX](86(_64)?|64)|[aA][mM][dD]64" AND NOT
+        ROUGHPY_PREFER_ACCELERATE)
+
+    # If we're looking for MKL then we might have installed it via pip.
+    # To make sure we can find this, let's use Python's importlib metadata to
+    # locate the directory containing MKLConfig.cmake and add the relevant
+    # directory to the prefix path.
+    execute_process(COMMAND ${Python_EXECUTABLE}
+            "${CMAKE_CURRENT_LIST_DIR}/tools/python-get-binary-obj-path.py"
+            "--directory" "mkl-devel" "cmake/mkl/MKLConfig.cmake"
+            RESULT_VARIABLE _python_mkl_dir_found
+            OUTPUT_VARIABLE _python_mkl_dir
+            OUTPUT_STRIP_TRAILING_WHITESPACE
+            ERROR_QUIET
+            )
+    if (NOT _python_mkl_dir_found AND EXISTS "${_python_mkl_dir}")
+        cmake_path(GET _python_mkl_dir PARENT_PATH _python_mkl_dir)
+        message(STATUS "Adding MKL dir from pip-installed mkl: ${_python_mkl_dir}")
+        list(APPEND CMAKE_PREFIX_PATH "${_python_mkl_dir}")
+        if (NOT MKL_ROOT)
+            set(MKL_ROOT "${_python_mkl_dir}")
+        endif ()
+        set(MKL_DIR "${_python_mkl_dir}")
+    endif ()
+
+    # Set the variables that determine the actual MKL library that we need to
+    # link. At the moment, we force 32-bit addressing on both 32- and 64-bit
+    # platforms, statically linked, and using the Intel OMP library (except on
+    # Windows).
     if (RPY_ARCH STREQUAL "x86")
         set(MKL_ARCH ia32)
     else ()
         set(MKL_ARCH intel64)
         set(MKL_INTERFACE lp64)
     endif ()
 
@@ -171,26 +211,21 @@
     endif ()
 
     find_package(MKL CONFIG)
     if (TARGET MKL::MKL)
         add_library(BLAS::BLAS ALIAS MKL::MKL)
         add_library(LAPACK::LAPACK ALIAS MKL::MKL)
 
-        #        if (DEFINED MKL_OMP_LIB AND MKL_OMP_LIB)
-        #            foreach (LANG IN ITEMS C CXX)
-        #                set(OpenMP_${LANG}_LIB_NAMES ${MKL_OMP_LIB} CACHE STRING "Intel OpenMP runtime library")
-        #            endforeach ()
-        #        endif ()
         if (DEFINED MKL_OMP_LIB AND MKL_OMP_LIB)
-            foreach (LANG IN ITEMS C CXX)
-                if (APPLE)
+            if (APPLE)
+                foreach (LANG IN ITEMS C CXX)
                     set(OpenMP_${LANG}_FLAGS "-XPreprocessor -fopenmp=${MKL_OMP_LIB}")
                     set(OpenMP_${LANG}_LIB_NAMES "${MKL_OMP_LIB}" CACHE STRING "libomp location for OpenMP")
-                endif ()
-            endforeach ()
+                endforeach ()
+            endif ()
             set(OpenMP_${MKL_OMP_LIB}_LIBRARY "${MKL_THREAD_LIB}")
         endif ()
     else ()
         set(BLA_SIZEOF_INTEGER 4)
         set(BLA_STATIC ON)
     endif ()
 elseif (APPLE)
@@ -202,73 +237,66 @@
 if (NOT TARGET BLAS::BLAS)
     find_package(BLAS REQUIRED)
 endif ()
 if (NOT TARGET LAPACK::LAPACK)
     find_package(LAPACK REQUIRED)
 endif ()
 
+if (APPLE AND NOT DEFINED MKL_OMP_LIB)
+    get_brew_prefix(_libomp_prefix libomp VERBOSE)
+
+    if (_libomp_prefix AND EXISTS ${_libomp_prefix})
+        list(APPEND CMAKE_PREFIX_PATH ${_libomp_prefix})
+    endif()
+endif()
+
 find_package(OpenMP REQUIRED COMPONENTS CXX)
 
 find_package(pybind11 REQUIRED)
 find_package(cereal REQUIRED)
 find_package(PCGRandom REQUIRED)
 
+# Now we get to adding our components. Let's do some global setup such as
+# setting the CXX standard and the shared library details.
+set(CMAKE_CXX_STANDARD 17)
+set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
-add_subdirectory(external/libalgebra_lite)
-#set_target_properties(Libalgebra_lite PROPERTIES NO_SONAME ON)
-
-#add_subdirectory(external/pybind11)
+if (LINUX)
+    set(CMAKE_INSTALL_RPATH "$ORIGIN")
+elseif (APPLE)
+    set(CMAKE_MACOSX_RPATH ON)
+endif ()
 
+add_subdirectory(external/libalgebra_lite)
 
-# Make an imported target for PCG-CPP because it is a
-# makefile based project
-#if(NOT TARGET PCGRandom::pcg_random)
-#    add_library(PCGRandom::pcg_random IMPORTED INTERFACE)
-#    target_include_directories(PCGRandom::pcg_random INTERFACE
-#            external/pcg-cpp/include)
-#endif()
-
-
-#add_subdirectory(external/recombine)
-
-set(LIBALGEBRA_NO_SERIALIZATION ON CACHE INTERNAL "")
-add_subdirectory(external/libalgebra)
-
-#add_subdirectory(external/csv-parser)
-# The csv-parser CMakeLists.txt leaves much to be desired
-# Let's fix some of the problems now
-#if(NOT TARGET csv::csv)
-#    add_library(csv::csv ALIAS csv)
-#    target_include_directories(csv INTERFACE
-#            external/csv-parser/include)
-#    set_target_properties(csv PROPERTIES POSITION_INDEPENDENT_CODE ON)
-#endif()
-
-#set(BUILD_DOC OFF CACHE INTERNAL "disable cereal docs")
-#set(BUILD_SANDBOX OFF CACHE INTERNAL "disable cereal sandbox examples")
-#set(SKIP_PERFORMANCE_COMPARISON ON CACHE INTERNAL "disable building cereal performance tests")
-#add_subdirectory(external/cereal)
 
 add_subdirectory(core)
 add_subdirectory(platform)
 add_subdirectory(scalars)
 add_subdirectory(intervals)
 add_subdirectory(algebra)
 add_subdirectory(streams)
 add_subdirectory(roughpy)
 
 if (ROUGHPY_GENERATE_DEVICE_CODE)
     add_subdirectory(device)
 endif ()
 
 if (ROUGHPY_BUILD_LA_CONTEXTS)
+    set(LIBALGEBRA_NO_SERIALIZATION ON CACHE INTERNAL "")
+    add_subdirectory(external/libalgebra)
     add_subdirectory(la_context)
 endif ()
 
 
+# TODO: Maybe we should replace this with a custom install target rather than
+# messing with the install directories.
+#set(CMAKE_INSTALL_LIBDIR "roughpy" CACHE STRING "install library dir")
+#set(CMAKE_INSTALL_BINDIR "roughpy" CACHE STRING "install binary dir")
+
 install(TARGETS
         RoughPy_PyModule
         EXPORT RoughPy_EXPORTS
         RUNTIME DESTINATION roughpy
         LIBRARY
         DESTINATION roughpy
         NAMELINK_SKIP
@@ -293,21 +321,7 @@
     get_target_property(_lib_deps ${_rpy_lib} RUNTIME_DEPENDENCIES)
     if (_lib_deps)
         list(APPEND _runtime_deps "${_lib_deps}")
         #        install(FILES ${_lib_deps} DESTINATION roughpy)
     endif ()
 endforeach ()
 install(FILES ${_runtime_deps} DESTINATION roughpy)
-
-#
-#install(EXPORT RoughPy_EXPORTS
-#        DESTINATION roughpy
-#        NAMESPACE RoughPy
-#        FILE RoughPy.cmake
-#            COMPONENT Development
-#            EXCLUDE_FROM_ALL
-#        )
-#
-#
-#if (TARGET MKL::MKL AND DEFINED MKL_THREAD_LIB)
-#    install(FILES ${MKL_THREAD_LIB} DESTINATION roughpy)
-#endif ()
```

### Comparing `roughpy-0.0.4/LICENSE.txt` & `roughpy-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/README.md` & `roughpy-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-![RoughPy Logo](branding/logo/logo_square_white.jpg)
+<center>
+  <img src="https://raw.githubusercontent.com/datasig-ac-uk/RoughPy/main/branding/logo/logo_square_white.jpg">
+</center><br>
+
 # RoughPy
 RoughPy is a package for working with streaming data as rough paths, and working with algebraic objects such as free tensors, shuffle tensors, and elements of the free Lie algebra.
 
 This library is currently in an alpha stage, and as such many features are still incomplete or not fully implemented. Please bear this in mind when looking at the source code.
 
 
 ## Installation
@@ -20,17 +23,26 @@
 You will need to make sure that vcpkg is available on your system before attempting to build RoughPy.
 The following commands should be sufficient to set up the environment for building RoughPy:
 ```bash
 git clone https://github.com/Microsoft/vcpkg.git tools/vcpkg
 tools/vcpkg/bootstrap-vcpkg.sh
 export CMAKE_TOOLCHAIN_FILE=$(pwd)/tools/vcpkg/scripts/buildsystems/vcpkg.cmake
 ```
-With this environment variable set, you should now be able to pip install either using the PyPI source distribution (using the `--no-binary :all:` flag), or directly from GitHub:
+With this environment variable set, most of the dependencies will be installed automatically during the build process.
+
+On MacOS with Apple Silicon you will need to install libomp (for example using Homebrew `brew install libomp`).
+This is not necessary on Intel based MacOS where the Intel iomp5 can be used instead. 
+The build system will use `brew --prefix libomp` to try to locate this library.
+(The actual `brew` executable can be customised by setting the `ROUGHPY_BREW_EXECUTABLE` CMake variable 
+or environment variable.)
+
+You should now be able to pip install either using the PyPI source distribution (using the `--no-binary :roughpy:` 
+flag), or directly from GitHub (recommended):
 ```bash
-pip install https://github.com/datasig-ac-uk/RoughPy.git
+pip install git+https://github.com/datasig-ac-uk/RoughPy.git
 ```
 It will take some time to build.
 
 ## Usage
 Following the NumPy (and related) convention, we import RoughPy under the alias `rp` as follows:
 ```python
 import roughpy as rp
```

### Comparing `roughpy-0.0.4/THANKS.txt` & `roughpy-0.0.5/THANKS.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/CMakeLists.txt` & `roughpy-0.0.5/algebra/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,23 +26,27 @@
         src/algebra_iterator.cpp
         src/lite_context.cpp
         src/lite_context.h
         src/float_lite_context.cpp
         src/double_lite_context.cpp
         src/rational_lite_context.cpp
         src/rational_poly_lite_context.cpp
+        src/libalgebra_lite_internal/algebra_type_caster.h
+        src/libalgebra_lite_internal/algebra_type_helper.h
         src/libalgebra_lite_internal/dense_vector_iterator.h
         src/libalgebra_lite_internal/free_tensor_info.h
         src/libalgebra_lite_internal/lie_basis_info.h
         src/libalgebra_lite_internal/lie_info.h
         src/libalgebra_lite_internal/lite_vector_selector.h
         src/libalgebra_lite_internal/shuffle_tensor_info.h
         src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h
         src/libalgebra_lite_internal/sparse_vector_iterator.h
         src/libalgebra_lite_internal/tensor_basis_info.h
+        src/libalgebra_lite_internal/unspecified_algebra_binary_op.h
+        src/libalgebra_lite_internal/vector_storage_type.h
         src/libalgebra_lite_internal/vector_type_helper.h
         src/tensor_basis.cpp
         src/lie_basis.cpp
         PUBLIC_HEADERS
         include/roughpy/algebra/algebra_fwd.h
         include/roughpy/algebra/algebra_base.h
         include/roughpy/algebra/algebra_impl.h
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_base.h`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,22 @@
 class AlgebraInterfaceBase
 {
 protected:
     context_pointer p_ctx;
     const scalars::ScalarType* p_coeff_type;
     VectorType m_vector_type;
     ImplementationType m_impl_type;
+    AlgebraType m_alg_type;
 
     explicit AlgebraInterfaceBase(
-            context_pointer&& ctx, VectorType vtype,
-            const scalars::ScalarType* stype, ImplementationType impl_type
+            context_pointer&& ctx,
+            VectorType vtype,
+            const scalars::ScalarType* stype,
+            ImplementationType impl_type,
+            AlgebraType alg_type
     );
 
 public:
     virtual ~AlgebraInterfaceBase();
 
     RPY_NO_DISCARD
     const context_pointer& context() const noexcept { return p_ctx; }
@@ -82,27 +86,33 @@
     RPY_NO_DISCARD
     VectorType storage_type() const noexcept { return m_vector_type; };
     RPY_NO_DISCARD
     const scalars::ScalarType* coeff_type() const noexcept
     {
         return p_coeff_type;
     };
+    RPY_NO_DISCARD
+    AlgebraType alg_type() const noexcept { return m_alg_type; }
+
 };
 
 template <typename Algebra, typename BasisType>
 class AlgebraBasicProperties : public AlgebraInterfaceBase
 {
 protected:
     BasisType m_basis;
 
     AlgebraBasicProperties(
-            context_pointer&& ctx, VectorType vtype,
-            const scalars::ScalarType* stype, ImplementationType impl_type
+            context_pointer&& ctx,
+            VectorType vtype,
+            const scalars::ScalarType* stype,
+            ImplementationType impl_type
     )
-        : AlgebraInterfaceBase(std::move(ctx), vtype, stype, impl_type),
+        : AlgebraInterfaceBase(std::move(ctx), vtype, stype, impl_type,
+                               Algebra::s_alg_type),
           m_basis(basis_setup_helper<Algebra>::get(context()))
     {}
 
 public:
     using algebra_t = Algebra;
     using basis_t = BasisType;
     using id_t = uintptr_t;
@@ -323,14 +333,18 @@
 
     friend struct algebra_access<typename Interface::algebra_interface_t>;
 
 public:
     explicit AlgebraBase(std::unique_ptr<Interface> impl)
         : p_impl(std::move(impl))
     {}
+    explicit AlgebraBase(UnspecifiedAlgebraType&& impl)
+            : p_impl(reinterpret_cast<Interface*>(impl.release()))
+    {}
+
     explicit AlgebraBase(Interface* impl) : p_impl(impl) {}
 
     using interface_t = Interface;
 
     using basis_type = typename interface_t::basis_t;
     using key_type = typename interface_t::key_type;
 
@@ -394,14 +408,27 @@
     RPY_NO_DISCARD
     constexpr operator bool() const noexcept
     {
         return static_cast<bool>(p_impl);
     }
 
     RPY_NO_DISCARD
+    explicit inline operator const Interface*() const noexcept
+    {
+        return p_impl.get();
+    }
+
+    RPY_NO_DISCARD
+    explicit inline operator Interface*() noexcept
+    {
+        return p_impl.get();
+    }
+
+
+    RPY_NO_DISCARD
     dimn_t dimension() const;
     RPY_NO_DISCARD
     dimn_t size() const;
     RPY_NO_DISCARD
     bool is_zero() const;
     RPY_NO_DISCARD
     context_pointer context() const noexcept;
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base_impl.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_base_impl.h`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,15 @@
 template <
         typename Interface,
         template <typename, template <typename> class> class DerivedImpl>
 typename Interface::algebra_t
 AlgebraBase<Interface, DerivedImpl>::sdiv(const scalars::Scalar& rhs) const
 {
     if (is_equivalent_to_zero(*this)) { return algebra_t(); }
-    if (rhs.is_zero()) { throw std::invalid_argument("cannot divide by zero"); }
+    if (rhs.is_zero()) { RPY_THROW(std::invalid_argument, "cannot divide by zero"); }
     // The implementation should perform the necessary scalar casting
     return p_impl->sdiv(rhs);
 }
 
 template <
         typename Interface,
         template <typename, template <typename> class> class DerivedImpl>
@@ -471,15 +471,15 @@
         typename Interface,
         template <typename, template <typename> class> class DerivedImpl>
 typename Interface::algebra_t&
 AlgebraBase<Interface, DerivedImpl>::sdiv_inplace(const scalars::Scalar& rhs)
 {
     if (!is_equivalent_to_zero(*this)) {
         if (rhs.is_zero()) {
-            throw std::invalid_argument("cannot divide by zero");
+            RPY_THROW(std::invalid_argument, "cannot divide by zero");
         }
         p_impl->sdiv_inplace(rhs);
     }
     return downcast(*this);
 }
 
 template <
@@ -528,15 +528,15 @@
         const algebra_t& lhs, const scalars::Scalar& rhs
 )
 {
     if (!is_equivalent_to_zero(lhs)) {
         RPY_CHECK_CONTEXTS(lhs);
 
         if (rhs.is_zero()) {
-            throw std::invalid_argument("cannot divide by zero");
+            RPY_THROW(std::invalid_argument, "cannot divide by zero");
         }
         if (!is_equivalent_to_zero(*this)) {
             p_impl->add_scal_div(lhs, rhs);
         } else {
             *this = lhs.sdiv(rhs);
         }
     }
@@ -550,15 +550,15 @@
         const algebra_t& lhs, const scalars::Scalar& rhs
 )
 {
     if (!is_equivalent_to_zero(lhs)) {
         RPY_CHECK_CONTEXTS(lhs);
 
         if (rhs.is_zero()) {
-            throw std::invalid_argument("cannot divide by zero");
+            RPY_THROW(std::invalid_argument, "cannot divide by zero");
         }
         if (!is_equivalent_to_zero(*this)) {
             p_impl->sub_scal_div(lhs, rhs);
         } else {
             *this = lhs.sdiv(rhs).uminus();
         }
     }
@@ -626,15 +626,15 @@
         const algebra_t& lhs, const scalars::Scalar& rhs
 )
 {
     if (!is_equivalent_to_zero(lhs)) {
         RPY_CHECK_CONTEXTS(lhs);
 
         if (rhs.is_zero()) {
-            throw std::invalid_argument("cannot divide by zero");
+            RPY_THROW(std::invalid_argument, "cannot divide by zero");
         }
         if (!is_equivalent_to_zero(*this)) { p_impl->mul_sdiv(lhs, rhs); }
     } else if (!is_equivalent_to_zero(*this)) {
         p_impl->clear();
     }
     return downcast(*this);
 }
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_bundle.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_impl.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_bundle_impl.h`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     const BundleImpl& get_data() const noexcept override { return data(); }
 
     BundleImpl&& take_data() override
     {
         if RPY_IF_CONSTEXPR (is_same<storage_base_t,
                                      BorrowedStorageModel<BundleImpl>>::value) {
-            throw std::runtime_error("cannot take from a borrowed algebra");
+            RPY_THROW(std::runtime_error, "cannot take from a borrowed algebra");
         } else {
             return std::move(data());
         }
     }
 
     template <typename... Args>
     explicit AlgebraBundleImplementation(context_pointer&& ctx, Args&&... args)
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_fwd.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_fwd.h`

 * *Files 4% similar despite different names*

```diff
@@ -47,27 +47,33 @@
 
 enum class VectorType
 {
     Dense,
     Sparse
 };
 
+template <VectorType>
+struct vector_type_tag {};
+
 /**
  * @brief Different algebra types required by RoughPy
  */
 enum class AlgebraType : uint32_t
 {
     FreeTensor,
     ShuffleTensor,
     Lie,
     FreeTensorBundle,
     ShuffleTensorBundle,
     LieBundle
 };
 
+template <AlgebraType>
+struct algebra_type_tag {};
+
 template <typename Interface>
 struct algebra_access;
 
 template <typename Wrapper, typename Algebra>
 struct algebra_info;
 
 template <typename Algebra>
@@ -78,14 +84,15 @@
 
 namespace dtl {
 
 class AlgebraInterfaceBase;
 
 }
 using RawUnspecifiedAlgebraType = dtl::AlgebraInterfaceBase*;
+using ConstRawUnspecifiedAlgebraType = const dtl::AlgebraInterfaceBase*;
 using UnspecifiedAlgebraType = std::unique_ptr<dtl::AlgebraInterfaceBase>;
 
 class FreeTensor;
 
 class Lie;
 
 class ShuffleTensor;
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_impl.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_impl.h`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     static constexpr ImplementationType s_type = ImplementationType::Borrowed;
 
     explicit BorrowedStorageModel(Impl* arg) : p_data(arg) {}
 
     Impl& data()
     {
         if (is_const<Impl>::value) {
-            throw std::runtime_error("cannot get mutable data from const object"
+            RPY_THROW(std::runtime_error,"cannot get mutable data from const object"
             );
         }
         return *p_data;
     }
     const Impl& data() const noexcept { return *p_data; }
 };
 
@@ -207,15 +207,15 @@
 
 public:
     Impl& get_data() noexcept override { return data(); }
     const Impl& get_data() const noexcept override { return data(); }
     Impl&& take_data() override
     {
         if (is_same<storage_base_t, BorrowedStorageModel<Impl>>::value) {
-            throw std::runtime_error("cannot take from a borrowed algebra");
+            RPY_THROW(std::runtime_error, "cannot take from a borrowed algebra");
         }
         return std::move(data());
     }
 
     template <typename... Args>
     explicit AlgebraImplementation(context_pointer&& ctx, Args&&... args)
         : access_layer_t(
@@ -579,15 +579,15 @@
         if (this->storage_type() == arg->storage_type()) {
             return algebra_cast<const Impl&>(*arg);
         }
         return take_algebra<Impl, Interface>(
                 this->context()->convert(arg, this->storage_type())
         );
     }
-    throw std::invalid_argument("cannot convert argument");
+    RPY_THROW(std::invalid_argument, "cannot convert argument");
 }
 
 template <
         typename Interface, typename Impl,
         template <typename> class StorageModel>
 void AlgebraImplementation<Interface, Impl, StorageModel>::add_scal_mul_impl(
         const algebra_t& arg, const scalars::Scalar& scalar,
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_info.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_iterator.h`

 * *Files 2% similar despite different names*

```diff
@@ -187,25 +187,25 @@
     return result;
 }
 template <typename Algebra>
 typename AlgebraIterator<Algebra>::reference
 AlgebraIterator<Algebra>::operator*() const
 {
     if (!p_interface) {
-        throw std::runtime_error("attempting to dereference an invalid iterator"
+        RPY_THROW(std::runtime_error,"attempting to dereference an invalid iterator"
         );
     }
     return {p_interface};
 }
 template <typename Algebra>
 typename AlgebraIterator<Algebra>::pointer
 AlgebraIterator<Algebra>::operator->() const
 {
     if (!p_interface) {
-        throw std::runtime_error("cannot dereference an invalid iterator");
+        RPY_THROW(std::runtime_error, "cannot dereference an invalid iterator");
     }
     return {p_interface};
 }
 template <typename Algebra>
 bool AlgebraIterator<Algebra>::operator==(const AlgebraIterator& other) const
 {
     if (!p_interface || !other.p_interface) { return false; }
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator_impl.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/algebra_iterator_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/basis.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/basis_impl.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/basis_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/basis_info.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/context.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/context.h`

 * *Files 9% similar despite different names*

```diff
@@ -83,23 +83,19 @@
             deg_t width, deg_t depth, const dimn_t* lie_sizes,
             const dimn_t* tensor_sizes
     );
 
 public:
     virtual ~ContextBase();
 
-    RPY_NO_DISCARD
-    deg_t width() const noexcept { return m_width; }
-    RPY_NO_DISCARD
-    deg_t depth() const noexcept { return m_depth; }
-
-    RPY_NO_DISCARD
-    dimn_t lie_size(deg_t deg) const noexcept;
-    RPY_NO_DISCARD
-    dimn_t tensor_size(deg_t deg) const noexcept;
+    RPY_NO_DISCARD deg_t width() const noexcept { return m_width; }
+    RPY_NO_DISCARD deg_t depth() const noexcept { return m_depth; }
+
+    RPY_NO_DISCARD dimn_t lie_size(deg_t deg) const noexcept;
+    RPY_NO_DISCARD dimn_t tensor_size(deg_t deg) const noexcept;
 };
 
 class RPY_EXPORT Context : public ContextBase
 {
     const scalars::ScalarType* p_ctype;
     string m_ctx_backend;
 
@@ -110,136 +106,144 @@
             const dimn_t* tensor_sizes = nullptr
     )
         : ContextBase(width, depth, lie_sizes, tensor_sizes), p_ctype(ctype),
           m_ctx_backend(std::move(context_backend))
     {}
 
 public:
-    RPY_NO_DISCARD
-    const scalars::ScalarType* ctype() const noexcept { return p_ctype; }
-    RPY_NO_DISCARD
-    const string& backend() const noexcept { return m_ctx_backend; }
-
-    RPY_NO_DISCARD
-    virtual context_pointer get_alike(deg_t new_depth) const = 0;
-    RPY_NO_DISCARD
-    virtual context_pointer get_alike(const scalars::ScalarType* new_ctype
-    ) const = 0;
-    RPY_NO_DISCARD
-    virtual context_pointer
+    RPY_NO_DISCARD const scalars::ScalarType* ctype() const noexcept
+    {
+        return p_ctype;
+    }
+    RPY_NO_DISCARD const string& backend() const noexcept
+    {
+        return m_ctx_backend;
+    }
+
+    RPY_NO_DISCARD virtual context_pointer get_alike(deg_t new_depth) const = 0;
+    RPY_NO_DISCARD virtual context_pointer
+    get_alike(const scalars::ScalarType* new_ctype) const
+            = 0;
+    RPY_NO_DISCARD virtual context_pointer
     get_alike(deg_t new_depth, const scalars::ScalarType* new_ctype) const
             = 0;
-    RPY_NO_DISCARD
-    virtual context_pointer get_alike(
+    RPY_NO_DISCARD virtual context_pointer get_alike(
             deg_t new_width, deg_t new_depth,
             const scalars::ScalarType* new_ctype
     ) const = 0;
 
-    RPY_NO_DISCARD
-    virtual bool check_compatible(const Context& other_ctx) const noexcept;
+    RPY_NO_DISCARD virtual bool check_compatible(const Context& other_ctx
+    ) const noexcept;
 
-    RPY_NO_DISCARD
-    virtual LieBasis get_lie_basis() const = 0;
-    RPY_NO_DISCARD
-    virtual TensorBasis get_tensor_basis() const = 0;
+    RPY_NO_DISCARD virtual LieBasis get_lie_basis() const = 0;
+    RPY_NO_DISCARD virtual TensorBasis get_tensor_basis() const = 0;
 
-    RPY_NO_DISCARD
-    virtual FreeTensor
+    RPY_NO_DISCARD virtual FreeTensor
     convert(const FreeTensor& arg, optional<VectorType> new_vec_type) const
             = 0;
-    RPY_NO_DISCARD
-    virtual ShuffleTensor
+    RPY_NO_DISCARD virtual ShuffleTensor
     convert(const ShuffleTensor& arg, optional<VectorType> new_vec_type) const
             = 0;
-    RPY_NO_DISCARD
-    virtual Lie convert(const Lie& arg, optional<VectorType> new_vec_type) const
+    RPY_NO_DISCARD virtual Lie
+    convert(const Lie& arg, optional<VectorType> new_vec_type) const
             = 0;
 
-    RPY_NO_DISCARD
-    virtual FreeTensor construct_free_tensor(const VectorConstructionData& arg
-    ) const = 0;
-    RPY_NO_DISCARD
-    virtual ShuffleTensor
+    RPY_NO_DISCARD virtual FreeTensor
+    construct_free_tensor(const VectorConstructionData& arg) const
+            = 0;
+    RPY_NO_DISCARD virtual ShuffleTensor
     construct_shuffle_tensor(const VectorConstructionData& arg) const
             = 0;
-    RPY_NO_DISCARD
-    virtual Lie construct_lie(const VectorConstructionData& arg) const = 0;
+    RPY_NO_DISCARD virtual Lie construct_lie(const VectorConstructionData& arg
+    ) const = 0;
 
-    RPY_NO_DISCARD
-    virtual UnspecifiedAlgebraType
+    RPY_NO_DISCARD virtual UnspecifiedAlgebraType
     construct(AlgebraType type, const VectorConstructionData& data) const
             = 0;
 
-    RPY_NO_DISCARD
-    FreeTensor zero_free_tensor(VectorType vtype) const;
-    RPY_NO_DISCARD
-    ShuffleTensor zero_shuffle_tensor(VectorType vtype) const;
-    RPY_NO_DISCARD
-    Lie zero_lie(VectorType vtype) const;
+    RPY_NO_DISCARD FreeTensor zero_free_tensor(VectorType vtype) const;
+    RPY_NO_DISCARD ShuffleTensor zero_shuffle_tensor(VectorType vtype) const;
+    RPY_NO_DISCARD Lie zero_lie(VectorType vtype) const;
 
 protected:
     void lie_to_tensor_fallback(FreeTensor& result, const Lie& arg) const;
     void tensor_to_lie_fallback(Lie& result, const FreeTensor& arg) const;
 
 public:
-    RPY_NO_DISCARD
-    virtual FreeTensor lie_to_tensor(const Lie& arg) const = 0;
-    RPY_NO_DISCARD
-    virtual Lie tensor_to_lie(const FreeTensor& arg) const = 0;
+    RPY_NO_DISCARD virtual FreeTensor lie_to_tensor(const Lie& arg) const = 0;
+    RPY_NO_DISCARD virtual Lie tensor_to_lie(const FreeTensor& arg) const = 0;
 
 protected:
     void
     cbh_fallback(FreeTensor& collector, const std::vector<Lie>& lies) const;
 
 public:
-    RPY_NO_DISCARD
-    virtual Lie cbh(const std::vector<Lie>& lies, VectorType vtype) const;
-    RPY_NO_DISCARD
-    virtual Lie cbh(const Lie& left, const Lie& right, VectorType vtype) const;
-
-    RPY_NO_DISCARD
-    virtual FreeTensor to_signature(const Lie& log_signature) const;
-    RPY_NO_DISCARD
-    virtual FreeTensor signature(const SignatureData& data) const = 0;
-    RPY_NO_DISCARD
-    virtual Lie log_signature(const SignatureData& data) const = 0;
+    RPY_NO_DISCARD virtual Lie
+    cbh(const std::vector<Lie>& lies, VectorType vtype) const;
+    RPY_NO_DISCARD virtual Lie
+    cbh(const Lie& left, const Lie& right, VectorType vtype) const;
+
+    RPY_NO_DISCARD virtual FreeTensor to_signature(const Lie& log_signature
+    ) const;
+    RPY_NO_DISCARD virtual FreeTensor signature(const SignatureData& data) const
+            = 0;
+    RPY_NO_DISCARD virtual Lie log_signature(const SignatureData& data) const
+            = 0;
 
-    RPY_NO_DISCARD
-    virtual FreeTensor sig_derivative(
+    RPY_NO_DISCARD virtual FreeTensor sig_derivative(
             const std::vector<DerivativeComputeInfo>& info, VectorType vtype
     ) const = 0;
 
     // Functions to aid serialization
-    RPY_NO_DISCARD
-    virtual std::vector<byte>
+    RPY_NO_DISCARD virtual std::vector<byte>
     to_raw_bytes(AlgebraType atype, RawUnspecifiedAlgebraType alg) const;
 
-    RPY_NO_DISCARD
-    virtual UnspecifiedAlgebraType
+    RPY_NO_DISCARD virtual UnspecifiedAlgebraType
     from_raw_bytes(AlgebraType atype, Slice<byte> raw_bytes) const;
+
+    virtual UnspecifiedAlgebraType free_multiply(
+            const ConstRawUnspecifiedAlgebraType left,
+            const ConstRawUnspecifiedAlgebraType right
+    ) const;
+
+    virtual UnspecifiedAlgebraType shuffle_multiply(
+            ConstRawUnspecifiedAlgebraType left,
+            ConstRawUnspecifiedAlgebraType right
+            ) const;
+
+    virtual UnspecifiedAlgebraType half_shuffle_multiply(
+            ConstRawUnspecifiedAlgebraType left,
+            ConstRawUnspecifiedAlgebraType right
+            ) const;
+
+    virtual UnspecifiedAlgebraType adjoint_to_left_multiply_by(
+            ConstRawUnspecifiedAlgebraType multiplier,
+            ConstRawUnspecifiedAlgebraType argument
+            ) const;
+
+
+
 };
 
-RPY_EXPORT
-base_context_pointer get_base_context(deg_t width, deg_t depth);
+RPY_EXPORT base_context_pointer get_base_context(deg_t width, deg_t depth);
 
-RPY_EXPORT
-context_pointer get_context(
+RPY_EXPORT context_pointer get_context(
         deg_t width, deg_t depth, const scalars::ScalarType* ctype,
         const std::vector<std::pair<string, string>>& preferences = {}
 );
 
 inline void check_contexts_compatible(const Context& ctx1, const Context& ctx2)
 {
     if (&ctx1 == &ctx2) {
         // Early exit if both reference the same object.
         return;
     }
 
     if (ctx1.width() != ctx2.width()) {
-        throw std::invalid_argument("contexts have incompatible width");
+        RPY_THROW(std::invalid_argument, "contexts have incompatible width");
     }
 
     const auto* ctype1 = ctx1.ctype();
     const auto* ctype2 = ctx2.ctype();
     if (ctype1 == ctype2) {
         // Both are OK if the ctypes are identical
         return;
@@ -263,16 +267,16 @@
             deg_t width, deg_t depth, const scalars::ScalarType* ctype,
             const preference_list& preferences
     ) const = 0;
     virtual optional<base_context_pointer>
     get_base_context(deg_t width, deg_t depth) const = 0;
 };
 
-RPY_EXPORT
-const ContextMaker* register_context_maker(std::unique_ptr<ContextMaker> maker);
+RPY_EXPORT const ContextMaker*
+register_context_maker(std::unique_ptr<ContextMaker> maker);
 
 template <typename Maker>
 class RegisterMakerHelper
 {
     const ContextMaker* maker = nullptr;
 
 public:
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/context_fwd.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/context_fwd.h`

 * *Files 18% similar despite different names*

```diff
@@ -36,25 +36,35 @@
 
 #include <roughpy/core/slice.h>
 
 #define RPY_MAKE_VTYPE_SWITCH(VTYPE)                                           \
     switch (VTYPE) {                                                           \
         case VectorType::Dense: return RPY_SWITCH_FN(VectorType::Dense);       \
         case VectorType::Sparse: return RPY_SWITCH_FN(VectorType::Sparse);     \
-        default: throw std::invalid_argument("invalid vector type");           \
+        default:                                                               \
+            RPY_UNREACHABLE();                                                 \
+            RPY_THROW(std::invalid_argument, "invalid vector type");                \
     }
 
 #define RPY_MAKE_ALGTYPE_SWITCH(ALGTYPE)                                       \
     switch (ALGTYPE) {                                                         \
         case AlgebraType::FreeTensor:                                          \
             return RPY_SWITCH_FN(AlgebraType::FreeTensor);                     \
         case AlgebraType::Lie: return RPY_SWITCH_FN(AlgebraType::Lie);         \
         case AlgebraType::ShuffleTensor:                                       \
             return RPY_SWITCH_FN(AlgebraType::ShuffleTensor);                  \
-        default: throw std::invalid_argument("invalid algebra type");          \
+        case AlgebraType::FreeTensorBundle:                                    \
+            return RPY_SWITCH_FN(AlgebraType::FreeTensorBundle);               \
+        case AlgebraType::ShuffleTensorBundle:                                 \
+            return RPY_SWITCH_FN(AlgebraType::ShuffleTensorBundle);            \
+        case AlgebraType::LieBundle:                                           \
+            return RPY_SWITCH_FN(AlgebraType::LieBundle);                      \
+        default:                                                               \
+            RPY_UNREACHABLE();                                                 \
+            RPY_THROW(std::invalid_argument, "invalid algebra type");               \
     }
 
 namespace rpy {
 namespace algebra {
 
 struct SignatureData;
 struct DerivativeComputeInfo;
```

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/fallback_operations.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/fallback_operations.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/free_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_fwd.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/free_tensor_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_impl.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/free_tensor_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/lie.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/lie.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/lie_basis.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/lie_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/lie_fwd.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/lie_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/linear_operator.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/linear_operator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/shuffle_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/include/roughpy/algebra/tensor_basis.h` & `roughpy-0.0.5/algebra/include/roughpy/algebra/tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/ContextFixture.cpp` & `roughpy-0.0.5/algebra/src/ContextFixture.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/ContextFixture.h` & `roughpy-0.0.5/algebra/src/ContextFixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/algebra_base.cpp` & `roughpy-0.0.5/algebra/src/algebra_base.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,22 @@
 
 #include <roughpy/algebra/context.h>
 
 using namespace rpy;
 using namespace rpy::algebra;
 
 algebra::dtl::AlgebraInterfaceBase::AlgebraInterfaceBase(
-        context_pointer&& ctx, VectorType vtype,
-        const scalars::ScalarType* stype, ImplementationType impl_type
+        context_pointer&& ctx,
+        VectorType vtype,
+        const scalars::ScalarType* stype,
+        ImplementationType impl_type,
+        AlgebraType alg_type
 )
     : p_ctx(std::move(ctx)), p_coeff_type(stype), m_vector_type(vtype),
-      m_impl_type(impl_type)
+      m_impl_type(impl_type), m_alg_type(alg_type)
 {}
 
 algebra::dtl::AlgebraInterfaceBase::~AlgebraInterfaceBase() = default;
 
 void rpy::algebra::dtl::print_empty_algebra(std::ostream& os) { os << "{ }"; }
 
 const rpy::scalars::ScalarType*
```

### Comparing `roughpy-0.0.4/algebra/src/algebra_iterator.cpp` & `roughpy-0.0.5/algebra/src/algebra_iterator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/basis.cpp` & `roughpy-0.0.5/algebra/src/basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/context.cpp` & `roughpy-0.0.5/algebra/src/context.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -237,20 +237,20 @@
     for (const auto& maker : maker_list) {
         if (maker->can_get(width, depth, ctype, preferences)) {
             found.push_back(maker.get());
         }
     }
 
     if (found.empty()) {
-        throw std::invalid_argument("cannot find a context maker for the "
+        RPY_THROW(std::invalid_argument,"cannot find a context maker for the "
                                     "width, depth, dtype, and preferences set");
     }
 
     if (found.size() > 1) {
-        throw std::invalid_argument(
+        RPY_THROW(std::invalid_argument,
                 "found multiple context maker candidates for specified width, "
                 "depth, dtype, and preferences set"
         );
     }
 
     return found[0]->get_context(width, depth, ctype, preferences);
 }
@@ -271,20 +271,20 @@
 {
     return false;
 }
 
 std::vector<byte>
 Context::to_raw_bytes(AlgebraType atype, RawUnspecifiedAlgebraType alg) const
 {
-    throw std::runtime_error("cannot generate raw byte representation");
+    RPY_THROW(std::runtime_error, "cannot generate raw byte representation");
 }
 UnspecifiedAlgebraType
 Context::from_raw_bytes(AlgebraType atype, Slice<byte> raw_bytes) const
 {
-    throw std::runtime_error("cannot load from raw bytes");
+    RPY_THROW(std::runtime_error, "cannot load from raw bytes");
 }
 
 void rpy::algebra::intrusive_ptr_release(const rpy::algebra::Context* ptr)
 {
     intrusive_ptr_release(static_cast<const boost::intrusive_ref_counter<
                                   ContextBase, boost::thread_safe_counter>*>(ptr
     ));
@@ -304,7 +304,40 @@
 }
 void rpy::algebra::intrusive_ptr_add_ref(const rpy::algebra::ContextBase* ptr)
 {
     intrusive_ptr_add_ref(static_cast<const boost::intrusive_ref_counter<
                                   ContextBase, boost::thread_safe_counter>*>(ptr
     ));
 }
+
+UnspecifiedAlgebraType Context::free_multiply(
+        const ConstRawUnspecifiedAlgebraType left,
+        const ConstRawUnspecifiedAlgebraType right
+) const
+{
+    RPY_THROW(std::runtime_error,"free tensor multiply is not implemented for "
+                                         "arbitrary types with this backend");
+}
+UnspecifiedAlgebraType Context::shuffle_multiply(
+        ConstRawUnspecifiedAlgebraType left,
+        ConstRawUnspecifiedAlgebraType right
+) const
+{
+    RPY_THROW(std::runtime_error,"shuffle multiply is not implemented for "
+                                         "arbitrary types with this backend");
+}
+UnspecifiedAlgebraType Context::half_shuffle_multiply(
+        ConstRawUnspecifiedAlgebraType left,
+        ConstRawUnspecifiedAlgebraType right
+) const
+{
+    RPY_THROW(std::runtime_error,"half shuffle multiply is not implemented for "
+                             "arbitrary types with this backend");
+}
+UnspecifiedAlgebraType Context::adjoint_to_left_multiply_by(
+        ConstRawUnspecifiedAlgebraType multiplier,
+        ConstRawUnspecifiedAlgebraType argument
+) const
+{
+    RPY_THROW(std::runtime_error,"adjoint of left multiply is not implemented for "
+                             "arbitrary types with this backend");
+}
```

### Comparing `roughpy-0.0.4/algebra/src/double_lite_context.cpp` & `roughpy-0.0.5/algebra/src/double_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/float_lite_context.cpp` & `roughpy-0.0.5/algebra/src/float_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/free_tensor.cpp` & `roughpy-0.0.5/algebra/src/free_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/hall_set_size.cpp` & `roughpy-0.0.5/algebra/src/hall_set_size.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/hall_set_size.h` & `roughpy-0.0.5/algebra/src/hall_set_size.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/free_tensor_info.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/free_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_basis_info.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/lie_basis_info.h`

 * *Files 1% similar despite different names*

```diff
@@ -70,23 +70,23 @@
     // The conversion methods are required, they are used in the trait
     // and in the algebra wrapper
     /// Conversion from impl_key_type to our_key_type
     static our_key_type
     convert_from_impl(storage_t basis, const impl_key_type& arg)
     {
         // The default is to take the index of arg as the return
-        return basis->key_to_index(arg);
+        return 1 + static_cast<our_key_type>(basis->key_to_index(arg));
     }
 
     /// Conversion from our_key_type to impl_key_type
     static impl_key_type
     convert_to_impl(storage_t basis, const our_key_type& arg)
     {
         // Default is to treat rpy keys as the index of impl keys
-        return basis->index_to_key(arg);
+        return basis->index_to_key(static_cast<dimn_t>(arg) - 1);
     }
 
     /*
      * A standard basis requires as a minimum:
      *      - key_to_string
      *      - dimension
      */
```

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_info.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/lie_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lite_vector_selector.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/lite_vector_selector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         return static_cast<scalar_t>(arg);
     }
 
     template <typename T>
     static enable_if_t<!is_convertible<const T&, scalar_t>::value, scalar_t>
     convert_to_scalar_t(const T&)
     {
-        throw std::runtime_error("cannot convert to scalar_t");
+        RPY_THROW(std::runtime_error, "cannot convert to scalar_t");
     }
 
 public:
     scalar_t as_scalar() const override
     {
         return convert_to_scalar_t(static_cast<const value_type&>(m_data));
     }
@@ -100,15 +100,15 @@
     {
         value_type tmp = static_cast<const value_type&>(m_data);
         type()->convert_copy({type(), &tmp}, data, 1, type_id);
         m_data = tmp;
     }
     ScalarPointer to_pointer() override
     {
-        throw std::runtime_error(
+        RPY_THROW(std::runtime_error,
                 "cannot get non-const pointer to proxy reference type"
         );
     }
     ScalarPointer to_pointer() const noexcept override
     {
         return {type(), &static_cast<const value_type&>(m_data)};
     }
```

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/tensor_basis_info.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/tensor_basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/vector_type_helper.h` & `roughpy-0.0.5/algebra/src/libalgebra_lite_internal/vector_type_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/lie.cpp` & `roughpy-0.0.5/algebra/src/lie.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/lie_basis.cpp` & `roughpy-0.0.5/algebra/src/lie_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/lite_context.cpp` & `roughpy-0.0.5/algebra/src/lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/lite_context.h` & `roughpy-0.0.5/algebra/src/lite_context.h`

 * *Files 16% similar despite different names*

```diff
@@ -49,35 +49,35 @@
 #include <roughpy/algebra/basis_impl.h>
 #include <roughpy/algebra/context.h>
 #include <roughpy/algebra/free_tensor.h>
 #include <roughpy/algebra/free_tensor_impl.h>
 #include <roughpy/algebra/lie.h>
 #include <roughpy/algebra/shuffle_tensor.h>
 
+#include "libalgebra_lite_internal/algebra_type_caster.h"
+#include "libalgebra_lite_internal/algebra_type_helper.h"
 #include "libalgebra_lite_internal/dense_vector_iterator.h"
 #include "libalgebra_lite_internal/free_tensor_info.h"
 #include "libalgebra_lite_internal/lie_basis_info.h"
 #include "libalgebra_lite_internal/lie_info.h"
 #include "libalgebra_lite_internal/lite_vector_selector.h"
 #include "libalgebra_lite_internal/shuffle_tensor_info.h"
 #include "libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h"
 #include "libalgebra_lite_internal/sparse_vector_iterator.h"
 #include "libalgebra_lite_internal/tensor_basis_info.h"
+#include "libalgebra_lite_internal/unspecified_algebra_binary_op.h"
 
 #include <libalgebra_lite/coefficients.h>
 #include <libalgebra_lite/maps.h>
 #include <libalgebra_lite/registry.h>
 
 namespace rpy {
 namespace algebra {
 
 namespace dtl {
-template <AlgebraType ATYpe>
-struct alg_type_tag {
-};
 
 class LiteContextBasisHolder
 {
 protected:
     lal::basis_pointer<lal::tensor_basis> p_tbasis;
     lal::basis_pointer<lal::hall_basis> p_lbasis;
 
@@ -111,14 +111,36 @@
 public:
     using scalar_type = typename coeff_traits::scalar_type;
     using rational_type = typename coeff_traits::rational_type;
 
 private:
     lal::maps m_maps;
 
+    template <AlgebraType AType, VectorType VType>
+    using arg_type_caster = algebra_type_caster<
+            Coefficients, algebra_type_tag<AType>, vector_type_tag<VType>>;
+
+    using binary_invoker = UnspecifiedFunctionInvoker<
+            arg_type_caster, LiteContext, ConstRawUnspecifiedAlgebraType,
+            ConstRawUnspecifiedAlgebraType>;
+
+    template <typename T>
+    RPY_NO_UBSAN static const T&
+    unspecified_cast(ConstRawUnspecifiedAlgebraType arg)
+    {
+        using info = dtl::alg_details_of<T>;
+        RPY_CHECK(arg != nullptr);
+        RPY_CHECK(arg->alg_type() == info::alg_type);
+        RPY_CHECK(arg->storage_type() == info::vec_type);
+        const auto* interface_ptr
+                = reinterpret_cast<const typename info::interface_type*>(arg);
+
+        return algebra_cast<T, typename info::interface_type>(*interface_ptr);
+    }
+
     template <typename OutType, typename InType>
     OutType convert_impl(
             const InType& arg,
             const lal::basis_pointer<typename OutType::basis_type>& basis,
             const std::shared_ptr<const typename OutType::multiplication_type>&
                     mul
     ) const;
@@ -174,21 +196,30 @@
             const free_tensor_t<VType>& perturbation
     ) const;
     template <VectorType VType>
     free_tensor_t<VType>
     sig_derivative_impl(const std::vector<DerivativeComputeInfo>& info) const;
 
     UnspecifiedAlgebraType
-    construct_impl(const VectorConstructionData& data, dtl::alg_type_tag<AlgebraType::FreeTensor>)
+    construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::FreeTensor>)
+            const;
+    UnspecifiedAlgebraType
+    construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::ShuffleTensor>)
+            const;
+    UnspecifiedAlgebraType
+    construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::Lie>)
+            const;
+    UnspecifiedAlgebraType
+    construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::FreeTensorBundle>)
             const;
     UnspecifiedAlgebraType
-    construct_impl(const VectorConstructionData& data, dtl::alg_type_tag<AlgebraType::ShuffleTensor>)
+    construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::ShuffleTensorBundle>)
             const;
     UnspecifiedAlgebraType
-    construct_impl(const VectorConstructionData& data, dtl::alg_type_tag<AlgebraType::Lie>)
+    construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::LieBundle>)
             const;
 
 public:
     explicit LiteContext(deg_t width, deg_t depth);
 
     context_pointer get_alike(deg_t new_depth) const override;
     context_pointer get_alike(const scalars::ScalarType* new_ctype
@@ -222,14 +253,44 @@
     FreeTensor lie_to_tensor(const Lie& arg) const override;
     Lie tensor_to_lie(const FreeTensor& arg) const override;
     FreeTensor signature(const SignatureData& data) const override;
     Lie log_signature(const SignatureData& data) const override;
     FreeTensor sig_derivative(
             const std::vector<DerivativeComputeInfo>& info, VectorType vtype
     ) const override;
+
+private:
+    template <typename Left, typename Right, typename FreeFunctionWrapper>
+    UnspecifiedAlgebraType algebra_free_multiply_func_impl2(
+            const Left& left, const Right& right, FreeFunctionWrapper&& wrapper
+    ) const
+    {
+        using OutType = decltype(wrapper(left, right));
+        using impl_t =
+                typename dtl::alg_details_of<OutType>::implementation_type;
+        return UnspecifiedAlgebraType(new impl_t(this, wrapper(left, right)));
+    }
+
+public:
+    UnspecifiedAlgebraType free_multiply(
+            ConstRawUnspecifiedAlgebraType left,
+            ConstRawUnspecifiedAlgebraType right
+    ) const override;
+    UnspecifiedAlgebraType shuffle_multiply(
+            ConstRawUnspecifiedAlgebraType left,
+            ConstRawUnspecifiedAlgebraType right
+    ) const override;
+    UnspecifiedAlgebraType half_shuffle_multiply(
+            ConstRawUnspecifiedAlgebraType left,
+            ConstRawUnspecifiedAlgebraType right
+    ) const override;
+    UnspecifiedAlgebraType adjoint_to_left_multiply_by(
+            ConstRawUnspecifiedAlgebraType multiplier,
+            ConstRawUnspecifiedAlgebraType argument
+    ) const override;
 };
 
 class LiteContextMaker : public ContextMaker
 {
     using ContextMaker::preference_list;
     context_pointer create_context(
             deg_t width, deg_t depth, const scalars::ScalarType* ctype,
@@ -405,15 +466,15 @@
     // directly
     const auto& arg_context = arg->context();
     if (arg_context == this) {
         return m_maps.lie_to_tensor(algebra_cast<lie_t<VType>>(*arg));
     }
 
     if (arg_context->width() != width()) {
-        throw std::invalid_argument(
+        RPY_THROW(std::invalid_argument,
                 "cannot perform conversion on algebras with different bases"
         );
     }
 
     return convert_impl<VType>(arg_context->lie_to_tensor(arg));
 }
 template <typename Coefficients>
@@ -424,15 +485,15 @@
 
     const auto& arg_context = arg->context();
     if (arg_context == this) {
         return m_maps.tensor_to_lie(algebra_cast<free_tensor_t<VType>>(*arg));
     }
 
     if (arg_context->width() != width()) {
-        throw std::invalid_argument(
+        RPY_THROW(std::invalid_argument,
                 "cannot perform conversion on algebras with different bases"
         );
     }
 
     return m_maps.tensor_to_lie(convert_impl<VType>(arg));
 }
 template <typename Coefficients>
@@ -546,54 +607,75 @@
     }
 
     return result;
 }
 
 template <typename Coefficients>
 UnspecifiedAlgebraType LiteContext<Coefficients>::
-        construct_impl(const VectorConstructionData& data, dtl::alg_type_tag<AlgebraType::FreeTensor>)
+        construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::FreeTensor>)
                 const
 {
 #define RPY_SWITCH_FN(VTYPE)                                                   \
     UnspecifiedAlgebraType(new FreeTensorImplementation<                       \
                            free_tensor_t<(VTYPE)>, OwnedStorageModel>(         \
             this,                                                              \
             construct_impl<free_tensor_t<(VTYPE)>>(data, p_tbasis, p_ftmul)    \
     ))
     RPY_MAKE_VTYPE_SWITCH(data.vector_type)
 #undef RPY_SWITCH_FN
 }
 template <typename Coefficients>
 UnspecifiedAlgebraType LiteContext<Coefficients>::
-        construct_impl(const VectorConstructionData& data, dtl::alg_type_tag<AlgebraType::ShuffleTensor>)
+        construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::ShuffleTensor>)
                 const
 {
 #define RPY_SWITCH_FN(VTYPE)                                                   \
     UnspecifiedAlgebraType(new AlgebraImplementation<                          \
                            ShuffleTensorInterface, shuffle_tensor_t<(VTYPE)>,  \
                            OwnedStorageModel>(                                 \
             this,                                                              \
             construct_impl<shuffle_tensor_t<(VTYPE)>>(data, p_tbasis, p_stmul) \
     ))
     RPY_MAKE_VTYPE_SWITCH(data.vector_type)
 #undef RPY_SWITCH_FN
 }
 template <typename Coefficients>
 UnspecifiedAlgebraType LiteContext<Coefficients>::
-        construct_impl(const VectorConstructionData& data, dtl::alg_type_tag<AlgebraType::Lie>)
+        construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::Lie>)
                 const
 {
 #define RPY_SWITCH_FN(VTYPE)                                                   \
     UnspecifiedAlgebraType(new AlgebraImplementation<                          \
                            LieInterface, lie_t<(VTYPE)>, OwnedStorageModel>(   \
             this, construct_impl<lie_t<(VTYPE)>>(data, p_lbasis, p_liemul)     \
     ))
     RPY_MAKE_VTYPE_SWITCH(data.vector_type)
 #undef RPY_SWITCH_FN
 }
+template <typename Coefficients>
+UnspecifiedAlgebraType LiteContext<Coefficients>::
+        construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::FreeTensorBundle>)
+                const
+{
+    RPY_THROW(std::runtime_error, "not implemented for FreeTensorBundle");
+}
+template <typename Coefficients>
+UnspecifiedAlgebraType LiteContext<Coefficients>::
+        construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::ShuffleTensorBundle>)
+                const
+{
+    RPY_THROW(std::runtime_error, "not implemented for ShuffleTensorBundle");
+}
+template <typename Coefficients>
+UnspecifiedAlgebraType LiteContext<Coefficients>::
+        construct_impl(const VectorConstructionData& data, algebra_type_tag<AlgebraType::LieBundle>)
+                const
+{
+    RPY_THROW(std::runtime_error, "not implemented for LieBundle");
+}
 
 template <typename Coefficients>
 LiteContext<Coefficients>::LiteContext(deg_t width, deg_t depth)
     : dtl::LiteContextBasisHolder(width, depth),
       Context(width, depth, scalars::ScalarType::of<scalar_type>(),
               string("libalgebra_lite"), p_lbasis->sizes().data(),
               p_tbasis->sizes().data()),
@@ -733,15 +815,15 @@
 #undef RPY_SWITCH_FN
 }
 template <typename Coefficients>
 UnspecifiedAlgebraType LiteContext<Coefficients>::construct(
         AlgebraType type, const VectorConstructionData& data
 ) const
 {
-#define RPY_SWITCH_FN(ATYPE) construct_impl(data, dtl::alg_type_tag<ATYPE>())
+#define RPY_SWITCH_FN(ATYPE) construct_impl(data, algebra_type_tag<ATYPE>())
     RPY_MAKE_ALGTYPE_SWITCH(type)
 #undef RPY_SWITCH_FN
 }
 template <typename Coefficients>
 FreeTensor LiteContext<Coefficients>::lie_to_tensor(const Lie& arg) const
 {
 #define RPY_SWITCH_FN(VTYPE) FreeTensor(this, lie_to_tensor_impl<VTYPE>(arg))
@@ -774,14 +856,119 @@
 ) const
 {
 #define RPY_SWITCH_FN(VTYPE) FreeTensor(this, sig_derivative_impl<VTYPE>(info))
     RPY_MAKE_VTYPE_SWITCH(vtype)
 #undef RPY_SWITCH_FN
 }
 
+namespace wrappers {
+
+struct FreeMultiply {
+    template <typename L, typename R>
+    auto operator()(const L& left, const R& right) const
+            -> decltype(lal::free_tensor_multiply(left, right))
+    {
+        return lal::free_tensor_multiply(left, right);
+    }
+    template <AlgebraType Type>
+    using compatible = integral_constant<
+            bool,
+            Type == AlgebraType::FreeTensor
+                    || Type == AlgebraType::ShuffleTensor>;
+};
+struct ShuffleMultiply {
+
+    template <typename L, typename R>
+    auto operator()(const L& left, const R& right) const
+            -> decltype(lal::shuffle_multiply(left, right))
+    {
+        return lal::shuffle_multiply(left, right);
+    }
+    template <AlgebraType Type>
+    using compatible = integral_constant<
+            bool,
+            Type == AlgebraType::FreeTensor
+                    || Type == AlgebraType::ShuffleTensor>;
+};
+
+struct HalfShuffleMultiply {
+
+    template <typename L, typename R>
+    auto operator()(const L& left, const R& right) const
+            -> decltype(lal::half_shuffle_multiply(left, right))
+    {
+        return lal::half_shuffle_multiply(left, right);
+    }
+    template <AlgebraType Type>
+    using compatible = integral_constant<
+            bool,
+            Type == AlgebraType::FreeTensor
+                    || Type == AlgebraType::ShuffleTensor>;
+};
+
+struct AdjointFreeMultiply {
+
+    template <typename M, typename A>
+    auto operator()(const M& multiplier, const A& arg) const
+            -> decltype(lal::left_free_tensor_multiply_adjoint(multiplier, arg))
+    {
+        return lal::left_free_tensor_multiply_adjoint(multiplier, arg);
+    }
+
+    template <AlgebraType Type>
+    using compatible = integral_constant<
+            bool,
+            Type == AlgebraType::FreeTensor
+                    || Type == AlgebraType::ShuffleTensor>;
+};
+
+}// namespace wrappers
+
+template <typename Coefficients>
+UnspecifiedAlgebraType LiteContext<Coefficients>::free_multiply(
+        ConstRawUnspecifiedAlgebraType left,
+        ConstRawUnspecifiedAlgebraType right
+) const
+{
+    return binary_invoker::eval(
+            this, wrappers::FreeMultiply(), move(left), move(right)
+    );
+}
+template <typename Coefficients>
+UnspecifiedAlgebraType LiteContext<Coefficients>::shuffle_multiply(
+        ConstRawUnspecifiedAlgebraType left,
+        ConstRawUnspecifiedAlgebraType right
+) const
+{
+    return binary_invoker::eval(
+            this, wrappers::ShuffleMultiply(), move(left), move(right)
+    );
+}
+template <typename Coefficients>
+UnspecifiedAlgebraType LiteContext<Coefficients>::half_shuffle_multiply(
+        ConstRawUnspecifiedAlgebraType left,
+        ConstRawUnspecifiedAlgebraType right
+) const
+{
+    return binary_invoker::eval(
+            this, wrappers::HalfShuffleMultiply(), move(left), move(right)
+    );
+}
+template <typename Coefficients>
+UnspecifiedAlgebraType LiteContext<Coefficients>::adjoint_to_left_multiply_by(
+        ConstRawUnspecifiedAlgebraType multiplier,
+        ConstRawUnspecifiedAlgebraType argument
+) const
+{
+    return binary_invoker::eval(
+            this, wrappers::AdjointFreeMultiply(), move(multiplier),
+            move(argument)
+    );
+}
+
 extern template class LiteContext<lal::float_field>;
 
 extern template class LiteContext<lal::double_field>;
 
 extern template class LiteContext<lal::rational_field>;
 
 extern template class LiteContext<lal::polynomial_ring>;
```

### Comparing `roughpy-0.0.4/algebra/src/rational_lite_context.cpp` & `roughpy-0.0.5/algebra/src/rational_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/rational_poly_lite_context.cpp` & `roughpy-0.0.5/algebra/src/rational_poly_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/shuffle_tensor.cpp` & `roughpy-0.0.5/algebra/src/shuffle_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/tensor_basis.cpp` & `roughpy-0.0.5/algebra/src/tensor_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/test_lie.cpp` & `roughpy-0.0.5/algebra/src/test_lie.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/testing/mock_context.cpp` & `roughpy-0.0.5/algebra/src/testing/mock_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/algebra/src/testing/mock_context.h` & `roughpy-0.0.5/algebra/src/testing/mock_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/branding/logo/logo_square_white.jpg` & `roughpy-0.0.5/branding/logo/logo_square_white.jpg`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/cmake/roughpy_helpers.cmake` & `roughpy-0.0.5/cmake/roughpy_helpers.cmake`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,62 @@
 include(GenerateExportHeader)
 include(GoogleTest OPTIONAL)
 
 
 set(ROUGHPY_LIBS CACHE INTERNAL "")
 set(ROUGHPY_RUNTIME_DEPS CACHE INTERNAL "")
 
+
+function(get_brew_prefix _out_var _package)
+
+    cmake_parse_arguments(
+            ""
+            "VERBOSE"
+            "BREW_EXECUTABLE"
+            ""
+            ${ARGN}
+    )
+
+    set(_executable brew)
+    if (_BREW_EXECUTABLE)
+        set(_executable "${_BREW_EXECUTABLE}")
+    elseif (DEFINED ROUGHPY_HOMEBREW_EXECUTABLE)
+        set(_executable "${ROUGHPY_HOMEBREW_EXECUTABLE}")
+    elseif (DEFINED ENV{ROUGHPY_HOMEBREW_EXECUTABLE})
+        set(_executable "$ENV{ROUGHPY_HOMEBREW_EXECUTABLE}")
+    endif ()
+
+    if (NOT _VERBOSE AND ENV{VERBOSE})
+        set(_VERBOSE ON)
+    endif ()
+
+    set(_verbosity_flag "")
+    if (_VERBOSE)
+        set(_verbosity_flag "ECHO_OUTPUT_VARIABLE ECHO_ERROR_VARIABLE")
+    endif ()
+    message(DEBUG "Locating ${_package} brew installation prefix")
+
+    execute_process(COMMANDS ${_executable}
+            "--prefix" "${_package}"
+            RESULT_VARIABLE _result
+            OUTPUT_VARIABLE _out
+            OUTPUT_STRIP_TRAILING_WHITESPACE
+            ${_verbosity_flat}
+            )
+
+    if (_result EQUAL 0)
+        message(STATUS "Brew located ${_package} at ${_out}")
+        set(${_out_var} "${_out}" PARENT_SCOPE)
+    else ()
+        message(DEBUG "Could not locate ${_package} using Brew")
+        set(${_out_var} "${_out_var}-NOTFOUND")
+    endif ()
+endfunction()
+
+
 function(_get_component_name _out_var _component)
     string(SUBSTRING ${_component} 0 1 _first_letter)
     string(SUBSTRING ${_component} 1 -1 _remaining)
     string(TOUPPER ${_first_letter} _first_letter)
     string(CONCAT _comp_name "${_first_letter}" "${_remaining}")
     set(${_out_var} ${_comp_name} PARENT_SCOPE)
 endfunction()
@@ -497,15 +545,15 @@
 bool algebra::${_class_name}Maker::can_get(deg_t width, deg_t depth, const scalars::ScalarType* ctype, const preference_list& preferences) const {
     return s_la_contexts.find(std::make_tuple(width, depth, ctype)) != s_la_contexts.end();
 }
 
 algebra::context_pointer algebra::${_class_name}Maker::get_context(deg_t width, deg_t depth, const scalars::ScalarType* ctype, const preference_list& preferences) const {
     auto found = s_la_contexts.find(std::make_tuple(width, depth, ctype));
     if (found == s_la_contexts.end()) {
-        throw std::runtime_error(\"cannot get context\");
+        RPY_THROW(std::runtime_error, \"cannot get context\");
     }
     return found->second;
 }
 
 optional<algebra::base_context_pointer> algebra::${_class_name}Maker::get_base_context(deg_t width, deg_t depth) const {
     for (const auto& item : s_la_contexts) {
         if (std::get<0>(item.first) == width && std::get<1>(item.first) == depth) {
```

### Comparing `roughpy-0.0.4/core/include/roughpy/core/alloc.h` & `roughpy-0.0.5/core/include/roughpy/core/alloc.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/core/include/roughpy/core/helpers.h` & `roughpy-0.0.5/core/include/roughpy/core/helpers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/core/include/roughpy/core/macros.h` & `roughpy-0.0.5/core/include/roughpy/core/macros.h`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 #ifndef ROUGHPY_CORE_MACROS_H
 #define ROUGHPY_CORE_MACROS_H
 
 #include <cassert>
 #include <stdexcept>
 #include <string>
+#include <sstream>
 
 #ifdef __has_builtin
 #  define RPY_HAS_BUILTIN(x) __has_builtin(x)
 #else
 #  define RPY_HAS_BUILTIN(x) 0
 #endif
 
@@ -57,14 +58,26 @@
 
 #ifdef __has_include
 #  define RPY_HAS_INCLUDE(x) __has_include(x)
 #else
 #  define RPY_HAS_INCLUDE(x) 0
 #endif
 
+/*
+ * MSVC has a bug where it treats __VA_ARGS__ as a single token in argument
+ * lists. To combat this, we use RPY_INVOKE_VA to invoke the overload macro with
+ * the __VA_ARGS__ in the token stream so that proper expansion occurs.
+ * See: https://stackoverflow.com/a/9338429
+ */
+#define RPY_INVOKE_VA(X, Y) X Y
+
+#define RPY_COUNT_ARGS_1(_4, _3, _2, _1, count, ...) count
+#define RPY_COUNT_ARGS(...) \
+    RPY_INVOKE_VA(RPY_COUNT_ARGS_1, (__VA_ARGS__, 4, 3, 2, 1, 0))
+
 #define RPY_STRINGIFY_IMPL(ARG) #ARG
 #define RPY_STRINGIFY(ARG) RPY_STRINGIFY_IMPL(ARG)
 
 #define RPY_JOIN_IMPL_IMPL(LHS, RHS) LHS##RHS
 #define RPY_JOIN_IMPL(LHS, RHS) RPY_JOIN_IMPL_IMPL(LHS, RHS)
 #define RPY_JOIN(LHS, RHS) RPY_JOIN_IMPL(LHS, RHS)
 
@@ -320,30 +333,56 @@
  *
  * Optionally, one can provide a message string literal that will be used
  * instead of the default, and an optional error type. The default error type
  * is a std::runtime_error.
  */
 namespace rpy {
 namespace errors {
+
 template <typename E>
-RPY_NO_RETURN RPY_INLINE_ALWAYS void
-check_fail(const char* msg, const char* filename, int lineno, const char* func)
+RPY_NO_RETURN RPY_INLINE_ALWAYS void throw_exception(
+        std::string msg, const char* filename, int lineno, const char* func
+)
 {
-    throw E(std::string(msg) + " at lineno " + std::to_string(lineno) + " in "
-            + filename + " in function " + func);
+    std::stringstream ss;
+    ss << msg
+       << " at lineno "
+       << lineno
+       << " in "
+       << filename
+       << " in function "
+       << func;
+    throw E(ss.str());
 }
+
+template <typename E>
+RPY_NO_RETURN RPY_INLINE_ALWAYS void throw_exception(
+        const char* msg, const char* filename, int lineno, const char* func
+)
+{
+    std::stringstream ss;
+    ss << msg
+       << " at lineno "
+       << lineno
+       << " in "
+       << filename
+       << " in function "
+       << func;
+    throw E(ss.str());
+}
+
 }// namespace errors
 }// namespace rpy
 
 // Dispatch the check macro on the number of arguments
 // See: https://stackoverflow.com/a/16683147/9225581
 #define RPY_CHECK_3(EXPR, MSG, TYPE)                                           \
     do {                                                                       \
         if (RPY_UNLIKELY(!(EXPR))) {                                           \
-            ::rpy::errors::check_fail<TYPE>(                                   \
+            ::rpy::errors::throw_exception<TYPE>(                              \
                     MSG, __FILE__, __LINE__, RPY_FUNC_NAME                     \
             );                                                                 \
         }                                                                      \
     } while (0)
 
 #define RPY_CHECK_2(EXPR, MSG) RPY_CHECK_3(EXPR, MSG, std::runtime_error)
 
@@ -351,17 +390,31 @@
 
 #define RPY_CHECK_CNT_IMPL(_1, _2, _3, COUNT, ...) COUNT
 // Always pass one more argument than expected, so clang doesn't complain about
 // empty parameter packs.
 #define RPY_CHECK_CNT(...) RPY_CHECK_CNT_IMPL(__VA_ARGS__, 3, 2, 1, 0)
 #define RPY_CHECK_SEL(NUM) RPY_JOIN(RPY_CHECK_, NUM)
 
-#define RPY_CHECK(...) RPY_CHECK_SEL(RPY_CHECK_CNT(__VA_ARGS__))(__VA_ARGS__)
+#define RPY_CHECK(...) RPY_INVOKE_VA( \
+    RPY_CHECK_SEL(RPY_COUNT_ARGS(__VA_ARGS__)), \
+    (__VA_ARGS__))
+
+#define RPY_THROW_2(EXC_TYPE, MSG)                                             \
+    ::rpy::errors::throw_exception<EXC_TYPE>(                                  \
+            MSG, __FILE__, __LINE__, RPY_FUNC_NAME                             \
+    )
+#define RPY_THROW_1(MSG) RPY_THROW_2(std::runtime_error, MSG)
+
+#define RPY_THROW_SEL(NUM) RPY_JOIN(RPY_THROW_, NUM)
+#define RPY_THROW_CNT_IMPL(_1, _2, COUNT, ...) COUNT
+#define RPY_THROW_CNT(...) RPY_THROW_CNT_IMPL(__VA_ARGS__, 2, 1, 0)
+#define RPY_THROW(...) RPY_INVOKE_VA( \
+    RPY_THROW_SEL(RPY_COUNT_ARGS(__VA_ARGS__)), \
+    (__VA_ARGS__))
 
 #ifdef RPY_DEBUG
 #  define RPY_DBG_ASSERT(ARG) assert(ARG)
 #else
 #  define RPY_DBG_ASSERT(ARG) (void) 0
 #endif
 
-
 #endif// ROUGHPY_CORE_MACROS_H
```

### Comparing `roughpy-0.0.4/core/include/roughpy/core/slice.h` & `roughpy-0.0.5/core/include/roughpy/core/slice.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/core/include/roughpy/core/traits.h` & `roughpy-0.0.5/core/include/roughpy/core/traits.h`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
 #include <boost/container_hash/hash.hpp>
 
 namespace rpy {
 
 using std::declval;
 using std::integral_constant;
+using std::move;
+using std::forward;
 
 using std::is_array;
 using std::is_class;
 using std::is_enum;
 using std::is_floating_point;
 using std::is_function;
 using std::is_integral;
@@ -128,16 +130,20 @@
 using boost::detected_t;
 using boost::remove_cv_ref_t;
 
 using boost::is_detected;
 
 #ifdef RPY_CPP_17
 using std::void_t;
+using std::invoke_result_t;
 #else
 using boost::void_t;
+
+template <typename F, typename... ArgTypes>
+using invoke_result_t = std::result_of_t<F(ArgTypes...)>;
 #endif
 
 /**
  * @brief Ensure that the type T is a pointer.
  *
  * Makes T a pointer if it isn't already a pointer.
  */
```

### Comparing `roughpy-0.0.4/core/include/roughpy/core/types.h` & `roughpy-0.0.5/core/include/roughpy/core/types.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/CMakeLists.txt` & `roughpy-0.0.5/device/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/cuda/CudaDeviceContext.cuh` & `roughpy-0.0.5/device/cuda/CudaDeviceContext.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/cuda/scalars/src/CUDAFloatType.cuh` & `roughpy-0.0.5/device/cuda/scalars/src/CUDAFloatType.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/cuda/scalars/src/CUDA_standard_scalar.cuh` & `roughpy-0.0.5/device/cuda/scalars/src/CUDA_standard_scalar.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -154,30 +154,30 @@
     } else if (dst.type() == host_type && src.type() == this) {
         handle_error(copy_from_device(dst.ptr(), src.cptr(), count));
     } else if (dst.type() == this) {
         std::vector<S> tmp(count);
 
         if (src.type() == nullptr) {
             if (!src.is_simple_integer()) {
-                throw std::runtime_error("unknown scalar type, cannot convert");
+                RPY_THROW(std::runtime_error, "unknown scalar type, cannot convert");
             }
 
             host_type->convert_copy({host_type, tmp.data()}, src, count);
         } else {
             src.type()->convert_copy({host_type, tmp.data()}, src, count);
         }
 
         handle_error(copy_to_device(dst.ptr(), tmp.data(), count));
     } else if (src.type() == this) {
         std::vector<S> tmp(count);
         handle_error(copy_from_device(tmp.data(), src.cptr(), count));
         dst.type()->convert_copy(dst, {host_type, tmp.data()}, count);
     } else {
         if (dst.type() == nullptr) {
-            throw std::runtime_error("destination type is null");
+            RPY_THROW(std::runtime_error, "destination type is null");
         }
         dst.type()->convert_copy(dst, src, count);
     }
 }
 template <typename S>
 void CUDAScalarType<S>::convert_copy(
         void* out, const void* in, std::size_t count, BasicScalarInfo info
```

### Comparing `roughpy-0.0.4/device/include/roughpy/device/core.h` & `roughpy-0.0.5/device/include/roughpy/device/core.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/include/roughpy/device/device_algebra_base.h` & `roughpy-0.0.5/device/include/roughpy/device/device_algebra_base.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/include/roughpy/device/device_context.h` & `roughpy-0.0.5/device/include/roughpy/device/device_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/kernels/binary_kernel.cuh` & `roughpy-0.0.5/device/kernels/binary_kernel.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/kernels/functors.h` & `roughpy-0.0.5/device/kernels/functors.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/kernels/tmp.cu` & `roughpy-0.0.5/device/kernels/tmp.cu`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/kernels/unary_kernel.cuh` & `roughpy-0.0.5/device/kernels/unary_kernel.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/src/device_algebra_base.cpp` & `roughpy-0.0.5/device/src/device_algebra_base.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/src/device_context.cpp` & `roughpy-0.0.5/device/src/device_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/src/device_free_tensor.cpp` & `roughpy-0.0.5/device/src/device_free_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/device/src/device_free_tensor.h` & `roughpy-0.0.5/device/src/device_free_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/docs/make.bat` & `roughpy-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/docs/source/conf.py` & `roughpy-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/examples/lie_to_tensor_formulae.py` & `roughpy-0.0.5/examples/lie_to_tensor_formulae.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/.clang-format` & `roughpy-0.0.5/external/libalgebra/.clang-format`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/.gitignore` & `roughpy-0.0.5/external/libalgebra/.gitignore`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/Dockerfile` & `roughpy-0.0.5/external/libalgebra/Dockerfile`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/Dockerfile.remote-cpp-env` & `roughpy-0.0.5/external/libalgebra/Dockerfile.remote-cpp-env`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/README.md` & `roughpy-0.0.5/external/libalgebra/README.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/benchmarks/antipode/antipode_bm.cpp` & `roughpy-0.0.5/external/libalgebra/benchmarks/antipode/antipode_bm.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/benchmarks/multiplication/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp` & `roughpy-0.0.5/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp` & `roughpy-0.0.5/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/cmake/Modules/FindBignum.cmake` & `roughpy-0.0.5/external/libalgebra/cmake/Modules/FindBignum.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP.cmake` & `roughpy-0.0.5/external/libalgebra/cmake/Modules/UnitTestPP.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake` & `roughpy-0.0.5/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/cmake/libalgebra_test_helper.cmake` & `roughpy-0.0.5/external/libalgebra/cmake/libalgebra_test_helper.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/_tensor_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/_tensor_basis.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/alg_types.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/alg_types.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/algebra.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/algebra.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/alternative_multiplications.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/alternative_multiplications.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/area_tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_multiplication.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/area_tensor_multiplication.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/base_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/base_basis.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/base_vector.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/base_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 05/02/2021.
 //
 
 #ifndef LIBALGEBRA_BASE_VECTOR_H
 #define LIBALGEBRA_BASE_VECTOR_H
 
 #include "libalgebra/basis.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/basis.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 09/02/2021.
 //
 
 #ifndef LIBALGEBRA_BASIS_H
 #define LIBALGEBRA_BASIS_H
 
 #include "implementation_types.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/coefficients/gmp_ser.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/coefficients/gmp_ser.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 26/10/2021.
 //
 
 #ifndef GMP_SER_GMP_SER_H
 #define GMP_SER_GMP_SER_H
 
 #include <gmp.h>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/coefficients.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/coefficients.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 25/06/2021.
 //
 
 #ifndef LIBALGEBRA_COEFFICIENTS_H
 #define LIBALGEBRA_COEFFICIENTS_H
 
 #include "detail/meta.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/composition_operator.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/composition_operator.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 28/01/2022.
 //
 
 #ifndef LIBALGEBRA_COMPOSITION_OPERATOR_H
 #define LIBALGEBRA_COMPOSITION_OPERATOR_H
 
 namespace alg {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/constlog2.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/constlog2.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/constpower.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/constpower.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/dense_storage.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/dense_storage.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 04/08/2021.
 //
 
 #ifndef LIBALGEBRA_DENSE_STORAGE_H
 #define LIBALGEBRA_DENSE_STORAGE_H
 
 #include <cassert>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/dense_vector.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/dense_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 08/02/2021.
 //
 
 #ifndef LIBALGEBRA_DENSE_VECTOR_H
 #define LIBALGEBRA_DENSE_VECTOR_H
 
 #include <utility>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/caching_tags.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/caching_tags.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 22/11/2021.
 //
 
 #ifndef LIBALGEBRA_CACHING_TAGS_H
 #define LIBALGEBRA_CACHING_TAGS_H
 
 namespace alg {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/function_extension_cache_base.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/function_extension_cache_base.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 20/01/2022.
 //
 
 #ifndef LIBALGEBRA_FUNCTION_EXTENSION_CACHE_BASE_H
 #define LIBALGEBRA_FUNCTION_EXTENSION_CACHE_BASE_H
 
 #include <map>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/integer_maths.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/integer_maths.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 10/02/2021.
 //
 
 #ifndef LIBALGEBRAUNITTESTS_INTEGER_MATHS_H
 #define LIBALGEBRAUNITTESTS_INTEGER_MATHS_H
 
 namespace alg {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/level_walkers.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/level_walkers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/meta.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/meta.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 08/02/2021.
 //
 
 #ifndef LIBALGEBRA_META_H
 #define LIBALGEBRA_META_H
 
 #include <array>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/platform.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/platform.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/reversing_permutation.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/reversing_permutation.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/smallest_int_type.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/smallest_int_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/dot_product_implementations.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/dot_product_implementations.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/free_extension.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/free_extension.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 22/11/2021.
 //
 
 #ifndef LIBALGEBRA_FREE_EXTENSION_H
 #define LIBALGEBRA_FREE_EXTENSION_H
 
 #include <map>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/functionals.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/functionals.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 16/11/2021.
 //
 
 #ifndef LIBALGEBRA_FUNCTIONALS_H
 #define LIBALGEBRA_FUNCTIONALS_H
 
 #include "implementation_types.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurko and Arend Janssen, Sam Morley
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/hall_set.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/hall_set.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 23/09/2021.
 //
 
 #ifndef LIBALGEBRA_HALL_SET_H
 #define LIBALGEBRA_HALL_SET_H
 
 #include <cassert>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/hybrid_vector.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/hybrid_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 12/02/2021.
 //
 
 #ifndef LIBALGEBRA_HYBRID_VECTOR_H
 #define LIBALGEBRA_HYBRID_VECTOR_H
 
 #include <algorithm>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/implementation_types.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/implementation_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/iterators.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/iterators.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 17/02/2021.
 //
 
 #ifndef LIBALGEBRA_VECTORS_ITERATORS_H
 #define LIBALGEBRA_VECTORS_ITERATORS_H
 
 #include <iterator>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/key_iterators.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/key_iterators.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 16/11/2021.
 //
 
 #ifndef LIBALGEBRA_KEY_ITERATORS_H
 #define LIBALGEBRA_KEY_ITERATORS_H
 
 #include <iterator>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/libalgebra.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/libalgebra.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
 
@@ -100,15 +100,18 @@
 template<typename Coeff, DEG n_letters, DEG max_degree = 0,
          template<typename, typename, typename...> class VectorType = vectors::template_vector_type_selector<free_tensor_basis<n_letters, max_degree>, Coeff>::template type,
          template <DEG, DEG> class FTMultiplication=free_tensor_multiplication,
          typename...>
 class free_tensor;
 
 /// Free Associative Shuffle Algebra.  Associative and Commutative.
-template<typename Coeff, DEG n_letters, DEG max_degree = 0, typename...>
+template<typename Coeff, DEG n_letters, DEG max_degree = 0,
+         template<typename, typename, typename...> class VectorType = vectors::template_vector_type_selector<shuffle_tensor_basis<n_letters, max_degree>, Coeff>::template type,
+         typename...
+         >
 class shuffle_tensor;
 
 /// Philip Hall Lie Basis.
 template<DEG n_letters, DEG MaxDegree>
 class hall_basis;
 
 /// Free Lie Associative Algebra Basis.  Associative and non commutative.
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/lie.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/lie.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/lie_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/lie_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/lie_inner_product.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/lie_inner_product.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 21/01/2022.
 //
 
 #ifndef LIBALGEBRA_LIE_INNER_PRODUCT_H
 #define LIBALGEBRA_LIE_INNER_PRODUCT_H
 
 #include "implementation_types.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/monomial_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/monomial_basis.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/mpfloat_coefficients.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/mpfloat_coefficients.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 24/01/2022.
 //
 
 #ifndef LIBALGEBRA_MPFLOAT_COEFFICIENTS_H
 #define LIBALGEBRA_MPFLOAT_COEFFICIENTS_H
 
 #include "implementation_types.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/multi_linear_operators.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/multi_linear_operators.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 21/01/2022.
 //
 
 #ifndef LIBALGEBRA_MULTI_LINEAR_OPERATORS_H
 #define LIBALGEBRA_MULTI_LINEAR_OPERATORS_H
 
 #include <libalgebra/vector_bundle.h>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/multi_polynomial.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/multi_polynomial.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/multiplication_helpers.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/multiplication_helpers.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 05/07/2021.
 //
 
 #ifndef LIBALGEBRA_MULTIPLICATION_HELPERS_H
 #define LIBALGEBRA_MULTIPLICATION_HELPERS_H
 
 namespace alg {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/operators.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/operators.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 29/10/2021.
 //
 
 #ifndef LIBALGEBRA_OPERATORS_H
 #define LIBALGEBRA_OPERATORS_H
 
 #include <type_traits>
@@ -205,28 +205,29 @@
                             const T* LA_RESTRICT param,
                             const DIMN* powers,
                             const DIMN* sizes,
                             DEG param_deg,
                             DEG arg_deg)
     {
         if (param_deg < arg_deg) {
+            auto* out_ptr = out;
             for (DEG d = param_deg; d <= arg_deg; ++d) {
                 auto result_deg = d - param_deg;
-                auto* out_ptr = out + sizes[result_deg - 1];
 
                 for (DIMN param_idx = 0; param_idx < powers[param_deg]; ++param_idx) {
                     const auto* in_ptr = in + param_idx * powers[result_deg];
                     const auto& param_val = param[param_idx];
 
                     for (DIMN i = 0; i < powers[result_deg]; ++i) {
                         out_ptr[i] += param_val * in_ptr[i];
                     }
                 }
 
                 in += powers[d];
+                out_ptr += powers[result_deg];
             }
         }
         else {
             auto& unit = out[0];
 
             for (DIMN i=0; i<powers[param_deg]; ++i) {
                 unit += param[i]*in[i];
@@ -282,15 +283,15 @@
         const auto& param_unit = param_ptr[0];
         if (param_unit != typename C::S(0)) {
             for (DIMN i = 0; i < arg.dimension(); ++i) {
                 out_ptr[i] = param_unit * arg_ptr[i];
             }
         }
 
-        for (DEG prefix_deg = 1; prefix_deg < lower_deg; ++prefix_deg) {
+        for (DEG prefix_deg = 1; prefix_deg <= lower_deg; ++prefix_deg) {
             arg_ptr += tsi::powers[prefix_deg - 1];
             param_ptr += tsi::powers[prefix_deg - 1];
 
             eval_single(out_ptr, arg_ptr, param_ptr, tsi::powers.data(), tsi::degree_sizes.data(), prefix_deg, arg_deg);
         }
     }
 };
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/poly_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/poly_basis.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/poly_lie.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/poly_lie_basis.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/polynomial_coefficients.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/polynomial_coefficients.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/polynomials.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/polynomials.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/rational_coefficients.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/rational_coefficients.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 15/10/2021.
 //
 
 #ifndef LIBALGEBRA_RATIONAL_COEFFICIENTS_H
 #define LIBALGEBRA_RATIONAL_COEFFICIENTS_H
 
 #ifndef LIBALGEBRA_NO_GMP
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/reconfigure_operator.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/reconfigure_operator.h`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 class recalibrate<change_depth<NewDepth>, Base> : Base
 {
     using old_type = typename Base::type;
 
     template<typename C, DEG W, DEG OD, template<typename, typename, typename...> class V, template<DEG, DEG> class M, typename... Args>
     static free_tensor<C, W, NewDepth, V, M, Args...> f(free_tensor<C, W, OD, V, M, Args...>& a);
 
-    template<typename C, DEG W, DEG OD, typename... Args>
-    static shuffle_tensor<C, W, NewDepth, Args...> f(shuffle_tensor<C, W, OD, Args...>& a);
+    template<typename C, DEG W, DEG OD, template<typename, typename, typename...> class V, typename... Args>
+    static shuffle_tensor<C, W, NewDepth, V, Args...> f(shuffle_tensor<C, W, OD, V, Args...>& a);
 
     template<typename C, DEG W, DEG OD, template<typename, typename, typename...> class V, typename... Args>
     static lie<C, W, NewDepth, V, Args...> f(lie<C, W, OD, V, Args...>& a);
 
 public:
     using type = decltype(f(std::declval<old_type&>()));
 };
@@ -61,16 +61,16 @@
 class recalibrate<change_coeffs<NewCoeffs>, Base> : Base
 {
     using old_type = typename Base::type;
 
     template<typename C, DEG W, DEG D, template<typename, typename, typename...> class V, template<DEG, DEG> class M, typename... Args>
     static free_tensor<NewCoeffs, W, D, V, M, Args...> f(free_tensor<C, W, D, V, M, Args...>& a);
 
-    template<typename C, DEG W, DEG D, typename... Args>
-    static shuffle_tensor<NewCoeffs, W, D, Args...> f(shuffle_tensor<C, W, D, Args...>& a);
+    template<typename C, DEG W, DEG D,template<typename, typename, typename...> class V, typename... Args>
+    static shuffle_tensor<NewCoeffs, W, D,V, Args...> f(shuffle_tensor<C, W, D,V, Args...>& a);
 
     template<typename C, DEG W, DEG D, template<typename, typename, typename...> class V, typename... Args>
     static lie<NewCoeffs, W, D, V, Args...> f(lie<C, W, D, V, Args...>& a);
 
 
 public:
     using type = decltype(f(std::declval<old_type&>()));
@@ -80,16 +80,16 @@
 class recalibrate<change_storage<NewVType, NewVArgs...>, Base> : Base
 {
     using old_type = typename Base::type;
 
     template<typename C, DEG W, DEG D, template<typename, typename, typename...> class V, template<DEG, DEG> class M, typename... Args>
     static free_tensor<C, W, D, NewVType, M, NewVArgs...> f(free_tensor<C, W, D, V, M, Args...>& a);
 
-    template<typename C, DEG W, DEG D, typename... Args>
-    static shuffle_tensor<C, W, D, Args...> f(shuffle_tensor<C, W, D, Args...>& a);
+    template<typename C, DEG W, DEG D,template<typename, typename, typename...> class V, typename... Args>
+    static shuffle_tensor<C, W, D,V, Args...> f(shuffle_tensor<C, W, D, V, Args...>& a);
 
     template<typename C, DEG W, DEG D, template<typename, typename, typename...> class V, typename... Args>
     static lie<C, W, D, NewVType, NewVArgs...> f(lie<C, W, D, V, Args...>& a);
 
 
 public:
     using type = decltype(f(std::declval<old_type&>()));
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/scalar_bundle.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/scalar_bundle.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/scalar_multiply_operator.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/scalar_multiply_operator.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 27/01/2022.
 //
 
 #ifndef LIBALGEBRA_SCALAR_MULTIPLY_OPERATOR_H
 #define LIBALGEBRA_SCALAR_MULTIPLY_OPERATOR_H
 
 #include <utility>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/sparse_vector.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/sparse_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
 
 ************************************************************* */
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/sum_operator.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/sum_operator.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 27/01/2022.
 //
 
 #ifndef LIBALGEBRA_SUM_OPERATOR_H
 #define LIBALGEBRA_SUM_OPERATOR_H
 
 namespace alg {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/tags.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/tags.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 09/02/2021.
 //
 
 #ifndef LIBALGEBRA_TAGS_H
 #define LIBALGEBRA_TAGS_H
 
 #include <type_traits>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/tensor.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/tensor.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
 
@@ -2659,15 +2659,17 @@
 using area_tensor_multiplication =
         base_multiplication<area_tensor_multiplier<Width, Depth>>;
 
 template<DEG Width, DEG Depth>
 using shuffle_tensor_multiplication =
         base_multiplication<shuffle_tensor_multiplier<Width, Depth>>;
 
-template<typename Coeff, DEG n_letters, DEG max_degree, typename...>
+template<typename Coeff, DEG n_letters, DEG max_degree,
+         template <typename, typename, typename...> class VectorType,
+        typename...>
 class shuffle_tensor;
 
 /**
  * @brief A specialisation of the algebra class with a free tensor basis.
  *
  * Mathematically, the algebra of free_tensor instances is a free associative
  * algebra. With respect to the inherited algebra class, the essential
@@ -2970,29 +2972,34 @@
  * this class is the basis class used, and in particular the basis::prod()
  * member function. Thus, the most important information is in the definition
  * of shuffle_tensor_basis. Notice that this associative algebra of free
  * tensors includes as a sub-algebra the associative algebra corresponding to
  * the SCALAR type. This is permitted by the existence of empty keys in
  * shuffle_tensor_basis.
  */
-template<typename Coeff, DEG n_letters, DEG max_degree, typename...>
+template<typename Coeff, DEG n_letters, DEG max_degree,
+         template <typename, typename, typename...> class VectorType,
+         typename... ExtraArgs>
 class shuffle_tensor : public algebra<
                                shuffle_tensor_basis<n_letters, max_degree>,
                                Coeff,
-                               shuffle_tensor_multiplication<n_letters, max_degree>>
+                               shuffle_tensor_multiplication<n_letters, max_degree>,
+                               VectorType,
+                               shuffle_tensor<Coeff, n_letters, max_degree, VectorType, ExtraArgs...>
+                               >
 {
     typedef shuffle_tensor_multiplication<n_letters, max_degree> multiplication_t;
 
 public:
     /// The basis type.
     typedef shuffle_tensor_basis<n_letters, max_degree> BASIS;
     /// Import of the KEY type.
     typedef typename BASIS::KEY KEY;
     /// The algebra type.
-    typedef algebra<BASIS, Coeff, multiplication_t> ALG;
+    typedef algebra<BASIS, Coeff, multiplication_t, VectorType, shuffle_tensor> ALG;
 
     typedef typename Coeff::SCA SCA;
     typedef typename Coeff::RAT RAT;
 
     /// The sparse_vector type.
     typedef typename ALG::VECT VECT;
 
@@ -3010,18 +3017,18 @@
 
     /// Copy constructor.
     shuffle_tensor(const shuffle_tensor& t)
         : ALG(t)
     {}
 
     /// Constructs an instance from a free_tensor instance.
-    template<template<typename, typename, typename...> class VectorType, template <DEG, DEG> class FTM, typename... Args>
-    shuffle_tensor(const free_tensor<Coeff, n_letters, max_degree, VectorType, FTM, Args...>& t)
+    template<template<typename, typename, typename...> class OVectorType, template <DEG, DEG> class FTM, typename... Args>
+    shuffle_tensor(const free_tensor<Coeff, n_letters, max_degree, OVectorType, FTM, Args...>& t)
     {
-        typename free_tensor<Coeff, n_letters, max_degree, VectorType, FTM, Args...>::const_iterator i;
+        typename free_tensor<Coeff, n_letters, max_degree, OVectorType, FTM, Args...>::const_iterator i;
         for (i = t.begin(); i != t.end(); ++i) {
             (*this)[i->key()] += i->value();
         }
     }
 
     /// Constructs an instance from an algebra instance.
     shuffle_tensor(const ALG& a)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/tensor_basis.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/tensor_basis.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/tensor_operator.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/tensor_operator.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 27/01/2022.
 //
 /**
  * This is an implementation of a useful fact that the space of linear operators
  * from a vector space U to a vector space V can be identified with the tensor
  * product of U* (the dual of U) tensor product with V. Under this identification
  * the elementary tensor u* tensor v is identified with the operator
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/utils.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/utils.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿/* *************************************************************
+/* *************************************************************
 
 Copyright 2010 Terry Lyons, Stephen Buckley, Djalil Chafai,
 Greg Gyurkó and Arend Janssen.
 
 Distributed under the terms of the GNU General Public License,
 Version 3. (See accompanying file License.txt)
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/vector.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 01/02/2021.
 //
 
 #ifndef LIBALGEBRA_VECTOR_H
 #define LIBALGEBRA_VECTOR_H
 
 #include "implementation_types.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/vector_bundle.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/vector_bundle.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/libalgebra/vectors.h` & `roughpy-0.0.5/external/libalgebra/libalgebra/vectors.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿//
+//
 // Created by sam on 01/02/2021.
 //
 
 #ifndef LIBALGEBRA_VECTORS_H
 #define LIBALGEBRA_VECTORS_H
 
 #include "basis.h"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roughpy-0.0.4/external/libalgebra/tests/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/tests/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/SHOW.h` & `roughpy-0.0.5/external/libalgebra/tests/common/SHOW.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/compat.h` & `roughpy-0.0.5/external/libalgebra/tests/common/compat.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/helpers.h` & `roughpy-0.0.5/external/libalgebra/tests/common/helpers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/memfile.cpp` & `roughpy-0.0.5/external/libalgebra/tests/common/memfile.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/memfile.h` & `roughpy-0.0.5/external/libalgebra/tests/common/memfile.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/multi_test.h` & `roughpy-0.0.5/external/libalgebra/tests/common/multi_test.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/random_coeffs.h` & `roughpy-0.0.5/external/libalgebra/tests/common/random_coeffs.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/random_vector_generator.h` & `roughpy-0.0.5/external/libalgebra/tests/common/random_vector_generator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/reporter.cpp` & `roughpy-0.0.5/external/libalgebra/tests/common/reporter.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/reporter.h` & `roughpy-0.0.5/external/libalgebra/tests/common/reporter.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/rng.h` & `roughpy-0.0.5/external/libalgebra/tests/common/rng.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/run_tests.cpp` & `roughpy-0.0.5/external/libalgebra/tests/common/run_tests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/simple_basis.h` & `roughpy-0.0.5/external/libalgebra/tests/common/simple_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/common/time_and_details.h` & `roughpy-0.0.5/external/libalgebra/tests/common/time_and_details.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/HallSetTests.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/HallSetTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/LatticePathTests.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/LatticePathTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/SigHelpers.h` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/SigHelpers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/TreeBufferHelper.h` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/TreeBufferHelper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/brown_path_increments.h` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/brown_path_increments.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/categorical_path.h` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/categorical_path.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/makebm.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/makebm.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/speed_tests.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/speed_tests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/integration_tests/x64sigs.cpp` & `roughpy-0.0.5/external/libalgebra/tests/integration_tests/x64sigs.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         using key_type = typename tensor_basis::KEY;
         tensor_basis basis;
 
         using tensor_type = alg::free_tensor<coeff_ring, width, depth>;
 
         using shuffle_tensor_type = alg::shuffle_tensor<coeff_ring, width, depth>;
 
-        using operator_type = operators::dtl::adjoint_of_left_multiplication_operator_impl<tensor_type>;
+        template <typename T>
+        using operator_type = operators::dtl::adjoint_of_left_multiplication_operator_impl<T>;
 
         using sparse_traditional_tensor = alg::algebra<tensor_basis, coeff_ring, traditional_multiplication, alg::vectors::sparse_vector>;
         using dense_traditional_tensor = alg::algebra<tensor_basis, coeff_ring, traditional_multiplication, alg::vectors::dense_vector>;
 
         scalar_type construct_expected(key_type key, LET lhs_offset, LET rhs_offset, DEG lhs_max = depth, DEG rhs_max = depth) const
         {
             auto deg = key.size();
@@ -119,14 +120,25 @@
 
             for (auto key : basis.iterate_keys_to_deg(max_degree + 1)) {
                 result[key] = to_poly_key(key, offset);
             }
             return result;
         }
 
+        template <template <typename, typename, typename...> class VT>
+        alg::shuffle_tensor<coeff_ring, Width, Depth, VT> generic_shuffle_tensor(LET offset = 0, DEG max_degree = depth) const
+        {
+            alg::shuffle_tensor<coeff_ring, Width, Depth, VT> result;
+
+            for (auto key : basis.iterate_keys_to_deg(max_degree + 1)) {
+                result[key] = to_poly_key(key, offset);
+            }
+            return result;
+        }
+
         tensor_type generic_tensor(LET offset = 0, DEG max_degree = depth) const
         {
             tensor_type result;
 
             for (auto key : basis.iterate_keys_to_deg(max_degree + 1)) {
                 result[key] = to_poly_key(key, offset);
             }
@@ -140,16 +152,17 @@
 
             for (auto key : basis.iterate_keys_to_deg(max_degree + 1)) {
                 result[key] = to_poly_key(key, offset);
             }
             return result;
         }
 
-        shuffle_tensor_type construct_expected(LET tensor_offset, LET shuffle_offset) {
-            shuffle_tensor_type result;
+        template <typename Shuffle=shuffle_tensor_type>
+        Shuffle construct_expected(LET tensor_offset, LET shuffle_offset) {
+            Shuffle result;
 
             for (auto&& key : basis.iterate_keys()) {
                 for (DEG i=0; i<=key.size(); ++i) {
                     auto right(key);
                     auto left = right.split_n(i);
                     result.add_scal_prod(right, to_poly_key(left, tensor_offset) * to_poly_key(key, shuffle_offset));
                 }
@@ -177,40 +190,53 @@
     using PolyMultiplicationTests55 = PolyMultiplicationTests<5, 5>;
     TEST_FIXTURE(PolyMultiplicationTests55, IdentityTest)
     {
 
         tensor_type this_tensor(scalar_type(1));
         shuffle_tensor_type this_shuffle_tensor(scalar_type(1));
 
-        operator_type adjoint(this_tensor);
+        operator_type<tensor_type> adjoint(this_tensor);
 
         CHECK_EQUAL(this_shuffle_tensor, adjoint(this_shuffle_tensor));
 
 
     }
 
     TEST_FIXTURE(PolyMultiplicationTests55, PolynomialTest)
     {
 
         tensor_type this_tensor(scalar_type(1));
         shuffle_tensor_type this_shuffle_tensor = generic_shuffle_tensor(2);
 
-        operator_type adjoint(this_tensor);
+        operator_type<tensor_type> adjoint(this_tensor);
 
         CHECK_EQUAL(this_shuffle_tensor, adjoint(this_shuffle_tensor));
 
 
     }
 
 
     TEST_FIXTURE(PolyMultiplicationTests55, FullTest) {
         tensor_type this_tensor(generic_tensor(1));
         shuffle_tensor_type  this_shuffle_tensor(generic_shuffle_tensor(2));
 
-        operator_type adjoint(this_tensor);
+        operator_type<tensor_type> adjoint(this_tensor);
 
         auto expected = construct_expected(1, 2);
 
         CHECK_EQUAL(expected, adjoint(this_shuffle_tensor));
     }
 
+    TEST_FIXTURE(PolyMultiplicationTests55, FullTestDense) {
+        auto this_tensor(generic_tensor<traditional_multiplication, alg::vectors::dense_vector>(1));
+        auto this_shuffle_tensor(generic_shuffle_tensor<alg::vectors::dense_vector>(2));
+
+        operator_type<decltype(this_tensor)> adjoint(this_tensor);
+
+        auto expected = construct_expected<decltype(this_shuffle_tensor)>(1, 2);
+
+        auto adj = adjoint(this_shuffle_tensor);
+//        CHECK_EQUAL(expected, adj);
+        CHECK_EQUAL(decltype(this_shuffle_tensor)(), expected-adj);
+    }
+
 }// SUITE adjoint
```

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_basis.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/fixture.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/framework_fixture.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/framework_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_dense.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp` & `roughpy-0.0.5/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra_lite/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #set(CMAKE_CXX_STANDARD 14)
 #set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set_property(GLOBAL PROPERTY USE_FOLDERS ON)
 
 include(GenerateExportHeader)
 include(GNUInstallDirs)
 
+option(LIBALGEBRA_LITE_BUILD_TESTS OFF "Build tests for libalgebra lite")
 
 find_package(Boost REQUIRED)
 
 add_library(Libalgebra_lite SHARED
         src/algebra/lie_multiplier.cpp
         src/algebra/polynomial_multiplier.cpp
         src/algebra/polynomial.cpp
@@ -96,21 +97,17 @@
 configure_file(cmake/config.h.in config.h NO_SOURCE_PERMISSIONS @ONLY)
 configure_file(cmake/rationals.h.in rationals.h NO_SOURCE_PERMISSIONS @ONLY)
 
 
 install(TARGETS Libalgebra_lite
         EXPORT Libalgebra_liteTargets
         PUBLIC_HEADER DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}/libalgebra_lite"
-        COMPONENT Development
-        EXCLUDE_FROM_ALL
         RUNTIME DESTINATION "${CMAKE_INSTALL_BINDIR}"
         LIBRARY DESTINATION "${CMAKE_INSTALL_LIBDIR}"
         ARCHIVE DESTINATION "${CMAKE_INSTALL_LIBDIR}"
-        COMPONENT Development
-        EXCLUDE_FROM_ALL
         )
 install(DIRECTORY ${CMAKE_CURRENT_LIST_DIR}/include/libalgebra_lite
         DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}
         COMPONENT Development
         EXCLUDE_FROM_ALL
         )
 install(FILES ${CMAKE_CURRENT_BINARY_DIR}/config.h
@@ -143,9 +140,11 @@
         ${CMAKE_CURRENT_BINARY_DIR}/Libalgebra_liteConfig.cmake
         ${CMAKE_CURRENT_BINARY_DIR}/Libalgebra_liteVersion.cmake
         DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/Libalgebra_lite
         COMPONENT Development
         EXCLUDE_FROM_ALL
         )
 
-enable_testing()
-add_subdirectory(tests)
+if(CMAKE_IS_TOP_LEVEL OR LIBALGEBRA_LITE_BUILD_TESTS)
+    enable_testing()
+    add_subdirectory(tests)
+endif()
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/cmake/lalhelpers.cmake` & `roughpy-0.0.5/external/libalgebra_lite/cmake/lalhelpers.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/cmake/rationals.h.in` & `roughpy-0.0.5/external/libalgebra_lite/cmake/rationals.h.in`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/algebra.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/algebra.h`

 * *Files 5% similar despite different names*

```diff
@@ -708,14 +708,18 @@
     }
 
     std::shared_ptr<const multiplication_type> multiplication() const noexcept
     {
         return p_mult;
     }
 
+    algebra create_alike() const {
+        return algebra(this->get_basis(), p_mult);
+    }
+
     algebra& add_mul(const algebra& lhs, const algebra& rhs)
     {
         using traits = multiplication_traits<Multiplication>;
         traits::multiply_and_add(
                 *multiplication(), *this, lhs, rhs,
                 [](scalar_type s) { return s; }
         );
@@ -901,52 +905,40 @@
 }
 
 template <typename Algebra>
 enable_if_t<dtl::is_algebra<Algebra>::value, Algebra>
 commutator(const Algebra& lhs, const Algebra& rhs)
 {
     using traits = multiplication_traits<typename Algebra::multiplication_type>;
-    using cring = typename Algebra::coefficient_ring;
+    using scalar_type = typename Algebra::scalar_type;
 
     auto multiplication = lhs.multiplication();
     if (!multiplication) { multiplication = rhs.multiplication(); }
 
     Algebra result(lhs.get_basis(), multiplication);
     if (multiplication && !lhs.empty() && !rhs.empty()) {
         traits::multiply_and_add(*multiplication, result, lhs, rhs);
         traits::multiply_and_add(
-                *multiplication, result, rhs, lhs, cring::uminus
+                *multiplication, result, rhs, lhs, [](const scalar_type& arg) {
+                    return -arg;
+                }
         );
     }
     return result;
 }
 
-template <
-        typename Multiplication, typename Coefficients, typename LBasis,
-        template <typename, typename> class LVectorType,
-        template <typename> class LStorageModel, typename RBasis,
-        template <typename, typename> class RVectorType,
-        template <typename> class RStorageModel>
-enable_if_t<
-        multiplication_traits<Multiplication>::template compatible_with<
-                LBasis>::value
-                && multiplication_traits<Multiplication>::
-                        template compatible_with<RBasis>::value,
-        vector<LBasis, Coefficients, LVectorType, LStorageModel>>
-multiply(
-        const Multiplication& multiplication,
-        const vector<LBasis, Coefficients, LVectorType, LStorageModel>& lhs,
-        const vector<RBasis, Coefficients, RVectorType, RStorageModel>& rhs
-)
-{
-    using traits = multiplication_traits<Multiplication>;
-    vector<LBasis, Coefficients, LVectorType, LStorageModel> result(lhs.basis()
-    );
 
-    traits::multiply_and_add(multiplication, result, lhs, rhs);
 
+template <typename Multiplication, typename LVector, typename RVector>
+LVector multiply(const Multiplication& multiplication, const LVector& left,
+                 const
+                 RVector& right) {
+    using traits = multiplication_traits<Multiplication>;
+    LVector result = left.create_alike();
+    traits::multiply_and_add(multiplication, result, left, right);
     return result;
 }
 
+
 }// namespace lal
 
 #endif// LIBALGEBRA_LITE_ALGEBRA_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h`

 * *Files 4% similar despite different names*

```diff
@@ -3,98 +3,94 @@
 //
 
 #ifndef LIBALGEBRA_LITE_DENSE_VECTOR_H
 #define LIBALGEBRA_LITE_DENSE_VECTOR_H
 
 #include "implementation_types.h"
 
-
 #include <memory>
 #include <type_traits>
 
 #include "basis_traits.h"
 #include "coefficients.h"
 #include "vector_base.h"
 #include "vector_traits.h"
 
-
-
 namespace lal {
 
-
 namespace dtl {
 
 template <typename Basis, typename Scalar, typename Iterator>
 class dense_vector_const_iterator;
 
 template <typename Basis, typename Scalar, typename Iterator>
 class dense_vector_iterator;
 
-} // namespace dtl
+}// namespace dtl
 
 template <typename Basis>
 class key_range;
 
-
-template <typename Basis, typename Coefficients,
-          template <typename, typename...> class VectorType,
-          typename... Args>
+template <
+        typename Basis, typename Coefficients,
+        template <typename, typename...> class VectorType, typename... Args>
 class dense_vector_base : public vectors::vector_base<Basis, Coefficients>
 {
-    using vec_base     = vectors::vector_base<Basis, Coefficients>;
-    using typename vec_base::coeff_traits;
+    using vec_base = vectors::vector_base<Basis, Coefficients>;
     using typename vec_base::basis_traits;
+    using typename vec_base::coeff_traits;
+
 public:
-    using typename vec_base::basis_type;
-    using typename vec_base::key_type;
     using typename vec_base::basis_pointer;
+    using typename vec_base::basis_type;
     using typename vec_base::coefficient_ring;
-    using typename vec_base::scalar_type;
+    using typename vec_base::key_type;
     using typename vec_base::rational_type;
+    using typename vec_base::scalar_type;
 
 private:
     using storage_type = VectorType<scalar_type, Args...>;
 
     using vec_base::p_basis;
-    storage_type m_storage {};
+    storage_type m_storage{};
     deg_t m_degree = 0;
 
 public:
-
-    using size_type         = typename storage_type::size_type;
-    using difference_type   = typename storage_type::difference_type;
-    using iterator          = dtl::dense_vector_iterator<Basis, scalar_type,
-                                typename storage_type::iterator>;
-    using const_iterator    = dtl::dense_vector_const_iterator<Basis, scalar_type,
-                                typename storage_type::const_iterator>;
-    using pointer           = typename storage_type::pointer;
-    using const_pointer     = typename storage_type::const_pointer;
-    using reference         = typename storage_type::reference;
-    using const_reference   = typename storage_type::const_reference;
+    using size_type = typename storage_type::size_type;
+    using difference_type = typename storage_type::difference_type;
+    using iterator = dtl::dense_vector_iterator<
+            Basis, scalar_type, typename storage_type::iterator>;
+    using const_iterator = dtl::dense_vector_const_iterator<
+            Basis, scalar_type, typename storage_type::const_iterator>;
+    using pointer = typename storage_type::pointer;
+    using const_pointer = typename storage_type::const_pointer;
+    using reference = typename storage_type::reference;
+    using const_reference = typename storage_type::const_reference;
 
     dense_vector_base(basis_pointer basis, key_type k, scalar_type s)
         : vec_base(basis), m_storage()
     {
         auto index = p_basis->key_to_index(k);
         resize(index);
         m_storage[index] = s;
     }
 
-    explicit dense_vector_base(basis_pointer basis) : vec_base(basis)
-    {}
+    explicit dense_vector_base(basis_pointer basis) : vec_base(basis) {}
 
-    dense_vector_base(basis_pointer basis, std::initializer_list<scalar_type> args)
-            : vec_base(basis), m_storage(args)
+    dense_vector_base(
+            basis_pointer basis, std::initializer_list<scalar_type> args
+    )
+        : vec_base(basis), m_storage(args)
     {
         resize(args.size());
     }
 
-    template<typename InputIt>
+    template <typename InputIt>
     dense_vector_base(basis_pointer basis, InputIt begin, InputIt end)
-            : vec_base(basis), m_storage(begin, end)
+        : vec_base(basis), m_storage(begin, end)
     {
         resize(m_storage.size());
     }
 
     explicit dense_vector_base(basis_pointer basis, size_type n)
         : vec_base(basis), m_storage()
     {
@@ -104,39 +100,44 @@
     template <typename S>
     explicit dense_vector_base(basis_pointer basis, size_type n, const S& val)
         : vec_base(basis), m_storage()
     {
         resize(n, val);
     }
 
+    void swap(dense_vector_base& right) {
+        std::swap(m_storage, right.m_storage);
+        std::swap(m_degree, right.m_degree);
+        vec_base::swap(right);
+    }
 
 private:
-
     size_type adjust_size(size_type n) const noexcept
     {
         auto next = basis_traits::get_next_dimension(*p_basis, n);
-        return std::min(basis_traits::max_dimension(*p_basis),
-                next.first);
+        return std::min(basis_traits::max_dimension(*p_basis), next.first);
     }
 
 public:
-
     void update_degree(deg_t degree) noexcept { m_degree = degree; }
 
-    void reserve_exact(size_type n, deg_t degree=0) {
+    void reserve_exact(size_type n, deg_t degree = 0)
+    {
         m_storage.reserve(n);
         m_degree = degree;
     }
 
-    void resize_exact(size_type n, deg_t degree=0) {
+    void resize_exact(size_type n, deg_t degree = 0)
+    {
         m_storage.resize(n, coefficient_ring::zero());
         m_degree = degree;
     }
 
-    void resize_exact(size_type n, const scalar_type& scalar, deg_t degree=0) {
+    void resize_exact(size_type n, const scalar_type& scalar, deg_t degree = 0)
+    {
         m_storage.resize(n, scalar);
         m_degree = degree;
     }
 
     void reserve(size_type n)
     {
         auto next = basis_traits::get_next_dimension(*p_basis, n);
@@ -153,40 +154,56 @@
     {
         auto next = basis_traits::get_next_dimension(*p_basis, n);
         resize_exact(next.first, val, next.second);
     }
 
     iterator begin() noexcept { return iterator(&*p_basis, m_storage.begin()); }
     iterator end() noexcept { return iterator(&*p_basis, m_storage.end()); }
-    const_iterator begin() const noexcept { return const_iterator(&*p_basis, m_storage.begin()); }
-    const_iterator end() const noexcept { return const_iterator(&*p_basis, m_storage.end()); }
-    const_iterator cbegin() const noexcept { return const_iterator(&*p_basis, m_storage.begin()); }
-    const_iterator cend() const noexcept { return const_iterator(&*p_basis, m_storage.end()); }
+    const_iterator begin() const noexcept
+    {
+        return const_iterator(&*p_basis, m_storage.begin());
+    }
+    const_iterator end() const noexcept
+    {
+        return const_iterator(&*p_basis, m_storage.end());
+    }
+    const_iterator cbegin() const noexcept
+    {
+        return const_iterator(&*p_basis, m_storage.begin());
+    }
+    const_iterator cend() const noexcept
+    {
+        return const_iterator(&*p_basis, m_storage.end());
+    }
 
-    size_type size() const noexcept {
+    size_type size() const noexcept
+    {
         const auto& zero = Coefficients::zero();
-        return std::count_if(m_storage.begin(), m_storage.end(), [&zero] (const scalar_type& s) { return s != zero; });
+        return std::count_if(
+                m_storage.begin(), m_storage.end(),
+                [&zero](const scalar_type& s) { return s != zero; }
+        );
     }
     constexpr size_type dimension() const noexcept { return m_storage.size(); }
     constexpr deg_t degree() const noexcept { return m_degree; }
     constexpr bool empty() const noexcept { return m_storage.empty(); }
 
     template <typename Index>
     reference operator[](Index idx) noexcept
     {
         auto key = p_basis->key_to_index(idx);
-        if (key >= m_storage.size()) {
-            resize(key);
-        }
+        if (key >= m_storage.size()) { resize(key); }
         return m_storage[key];
     }
 
     template <typename Index>
     const_reference operator[](Index idx) const noexcept
-    { return m_storage[p_basis->key_to_index(idx)]; }
+    {
+        return m_storage[p_basis->key_to_index(idx)];
+    }
 
     pointer as_mut_ptr() noexcept { return m_storage.data(); }
     const_pointer as_ptr() const noexcept { return m_storage.data(); }
 
     void clear() noexcept(noexcept(m_storage.clear())) { m_storage.clear(); }
 
     // these need to be implemented in terms of kernels.
@@ -208,164 +225,151 @@
     }
 
     template <typename UnaryOp>
     dense_vector_base& inplace_unary_op(UnaryOp op)
     {
         const auto begin = m_storage.begin();
         const auto end = m_storage.end();
-        for (auto it=begin; it != end; ++it) {
-            op(*it);
-        }
+        for (auto it = begin; it != end; ++it) { op(*it); }
         return *this;
     }
 
     template <typename BinaryOp>
     dense_vector_base binary_op(const dense_vector_base& arg, BinaryOp op) const
     {
         dense_vector_base result(p_basis);
 
         const difference_type lhs_size(m_storage.size());
         const difference_type rhs_size(arg.m_storage.size());
 
-        result.reserve_exact(std::max(lhs_size, rhs_size), std::max(m_degree, arg.m_degree));
+        result.reserve_exact(
+                std::max(lhs_size, rhs_size), std::max(m_degree, arg.m_degree)
+        );
 
         const auto mid = std::min(lhs_size, rhs_size);
         const auto& zero = coefficient_ring::zero();
 
-        for (difference_type i=0; i<mid; ++i) {
+        for (difference_type i = 0; i < mid; ++i) {
             result.m_storage.emplace_back(op(m_storage[i], arg.m_storage[i]));
         }
 
-        for (auto i=mid; i<lhs_size; ++i) {
+        for (auto i = mid; i < lhs_size; ++i) {
             result.m_storage.emplace_back(op(m_storage[i], zero));
         }
 
-        for (auto i=mid; i<rhs_size; ++i) {
+        for (auto i = mid; i < rhs_size; ++i) {
             result.m_storage.emplace_back(op(zero, arg.m_storage[i]));
         }
 
         return result;
     }
 
     template <typename InplaceBinaryOp>
-    dense_vector_base& inplace_binary_op(const dense_vector_base& rhs, InplaceBinaryOp op)
+    dense_vector_base&
+    inplace_binary_op(const dense_vector_base& rhs, InplaceBinaryOp op)
     {
         const difference_type lhs_size(m_storage.size());
         const difference_type rhs_size(rhs.m_storage.size());
 
-        if (rhs_size > lhs_size) {
-            resize_exact(rhs_size, rhs.m_degree);
-        }
+        if (rhs_size > lhs_size) { resize_exact(rhs_size, rhs.m_degree); }
 
         const auto& zero = coefficient_ring::zero();
         const auto mid = std::min(lhs_size, rhs_size);
 
-        for (difference_type i=0; i<mid; ++i) {
+        for (difference_type i = 0; i < mid; ++i) {
             op(m_storage[i], rhs.m_storage[i]);
         }
 
-        for (auto i=mid; i<lhs_size; ++i) {
-            op(m_storage[i], zero);
-        }
+        for (auto i = mid; i < lhs_size; ++i) { op(m_storage[i], zero); }
 
-        for (auto i=mid; i<rhs_size; ++i) {
+        for (auto i = mid; i < rhs_size; ++i) {
             op(m_storage[i], rhs.m_storage[i]);
         }
 
         return *this;
     }
 
-    bool operator==(const dense_vector_base& rhs) const noexcept {
+    bool operator==(const dense_vector_base& rhs) const noexcept
+    {
         auto mid = std::min(m_storage.size(), rhs.m_storage.size());
 
-        for (dimn_t i=0; i<mid; ++i) {
-            if (m_storage[i] != rhs.m_storage[i]) {
-                return false;
-            }
+        for (dimn_t i = 0; i < mid; ++i) {
+            if (m_storage[i] != rhs.m_storage[i]) { return false; }
         }
 
         const auto& zero = coefficient_ring::zero();
 
-        for (dimn_t i=mid; i<m_storage.size(); ++i) {
-            if (m_storage[i] != zero) {
-                return false;
-            }
+        for (dimn_t i = mid; i < m_storage.size(); ++i) {
+            if (m_storage[i] != zero) { return false; }
         }
 
-        for (dimn_t i=mid; i<rhs.m_storage.size(); ++i) {
-            if (rhs.m_storage[i] != zero) {
-                return false;
-            }
+        for (dimn_t i = mid; i < rhs.m_storage.size(); ++i) {
+            if (rhs.m_storage[i] != zero) { return false; }
         }
 
         return true;
     }
-
 };
 
-
 template <typename Basis, typename Coefficients>
 using dense_vector = dense_vector_base<Basis, Coefficients, std::vector>;
 
-namespace dtl {
-
 
+namespace dtl {
 
 template <typename KeyRef, typename ScaRef>
 class dense_iterator_item
 {
     template <typename B, typename C, typename I>
     friend class dense_vector_iterator;
 
     template <typename B, typename C, typename I>
     friend class dense_vector_const_iterator;
 
     KeyRef m_key;
     ScaRef m_sca;
 
-    dense_iterator_item(KeyRef key, ScaRef sca)
-        : m_key(key), m_sca(sca)
-    {}
+    dense_iterator_item(KeyRef key, ScaRef sca) : m_key(key), m_sca(sca) {}
 
 public:
-
     dense_iterator_item* operator->() noexcept { return this; }
 
     KeyRef key() const noexcept { return m_key; }
     ScaRef value() const noexcept { return m_sca; }
 };
 
 template <typename Basis, typename Coefficients, typename Iterator>
 class dense_vector_iterator
 {
     using basis_traits = basis_trait<Basis>;
     using key_type = typename basis_traits::key_type;
     using coeff_traits = coefficient_trait<Coefficients>;
     using scalar_type = typename coeff_traits::scalar_type;
     using basis_pointer = lal::basis_pointer<Basis>;
-//    using iterator_category = std::forward_iterator_tag;
+    //    using iterator_category = std::forward_iterator_tag;
 
     const Basis* p_basis = nullptr;
     Iterator p_data;
     key_type m_key;
 
     using it_traits = std::iterator_traits<Iterator>;
 
 public:
     using difference_type = std::ptrdiff_t;
-    using value_type = dtl::dense_iterator_item<const key_type&, typename it_traits::reference>;
+    using value_type = dtl::dense_iterator_item<
+            const key_type&, typename it_traits::reference>;
     using reference = value_type;
     using pointer = value_type;
     using iterator_category = std::forward_iterator_tag;
 
-
     dense_vector_iterator() = default;
 
     dense_vector_iterator(const Basis* basis, Iterator data)
-        : p_basis(basis), p_data(data), m_key(basis_traits::index_to_key(*basis, 0))
+        : p_basis(basis), p_data(data),
+          m_key(basis_traits::index_to_key(*basis, 0))
     {}
 
     dense_vector_iterator& operator++()
     {
         ++p_data;
         ++m_key;
         return *this;
@@ -374,37 +378,29 @@
     const dense_vector_iterator operator++(int)
     {
         auto current(*this);
         operator++();
         return current;
     }
 
-    reference operator*() const noexcept
-    {
-        return {m_key, *p_data};
-    }
+    reference operator*() const noexcept { return {m_key, *p_data}; }
 
-    pointer operator->() const noexcept
-    {
-        return {m_key, *p_data};
-    }
+    pointer operator->() const noexcept { return {m_key, *p_data}; }
 
     bool operator==(const dense_vector_iterator& other) const noexcept
     {
         return p_data == other.p_data;
     }
 
     bool operator!=(const dense_vector_iterator& other) const noexcept
     {
         return p_data != other.p_data;
     }
 };
 
-
-
 template <typename Basis, typename Coefficients, typename Iterator>
 class dense_vector_const_iterator
 {
     using basis_traits = basis_trait<Basis>;
     using key_type = typename basis_traits::key_type;
     using coeff_traits = coefficient_trait<Coefficients>;
     using scalar_type = typename coeff_traits::scalar_type;
@@ -412,25 +408,26 @@
     const Basis* p_basis = nullptr;
     Iterator p_data;
     key_type m_key;
 
     using it_traits = std::iterator_traits<Iterator>;
 
 public:
-
-    using value_type = dtl::dense_iterator_item<const key_type&, typename it_traits::reference>;
+    using value_type = dtl::dense_iterator_item<
+            const key_type&, typename it_traits::reference>;
     using reference = value_type;
     using pointer = value_type;
     using difference_type = std::ptrdiff_t;
     using iterator_category = std::forward_iterator_tag;
 
     dense_vector_const_iterator() = default;
 
     dense_vector_const_iterator(const Basis* basis, Iterator data)
-        : p_basis(basis), p_data(data), m_key(basis_traits::index_to_key(*basis, 0))
+        : p_basis(basis), p_data(data),
+          m_key(basis_traits::index_to_key(*basis, 0))
     {}
 
     dense_vector_const_iterator& operator++()
     {
         ++p_data;
         basis_traits::advance_key(*p_basis, m_key);
         return *this;
@@ -439,36 +436,27 @@
     const dense_vector_const_iterator operator++(int)
     {
         auto current(*this);
         operator++();
         return current;
     }
 
-    reference operator*() const noexcept
-    {
-        return {m_key, *p_data};
-    }
+    reference operator*() const noexcept { return {m_key, *p_data}; }
 
-    pointer operator->() const noexcept
-    {
-        return {m_key, *p_data};
-    }
+    pointer operator->() const noexcept { return {m_key, *p_data}; }
 
     bool operator==(const dense_vector_const_iterator& other) const noexcept
     {
         return p_data == other.p_data;
     }
 
     bool operator!=(const dense_vector_const_iterator& other) const noexcept
     {
         return p_data != other.p_data;
     }
 };
 
+}// namespace dtl
 
-} // namespace dtl
-
-
-
-} // namespace lal
+}// namespace lal
 
-#endif //LIBALGEBRA_LITE_DENSE_VECTOR_H
+#endif// LIBALGEBRA_LITE_DENSE_VECTOR_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/macros.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/detail/macros.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/traits.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/detail/traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h`

 * *Files 16% similar despite different names*

```diff
@@ -558,15 +558,15 @@
     {
         if (degree == 0) {
             // Degree 0 is easy, just copy the data from src to dst.
             *dst = *src;
         } else if (degree == 1) {
             // Degree 1 is like degree 0, no permutation is needed so we only
             // need to worry about signing
-            for (dimn_t i = 0; i < p_basis->width(); ++i) {
+            for (dimn_t i = 0; i < static_cast<dimn_t>(p_basis->width()); ++i) {
                 if (do_signing) {
                     dst[i] = -src[i];
                 } else {
                     dst[i] = src[i];
                 }
             }
         } else {
@@ -600,21 +600,21 @@
     {
         auto middle_degree = degree - 2 * tile_letters;
         auto stride = p_basis->powers()[degree - tile_letters];
         unpacked_tensor_word word(p_basis->width(), middle_degree);
 
         for (dimn_t i = 0; i < p_basis->powers()[middle_degree]; ++i, ++word) {
             auto ridx = word.to_reverse_index();
-//            auto ridx = p_basis->reverse_idx(middle_degree, i);
+            //            auto ridx = p_basis->reverse_idx(middle_degree, i);
 
-            read_tile(src + i*tile_width, stride);
+            read_tile(src + i * tile_width, stride);
             if (do_signing && !is_even(degree)) { sign_tile(); }
             permute_tile();
 
-            write_tile(dst + ridx*tile_width, stride);
+            write_tile(dst + ridx * tile_width, stride);
         }
     }
 
     template <template <typename, typename> class VectorType>
     void handle_antipode(
             VectorType<tensor_basis, Coefficients>& result,
             const VectorType<tensor_basis, Coefficients>& arg
@@ -646,17 +646,17 @@
         if (tile_size > 0) {
             tile = new scalar_type[tile_size]{};
 
             std::unordered_set<dimn_t> seen;
 
             for (dimn_t i = 0; i < tile_width; ++i) {
                 auto ri = p_basis->reverse_idx(tile_letters, i);
-                for (dimn_t j=0; j<tile_width; ++j) {
+                for (dimn_t j = 0; j < tile_width; ++j) {
                     auto rj = p_basis->reverse_idx(tile_letters, j);
-                    auto idx = i*tile_width + j;
+                    auto idx = i * tile_width + j;
                     auto ridx = rj * tile_width + ri;
                     if (ridx != idx && seen.find(idx) == seen.end()) {
                         seen.insert(idx);
                         seen.insert(ridx);
                         permute.push_back({idx, ridx});
                     }
                 }
@@ -706,15 +706,15 @@
     auto* optr = result.as_mut_ptr();
     const auto* iptr = arg.as_ptr();
     const auto max_degree = arg.degree();
     result.update_degree(max_degree);
     deg_t deg = 0;
 
     const auto untiled_levels = (tile_letters > 0)
-            ?  std::min(max_degree, 2 * tile_letters - 1)
+            ? std::min(max_degree, 2 * tile_letters - 1)
             : max_degree;
 
     for (; deg <= untiled_levels; ++deg) {
         handle_dense_untiled_level(optr, iptr, deg);
         optr += p_basis->powers()[deg];
         iptr += p_basis->powers()[deg];
     }
@@ -722,15 +722,14 @@
     // Handle the higher levels with tiling.
     // Note this loop will do nothing if all the levels have already been done
     for (; deg <= max_degree; ++deg) {
         handle_dense_tiled_level(optr, iptr, deg);
         optr += p_basis->powers()[deg];
         iptr += p_basis->powers()[deg];
     }
-
 }
 
 }// namespace dtl
 
 template <
         typename Coefficients, template <typename, typename> class VectorType,
         template <typename> class StorageModel>
@@ -786,14 +785,19 @@
         : algebra_type(basis, mul, key_type(0, 0), std::move(arg))
     {}
 
     free_tensor(basis_pointer basis, scalar_type arg)
         : algebra_type(basis, key_type(0, 0), std::move(arg))
     {}
 
+    free_tensor create_alike() const
+    {
+        return free_tensor(this->get_basis(), this->multiplication());
+    }
+
     free_tensor& fmexp_inplace(const free_tensor& exp_arg)
     {
         free_tensor original(*this), x(exp_arg);
 
         x[key_type(0, 0)] = scalar_type(0);
 
         auto degree = this->basis().depth();
@@ -861,17 +865,17 @@
         }
 
         return result;
     }
 
     friend free_tensor inverse(const free_tensor& arg)
     {
-
-        const auto& a = arg[key_type(0, 0)];
-        assert(a != Coefficients::zero());
+        const auto& unit = arg[key_type(0, 0)];
+        assert(coefficient_ring::is_invertible(unit));
+        const auto& a = coefficient_ring::as_rational(arg[key_type(0, 0)]);
         auto x = arg;
         x[key_type(0, 0)] = Coefficients::zero();
 
         const auto degree = arg.basis().depth();
         free_tensor a_inverse(
                 arg.get_basis(), arg.multiplication(), scalar_type(1) / a
         );
@@ -889,10 +893,209 @@
         dtl::antipode_helper<Coefficients> helper(arg.get_basis());
         return helper(arg);
     }
 };
 
 LAL_EXPORT_TEMPLATE_CLASS(multiplication_registry, free_tensor_multiplication)
 
+template <typename LTensor, typename RTensor>
+inline LTensor free_tensor_multiply(const LTensor& left, const RTensor& right)
+{
+    const auto ftm = multiplication_registry<free_tensor_multiplication>::get(
+            left.basis()
+    );
+    return multiply(*ftm, left, right);
+}
+
+namespace dtl {
+inline namespace unstable {
+
+template <typename Tensor>
+class left_ftm_adjoint
+{
+    const Tensor* multiplier;
+
+    using coefficient_ring = typename Tensor::coefficient_ring;
+    using s_t = typename coefficient_ring::scalar_type;
+
+public:
+    explicit left_ftm_adjoint(const Tensor& arg) : multiplier(&arg) {}
+
+    template <typename Shuffle>
+    enable_if_t<
+            is_same<typename Tensor::coefficient_ring,
+                    typename Shuffle::coefficient_ring>::value
+                    && is_same<
+                            typename Shuffle::basis_type, tensor_basis>::value,
+            Shuffle>
+    operator()(const Shuffle& arg) const
+    {
+        Shuffle result(arg.get_basis(), arg.multiplication());
+        eval(result.base_vector(), arg.base_vector(),
+             multiplier->base_vector());
+        return result;
+    }
+
+private:
+    template <typename V, typename B>
+    enable_if_t<is_same<typename V::basis_type, tensor_basis>::value>
+    eval(V& result, const V& arg, const B& mul) const
+    {
+        using s_t = typename coefficient_ring::scalar_type;
+        for (auto&& pr : mul) {
+            const auto& val = pr.value();
+            result.inplace_binary_op(
+                    shift_down(arg, pr.key()),
+                    [&val](const s_t& l, const s_t& r) { return l + val * r; }
+            );
+        }
+    }
+
+    template <
+            template <typename, typename...> class VSM,
+            template <typename, typename> class BT>
+    void
+    eval(dense_vector_base<tensor_basis, coefficient_ring, VSM>& result,
+         const dense_vector_base<tensor_basis, coefficient_ring, VSM>& arg,
+         const BT<tensor_basis, coefficient_ring>& mul) const
+    {
+        const auto& basis = result.basis();
+        const auto& powers = basis.powers();
+
+        const auto arg_deg = arg.degree();
+        result.resize_exact(basis.size(arg_deg));
+
+        for (auto&& pr : mul) {
+            const auto key = pr.key();
+            const auto prefix_degree = key.degree();
+            const auto index = key.index();
+            const auto& value = pr.value();
+
+            for (deg_t degree = prefix_degree; degree <= arg_deg; ++degree) {
+                auto suffix_degree = degree - prefix_degree;
+                auto* optr = result.as_mut_ptr()
+                        + basis.start_of_degree(suffix_degree);
+                const auto* iptr = arg.as_ptr() + index * powers[suffix_degree];
+
+                for (dimn_t i = 0; i < powers[suffix_degree]; ++i) {
+                    optr[i] += value * iptr[i];
+                }
+            }
+        }
+    }
+
+    template <
+            template <typename, typename...> class VSM,
+            template <typename, typename...> class BSM>
+    void
+    eval(dense_vector_base<tensor_basis, coefficient_ring, VSM>& result,
+         const dense_vector_base<tensor_basis, coefficient_ring, VSM>& arg,
+         const dense_vector_base<tensor_basis, coefficient_ring, BSM>& mul
+    ) const
+    {
+        const auto& basis = result.basis();
+        const auto* sizes = basis.sizes().data();
+        const auto* powers = basis.powers().data();
+
+        const auto arg_deg = arg.degree();
+        const auto param_deg = mul.degree();
+        const auto target_deg = std::min(arg_deg, param_deg);
+        result.resize_exact(sizes[arg_deg]);
+
+        auto* optr = result.as_mut_ptr();
+        const auto* aptr = arg.as_ptr();
+        const auto* pptr = mul.as_ptr();
+
+        const auto& param_unit = *pptr;
+
+        if (param_unit != coefficient_ring::zero()) {
+            for (dimn_t i = 0; i < arg.dimension(); ++i) {
+                optr[i] = param_unit * aptr[i];
+            }
+        }
+
+//        aptr += 1;
+//        pptr += 1;
+        for (deg_t prefix_deg = 1; prefix_deg <= target_deg; ++prefix_deg) {
+            aptr += powers[prefix_deg-1];
+            pptr += powers[prefix_deg-1];
+            eval_single_dense(
+                    optr, aptr, pptr, powers, sizes, prefix_deg, arg_deg
+            );
+
+        }
+    }
+
+    template <typename Arg>
+    static Arg shift_down(const Arg& arg, typename tensor_basis::key_type word)
+    {
+        const auto& basis = arg.basis();
+        Arg result(arg);
+        Arg working(arg.get_basis());
+
+        while (word.degree() > 0) {
+            auto parents = basis.parents(word);
+            word = parents.second;
+
+            for (auto&& pr : result) {
+                auto key = pr.key();
+                auto prparents = basis.parents(key);
+                if (key.degree() > 0 && prparents.first == parents.first) {
+                    working[prparents.second]
+                            = static_cast<const Arg&>(result)[key];
+                }
+            }
+            result.swap(working);
+            working.clear();
+        }
+        return result;
+    }
+
+    static void eval_single_dense(
+            s_t* LAL_RESTRICT optr, const s_t* LAL_RESTRICT aptr,
+            const s_t* LAL_RESTRICT pptr, const dimn_t* powers,
+            const dimn_t* sizes, deg_t param_deg, deg_t arg_deg
+    )
+    {
+        assert(param_deg <= arg_deg);
+        if (param_deg == arg_deg) {
+            auto& unit = optr[0];
+            for (dimn_t i=0; i<powers[param_deg]; ++i) {
+                unit += pptr[i]*aptr[i];
+            }
+            return;
+        }
+
+
+        auto* dst = optr;
+        for (deg_t degree = param_deg; degree <= arg_deg; ++degree) {
+            auto result_deg = degree - param_deg;
+
+            for (dimn_t pidx = 0; pidx < powers[param_deg]; ++pidx) {
+                const auto* src = aptr + pidx*powers[result_deg];
+                const auto& val = pptr[pidx];
+
+                for (dimn_t aidx = 0; aidx < powers[result_deg]; ++aidx) {
+                    dst[aidx] += val * src[aidx];
+                }
+            }
+
+            aptr += powers[degree];
+            dst += powers[result_deg];
+        }
+    }
+};
+
+}// namespace unstable
+}// namespace dtl
+
+template <typename Tensor, typename Shuffle>
+Shuffle
+left_free_tensor_multiply_adjoint(const Tensor& param, const Shuffle& arg)
+{
+    dtl::left_ftm_adjoint<Tensor> op(param);
+    return op(arg);
+}
+
 }// namespace lal
 
 #endif// LIBALGEBRA_LITE_FREE_TENSOR_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/hall_set.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/hall_set.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/index_key.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/index_key.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/key_range.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/key_range.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/lie.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/lie.h`

 * *Files 13% similar despite different names*

```diff
@@ -7,71 +7,75 @@
 
 #include "implementation_types.h"
 #include "libalgebra_lite_export.h"
 
 #include <mutex>
 #include <unordered_map>
 
-#include <boost/functional/hash.hpp>
 #include <boost/container/small_vector.hpp>
+#include <boost/functional/hash.hpp>
 
 #include "algebra.h"
 #include "hall_set.h"
 #include "registry.h"
 
 namespace lal {
 
 class lie_multiplier;
 
 LAL_EXPORT_TEMPLATE_CLASS(base_multiplier, lie_multiplier, hall_basis, 2)
 
-class LIBALGEBRA_LITE_EXPORT lie_multiplier : public base_multiplier<lie_multiplier, hall_basis, 2>
+class LIBALGEBRA_LITE_EXPORT lie_multiplier
+    : public base_multiplier<lie_multiplier, hall_basis, 2>
 {
     using base_type = base_multiplier<lie_multiplier, hall_basis, 2>;
 
     deg_t m_width;
 
     using typename base_type::key_type;
     using typename base_type::product_type;
     using typename base_type::reference;
 
     using parent_type = std::pair<key_type, key_type>;
 
-    mutable std::unordered_map<parent_type, product_type, boost::hash<parent_type>> m_cache;
+    mutable std::unordered_map<
+            parent_type, product_type, boost::hash<parent_type>>
+            m_cache;
     mutable std::recursive_mutex m_lock;
 
-    product_type key_prod_impl(const hall_basis& basis, key_type lhs, key_type rhs) const;
+    product_type
+    key_prod_impl(const hall_basis& basis, key_type lhs, key_type rhs) const;
 
 public:
     using basis_type = hall_basis;
 
-    explicit lie_multiplier(deg_t width) : m_width(width)
-    {}
-
-    reference operator()(const hall_basis& basis, key_type lhs, key_type rhs) const;
-
+    explicit lie_multiplier(deg_t width) : m_width(width) {}
 
+    reference
+    operator()(const hall_basis& basis, key_type lhs, key_type rhs) const;
 };
 
-
-struct LIBALGEBRA_LITE_EXPORT lie_multiplication : public base_multiplication<lie_multiplier>
-{
+struct LIBALGEBRA_LITE_EXPORT lie_multiplication
+    : public base_multiplication<lie_multiplier> {
     using base = base_multiplication<lie_multiplier>;
     using base::base;
 };
 
-
-
-template<typename Coefficients,
-        template<typename, typename> class VectorType,
-        template<typename> class StorageModel>
-using lie = algebra<hall_basis,
-                    Coefficients,
-                    lie_multiplication,
-                    VectorType,
-                    StorageModel>;
+template <
+        typename Coefficients, template <typename, typename> class VectorType,
+        template <typename> class StorageModel>
+using lie = algebra<
+        hall_basis, Coefficients, lie_multiplication, VectorType, StorageModel>;
 
 LAL_EXPORT_TEMPLATE_CLASS(multiplication_registry, lie_multiplication)
 
-} // namespace lal
+template <typename LLie, typename RLie>
+inline LLie lie_multiply(const LLie& left, const RLie& right)
+{
+    const auto liem
+            = multiplication_registry<lie_multiplication>::get(left.basis());
+    return multiply(*liem, left, right);
+}
+
+}// namespace lal
 
-#endif //LIBALGEBRA_LITE_LIE_H
+#endif// LIBALGEBRA_LITE_LIE_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/maps.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/maps.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,59 +6,55 @@
 #define LIBALGEBRA_LITE_MAPS_H
 
 #include "implementation_types.h"
 #include "libalgebra_lite_export.h"
 
 #include <boost/container/small_vector.hpp>
 
-#include "tensor_basis.h"
 #include "free_tensor.h"
 #include "lie.h"
+#include "tensor_basis.h"
 
 namespace lal {
 
-
 namespace dtl {
 
 class generic_commutator
 {
     const tensor_basis& m_basis;
     const free_tensor_multiplication& m_mul;
 
 public:
     using key_type = typename tensor_basis::key_type;
     using pair_type = std::pair<key_type, int>;
     using tensor_type = boost::container::small_vector<pair_type, 1>;
     using ref_type = const boost::container::small_vector_base<pair_type>&;
 
-    generic_commutator(const tensor_basis& basis, const free_tensor_multiplication& mul)
+    generic_commutator(
+            const tensor_basis& basis, const free_tensor_multiplication& mul
+    )
         : m_basis(basis), m_mul(mul)
     {}
 
     tensor_type operator()(ref_type lhs, ref_type rhs) const;
-
-
 };
 
-struct rbracketing_cache_item
-{
+struct rbracketing_cache_item {
     using key_type = typename tensor_basis::key_type;
     boost::container::small_vector<std::pair<key_type, int>, 1> value;
     bool set = false;
 };
 
-
 class LIBALGEBRA_LITE_EXPORT maps_implementation
 {
     const tensor_basis* p_tensor_basis;
     const hall_basis* p_lie_basis;
     std::shared_ptr<const lie_multiplication> p_lie_mul;
     std::shared_ptr<const free_tensor_multiplication> p_ftensor_mul;
 
-
 public:
     using lkey_type = typename hall_basis::key_type;
     using tkey_type = typename tensor_basis::key_type;
     using generic_scalar_type = int;
 
     using lie_pair = std::pair<lkey_type, generic_scalar_type>;
     using tensor_pair = std::pair<tkey_type, generic_scalar_type>;
@@ -67,106 +63,121 @@
 
     using gtensor_ref = const boost::container::small_vector_base<tensor_pair>&;
     using glie_ref = const boost::container::small_vector_base<lie_pair>&;
 
 private:
     static generic_tensor expand_letter(let_t letter);
 
-    hall_extension<decltype(&expand_letter),
-                   generic_commutator,
-                   gtensor_ref> m_expand;
+    hall_extension<decltype(&expand_letter), generic_commutator, gtensor_ref>
+            m_expand;
 
-    mutable std::unordered_map<tkey_type, dtl::rbracketing_cache_item> m_rbracketing_cache;
+    mutable std::unordered_map<tkey_type, dtl::rbracketing_cache_item>
+            m_rbracketing_cache;
     mutable std::recursive_mutex m_rbracketing_lock;
-public:
-
 
+public:
     maps_implementation(const tensor_basis* tbasis, const hall_basis* lbasis)
-        : p_tensor_basis(tbasis),
-          p_lie_basis(lbasis),
-          p_lie_mul(multiplication_registry<lie_multiplication>::get(lbasis->width())),
-          p_ftensor_mul(multiplication_registry<free_tensor_multiplication>::get(tbasis->width())),
-          m_expand(p_lie_basis->get_hall_set(), &expand_letter, generic_commutator(*p_tensor_basis, *p_ftensor_mul))
-    { }
+        : p_tensor_basis(tbasis), p_lie_basis(lbasis),
+          p_lie_mul(multiplication_registry<lie_multiplication>::get(
+                  lbasis->width()
+          )),
+          p_ftensor_mul(
+                  multiplication_registry<free_tensor_multiplication>::get(
+                          tbasis->width()
+                  )
+          ),
+          m_expand(
+                  p_lie_basis->get_hall_set(), &expand_letter,
+                  generic_commutator(*p_tensor_basis, *p_ftensor_mul)
+          )
+    {}
 
     glie_ref rbracketing(tkey_type tkey) const;
     gtensor_ref expand(lkey_type lkey) const;
-
 };
 
-
-} // namespace dtl
-
+}// namespace dtl
 
 class LIBALGEBRA_LITE_EXPORT maps
 {
     basis_pointer<tensor_basis> p_tensor_basis;
     basis_pointer<hall_basis> p_lie_basis;
     const dtl::maps_implementation* p_impl;
-public:
 
+public:
     using tkey_type = typename tensor_basis::key_type;
     using lkey_type = typename hall_basis::key_type;
-    using generic_scalar_type = typename dtl::maps_implementation::generic_scalar_type;
+    using generic_scalar_type =
+            typename dtl::maps_implementation::generic_scalar_type;
     using generic_lie = typename dtl::maps_implementation::generic_lie;
     using generic_tensor = typename dtl::maps_implementation::generic_tensor;
     using glie_ref = typename dtl::maps_implementation::glie_ref;
     using gtensor_ref = typename dtl::maps_implementation::gtensor_ref;
 
     maps(basis_pointer<tensor_basis> tbasis, basis_pointer<hall_basis> lbasis);
     maps(deg_t width, deg_t depth);
     ~maps();
 
-    glie_ref rbracketing(tkey_type tkey) const { return p_impl->rbracketing(tkey); }
+    glie_ref rbracketing(tkey_type tkey) const
+    {
+        return p_impl->rbracketing(tkey);
+    }
     gtensor_ref expand(lkey_type lkey) const { return p_impl->expand(lkey); }
 
-
-
-    template <typename Coefficients,
-              template <typename, typename> class VectorType,
-              template <typename> class StorageModel>
+    template <
+            typename Coefficients,
+            template <typename, typename> class VectorType,
+            template <typename> class StorageModel>
     free_tensor<Coefficients, VectorType, StorageModel>
     lie_to_tensor(const lie<Coefficients, VectorType, StorageModel>& arg) const
     {
-        using scalar_type = typename coefficient_trait<Coefficients>::scalar_type;
+        using scalar_type =
+                typename coefficient_trait<Coefficients>::scalar_type;
         if (arg.basis().width() != p_lie_basis->width()) {
             throw std::invalid_argument("mismatched width");
         }
 
         auto max_deg = p_lie_basis->depth();
-        free_tensor<Coefficients, VectorType, StorageModel> result(p_tensor_basis);
+        free_tensor<Coefficients, VectorType, StorageModel> result(
+                p_tensor_basis
+        );
         if (arg.basis().depth() <= max_deg) {
             for (auto outer : arg) {
                 auto val = outer.value();
                 for (auto inner : expand(outer.key())) {
                     assert(inner.first.degree() == outer.key().degree());
-                    result.add_scal_prod(inner.first, scalar_type(inner.second) * val);
+                    result.add_scal_prod(
+                            inner.first, scalar_type(inner.second) * val
+                    );
                 }
-
             }
         } else {
             for (auto outer : arg) {
                 auto key = outer.key();
                 auto val = outer.value();
                 if (p_lie_basis->degree(key) <= max_deg) {
                     for (auto inner : expand(key)) {
                         assert(outer.key().degree() == inner.first.degree());
-                        result.add_scal_prod(inner.first, scalar_type(inner.second) * val);
+                        result.add_scal_prod(
+                                inner.first, scalar_type(inner.second) * val
+                        );
                     }
                 }
             }
         }
         return result;
     }
 
-    template <typename Coefficients,
+    template <
+            typename Coefficients,
             template <typename, typename> class VectorType,
             template <typename> class StorageModel>
     lie<Coefficients, VectorType, StorageModel>
-    tensor_to_lie(const free_tensor<Coefficients, VectorType, StorageModel>& arg) const
+    tensor_to_lie(const free_tensor<Coefficients, VectorType, StorageModel>& arg
+    ) const
     {
         using scalar_type = typename Coefficients::scalar_type;
         using rational_type = typename Coefficients::rational_type;
 
         if (arg.basis().width() != p_tensor_basis->width()) {
             throw std::invalid_argument("mismatched width");
         }
@@ -174,40 +185,42 @@
 
         lie<Coefficients, VectorType, StorageModel> result(p_lie_basis);
 
         if (arg.basis().depth() <= max_deg) {
             for (auto&& outer : arg) {
                 auto key = outer.key();
                 auto deg = key.degree();
-                if (deg > 0 ) {
+                if (deg > 0) {
                     auto val = outer.value() / rational_type(deg);
                     for (auto inner : rbracketing(key)) {
                         assert(inner.first.degree() == deg);
-                        result.add_scal_prod(inner.first, scalar_type(inner.second)*val);
+                        result.add_scal_prod(
+                                inner.first, scalar_type(inner.second) * val
+                        );
                     }
                 }
             }
         } else {
             for (auto outer : arg) {
                 auto key = outer.key();
                 auto deg = static_cast<deg_t>(key.degree());
-                if (deg > 0 ){
+                if (deg > 0) {
                     auto val = outer.value() / deg;
                     if (deg <= max_deg) {
                         for (auto inner : rbracketing(key)) {
-                            assert(inner.first.degree() == static_cast<dimn_t>(deg));
-                            result.add_scal_prod(inner.first, Coefficients::mul(scalar_type(inner.second), val));
+                            assert(inner.first.degree()
+                                   == static_cast<dimn_t>(deg));
+                            result.add_scal_prod(
+                                    inner.first, scalar_type(inner.second) * val
+                            );
                         }
                     }
                 }
             }
         }
         return result;
     }
 };
 
+}// namespace lal
 
-} // namespace alg
-
-
-
-#endif //LIBALGEBRA_LITE_MAPS_H
+#endif// LIBALGEBRA_LITE_MAPS_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/operators.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/operators.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/polynomial.h`

 * *Files 18% similar despite different names*

```diff
@@ -6,115 +6,147 @@
 #define LIBALGEBRA_LITE_POLYNOMIAL_H
 
 #include "implementation_types.h"
 #include "libalgebra_lite_export.h"
 
 #include <boost/container/small_vector.hpp>
 
-#include "polynomial_basis.h"
-#include "sparse_vector.h"
 #include "algebra.h"
 #include "coefficients.h"
+#include "polynomial_basis.h"
 #include "registry.h"
+#include "sparse_vector.h"
 
 namespace lal {
 
-class LIBALGEBRA_LITE_EXPORT polynomial_multiplier {
+class LIBALGEBRA_LITE_EXPORT polynomial_multiplier
+{
     using letter_type = typename polynomial_basis::letter_type;
     using key_type = typename polynomial_basis::key_type;
 
-    using product_type = boost::container::small_vector<std::pair<key_type, int>, 1>;
+    using product_type
+            = boost::container::small_vector<std::pair<key_type, int>, 1>;
 
 public:
-
     using basis_type = polynomial_basis;
 
-    product_type operator()(const polynomial_basis& basis,
-            const key_type& lhs, const key_type& rhs) const;
-
+    product_type operator()(
+            const polynomial_basis& basis, const key_type& lhs,
+            const key_type& rhs
+    ) const;
 };
 
-template<>
-class LIBALGEBRA_LITE_EXPORT multiplication_registry<base_multiplication<polynomial_multiplier>>
+template <>
+class LIBALGEBRA_LITE_EXPORT
+        multiplication_registry<base_multiplication<polynomial_multiplier>>
 {
     using multiplication = base_multiplication<polynomial_multiplier>;
-public:
 
+public:
     static std::shared_ptr<const multiplication> get();
     template <typename Basis>
-    static std::shared_ptr<const multiplication> get(const Basis&) { return get(); }
+    static std::shared_ptr<const multiplication> get(const Basis&)
+    {
+        return get();
+    }
 };
 
-template<typename Coefficients>
-class polynomial : public algebra<polynomial_basis,
-                                  Coefficients,
-                                  base_multiplication<polynomial_multiplier>,
-                                  sparse_vector,
-                                  dtl::standard_storage
-> {
-    using base = algebra<polynomial_basis,
-                         Coefficients,
-                         base_multiplication<polynomial_multiplier>,
-                         sparse_vector,
-                         dtl::standard_storage>;
+template <typename Coefficients>
+class polynomial : public algebra<
+                           polynomial_basis, Coefficients,
+                           base_multiplication<polynomial_multiplier>,
+                           sparse_vector, dtl::standard_storage>
+{
+    using base = algebra<
+            polynomial_basis, Coefficients,
+            base_multiplication<polynomial_multiplier>, sparse_vector,
+            dtl::standard_storage>;
 
 public:
     using multiplication_type = base_multiplication<polynomial_multiplier>;
     using base::base;
 
-    polynomial() : base(basis_registry<polynomial_basis>::get())
-    {}
+    polynomial() : base(basis_registry<polynomial_basis>::get()) {}
 
     template <typename Scalar>
     explicit polynomial(Scalar s)
         : base(basis_registry<polynomial_basis>::get(),
-               multiplication_registry<multiplication_type>::get(),
-                monomial(),
+               multiplication_registry<multiplication_type>::get(), monomial(),
                typename base::scalar_type(s))
     {}
 
     template <typename Key, typename Scalar>
     explicit polynomial(Key k, Scalar s)
         : base(basis_registry<polynomial_basis>::get(),
                multiplication_registry<multiplication_type>::get())
     {
         (*this)[typename base::key_type(k)] = typename base::scalar_type(s);
     }
 
-    template<typename IndeterminateMap>
-    typename polynomial::scalar_type operator()(const IndeterminateMap& arg) const noexcept
+    template <typename IndeterminateMap>
+    typename polynomial::scalar_type operator()(const IndeterminateMap& arg
+    ) const noexcept
     {
         using ring = typename polynomial::coefficient_ring;
         auto ans = ring::zero();
         for (const auto& item : *this) {
             auto key_result = item.first.template eval<ring>(arg);
             ring::add_inplace(ans, ring::mul(item.second, key_result));
         }
         return ans;
     }
-
 };
 
 LAL_EXPORT_TEMPLATE_CLASS(polynomial, double_field)
 LAL_EXPORT_TEMPLATE_CLASS(polynomial, float_field)
 LAL_EXPORT_TEMPLATE_CLASS(polynomial, rational_field)
 
 using double_poly = polynomial<double_field>;
 using float_poly = polynomial<float_field>;
 using rational_poly = polynomial<rational_field>;
 
-LAL_EXPORT_TEMPLATE_STRUCT(coefficient_ring, double_poly, double)
-LAL_EXPORT_TEMPLATE_STRUCT(coefficient_ring, float_poly, float)
-LAL_EXPORT_TEMPLATE_STRUCT(coefficient_ring, rational_poly, typename rational_field::scalar_type)
-
-
-
-using polynomial_ring = coefficient_ring<polynomial<rational_field>, typename rational_field::scalar_type>;
+template <typename Field>
+struct coefficient_ring<polynomial<Field>, typename Field::rational_type>
+{
+    using scalar_type = polynomial<Field>;
+    using rational_type = typename Field::rational_type;
 
+    static const scalar_type& zero() noexcept
+    {
+        static const scalar_type zero;
+        return zero;
+    }
+    static const scalar_type& one() noexcept
+    {
+        static const scalar_type one(1);
+        return one;
+    }
+    static const scalar_type& mone() noexcept
+    {
+        static const scalar_type mone(-1);
+        return mone;
+    }
 
+    static inline bool is_invertible(const scalar_type& arg) {
+        return arg.size() == 1
+                && arg.degree() == 0
+                && Field::is_invertible(arg.begin()->value());
+    }
+    static constexpr const rational_type& as_rational(const scalar_type& arg)
+            noexcept {
+        return Field::as_rational(arg.begin()->value());
+    }
 
+};
 
-} // namespace lal
+LAL_EXPORT_TEMPLATE_STRUCT(coefficient_ring, double_poly, double)
+LAL_EXPORT_TEMPLATE_STRUCT(coefficient_ring, float_poly, float)
+LAL_EXPORT_TEMPLATE_STRUCT(
+        coefficient_ring, rational_poly, typename rational_field::scalar_type
+)
 
+using polynomial_ring = coefficient_ring<
+        polynomial<rational_field>, typename rational_field::scalar_type>;
 
+}// namespace lal
 
-#endif //LIBALGEBRA_LITE_POLYNOMIAL_H
+#endif// LIBALGEBRA_LITE_POLYNOMIAL_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/registry.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/registry.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 
 namespace lal {
 
 class left_half_shuffle_tensor_multiplier;
 
 class right_half_shuffle_tensor_multiplier;
 
-LAL_EXPORT_TEMPLATE_CLASS(base_multiplier, left_half_shuffle_tensor_multiplier, tensor_basis)
-LAL_EXPORT_TEMPLATE_CLASS(base_multiplier, right_half_shuffle_tensor_multiplier, tensor_basis)
+LAL_EXPORT_TEMPLATE_CLASS(
+        base_multiplier, left_half_shuffle_tensor_multiplier, tensor_basis
+)
+LAL_EXPORT_TEMPLATE_CLASS(
+        base_multiplier, right_half_shuffle_tensor_multiplier, tensor_basis
+)
 
 #if 0
 class free_tensor_multiplication
 {
 
 
 
@@ -257,131 +261,183 @@
 
     }
 
 };
 #endif
 
 class LIBALGEBRA_LITE_EXPORT left_half_shuffle_tensor_multiplier
-    : public base_multiplier<left_half_shuffle_tensor_multiplier,
-                             tensor_basis> {
-    using base_type =
-        base_multiplier<left_half_shuffle_tensor_multiplier, tensor_basis>;
+    : public base_multiplier<left_half_shuffle_tensor_multiplier, tensor_basis>
+{
+    using base_type = base_multiplier<
+            left_half_shuffle_tensor_multiplier, tensor_basis>;
 
     using typename base_type::key_type;
     using typename base_type::product_type;
     using typename base_type::reference;
 
     using parent_type = std::pair<key_type, key_type>;
 
-    mutable std::unordered_map<parent_type, product_type,
-                               boost::hash<parent_type>>
-        m_cache;
+    mutable std::unordered_map<
+            parent_type, product_type, boost::hash<parent_type>>
+            m_cache;
     mutable std::recursive_mutex m_lock;
 
-    product_type key_prod_impl(const tensor_basis &basis, key_type lhs,
-                               key_type rhs) const;
+    product_type
+    key_prod_impl(const tensor_basis& basis, key_type lhs, key_type rhs) const;
 
     deg_t m_width;
 
 protected:
-    product_type shuffle(const tensor_basis &basis, key_type lhs,
-                         key_type rhs) const;
+    product_type
+    shuffle(const tensor_basis& basis, key_type lhs, key_type rhs) const;
 
 public:
     using basis_type = tensor_basis;
 
-    explicit left_half_shuffle_tensor_multiplier(deg_t width)
-        : m_width(width) {}
+    explicit left_half_shuffle_tensor_multiplier(deg_t width) : m_width(width)
+    {}
 
-    reference operator()(const tensor_basis &basis, key_type lhs,
-                         key_type rhs) const;
+    reference
+    operator()(const tensor_basis& basis, key_type lhs, key_type rhs) const;
 };
 
 class LIBALGEBRA_LITE_EXPORT right_half_shuffle_tensor_multiplier
-    : public base_multiplier<right_half_shuffle_tensor_multiplier,
-                             tensor_basis> {
-    using base_type =
-        base_multiplier<right_half_shuffle_tensor_multiplier, tensor_basis>;
+    : public base_multiplier<right_half_shuffle_tensor_multiplier, tensor_basis>
+{
+    using base_type = base_multiplier<
+            right_half_shuffle_tensor_multiplier, tensor_basis>;
 
     using typename base_type::key_type;
     using typename base_type::product_type;
     using typename base_type::reference;
 
     using parent_type = std::pair<key_type, key_type>;
 
-    mutable std::unordered_map<parent_type, product_type,
-                               boost::hash<parent_type>>
-        m_cache;
+    mutable std::unordered_map<
+            parent_type, product_type, boost::hash<parent_type>>
+            m_cache;
     mutable std::recursive_mutex m_lock;
 
-    product_type key_prod_impl(const tensor_basis &basis, key_type lhs,
-                               key_type rhs) const;
+    product_type
+    key_prod_impl(const tensor_basis& basis, key_type lhs, key_type rhs) const;
 
-    parent_type split_at_right(const tensor_basis &basis,
-                               key_type key) const noexcept;
+    parent_type
+    split_at_right(const tensor_basis& basis, key_type key) const noexcept;
 
     deg_t m_width;
 
 protected:
-    product_type shuffle(const tensor_basis &basis, key_type lhs,
-                         key_type rhs) const;
+    product_type
+    shuffle(const tensor_basis& basis, key_type lhs, key_type rhs) const;
 
 public:
     using basis_type = tensor_basis;
 
-    explicit right_half_shuffle_tensor_multiplier(deg_t width)
-        : m_width(width) {}
+    explicit right_half_shuffle_tensor_multiplier(deg_t width) : m_width(width)
+    {}
 
-    reference operator()(const tensor_basis &basis, key_type lhs,
-                         key_type rhs) const;
+    reference
+    operator()(const tensor_basis& basis, key_type lhs, key_type rhs) const;
 };
 
-using half_shuffle_tensor_multiplier LAL_UNUSED = left_half_shuffle_tensor_multiplier;
+using half_shuffle_tensor_multiplier LAL_UNUSED
+        = left_half_shuffle_tensor_multiplier;
 
 class LIBALGEBRA_LITE_EXPORT shuffle_tensor_multiplier
-    : protected left_half_shuffle_tensor_multiplier {
-    using base_type =
-        base_multiplier<left_half_shuffle_tensor_multiplier, tensor_basis>;
+    : protected left_half_shuffle_tensor_multiplier
+{
+    using base_type = base_multiplier<
+            left_half_shuffle_tensor_multiplier, tensor_basis>;
     using half_type = left_half_shuffle_tensor_multiplier;
 
 public:
     using basis_type = tensor_basis;
 
     using half_type::half_type;
 
-    typename base_type::product_type
-    operator()(const tensor_basis &basis, typename base_type::key_type lhs,
-               typename base_type::key_type rhs) const;
+    typename base_type::product_type operator()(
+            const tensor_basis& basis, typename base_type::key_type lhs,
+            typename base_type::key_type rhs
+    ) const;
 };
 
-using left_half_shuffle_multiplication =
-    base_multiplication<left_half_shuffle_tensor_multiplier>;
+using left_half_shuffle_multiplication
+        = base_multiplication<left_half_shuffle_tensor_multiplier>;
 using half_shuffle_multiplication LAL_UNUSED = left_half_shuffle_multiplication;
-using right_half_shuffle_multiplication =
-    base_multiplication<right_half_shuffle_tensor_multiplier>;
-using shuffle_tensor_multiplication =
-    base_multiplication<shuffle_tensor_multiplier>;
-
-LAL_EXPORT_TEMPLATE_CLASS(multiplication_registry, left_half_shuffle_multiplication)
-LAL_EXPORT_TEMPLATE_CLASS(multiplication_registry, right_half_shuffle_multiplication)
-LAL_EXPORT_TEMPLATE_CLASS(multiplication_registry, shuffle_tensor_multiplication)
-
-
-template <typename Coefficients, template <typename, typename> class VectorType,
-    template <typename> class StorageModel>
-class shuffle_tensor : public unital_algebra<tensor_basis, Coefficients, shuffle_tensor_multiplication,
-                                      VectorType, StorageModel> {
-    using algebra_type = unital_algebra<tensor_basis, Coefficients, shuffle_tensor_multiplication,
-                                 VectorType, StorageModel>;
+using right_half_shuffle_multiplication
+        = base_multiplication<right_half_shuffle_tensor_multiplier>;
+using shuffle_tensor_multiplication
+        = base_multiplication<shuffle_tensor_multiplier>;
+
+LAL_EXPORT_TEMPLATE_CLASS(
+        multiplication_registry, left_half_shuffle_multiplication
+)
+LAL_EXPORT_TEMPLATE_CLASS(
+        multiplication_registry, right_half_shuffle_multiplication
+)
+LAL_EXPORT_TEMPLATE_CLASS(
+        multiplication_registry, shuffle_tensor_multiplication
+)
+
+template <
+        typename Coefficients, template <typename, typename> class VectorType,
+        template <typename> class StorageModel>
+class shuffle_tensor
+    : public unital_algebra<
+              tensor_basis, Coefficients, shuffle_tensor_multiplication,
+              VectorType, StorageModel>
+{
+    using algebra_type = unital_algebra<
+            tensor_basis, Coefficients, shuffle_tensor_multiplication,
+            VectorType, StorageModel>;
 
 public:
-
     using algebra_type::algebra_type;
 
+    shuffle_tensor create_alike() const {
+        return shuffle_tensor(this->get_basis(), this->multiplication());
+    }
 };
 
-} // namespace lal
+template <typename LTensor, typename RTensor>
+inline LTensor
+left_half_shuffle_multiply(const LTensor& left, const RTensor& right)
+{
 
+    const auto lhsm
+            = multiplication_registry<left_half_shuffle_multiplication>::get(
+                    left.basis()
+            );
+    return multiply(*lhsm, left, right);
+}
+
+template <typename LTensor, typename RTensor>
+inline LTensor
+right_half_shuffle_multiply(const LTensor& left, const RTensor& right)
+{
+    auto rhsm = multiplication_registry<right_half_shuffle_multiplication>::get(
+            left.basis()
+    );
+    return multiply(*rhsm, left, right);
+}
 
+template <typename LTensor, typename RTensor>
+inline LTensor half_shuffle_multiply(const LTensor& left, const RTensor& right)
+{
+    const auto hsm = multiplication_registry<half_shuffle_multiplication>::get(
+            left.basis()
+            );
+    return multiply(*hsm, left, right);
+}
+
+template <typename LTensor, typename RTensor>
+inline LTensor shuffle_multiply(const LTensor& left, const RTensor& right)
+{
+    const auto sm = multiplication_registry<shuffle_tensor_multiplication>::get(
+            left.basis()
+    );
+    return multiply(*sm, left, right);
+}
 
+}// namespace lal
 
-#endif //LIBALGEBRA_LITE_INCLUDE_LIBALGEBRA_LITE_SHUFFLE_TENSOR_H
+#endif// LIBALGEBRA_LITE_INCLUDE_LIBALGEBRA_LITE_SHUFFLE_TENSOR_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h`

 * *Files 6% similar despite different names*

```diff
@@ -5,73 +5,66 @@
 #ifndef LIBALGEBRA_LITE_SPARSE_VECTOR_H
 #define LIBALGEBRA_LITE_SPARSE_VECTOR_H
 
 #include "implementation_types.h"
 
 #include <iterator>
 #include <map>
-#include <utility>
 #include <type_traits>
-
+#include <utility>
 
 #include "basis_traits.h"
 #include "coefficients.h"
 #include "vector_base.h"
 
-
-
 namespace lal {
 namespace dtl {
 
-#define LAL_MUTABLE_REF_iOP(OP)                                             \
-    template <typename Scalar>                                              \
-    Self& operator OP(Scalar arg) noexcept(noexcept(m_tmp OP arg))          \
-    {                                                                       \
-        m_tmp OP arg;                                                       \
-        return *this;                                                       \
+#define LAL_MUTABLE_REF_iOP(OP)                                                \
+    template <typename Scalar>                                                 \
+    Self& operator OP(Scalar arg) noexcept(noexcept(m_tmp OP arg))             \
+    {                                                                          \
+        m_tmp OP arg;                                                          \
+        return *this;                                                          \
     }
 
-#define LAL_MUTABLE_REF_COMPARE(OP)                                         \
-    template <typename Scalar>                                              \
-    bool operator OP(Scalar arg) noexcept(noexcept(m_tmp OP arg))           \
-    {                                                                       \
-        return m_tmp OP arg;                                                \
+#define LAL_MUTABLE_REF_COMPARE(OP)                                            \
+    template <typename Scalar>                                                 \
+    bool operator OP(Scalar arg) noexcept(noexcept(m_tmp OP arg))              \
+    {                                                                          \
+        return m_tmp OP arg;                                                   \
     }
 
-
 template <typename Vector>
 class sparse_mutable_reference
 {
     using map_type = typename Vector::map_type;
     using iterator_type = typename map_type::iterator;
 
     Vector& m_vector;
     iterator_type m_it;
     typename Vector::key_type m_key;
     typename Vector::scalar_type m_tmp;
 
     using Self = sparse_mutable_reference;
 
 public:
-
     using key_type = typename Vector::key_type;
     using scalar_type = typename Vector::scalar_type;
 
     sparse_mutable_reference(Vector& vect, iterator_type it)
         : m_vector(vect), m_it(it), m_key(it->first), m_tmp(it->second)
     {
         assert(it != m_vector.m_data.end());
     }
 
     sparse_mutable_reference(Vector& vect, const key_type& key)
         : m_vector(vect), m_it(vect.m_data.find(key)), m_key(key), m_tmp(0)
     {
-        if (m_it != m_vector.m_data.end()) {
-            m_tmp = m_it->second;
-        }
+        if (m_it != m_vector.m_data.end()) { m_tmp = m_it->second; }
     }
 
     ~sparse_mutable_reference()
     {
         if (m_tmp != scalar_type(0)) {
             if (m_it != m_vector.m_data.end()) {
                 m_it->second = m_tmp;
@@ -79,52 +72,49 @@
                 m_vector.insert_new_value(m_key, m_tmp);
             }
         } else if (m_it != m_vector.m_data.end()) {
             m_vector.m_data.erase(m_it);
         }
     }
 
-    operator const scalar_type& () const noexcept // NOLINT(google-explicit-constructor)
+    operator const scalar_type&(
+    ) const noexcept// NOLINT(google-explicit-constructor)
     {
         return m_tmp;
     }
-//
-//    template <typename S>
-//    std::enable_if_t<std::is_constructible<scalar_type, S>::value, sparse_mutable_reference&>
-//    operator=(S val) {
-//       m_tmp = scalar_type(val);
-//        return *this;
-//    }
-
-
-    LAL_MUTABLE_REF_iOP(=)
-    LAL_MUTABLE_REF_iOP(+=)
-    LAL_MUTABLE_REF_iOP(-=)
-    LAL_MUTABLE_REF_iOP(*=)
-    LAL_MUTABLE_REF_iOP(/=)
-    LAL_MUTABLE_REF_iOP(<<=)
-    LAL_MUTABLE_REF_iOP(>>=)
-    LAL_MUTABLE_REF_iOP(|=)
-    LAL_MUTABLE_REF_iOP(&=)
-    LAL_MUTABLE_REF_iOP(^=)
-    LAL_MUTABLE_REF_iOP(%=)
-
-    LAL_MUTABLE_REF_COMPARE(==)
-    LAL_MUTABLE_REF_COMPARE(!=)
-    LAL_MUTABLE_REF_COMPARE(<)
-    LAL_MUTABLE_REF_COMPARE(<=)
-    LAL_MUTABLE_REF_COMPARE(>)
-    LAL_MUTABLE_REF_COMPARE(>=)
-
-    friend constexpr bool
-    operator==(const scalar_type lhs, const sparse_mutable_reference& rhs)
-    noexcept {
+    //
+    //    template <typename S>
+    //    std::enable_if_t<std::is_constructible<scalar_type, S>::value,
+    //    sparse_mutable_reference&> operator=(S val) {
+    //       m_tmp = scalar_type(val);
+    //        return *this;
+    //    }
+
+    LAL_MUTABLE_REF_iOP(=) LAL_MUTABLE_REF_iOP(+=) LAL_MUTABLE_REF_iOP(
+            -=
+    ) LAL_MUTABLE_REF_iOP(*=) LAL_MUTABLE_REF_iOP(/=) LAL_MUTABLE_REF_iOP(<<=)
+            LAL_MUTABLE_REF_iOP(>>=) LAL_MUTABLE_REF_iOP(|=) LAL_MUTABLE_REF_iOP(
+                    &=
+            ) LAL_MUTABLE_REF_iOP(^=) LAL_MUTABLE_REF_iOP(%=)
+
+                    LAL_MUTABLE_REF_COMPARE(==) LAL_MUTABLE_REF_COMPARE(
+                            !=
+                    ) LAL_MUTABLE_REF_COMPARE(<) LAL_MUTABLE_REF_COMPARE(<=)
+                            LAL_MUTABLE_REF_COMPARE(>) LAL_MUTABLE_REF_COMPARE(
+                                    >=
+                            )
+
+                                    friend constexpr bool
+                                    operator==(
+                                            const scalar_type lhs,
+                                            const sparse_mutable_reference& rhs
+                                    ) noexcept
+    {
         return lhs == rhs.m_tmp;
     }
-
 };
 
 #undef LAL_MUTABLE_REF_COMPARE
 #undef LAL_MUTABLE_REF_iOP
 
 template <typename Vector, typename Iterator, typename Parent>
 class sparse_iterator_base
@@ -134,76 +124,80 @@
     Iterator m_it;
 
     using traits = std::iterator_traits<Iterator>;
 
     using key_type = typename traits::value_type::first_type;
     using scalar_type = typename traits::value_type::second_type;
 
-
 public:
     using difference_type = std::ptrdiff_t;
     using value_type = Parent;
     using reference = Parent&;
     using const_reference = const Parent&;
     using pointer = Parent*;
     using const_pointer = const Parent*;
     using iterator_category = std::forward_iterator_tag;
 
-
-
-    sparse_iterator_base() : p_vector(nullptr), m_it()
-    {}
+    sparse_iterator_base() : p_vector(nullptr), m_it() {}
 
     sparse_iterator_base(Vector* vector, Iterator it)
         : p_vector(vector), m_it(it)
     {
         assert(vector != nullptr);
     }
 
     sparse_iterator_base(Vector& vector, Iterator it)
         : p_vector(&vector), m_it(it)
     {}
 
-    Parent& operator++() noexcept { ++m_it; return static_cast<Parent&>(*this); }
+    Parent& operator++() noexcept
+    {
+        ++m_it;
+        return static_cast<Parent&>(*this);
+    }
     const Parent operator++(int) noexcept
     {
         Parent result(p_vector, m_it);
         ++m_it;
         return result;
     }
 
-    const Parent& operator*() const noexcept { return static_cast<const Parent&>(*this); }
-    const Parent* operator->() const noexcept { return static_cast<const Parent*>(this); }
+    const Parent& operator*() const noexcept
+    {
+        return static_cast<const Parent&>(*this);
+    }
+    const Parent* operator->() const noexcept
+    {
+        return static_cast<const Parent*>(this);
+    }
 
     bool operator==(const sparse_iterator_base& other) const noexcept
     {
         return m_it == other.m_it;
     }
     bool operator!=(const sparse_iterator_base& other) const noexcept
     {
         return m_it != other.m_it;
     }
 };
 
-
-
 template <typename Vector, typename Iterator>
 class sparse_iterator;
 
 template <typename Vector>
 class sparse_iterator<Vector, typename Vector::map_type::iterator>
-        : public sparse_iterator_base<
-                Vector,
-                typename Vector::map_type::iterator,
-                sparse_iterator<Vector, typename Vector::map_type::iterator>>
+    : public sparse_iterator_base<
+              Vector, typename Vector::map_type::iterator,
+              sparse_iterator<Vector, typename Vector::map_type::iterator>>
 {
-    using base = sparse_iterator_base<Vector,
-                                      typename Vector::map_type::iterator,
-                                      sparse_iterator<Vector, typename Vector::map_type::iterator>>;
+    using base = sparse_iterator_base<
+            Vector, typename Vector::map_type::iterator,
+            sparse_iterator<Vector, typename Vector::map_type::iterator>>;
     using base_iterator = typename Vector::map_type::iterator;
+
 public:
     using difference_type = std::ptrdiff_t;
     using value_type = sparse_iterator;
     using reference = sparse_iterator&;
     using pointer = sparse_iterator*;
     using iterator_category = std::forward_iterator_tag;
 
@@ -222,86 +216,91 @@
         assert(base::p_vector != nullptr);
         return value_reference(*base::p_vector, base::m_it);
     }
 };
 
 template <typename Vector>
 class sparse_iterator<Vector, typename Vector::map_type::const_iterator>
-    : public sparse_iterator_base<Vector,
-                                  typename Vector::map_type::const_iterator,
-        sparse_iterator<Vector, typename Vector::map_type::const_iterator>>
+    : public sparse_iterator_base<
+              Vector, typename Vector::map_type::const_iterator,
+              sparse_iterator<
+                      Vector, typename Vector::map_type::const_iterator>>
 {
-    using base = sparse_iterator_base<Vector,
-                                      typename Vector::map_type::const_iterator,
-                                      sparse_iterator<Vector, typename Vector::map_type::const_iterator>>;
+    using base = sparse_iterator_base<
+            Vector, typename Vector::map_type::const_iterator,
+            sparse_iterator<Vector, typename Vector::map_type::const_iterator>>;
     using base_iterator = typename Vector::map_type::const_iterator;
+
 public:
     using difference_type = std::ptrdiff_t;
     using iterator_category = std::forward_iterator_tag;
     using value_type = sparse_iterator;
     using reference = sparse_iterator&;
     using pointer = sparse_iterator*;
 
     using base::base;
 
     const typename base::key_type& key() const noexcept
-    { return base::m_it->first; }
+    {
+        return base::m_it->first;
+    }
     const typename base::scalar_type& value() const noexcept
-    { return base::m_it->second; }
+    {
+        return base::m_it->second;
+    }
 };
 
-
-
-
-} // namespace dtl
-
+}// namespace dtl
 
 template <typename Basis, typename Coefficients>
 class sparse_vector : public vectors::vector_base<Basis, Coefficients>
 {
     using vec_base = vectors::vector_base<Basis, Coefficients>;
     using typename vec_base::basis_traits;
     using typename vec_base::coeff_traits;
 
     friend class dtl::sparse_mutable_reference<sparse_vector>;
 
-
 public:
-
-    using typename vec_base::basis_type;
-    using typename vec_base::key_type;
     using typename vec_base::basis_pointer;
+    using typename vec_base::basis_type;
     using typename vec_base::coefficient_ring;
-    using typename vec_base::scalar_type;
+    using typename vec_base::key_type;
     using typename vec_base::rational_type;
+    using typename vec_base::scalar_type;
     using map_type = std::map<key_type, scalar_type>;
 
 private:
     map_type m_data;
     deg_t m_degree = 0;
     using vec_base::p_basis;
 
-    friend class dtl::sparse_iterator<sparse_vector, typename map_type::iterator>;
-    friend class dtl::sparse_iterator<const sparse_vector, typename map_type::const_iterator>;
+    friend class dtl::sparse_iterator<
+            sparse_vector, typename map_type::iterator>;
+    friend class dtl::sparse_iterator<
+            const sparse_vector, typename map_type::const_iterator>;
 
 protected:
     sparse_vector(basis_pointer basis, map_type&& arg)
         : vec_base(basis), m_data(arg)
     {}
 
 public:
-
     using reference = dtl::sparse_mutable_reference<sparse_vector>;
     using const_reference = const scalar_type&;
 
-    using iterator = dtl::sparse_iterator<sparse_vector, typename map_type::iterator>;
-    using const_iterator = dtl::sparse_iterator<const sparse_vector, typename map_type::const_iterator>;
+    using iterator
+            = dtl::sparse_iterator<sparse_vector, typename map_type::iterator>;
+    using const_iterator = dtl::sparse_iterator<
+            const sparse_vector, typename map_type::const_iterator>;
 
     template <typename Scalar>
-    explicit sparse_vector(basis_pointer basis, std::initializer_list<Scalar> args)
+    explicit sparse_vector(
+            basis_pointer basis, std::initializer_list<Scalar> args
+    )
         : vec_base(basis)
     {
         assert(args.size() == 1);
         m_data[key_type()] = scalar_type(*args.begin());
     }
 
     template <typename Key, typename Scalar>
@@ -311,123 +310,120 @@
         scalar_type tmp(s);
         if (tmp != coefficient_ring::zero()) {
             m_data.insert(std::make_pair(key_type(k), tmp));
             update_degree_for_key(k);
         }
     }
 
-    explicit sparse_vector(basis_pointer basis) : vec_base(basis)
-    {
-    }
+    explicit sparse_vector(basis_pointer basis) : vec_base(basis) {}
 
+    void swap(sparse_vector& right) {
+        std::swap(m_data, right.m_data);
+        std::swap(m_degree, right.m_degree);
+        vec_base::swap(right);
+    }
 
     constexpr dimn_t size() const noexcept { return m_data.size(); }
     constexpr bool empty() const noexcept { return m_data.empty(); }
     constexpr dimn_t dimension() const noexcept { return size(); }
     deg_t degree() const noexcept
     {
         deg_t result = 0;
         for (const auto& item : m_data) {
             auto d = p_basis->degree(item.first);
-            if (d > result) {
-                result = d;
-            }
+            if (d > result) { result = d; }
         }
         return result;
     }
-    dimn_t capacity() const noexcept { return basis_traits::max_dimension(*p_basis); }
+    dimn_t capacity() const noexcept
+    {
+        return basis_traits::max_dimension(*p_basis);
+    }
 
     void update_degree(deg_t degree) noexcept { m_degree = degree; }
 
     iterator begin() noexcept { return {*this, m_data.begin()}; }
     iterator end() noexcept { return {*this, m_data.end()}; }
     const_iterator begin() const noexcept { return {*this, m_data.begin()}; }
     const_iterator end() const noexcept { return {*this, m_data.end()}; }
 
     const_iterator cbegin() const noexcept { return begin(); }
     const_iterator cend() const noexcept { return end(); }
 
     const_reference operator[](const key_type& key) const noexcept
     {
         auto val = m_data.find(key);
-        if (val != m_data.end()) {
-            return val->second;
-        }
+        if (val != m_data.end()) { return val->second; }
         return coefficient_ring::zero();
     }
 
     reference operator[](const key_type& key) noexcept
     {
         return reference(*this, key);
     }
 
 private:
-
-    template <typename Tag=typename basis_traits::degree_tag>
-    std::enable_if_t<
-        std::is_same<
-            Tag,
-            with_degree_tag
-        >::value
-    >
-    update_degree_for_key(const key_type& key) {
+    template <typename Tag = typename basis_traits::degree_tag>
+    std::enable_if_t<std::is_same<Tag, with_degree_tag>::value>
+    update_degree_for_key(const key_type& key)
+    {
         auto degree = p_basis->degree(key);
         if (m_degree < degree && degree < basis_traits::max_degree(*p_basis)) {
             m_degree = degree;
         }
     }
 
-    template <typename Tag=typename basis_traits::degree_tag>
-    std::enable_if_t<
-        std::is_same<
-            Tag,
-            without_degree_tag
-        >::value
-    >
-    update_degree_for_key(const key_type&) {
+    template <typename Tag = typename basis_traits::degree_tag>
+    std::enable_if_t<std::is_same<Tag, without_degree_tag>::value>
+    update_degree_for_key(const key_type&)
+    {
         // Do Nothing
     }
 
 public:
-
-    void insert_new_value(const key_type& key, const scalar_type& value) {
+    void insert_new_value(const key_type& key, const scalar_type& value)
+    {
         m_data[key] = value;
         update_degree_for_key(key);
     }
 
-    void clear() noexcept
-    { m_data.clear(); }
+    void clear() noexcept { m_data.clear(); }
 
     template <typename UnaryOp>
     sparse_vector unary_op(UnaryOp op) const
     {
         map_type data;
-//        data.reserve(m_data.size());
-        const auto &zero = Coefficients::zero();
+        //        data.reserve(m_data.size());
+        const auto& zero = Coefficients::zero();
         for (const auto& item : m_data) {
             auto tmp = op(item.second);
-            if (tmp != zero) {
-                data.emplace(item.first, std::move(tmp));
-            }
+            if (tmp != zero) { data.emplace(item.first, std::move(tmp)); }
         }
         return {p_basis, std::move(data)};
     }
     template <typename UnaryOp>
-    sparse_vector& inplace_unary_op(UnaryOp op)
+    sparse_vector& inplace_unary_op(UnaryOp&& op)
     {
-        auto tmp = this->unary_op([op] (const scalar_type& arg) { auto tmp = arg; op(tmp); return tmp; });
+        auto tmp = this->unary_op(
+            [op = forward<UnaryOp>(op)](const scalar_type& arg) {
+            auto tmp = arg;
+            op(tmp);
+            return tmp;
+        });
         std::swap(m_data, tmp.m_data);
         return *this;
     }
 
     template <typename BinOp>
-    sparse_vector binary_op(const sparse_vector& rhs, BinOp op) const
+    sparse_vector binary_op(const sparse_vector& rhs, BinOp&& op) const
     {
         sparse_vector tmp(*this);
-        tmp.inplace_binary_op(rhs, [op](scalar_type& l, const scalar_type& r) {
+        tmp.inplace_binary_op(rhs, [op=forward<BinOp>(op)](scalar_type& l,
+                                                             const
+                                                scalar_type& r) {
             l = op(l, r);
         });
 
         return tmp;
     }
 
     template <typename BinOp>
@@ -452,34 +448,29 @@
                 assert(rit->second != zero);
                 scalar_type new_val = zero;
                 op(new_val, rit->second);
                 insert_new_value(rit->first, new_val);
             }
         }
 
-
         return *this;
     }
 
+    bool operator==(const sparse_vector& rhs) const noexcept
+    {
 
-    bool operator==(const sparse_vector& rhs) const noexcept {
-
-        if (m_data.size() != rhs.m_data.size()) {
-            return false;
-        }
+        if (m_data.size() != rhs.m_data.size()) { return false; }
 
         for (auto&& ritem : rhs.m_data) {
             auto found = m_data.find(ritem.first);
             if (found == m_data.end() || found->second != ritem.second) {
                 return false;
             }
         }
 
         return true;
     }
-
 };
 
+}// namespace lal
 
-} // namespace lal
-
-#endif //LIBALGEBRA_LITE_SPARSE_VECTOR_H
+#endif// LIBALGEBRA_LITE_SPARSE_VECTOR_H
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector.h`

 * *Files 8% similar despite different names*

```diff
@@ -180,26 +180,29 @@
         : base_type(std::move(basis), key_type(key), scalar_type(s)) {}
 
     explicit vector(basis_pointer basis) : base_type(std::move(basis)) {}
 
     vector(basis_pointer basis, std::initializer_list<scalar_type> args)
         : base_type(vector_type(basis, args)) {}
 
-    vector(basis_pointer basis, const vector_type &arg)
+    explicit vector(const vector_type &arg)
         : base_type(vector_type(arg)) {
     }
 
+
     vector& operator=(const vector&) = default;
     vector& operator=(vector&&) noexcept = default;
 
 
     vector clone() const {
         return vector(*this);
     }
 
+    vector create_alike() const { return vector(get_basis()); }
+
     vector_type &base_vector() noexcept { return base_type::instance(); }
     const vector_type &base_vector() const noexcept { return base_type::instance(); }
 
     dimn_t size() const noexcept {
         return base_type::instance().size();
     }
 
@@ -256,61 +259,63 @@
             std::declval<F>()
         ))>>
         : std::true_type {
     };
 
 public:
 
-    template <typename Iter, typename C>
-    std::enable_if_t<
-        has_iterator_inplace_binop<
-            vector_type,
-            decltype(coefficient_ring::template add_inplace<>),
-            Iter
-        >::value,
-        vector &>
-    add_inplace(Iter begin, Iter end) {
-        return base_type::instance()
-            .inplace_binop(begin, end, coefficient_ring::add_inplace);
-    }
-
-    template <typename Iter>
-    std::enable_if_t<
-        has_iterator_inplace_binop<
-            vector_type,
-            decltype(coefficient_ring::template add_inplace<>),
-            Iter>::value,
-        vector &>
-    sub_inplace(Iter begin, Iter end) {
-        return base_type::instance()
-            .inplace_binop(begin, end, coefficient_ring::sub_inplace);
-    }
+//    template <typename Iter, typename C>
+//    std::enable_if_t<
+//        has_iterator_inplace_binop<
+//            vector_type,
+//            decltype(coefficient_ring::template add_inplace<>),
+//            Iter
+//        >::value,
+//        vector &>
+//    add_inplace(Iter begin, Iter end) {
+//        return base_type::instance()
+//            .inplace_binop(begin, end, coefficient_ring::add_inplace);
+//    }
+//
+//    template <typename Iter>
+//    std::enable_if_t<
+//        has_iterator_inplace_binop<
+//            vector_type,
+//            decltype(coefficient_ring::template add_inplace<>),
+//            Iter>::value,
+//        vector &>
+//    sub_inplace(Iter begin, Iter end) {
+//        return base_type::instance()
+//            .inplace_binop(begin, end, coefficient_ring::sub_inplace);
+//    }
 
     template <typename Iter>
-    std::enable_if_t<
-        !has_iterator_inplace_binop<
-            vector_type,
-            decltype(coefficient_ring::template add_inplace<>),
-            Iter>::value,
-        vector &>
+//    std::enable_if_t<
+//        !has_iterator_inplace_binop<
+//            vector_type,
+//            decltype(coefficient_ring::template add_inplace<>),
+//            Iter>::value,
+//        vector &>
+    vector&
     add_inplace(Iter begin, Iter end) {
         const auto &self = base_type::instance();
         for (auto it = begin; it != end; ++it) {
             self[it->first] += it->second;
         }
         return *this;
     }
 
     template <typename Iter>
-    std::enable_if_t<
-        !has_iterator_inplace_binop<
-            vector_type,
-            decltype(coefficient_ring::template sub_inplace<>),
-            Iter>::value,
-        vector &>
+//    std::enable_if_t<
+//        !has_iterator_inplace_binop<
+//            vector_type,
+//            decltype(coefficient_ring::template sub_inplace<>),
+//            Iter>::value,
+//        vector &>
+    vector&
     sub_inplace(Iter begin, Iter end) {
         const auto &self = base_type::instance();
         for (auto it = begin; it != end; ++it) {
             self[it->first] -= it->second;
         }
     }
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_base.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector_base.h`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,19 @@
     using key_type              = typename basis_traits::key_type;
     using coefficient_ring      = typename coeff_traits::coefficient_ring;
     using scalar_type           = typename coeff_traits::scalar_type;
     using rational_type         = typename coeff_traits::rational_type;
 
     basis_pointer get_basis() const noexcept { return p_basis; }
     const Basis& basis() const noexcept { return *p_basis; }
+
+    void swap(vector_base& other) {
+        std::swap(p_basis, other.p_basis);
+    }
+
 };
 
 
 } // namespace vectors
 } // namespace lal
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h` & `roughpy-0.0.5/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/algebra/lie_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/algebra/lie_multiplier.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 namespace lal {
 
 template class base_multiplier<lie_multiplier, hall_basis, 2>;
 
 lie_multiplier::product_type
 lie_multiplier::key_prod_impl(const hall_basis& basis, key_type lhs, key_type rhs) const
 {
+    assert(basis.width() == m_width);
+
     if (lhs>rhs) {
         return lie_multiplier::uminus(operator()(basis, rhs, lhs));
     }
 
     product_type result;
     if (basis.degree(lhs) + basis.degree(rhs) > basis.depth()) {
         return result;
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/basis/hall_set.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/basis/hall_set.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -145,20 +145,21 @@
         assert(found->second.degree() == parent.first.degree() +parent.second.degree());
         return found->second;
     }
     return root_element;
 }
 dimn_t hall_set::index_of_key(hall_set::key_type arg) const noexcept
 {
+    assert(arg.degree() > 0);
     return arg.index() + size(deg_t(arg.degree())-1);
 }
 hall_set::key_type hall_set::key_of_index(hall_set::size_type index) const noexcept
 {
     auto found = std::lower_bound(
-            m_sizes.begin(),
+            ++m_sizes.begin(),
             m_sizes.end(),
             index,
             std::less_equal<>()
             );
     if (found == m_sizes.end()) {
         return root_element;
     }
```

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/basis/monomial.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/basis/monomial.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/basis/polynomial_basis.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/basis/polynomial_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/basis/tensor_basis.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/basis/tensor_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/src/maps.cpp` & `roughpy-0.0.5/external/libalgebra_lite/src/maps.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/lie/hall_basis.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/lie/hall_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_fixture.h` & `roughpy-0.0.5/external/libalgebra_lite/tests/lie/lie_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/lie/lie_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/maps/maps.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps_fixture.h` & `roughpy-0.0.5/external/libalgebra_lite/tests/maps/maps_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h` & `roughpy-0.0.5/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/CMakeLists.txt` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/dense_tensor.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/dense_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_basis.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/tensor_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_fixture.h` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/tensor_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/tests/utilities/packed_integer.cpp` & `roughpy-0.0.5/external/libalgebra_lite/tests/utilities/packed_integer.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/libalgebra_lite/vcpkg.json` & `roughpy-0.0.5/external/libalgebra_lite/vcpkg.json`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/CMakeLists.txt` & `roughpy-0.0.5/external/recombine/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/LICENSE.txt` & `roughpy-0.0.5/external/recombine/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/README.md` & `roughpy-0.0.5/external/recombine/README.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/CMakeLists.txt` & `roughpy-0.0.5/external/recombine/recombine/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/BufferConstructor.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/BufferConstructor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/Compare.cpp` & `roughpy-0.0.5/external/recombine/recombine/recombine/Compare.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp` & `roughpy-0.0.5/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/RdToPowers.cpp` & `roughpy-0.0.5/external/recombine/recombine/recombine/RdToPowers.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/SafeInt3.hpp` & `roughpy-0.0.5/external/recombine/recombine/recombine/SafeInt3.hpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.cpp` & `roughpy-0.0.5/external/recombine/recombine/recombine/TreeBufferHelper.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/TreeBufferHelper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/aligned_allocator.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/aligned_allocator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/lapack_defns.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/lapack_defns.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/lapack_fortran_definitions.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/lapack_fortran_definitions.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/recombine.cpp` & `roughpy-0.0.5/external/recombine/recombine/recombine/recombine.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/recombine.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/recombine.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/reweight.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/reweight.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/stdafx.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/stdafx.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/recombine/recombine/tjlUtilities.h` & `roughpy-0.0.5/external/recombine/recombine/recombine/tjlUtilities.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/test_recombine/CMakeLists.txt` & `roughpy-0.0.5/external/recombine/test_recombine/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h` & `roughpy-0.0.5/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h` & `roughpy-0.0.5/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp` & `roughpy-0.0.5/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/test_recombine/TestVec/utils.h` & `roughpy-0.0.5/external/recombine/test_recombine/TestVec/utils.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/external/recombine/test_recombine/test_recombine.cpp` & `roughpy-0.0.5/external/recombine/test_recombine/test_recombine.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/CMakeLists.txt` & `roughpy-0.0.5/intervals/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic.h` & `roughpy-0.0.5/intervals/include/roughpy/intervals/dyadic.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic_interval.h` & `roughpy-0.0.5/intervals/include/roughpy/intervals/dyadic_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/include/roughpy/intervals/interval.h` & `roughpy-0.0.5/intervals/include/roughpy/intervals/interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/include/roughpy/intervals/partition.h` & `roughpy-0.0.5/intervals/include/roughpy/intervals/partition.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/include/roughpy/intervals/real_interval.h` & `roughpy-0.0.5/intervals/include/roughpy/intervals/real_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/include/roughpy/intervals/segmentation.h` & `roughpy-0.0.5/intervals/include/roughpy/intervals/segmentation.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/dyadic.cpp` & `roughpy-0.0.5/intervals/src/dyadic.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/dyadic_interval.cpp` & `roughpy-0.0.5/intervals/src/dyadic_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/dyadic_searcher.cpp` & `roughpy-0.0.5/intervals/src/dyadic_searcher.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/dyadic_searcher.h` & `roughpy-0.0.5/intervals/src/dyadic_searcher.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/interval.cpp` & `roughpy-0.0.5/intervals/src/interval.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 using namespace rpy;
 using namespace rpy::intervals;
 
 param_t Interval::included_end() const
 {
     if (m_interval_type == IntervalType::Clopen) { return inf(); }
     if (m_interval_type == IntervalType::Opencl) { return sup(); }
-    throw std::runtime_error(
+    RPY_THROW(std::runtime_error,
             "included_end is not valid for intervals that are not half open");
 }
 param_t Interval::excluded_end() const
 {
     if (m_interval_type == IntervalType::Clopen) { return sup(); }
     if (m_interval_type == IntervalType::Opencl) { return inf(); }
-    throw std::runtime_error(
+    RPY_THROW(std::runtime_error,
             "excluded_end is not valid for intervals that are not half open");
 }
 bool Interval::contains_point(param_t arg) const noexcept
 {
     if (m_interval_type == IntervalType::Clopen) {
         return inf() <= arg && arg < sup();
     }
```

### Comparing `roughpy-0.0.4/intervals/src/partition.cpp` & `roughpy-0.0.5/intervals/src/partition.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     return RealInterval(m_intermediate_points[i - 1], m_intermediate_points[i],
                         type());
 }
 
 void Partition::insert_intermediate(param_t new_intermediate)
 {
     if (!contains_point(new_intermediate)) {
-        throw std::invalid_argument("provided intermediate does not lie "
+        RPY_THROW(std::invalid_argument,"provided intermediate does not lie "
                                     "within the interval");
     }
 
     // Use find-insert rather than push_back-sort since this should
     // require fewer comparisons
     auto insert_point
             = std::lower_bound(m_intermediate_points.begin(),
```

### Comparing `roughpy-0.0.4/intervals/src/real_interval.cpp` & `roughpy-0.0.5/intervals/src/real_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/scaled_predicate.cpp` & `roughpy-0.0.5/intervals/src/scaled_predicate.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/scaled_predicate.h` & `roughpy-0.0.5/intervals/src/scaled_predicate.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/segmentation.cpp` & `roughpy-0.0.5/intervals/src/segmentation.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/test_dyadic.cpp` & `roughpy-0.0.5/intervals/src/test_dyadic.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/test_dyadic_intervals.cpp` & `roughpy-0.0.5/intervals/src/test_dyadic_intervals.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/test_partition.cpp` & `roughpy-0.0.5/intervals/src/test_partition.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/intervals/src/test_real_interval.cpp` & `roughpy-0.0.5/intervals/src/test_real_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/CMakeLists.txt` & `roughpy-0.0.5/la_context/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/free_tensor_info.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/free_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/lie_basis_info.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/lie_basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/lie_info.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/lie_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/shuffle_tensor_info.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/shuffle_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/tensor_basis_info.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/tensor_basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/vector_iterator.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/vector_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_helper.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/vector_type_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_selector.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context/vector_type_selector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/la_context/include/roughpy/la_context.h` & `roughpy-0.0.5/la_context/include/roughpy/la_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
     const auto& arg_context = arg->context();
     if (arg_context == this) {
         maps_t<VType> maps;
         return maps.l2t(algebra_cast<lie_t<VType>>(*arg));
     }
 
     if (arg_context->width() != width()) {
-        throw std::invalid_argument(
+        RPY_THROW(std::invalid_argument,
                 "cannot perform conversion on algebras with different bases");
     }
 
     return convert_impl<VType>(arg_context->lie_to_tensor(arg));
 }
 template <deg_t Width, deg_t Depth, typename Coefficients>
 template <VectorType VType>
@@ -298,15 +298,15 @@
 
     maps_t<VType> maps;
     if (arg_context == this) {
         return maps.t2l(algebra_cast<free_tensor_t<VType>>(*arg));
     }
 
     if (arg_context->width() != width()) {
-        throw std::invalid_argument(
+        RPY_THROW(std::invalid_argument,
                 "cannot perform conversion on algebras with different bases");
     }
 
     return maps.t2l(convert_impl<VType>(arg));
 }
 template <deg_t Width, deg_t Depth, typename Coefficients>
 template <VectorType VType>
```

### Comparing `roughpy-0.0.4/la_context/src/la_context.cpp` & `roughpy-0.0.5/la_context/src/la_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/platform/CMakeLists.txt` & `roughpy-0.0.5/platform/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/platform/include/roughpy/platform/configuration.h` & `roughpy-0.0.5/platform/include/roughpy/platform/configuration.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/platform/include/roughpy/platform/filesystem.h` & `roughpy-0.0.5/platform/include/roughpy/platform/filesystem.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/platform/include/roughpy/platform/serialization.h` & `roughpy-0.0.5/platform/include/roughpy/platform/serialization.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/platform/include/roughpy/platform/serialization_instantiations.inl` & `roughpy-0.0.5/platform/include/roughpy/platform/serialization_instantiations.inl`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/platform/include/roughpy/platform.h` & `roughpy-0.0.5/platform/include/roughpy/platform.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/platform/src/configuration.cpp` & `roughpy-0.0.5/platform/src/configuration.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/pyproject.toml` & `roughpy-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/CMakeLists.txt` & `roughpy-0.0.5/roughpy/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         src/algebra/algebra.cpp
         src/algebra/algebra_iterator.cpp
         src/algebra/algebra_iterator.h
         src/algebra/basis.cpp
         src/algebra/basis.h
         src/algebra/context.cpp
         src/algebra/context.h
+        src/algebra/free_multiply_funcs.cpp
+        src/algebra/free_multiply_funcs.h
         src/algebra/free_tensor.h
         src/algebra/free_tensor.cpp
         src/algebra/lie.cpp
         src/algebra/lie.h
         src/algebra/lie_key.cpp
         src/algebra/lie_key.h
         src/algebra/lie_key_iterator.cpp
```

### Comparing `roughpy-0.0.4/roughpy/_roughpy.pyi` & `roughpy-0.0.5/roughpy/_roughpy.pyi`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/algebra.cpp` & `roughpy-0.0.5/roughpy/src/algebra/algebra.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -29,34 +29,40 @@
 //
 // Created by user on 14/03/23.
 //
 
 #include "algebra.h"
 
 #include "algebra_iterator.h"
+#include "basis.h"
 #include "free_tensor.h"
 #include "lie.h"
 #include "lie_key.h"
 #include "lie_key_iterator.h"
 #include "shuffle_tensor.h"
 #include "tensor_key.h"
 #include "tensor_key_iterator.h"
+#include "free_multiply_funcs.h"
 
 void rpy::python::init_algebra(pybind11::module_& m)
 {
 
     py::enum_<algebra::VectorType>(m, "VectorType")
             .value("DenseVector", algebra::VectorType::Dense)
             .value("SparseVector", algebra::VectorType::Sparse)
             .export_values();
 
     init_py_tensor_key(m);
     init_py_lie_key(m);
     init_tensor_key_iterator(m);
     init_lie_key_iterator(m);
+    init_basis(m);
     init_context(m);
     init_algebra_iterator(m);
 
     init_free_tensor(m);
     init_shuffle_tensor(m);
     init_lie(m);
+
+    init_free_multiply_funcs(m);
+
 }
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/algebra.h` & `roughpy-0.0.5/roughpy/src/algebra/algebra.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.cpp` & `roughpy-0.0.5/roughpy/src/algebra/algebra_iterator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.h` & `roughpy-0.0.5/roughpy/src/algebra/algebra_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/basis.cpp` & `roughpy-0.0.5/roughpy/src/algebra/basis.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -29,26 +29,32 @@
 #include "basis.h"
 
 #include <roughpy/algebra/basis.h>
 #include <roughpy/algebra/lie_basis.h>
 #include <roughpy/algebra/tensor_basis.h>
 
 #include "lie_key.h"
+#include "lie_key_iterator.h"
 #include "tensor_key.h"
+#include "tensor_key_iterator.h"
 
 using namespace rpy;
 using namespace rpy::algebra;
 using namespace pybind11::literals;
 
-template <typename T, typename K>
-static void wordlike_basis_setup(py::module_& m, const char* name)
+template <typename T, typename K, typename KIter>
+static py::class_<T> wordlike_basis_setup(py::module_& m, const char* name)
 {
 
     py::class_<T> basis(m, name);
 
+//    basis.def(py::init<deg_t, deg_t>([](deg_t width, deg_t depth) {
+//
+//         }));
+
     basis.def_property_readonly("width", &T::width);
     basis.def_property_readonly("depth", &T::depth);
     basis.def_property_readonly("dimension", &T::dimension);
 
     basis.def(
             "index_to_key",
             [](const T& self, dimn_t index) {
@@ -62,18 +68,30 @@
                 return self.key_to_index(0);
             },
             "key"_a
     );
 
     basis.def(
             "parents",
-            [](const T& self, const K& key) { return self.parents(0); }, "key"_a
+            [](const T& self, const K& key) { return self.parents(0); },
+            "key"_a
     );
     basis.def("size", &T::size);
+
+    basis.def("__iter__", [](const T& self) {
+        return KIter(self);
+    });
+
+    return basis;
 }
 
 void python::init_basis(py::module_& m)
 {
 
-    wordlike_basis_setup<TensorBasis, PyTensorKey>(m, "TensorBasis");
-    wordlike_basis_setup<LieBasis, PyLieKey>(m, "LieBasis");
+    wordlike_basis_setup<TensorBasis, PyTensorKey, PyTensorKeyIterator>(
+            m, "TensorBasis"
+    );
+
+    wordlike_basis_setup<LieBasis, PyLieKey, PyLieKeyIterator>(
+            m, "LieBasis"
+    );
 }
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/basis.h` & `roughpy-0.0.5/roughpy/src/algebra/basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/context.cpp` & `roughpy-0.0.5/roughpy/src/algebra/context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/context.h` & `roughpy-0.0.5/roughpy/src/algebra/context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/free_tensor.cpp` & `roughpy-0.0.5/roughpy/src/algebra/free_tensor.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -101,26 +101,26 @@
     options.type = helper.ctype;
     options.alternative_key = &alt;
 
     auto buffer = python::py_to_buffer(data, options);
 
     if (helper.ctype == nullptr) {
         if (options.type == nullptr) {
-            throw py::value_error("could not deduce appropriate scalar type");
+            RPY_THROW(py::value_error, "could not deduce appropriate scalar type");
         }
         helper.ctype = options.type;
     }
 
     if (helper.width == 0 && buffer.size() > 0) {
         helper.width = static_cast<deg_t>(buffer.size()) - 1;
     }
 
     if (!helper.ctx) {
         if (helper.width == 0 || helper.depth == 0) {
-            throw py::value_error(
+            RPY_THROW(py::value_error,
                     "you must provide either context or both width and depth"
             );
         }
         helper.ctx = get_context(helper.width, helper.depth, helper.ctype, {});
     }
 
     if (!helper.vtype_requested) {
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/free_tensor.h` & `roughpy-0.0.5/roughpy/src/algebra/free_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie.cpp` & `roughpy-0.0.5/roughpy/src/algebra/lie.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -58,27 +58,27 @@
     options.type = helper.ctype;
     options.allow_scalar = false;
 
     auto buffer = py_to_buffer(data, options);
 
     if (helper.ctype == nullptr) {
         if (options.type == nullptr) {
-            throw py::value_error("could not deduce an appropriate scalar_type"
+            RPY_THROW(py::value_error,"could not deduce an appropriate scalar_type"
             );
         }
         helper.ctype = options.type;
     }
 
     if (helper.width == 0 && buffer.size() > 0) {
         helper.width = static_cast<deg_t>(buffer.size());
     }
 
     if (!helper.ctx) {
         if (helper.width == 0 || helper.depth == 0) {
-            throw py::value_error(
+            RPY_THROW(py::value_error,
                     "you must provide either context or both width and depth"
             );
         }
         helper.ctx = get_context(helper.width, helper.depth, helper.ctype, {});
     }
 
     auto result = helper.ctx->construct_lie({std::move(buffer), helper.vtype});
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie.h` & `roughpy-0.0.5/roughpy/src/algebra/lie.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie_key.cpp` & `roughpy-0.0.5/roughpy/src/algebra/lie_key.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,15 @@
 
 public:
     explicit ToLieKeyHelper(deg_t w) : size(2), current(0), width(w) {}
 
     container_type parse_list(const py::handle& obj)
     {
         if (py::len(obj) != 2) {
-            throw py::value_error("list items must contain exactly two elements"
+            RPY_THROW(py::value_error,"list items must contain exactly two elements"
             );
         }
 
         auto left = obj[py::int_(0)];
         auto right = obj[py::int_(1)];
 
         return parse_pair(left, right);
@@ -317,15 +317,15 @@
     {
         if (py::isinstance<py::list>(obj)) { return parse_list(obj); }
         if (py::isinstance<py::int_>(obj)) {
             auto as_let = obj.cast<let_t>();
             if (as_let > max_letter) { max_letter = as_let; }
             return container_type{python::PyLieLetter::from_letter(as_let)};
         }
-        throw py::type_error("items must be either int or lists");
+        RPY_THROW(py::type_error, "items must be either int or lists");
     }
 
     container_type parse_pair(const py::handle& left, const py::handle& right)
     {
 
         auto left_tree = parse_single(left);
         auto right_tree = parse_single(right);
@@ -355,26 +355,26 @@
 
         return result;
     }
 
     container_type operator()(const py::handle& obj)
     {
         if (!py::isinstance<py::list>(obj)) {
-            throw py::type_error("expected a list with exactly two elements");
+            RPY_THROW(py::type_error, "expected a list with exactly two elements");
         }
         if (py::len(obj) != 2) {
-            throw py::value_error("expected list with exactly 2 elements");
+            RPY_THROW(py::value_error, "expected list with exactly 2 elements");
         }
         return parse_pair(obj[py::int_(0)], obj[py::int_(1)]);
     }
 
     deg_t get_width()
     {
         if (width != 0 && max_letter > width) {
-            throw py::value_error("a letter exceeds the width");
+            RPY_THROW(py::value_error, "a letter exceeds the width");
         } else {
             width = max_letter;
         }
         return width;
     }
 };
 
@@ -383,28 +383,28 @@
 static python::PyLieKey
 make_lie_key(const py::args& args, const py::kwargs& kwargs)
 {
     deg_t width = 0;
 
     if (kwargs.contains("width")) { width = kwargs["width"].cast<deg_t>(); }
 
-    if (args.empty()) { throw py::value_error("argument cannot be empty"); }
+    if (args.empty()) { RPY_THROW(py::value_error, "argument cannot be empty"); }
 
     if (py::isinstance<py::int_>(args[0])) {
         auto letter = args[0].cast<let_t>();
         if (width != 0 && letter > width) {
-            throw py::value_error("letter exceeds width");
+            RPY_THROW(py::value_error, "letter exceeds width");
         } else {
             width = deg_t(letter);
         }
         return python::PyLieKey(width, letter);
     }
 
     if (!py::isinstance<py::list>(args[0])) {
-        throw py::type_error("expected int or list");
+        RPY_THROW(py::type_error, "expected int or list");
     }
 
     ToLieKeyHelper helper(width);
 
     return python::PyLieKey(helper.get_width(), helper(args[0]));
 }
 void python::init_py_lie_key(py::module_& m)
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie_key.h` & `roughpy-0.0.5/roughpy/src/algebra/lie_key.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.cpp` & `roughpy-0.0.5/roughpy/src/streams/piecewise_abelian_stream.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -22,75 +22,75 @@
 // CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 // SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 // INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 // CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 // ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 // POSSIBILITY OF SUCH DAMAGE.
 
-#include "lie_key_iterator.h"
+//
+// Created by user on 18/03/23.
+//
 
-#include <roughpy/algebra/basis.h>
-#include <roughpy/algebra/context.h>
+#include "piecewise_abelian_stream.h"
 
-#include "context.h"
+#include <roughpy/streams/piecewise_abelian_stream.h>
+#include <roughpy/streams/stream.h>
+
+#include "args/kwargs_to_path_metadata.h"
+#include "stream.h"
 
 using namespace rpy;
 using namespace pybind11::literals;
 
-static const char* LKEY_ITERATOR_DOC
-        = R"eadoc(Iterator over range of Hall set members.
-)eadoc";
-
-python::PyLieKeyIterator::PyLieKeyIterator(
-        const py::object& ctx, key_type current, key_type end
+static const char* PW_LIE_STREAM_DOC
+        = R"rpydoc(A stream formed of a sequence of interval-Lie pairs.
+)rpydoc";
+
+static py::object construct_piecewise_lie_stream(
+        std::vector<std::pair<intervals::RealInterval, algebra::Lie>> lies,
+        const py::kwargs& kwargs
 )
-    : m_current(current), m_end(end)
 {
-    if (!py::isinstance(ctx, reinterpret_cast<PyObject*>(&RPyContext_Type))) {
-        throw py::type_error("expected a Context object");
+
+    auto pmd = python::kwargs_to_metadata(kwargs);
+
+    if (!pmd.ctx) {
+        if (pmd.width == 0 || pmd.depth == 0 || !pmd.scalar_type) {
+            RPY_THROW(py::value_error, "cannot deduce width/depth/ctype");
+        }
+        pmd.ctx = algebra::get_context(pmd.width, pmd.depth, pmd.scalar_type);
     }
-    p_ctx = python::ctx_cast(ctx.ptr());
-}
+    // TODO: make this more robust
 
-static python::PyLieKey
-to_py_lie_key(key_type k, const algebra::LieBasis& lbasis)
-{
-    auto width = lbasis.width();
+    using nl = std::numeric_limits<param_t>;
+    param_t a = nl::infinity();
+    param_t b = -nl::infinity();
+    for (auto& piece : lies) {
+        if (piece.first.inf() < a) { a = piece.first.inf(); }
+        if (piece.first.sup() > b) { b = piece.first.sup(); }
+    }
 
-    if (lbasis.letter(k)) { return python::PyLieKey(width, k); }
+    pmd.support = intervals::RealInterval(a, b);
 
-    auto lparent = *lbasis.lparent(k);
-    auto rparent = *lbasis.rparent(k);
+    streams::Stream result(streams::PiecewiseAbelianStream(
+            std::move(lies),
+            {pmd.width,
+             pmd.support ? *pmd.support : intervals::RealInterval(0, 1),
+             pmd.ctx, pmd.scalar_type,
+             pmd.vector_type ? *pmd.vector_type : algebra::VectorType::Dense,
+             pmd.resolution}
+    ));
 
-    if (lbasis.letter(lparent) && lbasis.letter(rparent)) {
-        return python::PyLieKey(lbasis.width(), lparent, rparent);
-    }
-    if (lbasis.letter(lparent)) {
-        return python::PyLieKey(width, lparent, to_py_lie_key(rparent, lbasis));
-    }
-    return python::PyLieKey(
-            width, to_py_lie_key(lparent, lbasis),
-            to_py_lie_key(rparent, lbasis)
+    return py::reinterpret_steal<py::object>(
+            python::RPyStream_FromStream(std::move(result))
     );
 }
 
-python::PyLieKey python::PyLieKeyIterator::next()
+void python::init_piecewise_lie_stream(py::module_& m)
 {
-    if (m_current > m_end) { throw py::stop_iteration(); }
-    auto current = m_current;
-    ++m_current;
-    return to_py_lie_key(current, p_ctx->get_lie_basis());
-}
 
-void python::init_lie_key_iterator(py::module_& m)
-{
-    py::class_<PyLieKeyIterator> klass(m, "LieKeyIterator", LKEY_ITERATOR_DOC);
-    klass.def(py::init<py::object>(), "context"_a);
-    klass.def(py::init<py::object, key_type>(), "context"_a, "start_key"_a);
-    klass.def(
-            py::init<py::object, key_type, key_type>(), "context"_a,
-            "start_key"_a, "end_key"_a
+    py::class_<streams::PiecewiseAbelianStream> klass(
+            m, "PiecewiseAbelianStream", PW_LIE_STREAM_DOC
     );
 
-    klass.def("__iter__", [](PyLieKeyIterator& self) { return self; });
-    klass.def("__next__", &PyLieKeyIterator::next);
+    klass.def_static("construct", &construct_piecewise_lie_stream);
 }
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.h` & `roughpy-0.0.5/roughpy/src/algebra/lie_key_iterator.h`

 * *Files 8% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 namespace rpy {
 namespace python {
 
 class PyLieKeyIterator
 {
     key_type m_current;
     key_type m_end;
-    algebra::context_pointer p_ctx;
+    algebra::LieBasis m_basis;
 
 public:
     explicit PyLieKeyIterator(
-            const py::object& ctx, key_type current = 1,
+            algebra::LieBasis basis, key_type current = 1,
             key_type end = std::numeric_limits<key_type>::max()
     );
 
     PyLieKey next();
 };
 
 void init_lie_key_iterator(py::module_& m);
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie_letter.cpp` & `roughpy-0.0.5/roughpy/src/algebra/lie_letter.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/lie_letter.h` & `roughpy-0.0.5/roughpy/src/algebra/lie_letter.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/setup_algebra_type.h` & `roughpy-0.0.5/roughpy/src/algebra/setup_algebra_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.cpp` & `roughpy-0.0.5/roughpy/src/algebra/shuffle_tensor.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -66,26 +66,26 @@
     options.type = helper.ctype;
     options.alternative_key = &alt;
 
     auto buffer = python::py_to_buffer(data, options);
 
     if (helper.ctype == nullptr) {
         if (options.type == nullptr) {
-            throw py::value_error("could not deduce appropriate scalar type");
+            RPY_THROW(py::value_error, "could not deduce appropriate scalar type");
         }
         helper.ctype = options.type;
     }
 
     if (helper.width == 0 && buffer.size() > 0) {
         helper.width = static_cast<deg_t>(buffer.size()) - 1;
     }
 
     if (!helper.ctx) {
         if (helper.width == 0 || helper.depth == 0) {
-            throw py::value_error(
+            RPY_THROW(py::value_error,
                     "you must provide either context or both width and depth"
             );
         }
         helper.ctx = get_context(helper.width, helper.depth, helper.ctype, {});
     }
 
     if (!helper.vtype_requested) {
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.h` & `roughpy-0.0.5/roughpy/src/algebra/shuffle_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/algebra/tensor_key.cpp` & `roughpy-0.0.5/roughpy/src/algebra/tensor_key.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -23,26 +23,25 @@
 // SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 // INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 // CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 // ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 // POSSIBILITY OF SUCH DAMAGE.
 
 #include "tensor_key.h"
+#include <roughpy/algebra/context.h>
 
 #include <algorithm>
 #include <sstream>
 
 using namespace rpy;
 using namespace pybind11::literals;
 
-python::PyTensorKey::PyTensorKey(key_type key, deg_t width, deg_t depth)
-    : m_key(key), m_width(width), m_depth(depth)
-{}
+
 python::PyTensorKey::PyTensorKey(algebra::TensorBasis basis, key_type key)
-    : m_key(key), m_width(basis.width()), m_depth(basis.depth())
+    : m_key(key), m_basis(move(basis))
 {}
 
 python::PyTensorKey::operator key_type() const noexcept { return m_key; }
 string python::PyTensorKey::to_string() const
 {
     std::stringstream ss;
     ss << '(';
@@ -53,44 +52,71 @@
         not_first = true;
     }
     ss << ')';
     return ss.str();
 }
 python::PyTensorKey python::PyTensorKey::lparent() const
 {
-    return python::PyTensorKey(0, 0, 0);
+    return python::PyTensorKey(m_basis, 0);
 }
 python::PyTensorKey python::PyTensorKey::rparent() const
 {
-    return python::PyTensorKey(0, 0, 0);
+    return python::PyTensorKey(m_basis, 0);
+}
+pair<python::PyTensorKey, python::PyTensorKey>
+python::PyTensorKey::split_n(deg_t n) const
+{
+    if (m_key == 0) {
+        return std::make_pair(PyTensorKey(m_basis, 0), PyTensorKey(m_basis, 0));
+    }
+    if (n <= 0) {
+        return std::make_pair(*this,PyTensorKey(m_basis, 0));
+    }
+    if (n >= m_basis.depth()) {
+        return std::make_pair(PyTensorKey(m_basis, 0), *this);
+    }
+
+    auto width = m_basis.width();
+    //TODO: needs better implementation
+    key_type shift = 1;
+    for (deg_t i=0; i<n; ++i) {
+        shift *= width;
+    }
+    auto left = (m_key - 1) / shift;
+    auto right = 1 + ((m_key - 1) % shift);
+
+    return std::make_pair(PyTensorKey(m_basis, left), PyTensorKey(m_basis, right));
+
 }
 bool python::PyTensorKey::is_letter() const
 {
-    return 1 <= m_key && m_key <= static_cast<key_type>(m_width);
+    return 1 <= m_key && m_key <= static_cast<key_type>(m_basis.width());
 }
-deg_t python::PyTensorKey::width() const { return m_width; }
-deg_t python::PyTensorKey::depth() const { return m_depth; }
-deg_t python::PyTensorKey::degree() const { return m_depth; }
+deg_t python::PyTensorKey::width() const { return m_basis.width(); }
+deg_t python::PyTensorKey::depth() const { return m_basis.depth(); }
+deg_t python::PyTensorKey::degree() const { return m_basis.depth(); }
 std::vector<let_t> python::PyTensorKey::to_letters() const
 {
     std::vector<let_t> letters;
-    letters.reserve(m_depth);
+    const auto width = m_basis.width();
+    const auto depth = m_basis.depth();
+    letters.reserve(depth);
     auto tmp = m_key;
     while (tmp) {
         tmp -= 1;
-        letters.push_back(1 + (tmp % m_width));
-        tmp /= m_width;
+        letters.push_back(1 + (tmp % width));
+        tmp /= width;
     }
     std::reverse(letters.begin(), letters.end());
     return letters;
 }
 bool python::PyTensorKey::equals(const python::PyTensorKey& other
 ) const noexcept
 {
-    return m_width == other.m_width && m_key == other.m_key;
+    return m_basis.width() == other.m_basis.width() && m_key == other.m_key;
 }
 bool python::PyTensorKey::less(const python::PyTensorKey& other) const noexcept
 {
     return m_key < other.m_key;
 }
 
 static python::PyTensorKey
@@ -102,18 +128,20 @@
         auto width = kwargs["width"].cast<deg_t>();
         auto depth = kwargs["depth"].cast<deg_t>();
         auto index = kwargs["index"].cast<key_type>();
 
         auto max_idx = (python::maths::power(dimn_t(width), depth + 1) - 1)
                 / (dimn_t(width) - 1);
         if (index >= max_idx) {
-            throw py::value_error("provided index exceeds maximum");
+            RPY_THROW(py::value_error, "provided index exceeds maximum");
         }
 
-        return python::PyTensorKey(index, width, depth);
+        auto ctx = algebra::get_context(width, depth,
+                                        scalars::ScalarType::of<float>());
+        return python::PyTensorKey(ctx->get_tensor_basis(), index);
     }
 
     if (!args.empty() && py::isinstance<py::sequence>(args[0])) {
         letters.reserve(py::len(args[0]));
         for (auto arg : args[0]) { letters.push_back(arg.cast<let_t>()); }
     } else {
         letters.reserve(py::len(args));
@@ -129,41 +157,48 @@
     } else if (!letters.empty()) {
         width = *max_elt;
     }
 
     if (kwargs.contains("depth")) { depth = kwargs["depth"].cast<deg_t>(); }
 
     if (letters.size() > static_cast<dimn_t>(depth)) {
-        throw py::value_error("number of letters exceeds specified depth");
+        RPY_THROW(py::value_error, "number of letters exceeds specified depth");
     }
 
     if (!letters.empty() && *max_elt > width) {
-        throw py::value_error("letter value exceeds alphabet size");
+        RPY_THROW(py::value_error, "letter value exceeds alphabet size");
     }
 
     key_type result = 0;
     auto wwidth = dimn_t(width);
     for (auto letter : letters) {
         result *= wwidth;
         result += key_type(letter);
     }
 
-    return python::PyTensorKey(result, width, depth);
+    auto ctx = algebra::get_context(
+            width, depth, scalars::ScalarType::of<float>()
+    );
+    return python::PyTensorKey(ctx->get_tensor_basis(), result);
 }
 
 void python::init_py_tensor_key(py::module_& m)
 {
     py::class_<PyTensorKey> klass(m, "TensorKey");
     klass.def(py::init(&construct_key));
 
     klass.def_property_readonly("width", &PyTensorKey::width);
     klass.def_property_readonly("max_degree", &PyTensorKey::depth);
 
+    klass.def("to_index", [](const PyTensorKey& key) {
+        return static_cast<key_type>(key);
+    });
     klass.def("degree", [](const PyTensorKey& key) {
         return key.to_letters().size();
     });
+    klass.def("split_n", &PyTensorKey::split_n, "n"_a);
 
     klass.def("__str__", &PyTensorKey::to_string);
     klass.def("__repr__", &PyTensorKey::to_string);
 
     klass.def("__eq__", &PyTensorKey::equals);
 }
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/tensor_key.h` & `roughpy-0.0.5/roughpy/src/algebra/tensor_key.h`

 * *Files 6% similar despite different names*

```diff
@@ -52,30 +52,30 @@
 }
 
 }// namespace maths
 
 class PyTensorKey
 {
     key_type m_key;
-    deg_t m_width;
-    deg_t m_depth;
+    algebra::TensorBasis m_basis;
 
 public:
     explicit PyTensorKey(algebra::TensorBasis basis, key_type key);
-    explicit PyTensorKey(key_type key, deg_t width, deg_t depth);
 
     explicit operator key_type() const noexcept;
 
     string to_string() const;
     PyTensorKey lparent() const;
     PyTensorKey rparent() const;
     bool is_letter() const;
 
     deg_t width() const;
     deg_t depth() const;
+    algebra::TensorBasis basis() const { return m_basis; }
+    pair<PyTensorKey, PyTensorKey> split_n(deg_t n) const;
 
     deg_t degree() const;
     std::vector<let_t> to_letters() const;
 
     bool equals(const PyTensorKey& other) const noexcept;
     bool less(const PyTensorKey& other) const noexcept;
 };
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.cpp` & `roughpy-0.0.5/roughpy/src/algebra/tensor_key_iterator.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -34,47 +34,52 @@
 using namespace rpy;
 using namespace pybind11::literals;
 
 static const char* TKEY_ITERATOR_DOC = R"eadoc(Iterator over tensor words.
 )eadoc";
 
 python::PyTensorKeyIterator::PyTensorKeyIterator(
-        deg_t width, deg_t depth, key_type current, key_type end
+        algebra::TensorBasis basis, key_type current, key_type end
 )
-    : m_current(current), m_end(end), m_width(width), m_depth(depth)
-{}
+    : m_current(current), m_end(end), m_basis(basis)
+{
+    auto dim = m_basis.dimension();
+    if (m_end >= dim) {
+        m_end = dim;
+    }
+}
 python::PyTensorKey python::PyTensorKeyIterator::next()
 {
     if (m_current >= m_end) { throw py::stop_iteration(); }
     auto current = m_current;
     ++m_current;
-    return PyTensorKey(current, m_width, m_depth);
+    return PyTensorKey(m_basis, current);
 }
 
 void python::init_tensor_key_iterator(py::module_& m)
 {
 
     py::class_<PyTensorKeyIterator> klass(
             m, "TensorKeyIterator", TKEY_ITERATOR_DOC
     );
 
     klass.def(
             py::init([](const PyTensorKey& start_key) {
                 return PyTensorKeyIterator(
-                        start_key.width(), start_key.depth(),
+                        start_key.basis(),
                         static_cast<key_type>(start_key)
                 );
             }),
             "start_key"_a
     );
     klass.def(
             py::init([](const PyTensorKey& start_key,
                         const PyTensorKey& end_key) {
                 return PyTensorKeyIterator(
-                        start_key.width(), start_key.depth(),
+                        start_key.basis(),
                         static_cast<key_type>(start_key),
                         static_cast<key_type>(end_key)
                 );
             }),
             "start_key"_a, "end_key"_a
     );
     klass.def("__iter__", [](PyTensorKeyIterator& self) { return self; });
```

### Comparing `roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.h` & `roughpy-0.0.5/roughpy/src/algebra/tensor_key_iterator.h`

 * *Files 6% similar despite different names*

```diff
@@ -39,20 +39,19 @@
 namespace rpy {
 namespace python {
 
 class PyTensorKeyIterator
 {
     key_type m_current;
     key_type m_end;
-    deg_t m_width;
-    deg_t m_depth;
+    algebra::TensorBasis m_basis;
 
 public:
     PyTensorKeyIterator(
-            deg_t width, deg_t depth, key_type current = 0,
+            algebra::TensorBasis basis, key_type current = 0,
             key_type end = std::numeric_limits<key_type>::max()
     );
 
     PyTensorKey next();
 };
 
 void init_tensor_key_iterator(py::module_& m);
```

### Comparing `roughpy-0.0.4/roughpy/src/args/convert_timestamp.cpp` & `roughpy-0.0.5/roughpy/src/args/convert_timestamp.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         result = PyFloat_AsDouble(normalised_delta);
         Py_XDECREF(normalised_delta);
     } else if (PyLong_Check(py_time_delta)) {
         result = PyLong_AsDouble(py_time_delta);
     } else if (PyFloat_Check(py_time_delta)) {
         result = PyFloat_AsDouble(py_time_delta);
     } else {
-        throw py::type_error("expected datetime, int, or float");
+        RPY_THROW(py::type_error, "expected datetime, int, or float");
     }
 
     return result;
 }
 
 py::object generic_to_timestamp(py::handle generic_timestamp)
 {
@@ -85,20 +85,20 @@
         auto* pdt = PyDateTime_FromTimestamp(generic_timestamp.ptr());
         if (pdt == nullptr) { throw py::error_already_set(); }
         return py::reinterpret_steal<py::object>(pdt);
     }
 
     // str objects should be parsed as if an ISO-8601 datetime string
     if (PyUnicode_Check(generic_timestamp.ptr())) {
-        throw py::type_error(
+        RPY_THROW(py::type_error,
                 "currently conversion from ISO-8601 strings is not supported"
         );
     }
 
-    throw py::type_error("unsupported type for conversion to datetime");
+    RPY_THROW(py::type_error, "unsupported type for conversion to datetime");
 }
 
 }// namespace
 
 rpy::param_t rpy::python::convert_delta_from_datetimes(
         py::handle current, py::handle previous,
         const rpy::python::PyDateTimeConversionOptions& options
```

### Comparing `roughpy-0.0.4/roughpy/src/args/convert_timestamp.h` & `roughpy-0.0.5/roughpy/src/args/convert_timestamp.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.cpp` & `roughpy-0.0.5/roughpy/src/args/kwargs_to_path_metadata.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     }
 
     if (kwargs.contains("ctx")) {
         auto ctx = kwargs["ctx"];
         if (!py::isinstance(
                     ctx, reinterpret_cast<PyObject*>(&RPyContext_Type)
             )) {
-            throw py::type_error("expected a Context object");
+            RPY_THROW(py::type_error, "expected a Context object");
         }
         md.ctx = python::ctx_cast(ctx.ptr());
         md.width = md.ctx->width();
         md.scalar_type = md.ctx->ctype();
 
         if (!md.schema) {
             md.schema = std::make_shared<streams::StreamSchema>();
```

### Comparing `roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.h` & `roughpy-0.0.5/roughpy/src/args/kwargs_to_path_metadata.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.cpp` & `roughpy-0.0.5/roughpy/src/args/kwargs_to_vector_construction.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.h` & `roughpy-0.0.5/roughpy/src/args/kwargs_to_vector_construction.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/args/numpy.cpp` & `roughpy-0.0.5/roughpy/src/args/numpy.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     return type;
 }
 pybind11::dtype python::ctype_to_npy_dtype(const scalars::ScalarType* type)
 {
     if (type == scalars::ScalarType::of<double>()) { return py::dtype("d"); }
     if (type == scalars::ScalarType::of<float>()) { return py::dtype("f"); }
 
-    throw py::type_error("unsupported data type");
+    RPY_THROW(py::type_error, "unsupported data type");
 }
 
 string python::npy_dtype_to_identifier(pybind11::dtype dtype)
 {
     string identifier;
 
     switch (dtype.num()) {
@@ -125,12 +125,12 @@
 
         case NPY_BOOL:
         case NPY_BYTE: identifier = "i8"; break;
         case NPY_UBYTE: identifier = "u8"; break;
         case NPY_SHORT: identifier = "i16"; break;
         case NPY_USHORT: identifier = "u16"; break;
 
-        default: throw py::type_error("unsupported dtype");
+        default: RPY_THROW(py::type_error, "unsupported dtype");
     }
 
     return identifier;
 }
```

### Comparing `roughpy-0.0.4/roughpy/src/args/numpy.h` & `roughpy-0.0.5/roughpy/src/args/numpy.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/args/parse_schema.cpp` & `roughpy-0.0.5/roughpy/src/args/parse_schema.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -21,30 +21,30 @@
     } else if (channel_str == "value") {
         return streams::ChannelType::Value;
     } else if (channel_str == "categorical") {
         return streams::ChannelType::Categorical;
     } else if (channel_str == "lie") {
         return streams::ChannelType::Lie;
     } else {
-        throw py::value_error("expected increment, value, categorical, or lie "
+        RPY_THROW(py::value_error,"expected increment, value, categorical, or lie "
                               "for channel type");
     }
 }
 
 streams::ChannelType python::py_to_channel_type(const py::object& arg)
 {
     if (py::isinstance<streams::ChannelType>(arg)) {
         return arg.cast<streams::ChannelType>();
     }
 
     if (py::isinstance<py::str>(arg)) {
         return string_to_channel_type(arg.cast<string>());
     }
 
-    throw py::type_error(
+    RPY_THROW(py::type_error,
             "no know conversion from "
             + arg.get_type().attr("__name__").cast<string>()
             + " to channel type"
     );
 }
 
 namespace {
@@ -118,46 +118,46 @@
     RPY_CHECK(len > 1);
     auto type = py_to_channel_type(data[0]);
 
     if (len == 1) {
         insert_item_to_schema(schema, std::move(label), type, py::dict());
     } else if (len == 2) {
         if (!py::isinstance<py::dict>(data[1])) {
-            throw py::type_error("options must be a dictionary if provided");
+            RPY_THROW(py::type_error, "options must be a dictionary if provided");
         }
         insert_item_to_schema(
                 schema, std::move(label), type,
                 py::reinterpret_borrow<py::dict>(data[1])
         );
     } else {
-        throw py::value_error("expected tuple (type [, options])");
+        RPY_THROW(py::value_error, "expected tuple , type [, options])");
     }
 }
 
 void handle_dict_item(StreamSchema* schema, string label, py::dict data)
 {
     /*
      * The item contains a mapping of key -> values, which must include "type",
      * along with any other options to be appended to the schema
      */
     if (!data.contains("type")) {
-        throw py::value_error("dict items must contain \"type\"");
+        RPY_THROW(py::value_error, "dict items must contain \"type\"");
     }
 
     auto type = py_to_channel_type(data["type"]);
     // Everything remaining should be an option to be passed
     auto data_copy = py::reinterpret_steal<py::dict>(PyDict_Copy(data.ptr()));
     PyDict_DelItemString(data_copy.ptr(), "type");
 
     insert_item_to_schema(schema, std::move(label), type, std::move(data_copy));
 }
 void handle_dict_item_no_label(StreamSchema* schema, py::dict data)
 {
     if (!data.contains("label")) {
-        throw py::value_error("dict items in a schema must contain \"label\"");
+        RPY_THROW(py::value_error, "dict items in a schema must contain \"label\"");
     }
     auto data_copy = py::reinterpret_steal<py::dict>(PyDict_Copy(data.ptr()));
 
     auto label = data_copy["label"].cast<string>();
     PyDict_DelItemString(data_copy.ptr(), "label");
 
     handle_dict_item(schema, std::move(label), std::move(data_copy));
@@ -179,15 +179,15 @@
             );
         } else if (py::isinstance<py::sequence>(item)) {
             handle_seq_item(
                     schema, label.cast<string>(),
                     py::reinterpret_borrow<py::sequence>(item)
             );
         } else {
-            throw py::type_error("unsupported type in schema specification");
+            RPY_THROW(py::type_error, "unsupported type in schema specification");
         }
     }
 }
 
 void handle_seq_schema(StreamSchema* schema, py::sequence data)
 {
 
@@ -197,15 +197,15 @@
                     schema, py::reinterpret_borrow<py::dict>(item)
             );
         } else if (py::isinstance<py::sequence>(item)) {
             handle_seq_item_no_label(
                     schema, py::reinterpret_borrow<py::sequence>(item)
             );
         } else {
-            throw py::type_error("unsupported type in schema specification");
+            RPY_THROW(py::type_error, "unsupported type in schema specification");
         }
     }
 }
 
 //void handle_timestamp_pair(StreamSchema* schema, py::object data);
 //
 //RPY_NO_DISCARD
@@ -338,15 +338,15 @@
 //        auto data_seq = py::reinterpret_borrow<py::sequence>(data);
 //
 //        for (auto&& it_data : data_seq) {
 //            auto inner = py::reinterpret_borrow<py::object>(it_data);
 //            handle_timestamp_pair(schema, std::move(inner));
 //        }
 //    } else {
-//        throw py::value_error("expected dict, tuple, or other sequence");
+//        RPY_THROW(py::value_error, "expected dict, tuple, or other sequence");
 //    }
 //}
 //
 //inline void handle_dict_stream(StreamSchema* schema, const py::dict& data)
 //{
 //    for (auto&& [timestamp, tick_value] : data) {
 //        handle_timestamp_pair(
@@ -366,15 +366,15 @@
 //        RPY_CHECK(len > 1);
 //        if (len == 2) {
 //            handle_timestamp_pair(schema, inner[1]);
 //        } else if (len <= 4) {
 //            auto right = inner[py::slice(1, {}, {})];
 //            handle_timestamp_pair(schema, right);
 //        } else {
-//            throw py::value_error("expected tuple with no more than 4 elements"
+//            RPY_THROW(py::value_error,"expected tuple with no more than 4 elements"
 //            );
 //        }
 //    }
 //}
 
 }// namespace
 
@@ -388,15 +388,15 @@
                 schema.get(), py::reinterpret_borrow<py::dict>(data)
         );
     } else if (py::isinstance<py::sequence>(data)) {
         handle_seq_schema(
                 schema.get(), py::reinterpret_borrow<py::sequence>(data)
         );
     } else {
-        throw py::type_error("expected dict or sequence");
+        RPY_THROW(py::type_error, "expected dict or sequence");
     }
 }
 
 // void python::parse_data_into_schema(std::shared_ptr<streams::StreamSchema>
 // schema, const py::object &data) {
 //     if (py::isinstance<py::dict>(data)) {
 ////        parse_schema_from_dict_data(schema.get(),
@@ -405,15 +405,15 @@
 //        py::reinterpret_borrow<py::dict>(data));
 //    } else if (py::isinstance<py::sequence>(data)) {
 ////        parse_schema_from_seq_data(schema.get(),
 /// py::reinterpret_borrow<py::sequence>(data));
 //        handle_tuple_sequence(schema.get(),
 //        py::reinterpret_borrow<py::sequence>(data));
 //    } else {
-//        throw py::type_error("expected sequential data");
+//        RPY_THROW(py::type_error, "expected sequential data");
 //    }
 //}
 //
 std::shared_ptr<streams::StreamSchema>
 rpy::python::parse_schema(const py::object& data)
 {
     auto result = std::make_shared<streams::StreamSchema>();
```

### Comparing `roughpy-0.0.4/roughpy/src/args/parse_schema.h` & `roughpy-0.0.5/roughpy/src/args/parse_schema.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/dlpack.h` & `roughpy-0.0.5/roughpy/src/dlpack.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/dlpack_LICENSE` & `roughpy-0.0.5/roughpy/src/dlpack_LICENSE`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/date_time_interval.cpp` & `roughpy-0.0.5/roughpy/src/intervals/date_time_interval.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 python::DateTimeInterval::DateTimeInterval(py::object dt_begin,
                                            py::object dt_end)
     : Interval(IntervalType::Clopen), m_dt_begin(std::move(dt_begin)),
       m_dt_end(std::move(dt_end))
 {
     if (Py_TYPE(m_dt_begin.ptr()) != Py_TYPE(m_dt_end.ptr())) {
-        throw py::type_error("both begin and end objects must have the same "
+        RPY_THROW(py::type_error,"both begin and end objects must have the same "
                              "type");
     }
 
     if (!is_py_datetime(m_dt_begin) || !is_py_date(m_dt_begin)
         || !is_py_time(m_dt_begin)) {
-        throw py::type_error("begin and end must be datetime, data, or time "
+        RPY_THROW(py::type_error,"begin and end must be datetime, data, or time "
                              "objects");
     }
 }
 
 param_t python::DateTimeInterval::inf() const { return 0.0; }
 param_t python::DateTimeInterval::sup() const
 {
```

### Comparing `roughpy-0.0.4/roughpy/src/intervals/date_time_interval.h` & `roughpy-0.0.5/roughpy/src/intervals/date_time_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/dyadic.cpp` & `roughpy-0.0.5/roughpy/src/intervals/dyadic.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/dyadic.h` & `roughpy-0.0.5/roughpy/src/intervals/dyadic.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.cpp` & `roughpy-0.0.5/roughpy/src/intervals/dyadic_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.h` & `roughpy-0.0.5/roughpy/src/intervals/dyadic_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/interval.cpp` & `roughpy-0.0.5/roughpy/src/intervals/interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/interval.h` & `roughpy-0.0.5/roughpy/src/intervals/interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/intervals.cpp` & `roughpy-0.0.5/roughpy/src/intervals/intervals.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/intervals.h` & `roughpy-0.0.5/roughpy/src/intervals/intervals.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/partition.cpp` & `roughpy-0.0.5/roughpy/src/intervals/partition.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/partition.h` & `roughpy-0.0.5/roughpy/src/intervals/partition.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/real_interval.cpp` & `roughpy-0.0.5/roughpy/src/intervals/real_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/real_interval.h` & `roughpy-0.0.5/roughpy/src/intervals/real_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/segmentation.cpp` & `roughpy-0.0.5/roughpy/src/intervals/segmentation.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/intervals/segmentation.h` & `roughpy-0.0.5/roughpy/src/intervals/segmentation.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/recombine.cpp` & `roughpy-0.0.5/roughpy/src/recombine.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     auto buffer = python::py_to_buffer(data, options);
 
     const auto& shape = options.shape;
     const auto ndim = shape.size();
 
     if (ndim < 2 || buffer.size() == 0) {
-        throw py::value_error("malformed data");
+        RPY_THROW(py::value_error, "malformed data");
     }
 
     auto no_data_points = shape[0];
     auto point_dimension = shape[1];
 
     return py::tuple();
 }
```

### Comparing `roughpy-0.0.4/roughpy/src/recombine.h` & `roughpy-0.0.5/roughpy/src/recombine.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/roughpy_module.cpp` & `roughpy-0.0.5/roughpy/src/roughpy_module.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/roughpy_module.h` & `roughpy-0.0.5/roughpy/src/roughpy_module.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.cpp` & `roughpy-0.0.5/roughpy/src/scalars/r_py_polynomial.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -958,15 +958,15 @@
     construct_inplace(&obj->m_data, std::move(arg));
 
     return reinterpret_cast<PyObject*>(obj);
 }
 scalars::monomial PyMonomial_AsMonomial(PyObject* py_monomial)
 {
     if (Py_TYPE(py_monomial) != &RPyMonomial_Type) {
-        throw std::invalid_argument("");
+        RPY_THROW(std::invalid_argument, "");
     }
 
     return cast_mon(py_monomial);
 }
 bool indeterminate_from_string(
         PyObject* py_string, scalars::indeterminate_type& out
 )
```

### Comparing `roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.h` & `roughpy-0.0.5/roughpy/src/scalars/r_py_polynomial.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/scalars/scalar_type.cpp` & `roughpy-0.0.5/roughpy/src/scalars/scalar_type.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -161,60 +161,63 @@
 
 void python::register_scalar_type(
         const scalars::ScalarType* ctype, pybind11::handle py_type
 )
 {
     auto& found = ctype_type_cache[ctype];
     if (static_cast<bool>(found)) {
-        throw std::runtime_error("ctype already registered");
+        RPY_THROW(std::runtime_error, "ctype already registered");
     }
 
     found = py::reinterpret_borrow<py::object>(py_type);
 }
 
 py::object python::to_ctype_type(const scalars::ScalarType* type)
 {
     // The GIL must be held because we're working with Python objects anyway.
-    if (type == nullptr) { throw std::runtime_error("no matching ctype"); }
+    if (type == nullptr) { RPY_THROW(std::runtime_error, "no matching ctype"); }
     const auto found = ctype_type_cache.find(type);
     if (found != ctype_type_cache.end()) { return found->second; }
 
-    throw std::runtime_error("no matching ctype for type " + type->info().name);
+    RPY_THROW(
+            std::runtime_error,
+            "no matching ctype for type " + type->info().name
+    );
 }
 
 char python::format_to_type_char(const string& fmt)
 {
 
     char python_format = 0;
     for (const auto& chr : fmt) {
         switch (chr) {
             case '<':// little-endian
 #if BOOST_ENDIAN_BIG_BYTE || BOOST_ENDIAN_BIG_WORD
-                throw std::runtime_error(
+                RPY_THROW(std::runtime_error,
                         "non-native byte ordering not supported"
                 );
 #else
                 break;
 #endif
             case '>':// big-endian
 #if BOOST_ENDIAN_LITTLE_BYTE || BOOST_ENDIAN_LITTLE_WORD
-                throw std::runtime_error(
+                RPY_THROW(std::runtime_error, 
                         "non-native byte ordering not supported"
                 );
 #else
                 break;
 #endif
             case '@':// native
             case '=':// native
 #if BOOST_ENDIAN_LITTLE_BYTE || BOOST_ENDIAN_LITTLE_WORD
                 break;
 #endif
             case '!':// network ( = big-endian )
 #if BOOST_ENDIAN_LITTLE_BYTE || BOOST_ENDIAN_LITTLE_WORD
-                throw std::runtime_error(
+                RPY_THROW(std::runtime_error,
                         "non-native byte ordering not supported"
                 );
 #else
                 break;
 #endif
             case '0':
             case '1':
@@ -267,15 +270,15 @@
             format = type_id_of<scalars::unsigned_size_type_marker>();
             break;
         case 'h': format = type_id_of<short>(); break;
         case 'H': format = type_id_of<unsigned short>(); break;
         case 'b':
         case 'c': format = type_id_of<char>(); break;
         case 'B': format = type_id_of<unsigned char>(); break;
-        default: throw std::runtime_error("Unrecognised data format");
+        default: RPY_THROW(std::runtime_error, "Unrecognised data format");
     }
 
     return format;
 }
 
 const scalars::ScalarType*
 python::py_buffer_to_scalar_type(const py::buffer_info& info)
@@ -284,15 +287,15 @@
 
     auto python_format = format_to_type_char(info.format);
 
     switch (python_format) {
         case 'f': return ScalarType::of<float>();
         case 'd': return ScalarType::of<double>();
         default:
-            throw py::type_error(
+            RPY_THROW(py::type_error,
                     "no matching type for buffer type " + string(&python_format)
             );
     }
     // TODO: Add custom type handling
 
     return ScalarType::of<double>();
 }
@@ -300,15 +303,15 @@
 {
     if (type.ptr() == reinterpret_cast<PyObject*>(&PyFloat_Type)) {
         return scalars::ScalarType::of<double>();
     } else if (type.ptr() == reinterpret_cast<PyObject*>(&PyLong_Type)) {
         return scalars::ScalarType::of<double>();
     }
 
-    throw py::type_error(
+    RPY_THROW(py::type_error,
             "no matching scalar type for type " + pytype_name(type)
     );
 }
 
 const scalars::ScalarType* python::py_arg_to_ctype(const pybind11::object& arg)
 {
     if (py::isinstance(arg, python::get_scalar_metaclass())) {
@@ -325,15 +328,15 @@
     if (type == scalars::ScalarType::of<float>()
         || type == scalars::ScalarType::of<double>()) {
         return py::reinterpret_borrow<py::type>(
                 reinterpret_cast<PyObject*>(&PyFloat_Type)
         );
     }
 
-    throw py::type_error("no matching type for type " + type->info().name);
+    RPY_THROW(py::type_error, "no matching type for type " + type->info().name);
 }
 
 void python::init_scalar_types(pybind11::module_& m)
 {
 
     PyScalarMetaType_type.tp_base = &PyType_Type;
     if (PyType_Ready(&PyScalarMetaType_type) < 0) {
```

### Comparing `roughpy-0.0.4/roughpy/src/scalars/scalar_type.h` & `roughpy-0.0.5/roughpy/src/scalars/scalar_type.h`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     register_scalar_type(ctype, h_class);
     m.add_object(name.c_str(), h_class);
 }
 
 inline const scalars::ScalarType* to_stype_ptr(const py::handle& arg)
 {
     if (!py::isinstance(arg, get_scalar_metaclass())) {
-        throw py::type_error("argument is not a valid scalar type");
+        RPY_THROW(py::type_error, "argument is not a valid scalar type");
     }
     return reinterpret_cast<PyScalarMetaType*>(arg.ptr())->tp_ctype;
 }
 
 char format_to_type_char(const string& fmt);
 string py_buffer_to_type_id(const py::buffer_info& info);
```

### Comparing `roughpy-0.0.4/roughpy/src/scalars/scalars.cpp` & `roughpy-0.0.5/roughpy/src/scalars/scalars.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         *ptr = object.cast<long long>();
     } else if (RPyPolynomial_Check(object.ptr())) {
         *ptr = RPyPolynomial_cast(object.ptr());
     } else {
         // TODO: other checks
 
         auto tp = py::type::of(object);
-        throw py::value_error(
+        RPY_THROW(py::value_error,
                 "bad conversion from " + tp.cast<string>() + " to "
                 + ptr.type()->info().name
         );
     }
 }
 
 void python::init_scalars(pybind11::module_& m)
@@ -115,14 +115,15 @@
     });
     klass.def("__repr__", [](const Scalar& self) {
         std::stringstream ss;
         ss << "Scalar(type=" << self.type()->info().name << ", value approx "
            << self.to_scalar_t() << ")";
         return ss.str();
     });
+    klass.def("to_float", &Scalar::to_scalar_t);
 
     RPY_WARNING_POP
 }
 
 /*
  * Everything that follows is for the implementation of py_to_buffer,
  * which is our primary way of constructing RoughPy objects from python
@@ -193,29 +194,29 @@
 {
 
     if (options.type != nullptr) {
         result = scalars::KeyScalarArray(options.type);
         result.allocate_scalars(no_values);
         result.allocate_keys(no_keys);
     } else if (no_values > 0) {
-        throw py::type_error("unable to deduce a suitable scalar type");
+        RPY_THROW(py::type_error, "unable to deduce a suitable scalar type");
     }
 }
 
 static bool try_fill_buffer_dlpack(
         scalars::KeyScalarArray& buffer, python::PyToBufferOptions& options,
         const py::handle& object
 )
 {
     py::capsule dlpack;
     dlpack = object.attr("__dlpack__")();
 
     auto* tensor = reinterpret_cast<DLManagedTensor*>(dlpack.get_pointer());
     if (tensor == nullptr) {
-        throw py::value_error("__dlpack__ returned invalid object");
+        RPY_THROW(py::value_error, "__dlpack__ returned invalid object");
     }
 
     auto& dltensor = tensor->dl_tensor;
     auto* data = reinterpret_cast<char*>(dltensor.data);
     auto ndim = dltensor.ndim;
     auto* shape = dltensor.shape;
     auto* strides = dltensor.strides;
@@ -322,22 +323,22 @@
 )
 {
     py::handle scalar;
     if (::is_scalar(object)) {
         if (ground_type == ground_data_type::UnSet) {
             ground_type = ground_data_type::Scalars;
         } else if (ground_type != ground_data_type::Scalars) {
-            throw py::value_error("inconsistent scalar/key-scalar-pair data");
+            RPY_THROW(py::value_error, "inconsistent scalar/key-scalar-pair data");
         }
         scalar = object;
     } else if (is_kv_pair(object, options.alternative_key)) {
         if (ground_type == ground_data_type::UnSet) {
             ground_type = ground_data_type::KeyValuePairs;
         } else if (ground_type != ground_data_type::KeyValuePairs) {
-            throw py::value_error("inconsistent scalar/key-scalar-pair data");
+            RPY_THROW(py::value_error, "inconsistent scalar/key-scalar-pair data");
         }
         scalar = object.cast<py::tuple>()[1];
     } else {
         // TODO: Check non-int/float scalar types
         return false;
     }
 
@@ -351,18 +352,18 @@
 static void compute_size_and_type_recurse(
         python::PyToBufferOptions& options, std::vector<py::object>& leaves,
         const py::handle& object, ground_data_type& ground_type, dimn_t depth
 )
 {
 
     if (!py::isinstance<py::sequence>(object)) {
-        throw py::type_error("unexpected type in array argument");
+        RPY_THROW(py::type_error, "unexpected type in array argument");
     }
     if (depth > options.max_nested) {
-        throw py::value_error(
+        RPY_THROW(py::value_error,
                 "maximum nested array limit reached in this context"
         );
     }
 
     auto sequence = py::reinterpret_borrow<py::sequence>(object);
     auto length = static_cast<idimn_t>(py::len(sequence));
 
@@ -370,15 +371,15 @@
         // We've not visited this depth before,
         // add our length to the list
         options.shape.push_back(length);
     } else if (ground_type == ground_data_type::Scalars) {
         // We have visited this depth before,
         // check our length is consistent with the others
         if (length != options.shape[depth]) {
-            throw py::value_error("ragged arrays are not supported");
+            RPY_THROW(py::value_error, "ragged arrays are not supported");
         }
     }
 
     if (length == 0) {
         // if the length is zero, there is nothing left to do
         return;
     }
@@ -408,33 +409,33 @@
                     options, leaves, sibling, ground_type, depth + 1
             );
         }
     } else if (py::isinstance<py::dict>(item0)) {
         auto dict = py::reinterpret_borrow<py::dict>(item0);
 
         if (depth == options.max_nested) {
-            throw py::value_error("maximum nested depth reached in this context"
+            RPY_THROW(py::value_error,"maximum nested depth reached in this context"
             );
         }
         switch (ground_type) {
             case ground_data_type::UnSet:
                 ground_type = ground_data_type::KeyValuePairs;
             case ground_data_type::KeyValuePairs: break;
-            default: throw py::type_error("mismatched types in array argument");
+            default: RPY_THROW(py::type_error, "mismatched types in array argument");
         }
 
         if (!dict.empty()) {
             auto kv = *dict.begin();
             check_and_set_dtype(options, kv.second);
         }
 
         leaves.push_back(dict);
 
     } else {
-        throw py::type_error("unexpected type in array argument");
+        RPY_THROW(py::type_error, "unexpected type in array argument");
     }
 }
 
 static arg_size_info compute_size_and_type(
         python::PyToBufferOptions& options, std::vector<py::object>& leaves,
         py::handle arg
 )
@@ -513,15 +514,15 @@
 {
     scalars::KeyScalarArray result(options.type);
 
     // First handle the single number cases
     if (py::isinstance<py::float_>(object)
         || py::isinstance<py::int_>(object)) {
         if (!options.allow_scalar) {
-            throw py::value_error("scalar value not permitted in this context");
+            RPY_THROW(py::value_error, "scalar value not permitted in this context");
         }
 
         check_and_set_dtype(options, object);
         update_dtype_and_allocate(result, options, 1, 0);
 
         assign_py_object_to_scalar(result, object);
     } else if (is_kv_pair(object, options.alternative_key)) {
```

### Comparing `roughpy-0.0.4/roughpy/src/scalars/scalars.h` & `roughpy-0.0.5/roughpy/src/scalars/scalars.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/BaseStream.cpp` & `roughpy-0.0.5/roughpy/src/streams/BaseStream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/BaseStream.h` & `roughpy-0.0.5/roughpy/src/streams/BaseStream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/brownian_stream.cpp` & `roughpy-0.0.5/roughpy/src/streams/brownian_stream.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         pmd.scalar_type = scalars::ScalarType::of<double>();
     }
 
     if (pmd.depth == 0) { pmd.depth = 2; }
 
     if (pmd.ctx == nullptr) {
         if (pmd.width == 0) {
-            throw std::invalid_argument("width must be provided");
+            RPY_THROW(std::invalid_argument, "width must be provided");
         }
         pmd.ctx = algebra::get_context(
                 pmd.width, pmd.depth, pmd.scalar_type, {}
         );
     }
 
     // TODO: Fix this up properly.
```

### Comparing `roughpy-0.0.4/roughpy/src/streams/brownian_stream.h` & `roughpy-0.0.5/roughpy/src/streams/brownian_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/externally_sourced_stream.cpp` & `roughpy-0.0.5/roughpy/src/streams/externally_sourced_stream.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -43,28 +43,28 @@
 #endif
             if (fs::exists(path)) {
                 uri = url();
                 uri.set_scheme_id(URIScheme::file);
                 uri.set_path(uri_string);
             }
         } catch (...) {
-            throw py::value_error(
+            RPY_THROW(py::value_error,
                     "could not parse path " + uri_string + " error code "
                     + uri_result.error().message()
             );
         }
 
     } else {
         uri = *uri_result;
     }
 
     auto factory = streams::ExternalDataStream::get_factory_for(uri);
 
     if (!factory) {
-        throw py::value_error("The uri " + uri_string + " is not supported");
+        RPY_THROW(py::value_error, "The uri " + uri_string + " is not supported");
     }
 
     //    factory.add_metadata({
     //        pmd.width,
     //        pmd.support,
     //        pmd.ctx,
     //        pmd.scalar_type,
```

### Comparing `roughpy-0.0.4/roughpy/src/streams/function_stream.cpp` & `roughpy-0.0.5/roughpy/src/streams/function_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/function_stream.h` & `roughpy-0.0.5/roughpy/src/streams/function_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.cpp` & `roughpy-0.0.5/roughpy/src/streams/lie_increment_stream.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -100,26 +100,26 @@
         num_increments = options.shape[0];
     }
 
     if (md.scalar_type == nullptr) {
         if (options.type != nullptr) {
             md.scalar_type = options.type;
         } else {
-            throw py::type_error("unable to deduce suitable scalar type");
+            RPY_THROW(py::type_error, "unable to deduce suitable scalar type");
         }
     }
 
     RPY_CHECK(
             buffer.size()
             == static_cast<dimn_t>(increment_size * num_increments)
     );
     RPY_CHECK(md.scalar_type != nullptr);
     if (!md.ctx) {
         if (md.width == 0 || md.depth == 0) {
-            throw py::value_error(
+            RPY_THROW(py::value_error,
                     "either ctx or both width and depth must be specified"
             );
         }
         md.ctx = algebra::get_context(md.width, md.depth, md.scalar_type);
     }
 
     auto effective_support
@@ -133,27 +133,27 @@
                     = py::reinterpret_borrow<py::buffer>(indices_arg).request();
             buffer_to_indices(indices, info);
         } else if (py::isinstance<py::int_>(indices_arg)) {
             // Interpret this as a column in the data;
             auto icol = indices_arg.cast<idimn_t>();
             if (icol < 0) { icol += increment_size; }
             if (icol < 0 || icol >= increment_size) {
-                throw py::value_error("index out of bounds");
+                RPY_THROW(py::value_error, "index out of bounds");
             }
 
             indices.reserve(num_increments);
             for (idimn_t i = 0; i < num_increments; ++i) {
                 indices.push_back(static_cast<param_t>(
                         buffer[i * increment_size + icol].to_scalar_t()
                 ));
             }
         } else if (py::isinstance<py::sequence>(indices_arg)) {
             indices = indices_arg.cast<std::vector<param_t>>();
         } else {
-            throw py::type_error("unexpected type provided to 'indices' "
+            RPY_THROW(py::type_error,"unexpected type provided to 'indices' "
                                  "argument");
         }
 
         if (!indices.empty()) {
             auto minmax = std::minmax_element(indices.begin(), indices.end());
             effective_support = intervals::RealInterval(
                     *minmax.first, *minmax.second + 1.0, md.interval_type
@@ -163,15 +163,15 @@
 
     if (indices.empty()) {
         indices.reserve(num_increments);
         for (idimn_t i = 0; i < num_increments; ++i) {
             indices.emplace_back(i);
         }
     } else if (static_cast<idimn_t>(indices.size()) != num_increments) {
-        throw py::value_error("mismatch between number of rows in data and "
+        RPY_THROW(py::value_error,"mismatch between number of rows in data and "
                               "number of indices");
     }
 
     auto result = streams::Stream(streams::LieIncrementStream(
             std::move(buffer).copy_or_move(), indices,
             {md.width, effective_support, md.ctx, md.scalar_type,
              md.vector_type ? *md.vector_type : algebra::VectorType::Dense,
@@ -185,15 +185,15 @@
             python::RPyStream_FromStream(std::move(result))
     );
 }
 
 RPY_UNUSED static streams::Stream
 lie_increment_path_from_values(const py::object& data, const py::kwargs& kwargs)
 {
-    throw std::runtime_error("Not implemented");
+    RPY_THROW(std::runtime_error, "Not implemented");
 }
 
 void python::init_lie_increment_stream(py::module_& m)
 {
 
     py::class_<streams::LieIncrementStream> klass(
             m, "LieIncrementStream", LIE_INCR_STREAM_DOC
```

### Comparing `roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.h` & `roughpy-0.0.5/roughpy/src/streams/lie_increment_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.cpp` & `roughpy-0.0.5/streams/include/roughpy/streams/piecewise_abelian_stream.h`

 * *Files 24% similar despite different names*

```diff
@@ -22,75 +22,90 @@
 // CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 // SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 // INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 // CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 // ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 // POSSIBILITY OF SUCH DAMAGE.
 
-//
-// Created by user on 18/03/23.
-//
+#ifndef ROUGHPY_STREAMS_PIECEWISE_LIE_STREAM_H_
+#define ROUGHPY_STREAMS_PIECEWISE_LIE_STREAM_H_
 
-#include "piecewise_abelian_stream.h"
+#include "stream_base.h"
 
-#include <roughpy/streams/piecewise_abelian_stream.h>
-#include <roughpy/streams/stream.h>
+#include <roughpy/algebra/context.h>
+#include <roughpy/algebra/free_tensor.h>
+#include <roughpy/algebra/lie.h>
+#include <roughpy/core/types.h>
+#include <roughpy/platform/serialization.h>
 
-#include "args/kwargs_to_path_metadata.h"
-#include "stream.h"
+namespace rpy {
+namespace streams {
 
-using namespace rpy;
-using namespace pybind11::literals;
-
-static const char* PW_LIE_STREAM_DOC
-        = R"rpydoc(A stream formed of a sequence of interval-Lie pairs.
-)rpydoc";
-
-static py::object construct_piecewise_lie_stream(
-        std::vector<std::pair<intervals::RealInterval, algebra::Lie>> lies,
-        const py::kwargs& kwargs
-)
+class PiecewiseAbelianStream : public StreamInterface
 {
+public:
+    using LiePiece = std::pair<intervals::RealInterval, algebra::Lie>;
 
-    auto pmd = python::kwargs_to_metadata(kwargs);
+private:
+    std::vector<LiePiece> m_data;
 
-    if (!pmd.ctx) {
-        if (pmd.width == 0 || pmd.depth == 0 || !pmd.scalar_type) {
-            throw py::value_error("cannot deduce width/depth/ctype");
-        }
-        pmd.ctx = algebra::get_context(pmd.width, pmd.depth, pmd.scalar_type);
+    RPY_NO_DISCARD
+    static inline scalars::Scalar
+    to_multiplier_upper(const intervals::RealInterval& interval, param_t param)
+    {
+        RPY_DBG_ASSERT(interval.inf() <= param && param <= interval.sup());
+        return scalars::Scalar((interval.sup() - param)
+                               / (interval.sup() - interval.inf()));
     }
-    // TODO: make this more robust
-
-    using nl = std::numeric_limits<param_t>;
-    param_t a = nl::infinity();
-    param_t b = -nl::infinity();
-    for (auto& piece : lies) {
-        if (piece.first.inf() < a) { a = piece.first.inf(); }
-        if (piece.first.sup() > b) { b = piece.first.sup(); }
+    RPY_NO_DISCARD
+    static inline scalars::Scalar
+    to_multiplier_lower(const intervals::RealInterval& interval, param_t param)
+    {
+        RPY_DBG_ASSERT(interval.inf() <= param && param <= interval.sup());
+        return scalars::Scalar((param - interval.inf())
+                               / (interval.sup() - interval.inf()));
     }
 
-    pmd.support = intervals::RealInterval(a, b);
+public:
+    PiecewiseAbelianStream(std::vector<LiePiece>&& arg, StreamMetadata&& md);
+    PiecewiseAbelianStream(std::vector<LiePiece>&& arg, StreamMetadata&& md,
+                           std::shared_ptr<StreamSchema> schema);
+
+    RPY_NO_DISCARD
+    bool empty(const intervals::Interval& interval) const noexcept override;
+
+protected:
+    RPY_NO_DISCARD
+    algebra::Lie log_signature_impl(const intervals::Interval& domain,
+                                    const algebra::Context& ctx) const override;
+
+public:
+    RPY_SERIAL_SERIALIZE_FN();
+};
 
-    streams::Stream result(streams::PiecewiseAbelianStream(
-            std::move(lies),
-            {pmd.width,
-             pmd.support ? *pmd.support : intervals::RealInterval(0, 1),
-             pmd.ctx, pmd.scalar_type,
-             pmd.vector_type ? *pmd.vector_type : algebra::VectorType::Dense,
-             pmd.resolution}
-    ));
-
-    return py::reinterpret_steal<py::object>(
-            python::RPyStream_FromStream(std::move(result))
-    );
+RPY_SERIAL_SERIALIZE_FN_IMPL(PiecewiseAbelianStream)
+{
+    RPY_SERIAL_SERIALIZE_NVP("metadata", metadata());
+    RPY_SERIAL_SERIALIZE_NVP("data", m_data);
 }
 
-void python::init_piecewise_lie_stream(py::module_& m)
-{
+}// namespace streams
+}// namespace rpy
 
-    py::class_<streams::PiecewiseAbelianStream> klass(
-            m, "PiecewiseAbelianStream", PW_LIE_STREAM_DOC
-    );
+#ifndef RPY_DISABLE_SERIALIZATION
+RPY_SERIAL_LOAD_AND_CONSTRUCT(rpy::streams::PiecewiseAbelianStream)
+{
+    using namespace rpy;
+    using namespace rpy::streams;
+    using LiePiece = typename PiecewiseAbelianStream::LiePiece;
+
+    StreamMetadata metadata;
+    RPY_SERIAL_SERIALIZE_VAL(metadata);
+    std::vector<LiePiece> data;
+    RPY_SERIAL_SERIALIZE_VAL(data);
 
-    klass.def_static("construct", &construct_piecewise_lie_stream);
+    construct(std::move(data), std::move(metadata));
 }
+
+#endif
+
+#endif// ROUGHPY_STREAMS_PIECEWISE_LIE_STREAM_H_
```

### Comparing `roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.h` & `roughpy-0.0.5/roughpy/src/streams/piecewise_abelian_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/py_schema_context.cpp` & `roughpy-0.0.5/roughpy/src/streams/py_schema_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/py_schema_context.h` & `roughpy-0.0.5/roughpy/src/streams/py_schema_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.cpp` & `roughpy-0.0.5/roughpy/src/streams/r_py_tick_construction_helper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,19 @@
 {
     auto& channel = p_schema->insert_categorical(std::move(label));
     if (!variant.is_none()) { channel.insert_variant(variant.cast<string>()); }
 }
 
 void python::RPyTickConstructionHelper::fail_timestamp_none()
 {
-    throw py::value_error("timestamp cannot be None when constructing stream");
+    RPY_THROW(py::value_error, "timestamp cannot be None when constructing stream");
 }
 void python::RPyTickConstructionHelper::fail_data_none()
 {
-    throw py::value_error("data cannot be None when constructing stream");
+    RPY_THROW(py::value_error, "data cannot be None when constructing stream");
 }
 
 void python::RPyTickConstructionHelper::add_tick(
         string label, py::object timestamp, py::object data,
         streams::ChannelType type, const py::kwargs& RPY_UNUSED_VAR kwargs
 )
 {
```

### Comparing `roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.h` & `roughpy-0.0.5/roughpy/src/streams/r_py_tick_construction_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/schema.cpp` & `roughpy-0.0.5/roughpy/src/streams/schema.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/schema.h` & `roughpy-0.0.5/roughpy/src/streams/schema.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/stream.cpp` & `roughpy-0.0.5/roughpy/src/streams/stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/stream.h` & `roughpy-0.0.5/roughpy/src/streams/stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/streams.cpp` & `roughpy-0.0.5/roughpy/src/streams/streams.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/streams.h` & `roughpy-0.0.5/roughpy/src/streams/streams.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/src/streams/tick_stream.cpp` & `roughpy-0.0.5/roughpy/src/streams/tick_stream.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -77,25 +77,28 @@
 
     parser.attr("parse_data")(data);
 
     auto& helper
             = parser.attr("helper").cast<python::RPyTickConstructionHelper&>();
 
     const auto& ticks = helper.ticks();
-    if (ticks.empty()) { throw py::value_error("tick data cannot be empty"); }
+    if (ticks.empty()) {
+        RPY_THROW(py::value_error, "tick data cannot be empty");
+    }
 
     //    if (!schema->is_final()) {
     //        python::parse_data_into_schema(schema, data);
     //        pmd.width = schema->width();
     //        schema->finalize();
     //    }
     if (!pmd.ctx) {
         pmd.width = schema->width();
         if (pmd.width == 0 || pmd.depth == 0 || pmd.scalar_type == nullptr) {
-            throw py::value_error(
+            RPY_THROW(
+                    py::value_error,
                     "either ctx or width, depth, and dtype must be provided"
             );
         }
         pmd.ctx = algebra::get_context(pmd.width, pmd.depth, pmd.scalar_type);
     } else if (pmd.width != pmd.ctx->width()) {
         // Recalibrate the width to match the data
         pmd.ctx = pmd.ctx->get_alike(pmd.width, pmd.depth, pmd.scalar_type);
@@ -155,15 +158,15 @@
 
         auto lie_elt = pmd.ctx->zero_lie(meta.cached_vector_type);
 
         auto channel_it = schema->find(tick.label);
         RPY_DBG_ASSERT(channel_it != schema->end());
         auto& channel = channel_it->second;
         auto idx = schema->label_to_stream_dim(tick.label);
-        auto key = static_cast<key_type>(idx);
+        auto key = schema->label_to_lie_key(tick.label);
         switch (tick.type) {
             case streams::ChannelType::Increment:
                 lie_elt[key]
                         += python::py_to_scalar(pmd.scalar_type, tick.data);
                 break;
             case streams::ChannelType::Value:
                 if (channel.is_lead_lag()) {
@@ -201,15 +204,17 @@
                     break;
                 }
             case streams::ChannelType::Categorical: {
                 lie_elt[key] += pmd.scalar_type->one();
                 break;
             }
             case streams::ChannelType::Lie:
-                throw py::value_error("Lie tick types currently not allowed");
+                RPY_THROW(
+                        py::value_error, "Lie tick types currently not allowed"
+                );
         }
 
         auto& existing = raw_data[di];
         if (existing) {
             existing = pmd.ctx->cbh(existing, lie_elt, meta.cached_vector_type);
         } else {
             existing = std::move(lie_elt);
@@ -314,16 +319,16 @@
 //
 // inline void handle_labeled_data(helper_t &helper,
 //                                param_t timestamp,
 //                                string_view label,
 //                                const py::object &tick_value) {
 //    auto type = helper.type_of(label);
 //    if (!type) {
-//        throw py::value_error("unexpected label " + string(label) + " in tick
-//        data");
+//        RPY_THROW(py::value_error,"unexpected label " + string(label) + " in
+//        tick data");
 //    }
 //
 //    handle_tick_value(helper, timestamp, label, *type, tick_value);
 //}
 //
 // void handle_timestamp_pair(helper_t &helper, param_t timestamp, py::object
 // tick_item) {
@@ -351,15 +356,15 @@
 //
 //        py::object value;
 //        if (len == 2) {
 //            value = py::reinterpret_borrow<py::object>(tuple_item[1]);
 //        } else if (len == 3) {
 //            value = py::reinterpret_borrow<py::object>(tuple_item[2]);
 //        } else {
-//            throw py::value_error("expected tuple (label, data) or (label,
+//            RPY_THROW(py::value_error,"expected tuple (label, data) or (label,
 //            type, data)");
 //        }
 //
 //        if (py::isinstance<py::sequence>(value)) {
 //            for (auto&& tick_value :
 //            py::reinterpret_steal<py::sequence>(value)) {
 //                auto inner = py::reinterpret_borrow<py::object>(tick_value);
@@ -411,11 +416,11 @@
 //         py::reinterpret_borrow<py::dict>(data));
 //     } else if (py::isinstance<py::sequence>(data)) {
 //         handle_tuple_sequence_tick_stream(
 //             helper,
 //             py::reinterpret_borrow<py::sequence>(data)
 //             );
 //     } else {
-//         throw py::type_error("expected dict or sequence of pairs");
+//         RPY_THROW(py::type_error, "expected dict or sequence of pairs");
 //     }
 //
 // }
```

### Comparing `roughpy-0.0.4/roughpy/src/streams/tick_stream.h` & `roughpy-0.0.5/roughpy/src/streams/tick_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/streams/__init__.py` & `roughpy-0.0.5/roughpy/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/roughpy/streams/tick_stream.py` & `roughpy-0.0.5/roughpy/streams/tick_stream.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/CMakeLists.txt` & `roughpy-0.0.5/scalars/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/conversion.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/conversion.h`

 * *Files 13% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 try_convert(ScalarPointer arg, const ScalarType* type = nullptr)
 {
     if (type == nullptr) { type = ScalarType::of<T>(); }
 
     if (arg.is_null()) { return T(0); }
     const auto* arg_type = arg.type();
     if (arg_type == nullptr) {
-        throw std::runtime_error("null type for non-zero value");
+        RPY_THROW(std::runtime_error, "null type for non-zero value");
     }
 
     auto cv = get_conversion(arg_type->id(), type->id());
     if (!cv) {
-        throw std::runtime_error(
+        RPY_THROW(std::runtime_error,
                 "no known conversion from " + arg_type->info().name
                 + " to type " + type->info().name
         );
     }
     T result;
     cv({type, &result}, arg, 1);
     return result;
```

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/key_scalar_array.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/key_scalar_array.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/owned_scalar_array.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/owned_scalar_array.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/random.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/random.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar.h`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
               = std::enable_if_t<!std::is_same<Scalar, std::decay_t<T>>::value>>
     Scalar& operator=(T arg)
     {
         if (p_type == nullptr) {
             p_type = ScalarType::of<std::decay_t<T>>();
         } else {
             if (is_const()) {
-                throw std::runtime_error(
+                RPY_THROW(std::runtime_error,
                         "attempting to assign value to const scalar");
             }
         }
 
         if (p_data == nullptr) {
             m_flags |= flags::OwnedPointer;
             ScalarPointer::operator=(p_type->allocate(1));
```

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_array.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_array.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_blas.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_blas.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_interface.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_interface.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_matrix.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_matrix.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_pointer.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_pointer.h`

 * *Files 2% similar despite different names*

```diff
@@ -330,15 +330,15 @@
      */
     template <typename T,
               typename = std::enable_if_t<
                       !std::is_const<std::remove_pointer_t<T>>::value>>
     RPY_NO_DISCARD ensure_pointer<T> raw_cast()
     {
         if (is_const()) {
-            throw std::runtime_error(
+            RPY_THROW(std::runtime_error,
                     "cannot cast const pointer to non-const pointer");
         }
         return static_cast<ensure_pointer<T>>(const_cast<void*>(p_data));
     }
 
     /**
      * @brief Dereference to get a scalar value
```

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_stream.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_traits.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_type.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalar_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars/scalars_fwd.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars/scalars_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/include/roughpy/scalars.h` & `roughpy-0.0.5/scalars/include/roughpy/scalars.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/scalar_blas_defs.h.in` & `roughpy-0.0.5/scalars/scalar_blas_defs.h.in`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/RationalType.cpp` & `roughpy-0.0.5/scalars/src/RationalType.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -101,34 +101,34 @@
     if (other.is_null()) { return scalar_type(0); }
     if (other.type() == this) {
         return *other.template raw_cast<const scalar_type>();
     }
 
     const ScalarType* type = other.type();
     if (type == nullptr) {
-        throw std::runtime_error("null type for non-zero value");
+        RPY_THROW(std::runtime_error, "null type for non-zero value");
     }
 
     auto cv = get_conversion(type->id(), this->id());
     if (cv) {
         scalar_type result;
         ScalarPointer result_ptr{this, &result};
         cv(result_ptr, other, 1);
         return result;
     }
 
-    throw std::runtime_error("could not convert " + type->info().name
+    RPY_THROW(std::runtime_error,"could not convert " + type->info().name
                              + " to scalar type " + info().name);
 }
 
 void RationalType::convert_copy(ScalarPointer dst, ScalarPointer src,
                                 dimn_t count) const
 {
     if (src.type() == nullptr) {
-        throw std::invalid_argument("source type cannot be null");
+        RPY_THROW(std::invalid_argument, "source type cannot be null");
     }
     convert_copy(dst, src.ptr(), count, src.type()->id());
 }
 
 template <typename F>
 static inline void convert_copy_ext(ScalarPointer& out, const void* in,
                                     std::size_t count)
@@ -159,15 +159,15 @@
                     convert_copy_basic<int32_t>(optr, in, info.lanes * count);
                     break;
                 case 64:
                     convert_copy_basic<int64_t>(optr, in, info.lanes * count);
                     break;
                 case 128:
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for integer type");
             }
             break;
         case ScalarTypeCode::UInt:
             switch (info.bits) {
                 case 8:
                     convert_copy_basic<uint8_t>(optr, in, info.lanes * count);
@@ -179,15 +179,15 @@
                     convert_copy_basic<uint32_t>(optr, in, info.lanes * count);
                     break;
                 case 64:
                     convert_copy_basic<uint64_t>(optr, in, info.lanes * count);
                     break;
                 case 128:
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for integer type");
             }
             break;
         case ScalarTypeCode::Float:
             switch (info.bits) {
                 case 16:
                     convert_copy_ext<half>(optr, in, info.lanes * count);
@@ -195,43 +195,43 @@
                 case 32:
                     convert_copy_basic<float>(optr, in, info.lanes * count);
                     break;
                 case 64:
                     convert_copy_basic<double>(optr, in, info.lanes * count);
                     break;
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for float type");
             }
             break;
         case ScalarTypeCode::BFloat:
             switch (info.bits) {
                 case 16:
                     convert_copy_ext<bfloat16>(optr, in, info.lanes * count);
                     break;
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for bfloat type");
             }
             break;
         case ScalarTypeCode::Bool:
         case ScalarTypeCode::OpaqueHandle: break;
         case ScalarTypeCode::Complex:
-        default: throw std::runtime_error("unsupported scalar type");
+        default: RPY_THROW(std::runtime_error, "unsupported scalar type");
     }
 }
 void RationalType::convert_copy(void* out, ScalarPointer in,
                                 std::size_t count) const
 {
     RPY_DBG_ASSERT(out != nullptr);
     RPY_DBG_ASSERT(!in.is_null());
     const auto* type = in.type();
 
     if (type == nullptr) {
-        throw std::runtime_error("null type for non-zero value");
+        RPY_THROW(std::runtime_error, "null type for non-zero value");
     }
 
     if (type == this) {
         const auto* in_begin = in.template raw_cast<const scalar_type>();
         const auto* in_end = in_begin + count;
         std::copy(in_begin, in_end, static_cast<scalar_type*>(out));
     } else {
@@ -306,20 +306,20 @@
     auto* ptr = lhs.raw_cast<scalar_type*>();
     *ptr *= try_convert(rhs);
 }
 void RationalType::div_inplace(ScalarPointer lhs, ScalarPointer rhs) const
 {
     RPY_CHECK(lhs);
     auto* ptr = lhs.raw_cast<scalar_type*>();
-    if (rhs.is_null()) { throw std::runtime_error("division by zero"); }
+    if (rhs.is_null()) { RPY_THROW(std::runtime_error, "division by zero"); }
 
     auto crhs = try_convert(rhs);
 
     if (crhs == scalar_type(0)) {
-        throw std::runtime_error("division by zero");
+        RPY_THROW(std::runtime_error, "division by zero");
     }
 
     *ptr /= crhs;
 }
 bool RationalType::are_equal(ScalarPointer lhs,
                              ScalarPointer rhs) const noexcept
 {
@@ -356,20 +356,20 @@
 {
     if (!lhs) { return zero(); }
     return Scalar(this, *lhs.raw_cast<const scalar_type*>() * try_convert(rhs));
 }
 Scalar RationalType::div(ScalarPointer lhs, ScalarPointer rhs) const
 {
     if (!lhs) { return zero(); }
-    if (rhs.is_null()) { throw std::runtime_error("division by zero"); }
+    if (rhs.is_null()) { RPY_THROW(std::runtime_error, "division by zero"); }
 
     auto crhs = try_convert(rhs);
 
     if (crhs == scalar_type(0)) {
-        throw std::runtime_error("division by zero");
+        RPY_THROW(std::runtime_error, "division by zero");
     }
 
     return Scalar(this,
                   static_cast<scalar_type>(*lhs.raw_cast<const scalar_type*>()
                                            / crhs));
 }
 bool RationalType::is_zero(ScalarPointer arg) const
@@ -390,27 +390,27 @@
 {
     return ScalarType::get_rng(bit_generator, seed);
 }
 void RationalType::swap(ScalarPointer lhs, ScalarPointer rhs) const
 {
 
     if (lhs.is_null() ^ rhs.is_null()) {
-        throw std::runtime_error("one of the pointers is null");
+        RPY_THROW(std::runtime_error, "one of the pointers is null");
     }
 
     if (lhs.type() != rhs.type()) {
-        throw std::runtime_error("cannot swap scalars of different types");
+        RPY_THROW(std::runtime_error, "cannot swap scalars of different types");
     }
 
     if (lhs.type() != this && lhs.type() != nullptr) {
         return lhs.type()->swap(lhs, rhs);
     }
 
     if (lhs.is_const() || rhs.is_const()) {
-        throw std::runtime_error("one or both of the scalars is const");
+        RPY_THROW(std::runtime_error, "one or both of the scalars is const");
     }
 
     std::swap(*lhs.raw_cast<scalar_type*>(), *rhs.raw_cast<scalar_type*>());
 }
 std::vector<byte> RationalType::to_raw_bytes(const ScalarPointer& ptr,
                                              dimn_t count) const
 {
```

### Comparing `roughpy-0.0.4/scalars/src/RationalType.h` & `roughpy-0.0.5/scalars/src/RationalType.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/ScalarTests.h` & `roughpy-0.0.5/scalars/src/ScalarTests.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/b_float_16_type.h` & `roughpy-0.0.5/scalars/src/b_float_16_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/bfloat16_random_generator.cpp` & `roughpy-0.0.5/scalars/src/bfloat16_random_generator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/bfloat16_random_generator.h` & `roughpy-0.0.5/scalars/src/bfloat16_random_generator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/double_type.cpp` & `roughpy-0.0.5/scalars/src/double_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/double_type.h` & `roughpy-0.0.5/scalars/src/double_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/float_blas.cpp` & `roughpy-0.0.5/scalars/src/float_blas.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 {
     RPY_CHECK(matrix.type() == type() && vector.type() == type());
 
     auto M = static_cast<blas::integer>(matrix.nrows());
     auto N = static_cast<blas::integer>(matrix.ncols());
 
     if (N != static_cast<blas::integer>(vector.size())) {
-        throw std::invalid_argument("inner matrix dimensions must agree");
+        RPY_THROW(std::invalid_argument, "inner matrix dimensions must agree");
     }
 
     const auto layout = blas::to_blas_layout(matrix.layout());
     OwnedScalarArray result(type(), M);
 
     // TODO: fix lda/ldb values
     switch (matrix.storage()) {
@@ -329,15 +329,15 @@
             ftmm(result, lhs, rhs, blas::Blas_Lo);
             break;
         case MatrixStorage::UpperTriangular:
             ftmm(result, lhs, rhs, blas::Blas_Up);
             break;
         case MatrixStorage::Diagonal: fdmm(result, lhs, rhs); break;
         default:
-            throw std::runtime_error("matrix-matrix multiplications of these "
+            RPY_THROW(std::runtime_error,"matrix-matrix multiplications of these "
                                      "formats is not currently supported");
     }
 }
 
 static void triangular_matrix_matrix(ScalarMatrix& result,
                                      const ScalarMatrix& lhs,
                                      blas::BlasUpLo lhs_uplo,
@@ -350,15 +350,15 @@
             ttmm(result, lhs, lhs_uplo, rhs, blas::Blas_Up);
             break;
         case MatrixStorage::LowerTriangular:
             ttmm(result, lhs, lhs_uplo, rhs, blas::Blas_Lo);
             break;
         case MatrixStorage::Diagonal: tdmm(result, lhs, lhs_uplo, rhs); break;
         default:
-            throw std::runtime_error("matrix-matrix multiplications of these "
+            RPY_THROW(std::runtime_error,"matrix-matrix multiplications of these "
                                      "formats is currently unsupported");
     }
 }
 static void diagonal_matrix_matrix(ScalarMatrix& result,
                                    const ScalarMatrix& lhs,
                                    const ScalarMatrix& rhs)
 {
@@ -368,26 +368,26 @@
             dtmm(result, lhs, rhs, blas::Blas_Lo);
             break;
         case MatrixStorage::UpperTriangular:
             dtmm(result, lhs, rhs, blas::Blas_Up);
             break;
         case MatrixStorage::Diagonal: ddmm(result, lhs, rhs); break;
         default:
-            throw std::runtime_error("matrix-matrix multiplications of these "
+            RPY_THROW(std::runtime_error,"matrix-matrix multiplications of these "
                                      "formats is currently unsupported");
     }
 }
 
 ScalarMatrix FloatBlas::matrix_matrix(const ScalarMatrix& lhs,
                                       const ScalarMatrix& rhs)
 {
     RPY_DBG_ASSERT(lhs.type() == rhs.type() && lhs.type() == type());
 
     if (lhs.ncols() != rhs.nrows()) {
-        throw std::invalid_argument("inner matrix dimensions must agree");
+        RPY_THROW(std::invalid_argument, "inner matrix dimensions must agree");
     };
 
     ScalarMatrix result(type(), lhs.nrows(), rhs.ncols());
 
     switch (lhs.storage()) {
         case MatrixStorage::FullMatrix:
             full_matrix_matrix(result, lhs, rhs);
@@ -406,23 +406,23 @@
     return result;
 }
 ScalarMatrix FloatBlas::solve_linear_system(const ScalarMatrix& coeff_matrix,
                                             const ScalarMatrix& target_matrix)
 {
 
     if (coeff_matrix.nrows() != target_matrix.nrows()) {
-        throw std::invalid_argument("incompatible matrix dimensions");
+        RPY_THROW(std::invalid_argument, "incompatible matrix dimensions");
     }
 
     if (coeff_matrix.nrows() < coeff_matrix.ncols()) {
-        throw std::invalid_argument(
+        RPY_THROW(std::invalid_argument,
                 "system is over-determined, used least squares instead");
     }
     if (coeff_matrix.nrows() > coeff_matrix.ncols()) {
-        throw std::invalid_argument("system is under-determined, no solution");
+        RPY_THROW(std::invalid_argument, "system is under-determined, no solution");
     }
 
     ScalarMatrix result = target_matrix.to_full();
 
     //    switch (coeff_matrix.storage()) {
     //        case MatrixStorage::FullMatrix:
     //
```

### Comparing `roughpy-0.0.4/scalars/src/float_blas.h` & `roughpy-0.0.5/scalars/src/float_blas.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/float_type.cpp` & `roughpy-0.0.5/scalars/src/float_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/float_type.h` & `roughpy-0.0.5/scalars/src/float_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/half_random_generator.cpp` & `roughpy-0.0.5/scalars/src/half_random_generator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/half_random_generator.h` & `roughpy-0.0.5/scalars/src/half_random_generator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/half_type.cpp` & `roughpy-0.0.5/scalars/src/half_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/half_type.h` & `roughpy-0.0.5/scalars/src/half_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/key_scalar_array.cpp` & `roughpy-0.0.5/scalars/src/key_scalar_array.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         p_keys = nullptr;
     }
     m_flags |= keys_owning_flag;
 }
 key_type* KeyScalarArray::keys()
 {
     if (keys_owned()) { return const_cast<key_type*>(p_keys); }
-    throw std::runtime_error("borrowed keys are not mutable");
+    RPY_THROW(std::runtime_error, "borrowed keys are not mutable");
 }
 
 KeyScalarArray::operator OwnedScalarArray() && noexcept
 {
     auto result = OwnedScalarArray(p_type, p_data, m_size);
     p_type = nullptr;
     p_data = nullptr;
```

### Comparing `roughpy-0.0.4/scalars/src/owned_scalar_array.cpp` & `roughpy-0.0.5/scalars/src/owned_scalar_array.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -65,24 +65,24 @@
 {
     const auto* type = value.type();
     if (type != nullptr) {
         ScalarPointer::operator=(type->allocate(count));
         m_size = count;
         type->convert_fill(*this, value.to_pointer(), count, "");
     } else {
-        throw std::runtime_error("scalar value has invalid type");
+        RPY_THROW(std::runtime_error, "scalar value has invalid type");
     }
 }
 
 OwnedScalarArray::OwnedScalarArray(const ScalarType* type, const void* data,
                                    dimn_t count)
     : ScalarArray(type)
 {
     if (type == nullptr) {
-        throw std::invalid_argument("cannot construct array with invalid type");
+        RPY_THROW(std::invalid_argument, "cannot construct array with invalid type");
     }
 
     ScalarPointer::operator=(type->allocate(count));
     m_size = count;
     type->convert_copy(const_cast<void*>(p_data), {nullptr, data}, count);
 }
```

### Comparing `roughpy-0.0.4/scalars/src/rational_poly_scalar_type.cpp` & `roughpy-0.0.5/scalars/src/rational_poly_scalar_type.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     );
 }
 void RationalPolyScalarType::convert_copy(
         ScalarPointer dst, ScalarPointer src, dimn_t count
 ) const
 {
     if (src.type() == nullptr) {
-        throw std::invalid_argument("source type cannot be null");
+        RPY_THROW(std::invalid_argument, "source type cannot be null");
     }
     convert_copy(dst, src.ptr(), count, src.type()->id());
 }
 
 template <typename F>
 static inline void
 convert_copy_ext(ScalarPointer& out, const void* in, dimn_t count)
@@ -150,15 +150,15 @@
                     convert_copy_ext<int32_t>(optr, in, info.lanes * count);
                     break;
                 case 64:
                     convert_copy_ext<int64_t>(optr, in, info.lanes * count);
                     break;
                 case 128:
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for integer type"
                     );
             }
             break;
         case ScalarTypeCode::UInt:
             switch (info.bits) {
                 case 8:
@@ -171,15 +171,15 @@
                     convert_copy_ext<uint32_t>(optr, in, info.lanes * count);
                     break;
                 case 64:
                     convert_copy_ext<uint64_t>(optr, in, info.lanes * count);
                     break;
                 case 128:
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for integer type"
                     );
             }
             break;
         case ScalarTypeCode::Float:
             switch (info.bits) {
                     //                case 16:
@@ -188,34 +188,34 @@
                 case 32:
                     convert_copy_ext<float>(optr, in, info.lanes * count);
                     break;
                 case 64:
                     convert_copy_ext<double>(optr, in, info.lanes * count);
                     break;
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for float type"
                     );
             }
             break;
         case ScalarTypeCode::BFloat:
             switch (info.bits) {
                     //                case 16:
                     //                    convert_copy_ext<bfloat16>(optr, in,
                     //                    info.lanes * count); break;
                 default:
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "invalid bit configuration for bfloat type"
                     );
             }
             break;
         case ScalarTypeCode::Bool:
         case ScalarTypeCode::OpaqueHandle: break;
         case ScalarTypeCode::Complex:
-        default: throw std::runtime_error("unsupported scalar type");
+        default: RPY_THROW(std::runtime_error, "unsupported scalar type");
     }
 }
 void RationalPolyScalarType::convert_copy(
         void* out, ScalarPointer in, std::size_t count
 ) const
 {
     RPY_DBG_ASSERT(out != nullptr);
@@ -339,20 +339,20 @@
             this,
             *lhs.template raw_cast<const scalar_type*>() * ::try_convert(rhs)
     );
 }
 Scalar RationalPolyScalarType::div(ScalarPointer lhs, ScalarPointer rhs) const
 {
     if (!lhs) { return zero(); }
-    if (rhs.is_null()) { throw std::runtime_error("division by zero"); }
+    if (rhs.is_null()) { RPY_THROW(std::runtime_error, "division by zero"); }
 
     auto divisor = try_convert<rational_scalar_type>(rhs);
 
     if (divisor == rational_scalar_type(0)) {
-        throw std::runtime_error("division by zero");
+        RPY_THROW(std::runtime_error, "division by zero");
     }
 
     return Scalar(this, *lhs.template raw_cast<scalar_type>() / divisor);
 }
 void RationalPolyScalarType::add_inplace(ScalarPointer lhs, ScalarPointer rhs)
         const
 {
@@ -376,20 +376,20 @@
 }
 void RationalPolyScalarType::div_inplace(ScalarPointer lhs, ScalarPointer rhs)
         const
 {
     RPY_CHECK(lhs);
     auto* ptr = lhs.raw_cast<scalar_type*>();
 
-    if (rhs.is_null()) { throw std::runtime_error("division by zero"); }
+    if (rhs.is_null()) { RPY_THROW(std::runtime_error, "division by zero"); }
 
     auto divisor = try_convert<rational_scalar_type>(rhs);
 
     if (divisor == rational_scalar_type(0)) {
-        throw std::runtime_error("division by zero");
+        RPY_THROW(std::runtime_error, "division by zero");
     }
 
     *ptr /= divisor;
 }
 bool RationalPolyScalarType::is_zero(ScalarPointer arg) const
 {
     return !static_cast<bool>(arg)
@@ -408,29 +408,29 @@
         os << *arg.raw_cast<const scalar_type*>();
     }
 }
 std::unique_ptr<RandomGenerator> RationalPolyScalarType::get_rng(
         const string& bit_generator, Slice<uint64_t> seed
 ) const
 {
-    throw std::runtime_error("no rng for rational polynomial scalars");
+    RPY_THROW(std::runtime_error, "no rng for rational polynomial scalars");
 }
 std::unique_ptr<BlasInterface> RationalPolyScalarType::get_blas() const
 {
-    throw std::runtime_error(
+    RPY_THROW(std::runtime_error,
             "no blas implementation for rational polynomial scalars"
     );
 }
 std::vector<byte> RationalPolyScalarType::to_raw_bytes(
         const ScalarPointer& ptr, dimn_t count
 ) const
 {
-    throw std::runtime_error("not implemented");
+    RPY_THROW(std::runtime_error, "not implemented");
 }
 ScalarPointer RationalPolyScalarType::from_raw_bytes(
         Slice<byte> raw_bytes, dimn_t count
 ) const
 {
-    throw std::runtime_error("not implemented");
+    RPY_THROW(std::runtime_error, "not implemented");
 }
 }// namespace scalars
 }// namespace rpy
```

### Comparing `roughpy-0.0.4/scalars/src/rational_poly_scalar_type.h` & `roughpy-0.0.5/scalars/src/rational_poly_scalar_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/scalar.cpp` & `roughpy-0.0.5/scalars/src/scalar.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -49,25 +49,25 @@
 {
     m_flags |= ptype;
 }
 
 Scalar::Scalar(ScalarInterface* other)
 {
     if (other == nullptr) {
-        throw std::invalid_argument("scalar interface pointer cannot be null");
+        RPY_THROW(std::invalid_argument, "scalar interface pointer cannot be null");
     }
     p_type = other->type();
     p_data = other;
     m_flags |= flags::InterfacePointer
             | (other->is_const() ? flags::IsConst : flags::IsMutable);
 }
 Scalar::Scalar(ScalarPointer ptr) : ScalarPointer(ptr)
 {
     if (p_data != nullptr && p_type == nullptr) {
-        throw std::runtime_error("non-zero scalars must have a type");
+        RPY_THROW(std::runtime_error, "non-zero scalars must have a type");
     }
 }
 
 Scalar::Scalar(const ScalarType* type)
     : ScalarPointer(type, static_cast<void*>(nullptr))
 {}
 Scalar::Scalar(scalar_t scal)
@@ -130,15 +130,15 @@
     // TODO: finish this off?
     return p_type->is_zero(to_pointer());
 }
 
 Scalar& Scalar::operator=(const Scalar& other)
 {
     if (is_const()) {
-        throw std::runtime_error("Cannot cast to a const value");
+        RPY_THROW(std::runtime_error, "Cannot cast to a const value");
     }
     if (this != std::addressof(other)) {
         if (is_interface()) {
             auto* iface
                     = static_cast<ScalarInterface*>(const_cast<void*>(p_data));
             iface->assign(other.to_pointer());
         } else {
@@ -177,15 +177,15 @@
         return static_cast<const ScalarInterface*>(p_data)->to_pointer();
     }
     return {p_type, p_data};
 }
 ScalarPointer Scalar::to_mut_pointer()
 {
     if (is_const()) {
-        throw std::runtime_error("cannot get non-const pointer to const value");
+        RPY_THROW(std::runtime_error, "cannot get non-const pointer to const value");
     }
     auto* ptr = const_cast<void*>(p_data);
     if (is_interface()) {
         return static_cast<ScalarInterface*>(ptr)->to_pointer();
     }
     return {p_type, ptr};
 }
@@ -233,25 +233,25 @@
 #undef RPY_SCALAR_OP
 
 Scalar Scalar::operator/(const Scalar& other) const
 {
     const ScalarType* type = (p_type != nullptr) ? p_type : other.p_type;
     if (type == nullptr) { return Scalar(); }
     if (other.p_data == nullptr) {
-        throw std::runtime_error("division by zero");
+        RPY_THROW(std::runtime_error, "division by zero");
     }
 
     return type->div(to_pointer(), other.to_pointer());
 }
 
 #define RPY_SCALAR_IOP(OP, MNAME)                                              \
     Scalar& Scalar::operator OP(const Scalar& other)                           \
     {                                                                          \
         if (is_const()) {                                                      \
-            throw std::runtime_error(                                          \
+            RPY_THROW(std::runtime_error,                                          \
                     "performing inplace operation on const scalar");           \
         }                                                                      \
                                                                                \
         if (p_type == nullptr) {                                               \
             RPY_DBG_ASSERT(p_data == nullptr);                                 \
             /* We just established that other.p_data != nullptr */             \
             RPY_DBG_ASSERT(other.p_type != nullptr);                           \
@@ -274,19 +274,19 @@
 RPY_SCALAR_IOP(+=, add)
 RPY_SCALAR_IOP(-=, sub)
 RPY_SCALAR_IOP(*=, mul)
 
 Scalar& Scalar::operator/=(const Scalar& other)
 {
     if (is_const()) {
-        throw std::runtime_error(
+        RPY_THROW(std::runtime_error,
                 "performing inplace operation on const scalar");
     }
     if (other.p_data == nullptr) {
-        throw std::runtime_error("division by zero");
+        RPY_THROW(std::runtime_error, "division by zero");
     }
     if (p_type == nullptr) {
         RPY_DBG_ASSERT(p_data == nullptr);
         RPY_DBG_ASSERT(other.p_type != nullptr);
         p_type = other.p_type;
     }
     if (p_data == nullptr) {
```

### Comparing `roughpy-0.0.4/scalars/src/scalar_array.cpp` & `roughpy-0.0.5/scalars/src/scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/scalar_blas.cpp` & `roughpy-0.0.5/scalars/src/scalar_blas.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/scalar_blas_impl.h` & `roughpy-0.0.5/scalars/src/scalar_blas_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/scalar_interface.cpp` & `roughpy-0.0.5/scalars/src/scalar_interface.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/scalar_matrix.cpp` & `roughpy-0.0.5/scalars/src/scalar_matrix.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     }
 }
 
 rpy::scalars::ScalarMatrix
 rpy::scalars::ScalarMatrix::to_full(rpy::scalars::MatrixLayout layout) const
 {
     if (p_type == nullptr) {
-        throw std::invalid_argument("cannot allocate matrix with no type");
+        RPY_THROW(std::invalid_argument, "cannot allocate matrix with no type");
     }
 
     ScalarMatrix result(p_type, m_nrows, m_ncols, m_storage, layout);
     to_full(result);
     return result;
 }
```

### Comparing `roughpy-0.0.4/scalars/src/scalar_pointer.cpp` & `roughpy-0.0.5/scalars/src/scalar_pointer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -39,27 +39,27 @@
 
 using namespace rpy;
 using namespace rpy::scalars;
 
 void* ScalarPointer::ptr()
 {
     if (is_const()) {
-        throw std::runtime_error(
+        RPY_THROW(std::runtime_error,
                 "attempting to convert const pointer to non-const pointer");
     }
     return const_cast<void*>(p_data);
 }
 Scalar ScalarPointer::deref() const noexcept
 {
     return Scalar(*this, (m_flags & ~owning_flag) | constness_flag);
 }
 Scalar ScalarPointer::deref_mut()
 {
     if (is_const()) {
-        throw std::runtime_error(
+        RPY_THROW(std::runtime_error,
                 "attempting to dereference const pointer to non-const value");
     }
     return Scalar(*this, m_flags & ~owning_flag);
 }
 Scalar ScalarPointer::operator*() { return deref_mut(); }
 Scalar ScalarPointer::operator*() const noexcept { return deref(); }
 ScalarPointer
```

### Comparing `roughpy-0.0.4/scalars/src/scalar_stream.cpp` & `roughpy-0.0.5/scalars/src/scalar_stream.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 ScalarStream::ScalarStream(const ScalarType* type)
     : m_stream(), m_elts_per_row(0), p_type(type)
 {}
 ScalarStream::ScalarStream(ScalarPointer base, std::vector<dimn_t> shape)
 {
     if (!base.is_null()) {
         p_type = base.type();
-        if (p_type == nullptr) { throw std::runtime_error("missing type"); }
+        if (p_type == nullptr) { RPY_THROW(std::runtime_error, "missing type"); }
         if (shape.empty()) {
-            throw std::runtime_error("strides cannot be empty");
+            RPY_THROW(std::runtime_error, "strides cannot be empty");
         }
 
         const auto* ptr = static_cast<const char*>(base.ptr());
         const auto itemsize = p_type->itemsize();
 
         dimn_t rows = shape[0];
         dimn_t cols = (shape.size() > 1) ? shape[1] : 1;
```

### Comparing `roughpy-0.0.4/scalars/src/scalar_type.cpp` & `roughpy-0.0.5/scalars/src/scalar_type.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                                                 const ScalarDeviceInfo& device)
 {
     return ScalarType::of<double>();
 }
 Scalar ScalarType::from(long long int numerator,
                         long long int denominator) const
 {
-    if (denominator == 0) { throw std::invalid_argument("division by zero"); }
+    if (denominator == 0) { RPY_THROW(std::invalid_argument, "division by zero"); }
     auto result = allocate(1);
     assign(result, numerator, denominator);
     return {result, flags::OwnedPointer};
 }
 void ScalarType::convert_fill(ScalarPointer out, ScalarPointer in, dimn_t count,
                               const string& id) const
 {
@@ -88,15 +88,15 @@
     for (dimn_t i = 1; i < count; ++i) {
         out_p += isize;
         convert_copy({this, out_p}, out, 1);
     }
 }
 Scalar ScalarType::parse(string_view str) const
 {
-    throw std::runtime_error("could not parse string");
+    RPY_THROW(std::runtime_error, "could not parse string");
 }
 Scalar ScalarType::one() const { return from(1, 1); }
 Scalar ScalarType::mone() const { return from(-1, 1); }
 Scalar ScalarType::zero() const { return from(0, 1); }
 Scalar ScalarType::copy(ScalarPointer source) const
 {
     auto result = allocate(1);
@@ -232,22 +232,22 @@
 void rpy::scalars::register_type(const ScalarType* type)
 {
     std::lock_guard<std::mutex> access(s_scalar_type_cache_lock);
 
     const auto& identifier = type->id();
     for (const auto& i : reserved) {
         if (identifier == i.first) {
-            throw std::runtime_error("cannot register identifier " + identifier
+            RPY_THROW(std::runtime_error,"cannot register identifier " + identifier
                                      + ", it is reserved");
         }
     }
 
     auto& entry = s_scalar_type_cache[identifier];
     if (entry != nullptr) {
-        throw std::runtime_error("type with id " + identifier
+        RPY_THROW(std::runtime_error,"type with id " + identifier
                                  + " is already registered");
     }
 
     entry = type;
 }
 const ScalarType* rpy::scalars::get_type(const string& id)
 {
@@ -255,15 +255,15 @@
     auto found = s_scalar_type_cache.find(id);
     if (found != s_scalar_type_cache.end()) { return found->second; }
 
     for (const auto& rsv : reserved) {
         if (id == rsv.first) { return nullptr; }
     }
 
-    throw std::runtime_error("no type with id " + id);
+    RPY_THROW(std::runtime_error, "no type with id " + id);
 }
 
 const ScalarType* scalars::get_type(const string& id,
                                     const ScalarDeviceInfo& device)
 {
     // TODO: Needs implementation
     return nullptr;
@@ -277,15 +277,15 @@
     }
 
     string ids(id);
     std::lock_guard<std::mutex> access(s_scalar_type_cache_lock);
     auto found = s_scalar_type_cache.find(ids);
     if (found != s_scalar_type_cache.end()) { return found->second->info(); }
 
-    throw std::runtime_error("Unrecognised type id " + ids);
+    RPY_THROW(std::runtime_error, "Unrecognised type id " + ids);
 }
 
 std::vector<const ScalarType*> rpy::scalars::list_types()
 {
     std::lock_guard<std::mutex> access(s_scalar_type_cache_lock);
     std::vector<const ScalarType*> result;
     result.reserve(s_scalar_type_cache.size());
@@ -375,42 +375,42 @@
                                                         const string& dst_id)
 {
     std::lock_guard<std::mutex> access(s_conversion_lock);
 
     auto found = s_conversion_cache.find(type_ids_to_key(src_id, dst_id));
     if (found != s_conversion_cache.end()) { return found->second; }
 
-    throw std::runtime_error("no conversion function from " + src_id + " to "
+    RPY_THROW(std::runtime_error,"no conversion function from " + src_id + " to "
                              + dst_id);
 }
 void rpy::scalars::register_conversion(const string& src_id,
                                        const string& dst_id,
                                        conversion_function converter)
 {
     std::lock_guard<std::mutex> access(s_conversion_lock);
 
     auto& found = s_conversion_cache[type_ids_to_key(src_id, dst_id)];
     if (found != nullptr) {
-        throw std::runtime_error("conversion from " + src_id + " to " + dst_id
+        RPY_THROW(std::runtime_error,"conversion from " + src_id + " to " + dst_id
                                  + " already registered");
     } else {
         found = std::move(converter);
     }
 }
 
 std::unique_ptr<RandomGenerator>
 ScalarType::get_rng(const string& bit_generator, Slice<uint64_t> seed) const
 {
-    throw std::runtime_error(
+    RPY_THROW(std::runtime_error,
             "no random number generators are defined for this scalar type");
 }
 
 std::unique_ptr<BlasInterface> ScalarType::get_blas() const
 {
-    throw std::runtime_error("No blas/lapack available for this scalar type");
+    RPY_THROW(std::runtime_error, "No blas/lapack available for this scalar type");
 }
 
 const std::string& rpy::scalars::id_from_basic_info(const BasicScalarInfo& info)
 {
     std::lock_guard<std::mutex> access(s_scalar_type_cache_lock);
 
     // Lanes are ignored in determining type.
@@ -418,31 +418,31 @@
     switch (info.code) {
         case ScalarTypeCode::Int:
             switch (info.bits) {
                 case 8: return reserved[I8IDX].second.id;
                 case 16: return reserved[I16IDX].second.id;
                 case 32: return reserved[I32IDX].second.id;
                 case 64: return reserved[I64IDX].second.id;
-                default: throw std::runtime_error("unsupported integer type");
+                default: RPY_THROW(std::runtime_error, "unsupported integer type");
             }
         case ScalarTypeCode::UInt:
             switch (info.bits) {
                 case 8: return reserved[U8IDX].second.id;
                 case 16: return reserved[U16IDX].second.id;
                 case 32: return reserved[U32IDX].second.id;
                 case 64: return reserved[U64IDX].second.id;
-                default: throw std::runtime_error("unsupported integer type");
+                default: RPY_THROW(std::runtime_error, "unsupported integer type");
             }
         case ScalarTypeCode::Float:
             switch (info.bits) {
                 case 32: return ScalarType::of<float>()->id();
                 case 64: return ScalarType::of<double>()->id();
-                default: throw std::runtime_error("unsupported float type");
+                default: RPY_THROW(std::runtime_error, "unsupported float type");
             }
-        default: throw std::runtime_error("unsupported scalar type");
+        default: RPY_THROW(std::runtime_error, "unsupported scalar type");
     }
 
     RPY_UNREACHABLE();
 }
 
 #undef I8IDX
 #undef I16IDX
```

### Comparing `roughpy-0.0.4/scalars/src/standard_random_generator.cpp` & `roughpy-0.0.5/scalars/src/standard_random_generator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/standard_random_generator.h` & `roughpy-0.0.5/scalars/src/standard_random_generator.h`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 StandardRandomGenerator<ScalarImpl, BitGenerator>::uniform_random_scalar(
         ScalarArray lower, ScalarArray upper, dimn_t count) const
 {
 
     std::vector<std::uniform_real_distribution<scalar_type>> dists;
 
     if (lower.size() != upper.size()) {
-        throw std::invalid_argument(
+        RPY_THROW(std::invalid_argument,
                 "mismatch dimensions between lower and upper limits");
     }
 
     dists.reserve(lower.size());
     for (dimn_t i = 0; i < lower.size(); ++i) {
         dists.emplace_back(scalar_cast<scalar_type>(lower[i]),
                            scalar_cast<scalar_type>(upper[i]));
```

### Comparing `roughpy-0.0.4/scalars/src/standard_scalar_type.h` & `roughpy-0.0.5/scalars/src/standard_scalar_type.h`

 * *Files 3% similar despite different names*

```diff
@@ -124,27 +124,27 @@
         }
     }
 
     void swap(ScalarPointer lhs, ScalarPointer rhs) const override
     {
 
         if (lhs.is_null() ^ rhs.is_null()) {
-            throw std::runtime_error("one of the pointers is null");
+            RPY_THROW(std::runtime_error, "one of the pointers is null");
         }
 
         if (lhs.type() != rhs.type()) {
-            throw std::runtime_error("cannot swap scalars of different types");
+            RPY_THROW(std::runtime_error, "cannot swap scalars of different types");
         }
 
         if (lhs.type() != this && lhs.type() != nullptr) {
             return lhs.type()->swap(lhs, rhs);
         }
 
         if (lhs.is_const() || rhs.is_const()) {
-            throw std::runtime_error("one or both of the scalars is const");
+            RPY_THROW(std::runtime_error, "one or both of the scalars is const");
         }
 
         std::swap(*lhs.raw_cast<ScalarImpl*>(), *rhs.raw_cast<ScalarImpl*>());
     }
 
 protected:
     ScalarImpl try_convert(ScalarPointer other) const
@@ -152,38 +152,38 @@
         if (other.is_null()) { return ScalarImpl(0); }
         if (other.type() == this) {
             return *other.template raw_cast<const ScalarImpl>();
         }
 
         const ScalarType* type = other.type();
         if (type == nullptr) {
-            throw std::runtime_error("null type for non-zero value");
+            RPY_THROW(std::runtime_error, "null type for non-zero value");
         }
 
         auto cv = get_conversion(type->id(), this->id());
         if (cv) {
             ScalarImpl result;
             ScalarPointer result_ptr{this, &result};
             cv(result_ptr, other, 1);
             return result;
         }
 
-        throw std::runtime_error("could not convert " + type->info().name
+        RPY_THROW(std::runtime_error,"could not convert " + type->info().name
                                  + " to scalar type " + info().name);
     }
 
 public:
     void convert_copy(void* out, ScalarPointer in, dimn_t count) const override
     {
         RPY_DBG_ASSERT(out != nullptr);
         RPY_DBG_ASSERT(!in.is_null());
         const auto* type = in.type();
 
         if (type == nullptr) {
-            throw std::runtime_error("null type for non-zero value");
+            RPY_THROW(std::runtime_error, "null type for non-zero value");
         }
 
         if (type == this) {
             const auto* in_begin = in.template raw_cast<const ScalarImpl>();
             const auto* in_end = in_begin + count;
             std::copy(in_begin, in_end, static_cast<ScalarImpl*>(out));
         } else {
@@ -243,15 +243,15 @@
     }
 
     void convert_copy(ScalarPointer dst, ScalarPointer src,
                       dimn_t count) const override
     {
         if (src.type() == nullptr) {
             if (src.is_simple_integer()) {
-                throw std::runtime_error(
+                RPY_THROW(std::runtime_error,
                         "no type associated with scalar value");
             }
             switch (src.simple_integer_config()) {
                 case flags::UnsignedInteger8:
                     convert_copy_basic<uint8_t>(dst, src.cptr(), count);
                     break;
                 case flags::UnsignedInteger16:
@@ -307,15 +307,15 @@
                         break;
                     case sizeof(int64_t) * CHAR_BIT:
                         convert_copy_basic<int64_t>(optr, in,
                                                     info.lanes * count);
                         break;
                         //                    case 128:
                     default:
-                        throw std::runtime_error(
+                        RPY_THROW(std::runtime_error,
                                 "invalid bit configuration for integer type");
                 }
                 break;
             case ScalarTypeCode::UInt:
                 switch (info.bits) {
                     case sizeof(uint8_t) * CHAR_BIT:
                         convert_copy_basic<uint8_t>(optr, in,
@@ -331,15 +331,15 @@
                         break;
                     case sizeof(uint64_t) * CHAR_BIT:
                         convert_copy_basic<uint64_t>(optr, in,
                                                      info.lanes * count);
                         break;
                         //                    case 128:
                     default:
-                        throw std::runtime_error(
+                        RPY_THROW(std::runtime_error,
                                 "invalid bit configuration for integer type");
                 }
                 break;
             case ScalarTypeCode::Float:
                 switch (info.bits) {
                     case sizeof(half) * CHAR_BIT:
                         convert_copy_basic<half>(optr, in, info.lanes * count);
@@ -348,33 +348,33 @@
                         convert_copy_basic<float>(optr, in, info.lanes * count);
                         break;
                     case sizeof(double) * CHAR_BIT:
                         convert_copy_basic<double>(optr, in,
                                                    info.lanes * count);
                         break;
                     default:
-                        throw std::runtime_error(
+                        RPY_THROW(std::runtime_error,
                                 "invalid bit configuration for float type");
                 }
                 break;
             case ScalarTypeCode::BFloat:
                 switch (info.bits) {
                     case sizeof(bfloat16) * CHAR_BIT:
                         convert_copy_basic<bfloat16>(optr, in,
                                                      info.lanes * count);
                         break;
                     default:
-                        throw std::runtime_error(
+                        RPY_THROW(std::runtime_error,
                                 "invalid bit configuration for bfloat type");
                 }
                 break;
             case ScalarTypeCode::Bool:
             case ScalarTypeCode::OpaqueHandle: break;
             case ScalarTypeCode::Complex:
-            default: throw std::runtime_error("unsupported scalar type");
+            default: RPY_THROW(std::runtime_error, "unsupported scalar type");
         }
     }
     void assign(ScalarPointer target, long long int numerator,
                 long long int denominator) const override
     {
         *target.raw_cast<ScalarImpl*>()
                 = ScalarImpl(numerator) / ScalarImpl(denominator);
@@ -409,20 +409,20 @@
         if (!lhs) { return zero(); }
         return Scalar(this,
                       *lhs.raw_cast<const ScalarImpl*>() * try_convert(rhs));
     }
     Scalar div(ScalarPointer lhs, ScalarPointer rhs) const override
     {
         if (!lhs) { return zero(); }
-        if (rhs.is_null()) { throw std::runtime_error("division by zero"); }
+        if (rhs.is_null()) { RPY_THROW(std::runtime_error, "division by zero"); }
 
         auto crhs = try_convert(rhs);
 
         if (crhs == ScalarImpl(0)) {
-            throw std::runtime_error("division by zero");
+            RPY_THROW(std::runtime_error, "division by zero");
         }
 
         return Scalar(this,
                       static_cast<ScalarImpl>(*lhs.raw_cast<const ScalarImpl*>()
                                               / crhs));
     }
     bool are_equal(ScalarPointer lhs, ScalarPointer rhs) const noexcept override
@@ -451,20 +451,20 @@
         auto* ptr = lhs.raw_cast<ScalarImpl*>();
         *ptr *= try_convert(rhs);
     }
     void div_inplace(ScalarPointer lhs, ScalarPointer rhs) const override
     {
         RPY_DBG_ASSERT(lhs);
         auto* ptr = lhs.raw_cast<ScalarImpl*>();
-        if (rhs.is_null()) { throw std::runtime_error("division by zero"); }
+        if (rhs.is_null()) { RPY_THROW(std::runtime_error, "division by zero"); }
 
         auto crhs = try_convert(rhs);
 
         if (crhs == ScalarImpl(0)) {
-            throw std::runtime_error("division by zero");
+            RPY_THROW(std::runtime_error, "division by zero");
         }
 
         *ptr /= crhs;
     }
     bool is_zero(ScalarPointer arg) const override
     {
         return !static_cast<bool>(arg)
```

### Comparing `roughpy-0.0.4/scalars/src/test_float_blas.cpp` & `roughpy-0.0.5/scalars/src/test_float_blas.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/test_key_scalar_array.cpp` & `roughpy-0.0.5/scalars/src/test_key_scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/test_pcg_standard_random.cpp` & `roughpy-0.0.5/scalars/src/test_pcg_standard_random.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/test_scalar.cpp` & `roughpy-0.0.5/scalars/src/test_scalar.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/test_scalar_array.cpp` & `roughpy-0.0.5/scalars/src/test_scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/test_scalar_matrix.cpp` & `roughpy-0.0.5/scalars/src/test_scalar_matrix.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/scalars/src/test_scalar_type.cpp` & `roughpy-0.0.5/scalars/src/test_scalar_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/setup.py` & `roughpy-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/CMakeLists.txt` & `roughpy-0.0.5/streams/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/brownian_stream.h` & `roughpy-0.0.5/streams/include/roughpy/streams/brownian_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/channels.h` & `roughpy-0.0.5/streams/include/roughpy/streams/channels.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/dyadic_caching_layer.h` & `roughpy-0.0.5/streams/include/roughpy/streams/dyadic_caching_layer.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/dynamically_constructed_stream.h` & `roughpy-0.0.5/streams/include/roughpy/streams/dynamically_constructed_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/external_data_stream.h` & `roughpy-0.0.5/streams/include/roughpy/streams/external_data_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/lie_increment_stream.h` & `roughpy-0.0.5/streams/include/roughpy/streams/lie_increment_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/piecewise_abelian_stream.h` & `roughpy-0.0.5/streams/src/brownian_stream.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -22,90 +22,62 @@
 // CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 // SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 // INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 // CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 // ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 // POSSIBILITY OF SUCH DAMAGE.
 
-#ifndef ROUGHPY_STREAMS_PIECEWISE_LIE_STREAM_H_
-#define ROUGHPY_STREAMS_PIECEWISE_LIE_STREAM_H_
+//
+// Created by user on 24/03/23.
+//
+#include <roughpy/streams/brownian_stream.h>
 
-#include "stream_base.h"
-
-#include <roughpy/algebra/context.h>
-#include <roughpy/algebra/free_tensor.h>
 #include <roughpy/algebra/lie.h>
-#include <roughpy/core/types.h>
-#include <roughpy/platform/serialization.h>
+#include <roughpy/scalars/key_scalar_array.h>
 
-namespace rpy {
-namespace streams {
+using namespace rpy;
+using namespace rpy::streams;
 
-class PiecewiseAbelianStream : public StreamInterface
+algebra::Lie BrownianStream::gaussian_increment(const algebra::Context& ctx,
+                                                param_t length) const
 {
-public:
-    using LiePiece = std::pair<intervals::RealInterval, algebra::Lie>;
-
-private:
-    std::vector<LiePiece> m_data;
-
-    RPY_NO_DISCARD
-    static inline scalars::Scalar
-    to_multiplier_upper(const intervals::RealInterval& interval, param_t param)
-    {
-        RPY_DBG_ASSERT(interval.inf() <= param && param <= interval.sup());
-        return scalars::Scalar((interval.sup() - param)
-                               / (interval.sup() - interval.inf()));
-    }
-    RPY_NO_DISCARD
-    static inline scalars::Scalar
-    to_multiplier_lower(const intervals::RealInterval& interval, param_t param)
-    {
-        RPY_DBG_ASSERT(interval.inf() <= param && param <= interval.sup());
-        return scalars::Scalar((param - interval.inf())
-                               / (interval.sup() - interval.inf()));
-    }
-
-public:
-    PiecewiseAbelianStream(std::vector<LiePiece>&& arg, StreamMetadata&& md);
-    PiecewiseAbelianStream(std::vector<LiePiece>&& arg, StreamMetadata&& md,
-                           std::shared_ptr<StreamSchema> schema);
-
-    RPY_NO_DISCARD
-    bool empty(const intervals::Interval& interval) const noexcept override;
-
-protected:
-    RPY_NO_DISCARD
-    algebra::Lie log_signature_impl(const intervals::Interval& domain,
-                                    const algebra::Context& ctx) const override;
-
-public:
-    RPY_SERIAL_SERIALIZE_FN();
-};
+    const auto& md = metadata();
+    scalars::KeyScalarArray incr(p_generator->normal_random(
+            scalars::Scalar(0.), scalars::Scalar(length), md.width));
+    return ctx.construct_lie({std::move(incr), md.cached_vector_type});
+}
 
-RPY_SERIAL_SERIALIZE_FN_IMPL(PiecewiseAbelianStream)
+algebra::Lie
+BrownianStream::log_signature_impl(const intervals::Interval& interval,
+                                   const algebra::Context& ctx) const
 {
-    RPY_SERIAL_SERIALIZE_NVP("metadata", metadata());
-    RPY_SERIAL_SERIALIZE_NVP("data", m_data);
+    return algebra::Lie();
 }
+pair<algebra::Lie, algebra::Lie> BrownianStream::compute_child_lie_increments(
+        DynamicallyConstructedStream::DyadicInterval left_di,
+        DynamicallyConstructedStream::DyadicInterval right_di,
+        const DynamicallyConstructedStream::Lie& parent_value) const
+{
+    const auto& md = metadata();
+    const auto mean = parent_value.smul(md.data_scalar_type->from(1, 2));
 
-}// namespace streams
-}// namespace rpy
+    auto length = ldexp(0.5, left_di.power());
 
-#ifndef RPY_DISABLE_SERIALIZATION
-RPY_SERIAL_LOAD_AND_CONSTRUCT(rpy::streams::PiecewiseAbelianStream)
+    const auto perturbation = gaussian_increment(*md.default_context, length);
+    return {mean.add(perturbation), mean.sub(perturbation)};
+}
+DynamicallyConstructedStream::Lie BrownianStream::make_new_root_increment(
+        DynamicallyConstructedStream::DyadicInterval di) const
 {
-    using namespace rpy;
-    using namespace rpy::streams;
-    using LiePiece = typename PiecewiseAbelianStream::LiePiece;
-
-    StreamMetadata metadata;
-    RPY_SERIAL_SERIALIZE_VAL(metadata);
-    std::vector<LiePiece> data;
-    RPY_SERIAL_SERIALIZE_VAL(data);
-
-    construct(std::move(data), std::move(metadata));
+    return gaussian_increment(*metadata().default_context, di.sup() - di.inf());
+}
+DynamicallyConstructedStream::Lie BrownianStream::make_neighbour_root_increment(
+        DynamicallyConstructedStream::DyadicInterval neighbour_di) const
+{
+    return gaussian_increment(*metadata().default_context,
+                              neighbour_di.sup() - neighbour_di.inf());
 }
 
-#endif
+#define RPY_SERIAL_IMPL_CLASSNAME rpy::streams::BrownianStream
+#define RPY_SERIAL_DO_SPLIT
 
-#endif// ROUGHPY_STREAMS_PIECEWISE_LIE_STREAM_H_
+#include <roughpy/platform/serialization_instantiations.inl>
```

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/schema.h` & `roughpy-0.0.5/streams/include/roughpy/streams/schema.h`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 #ifndef ROUGHPY_STREAMS_SCHEMA_H
 #define ROUGHPY_STREAMS_SCHEMA_H
 
 #include <roughpy/core/traits.h>
 #include <roughpy/core/types.h>
 
 #include <roughpy/algebra/algebra_fwd.h>
+#include <roughpy/algebra/lie_basis.h>
 #include <roughpy/intervals/interval.h>
 #include <roughpy/intervals/real_interval.h>
 #include <roughpy/platform/serialization.h>
 #include <roughpy/scalars/key_scalar_array.h>
 
 #include <boost/container/flat_map.hpp>
 
@@ -85,14 +86,15 @@
 
 public:
     using typename base_type::const_iterator;
     using typename base_type::iterator;
     using static_iterator = typename static_vec_type::iterator;
     using static_const_iterator = typename static_vec_type::const_iterator;
     using typename base_type::value_type;
+    using lie_key = typename algebra::LieBasis::key_type;
 
     using base_type::begin;
     using base_type::emplace_back;
     using base_type::end;
     using base_type::reserve;
     using base_type::size;
 
@@ -227,14 +229,17 @@
     bool is_final() const noexcept { return m_is_final; }
     void finalize() noexcept { m_is_final = true; }
 
     RPY_NO_DISCARD
     intervals::RealInterval
     adjust_interval(const intervals::Interval& arg) const;
 
+    RPY_NO_DISCARD
+    lie_key label_to_lie_key(const string& label);
+
     RPY_SERIAL_SERIALIZE_FN();
 };
 
 RPY_SERIAL_SERIALIZE_FN_IMPL(StreamSchema)
 {
     RPY_SERIAL_SERIALIZE_NVP("channels", static_cast<base_type&>(*this));
     RPY_SERIAL_SERIALIZE_NVP("is_final", m_is_final);
```

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/schema_context.h` & `roughpy-0.0.5/streams/include/roughpy/streams/schema_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/stream.h` & `roughpy-0.0.5/streams/include/roughpy/streams/stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/stream_base.h` & `roughpy-0.0.5/streams/include/roughpy/streams/stream_base.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/stream_construction_helper.h` & `roughpy-0.0.5/streams/include/roughpy/streams/stream_construction_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/include/roughpy/streams/tick_stream.h` & `roughpy-0.0.5/streams/include/roughpy/streams/tick_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/channels.cpp` & `roughpy-0.0.5/streams/src/channels.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         case ChannelType::Value:
             if (value_info.lead_lag) {
                 if (label == "lead") {
                     return 0;
                 } else if (label == "lag") {
                     return 1;
                 } else {
-                    throw std::runtime_error(
+                    RPY_THROW(std::runtime_error,
                             "unrecognised variant label for type value");
                 }
             } else {
                 return 0;
             }
         case ChannelType::Categorical: break;
         case ChannelType::Lie:
@@ -210,15 +210,15 @@
             RPY_CHECK(i < lie_info.width);
             return i;
     }
 
     auto it = std::find(categorical_info.variants.begin(),
                         categorical_info.variants.end(), label);
     if (it == categorical_info.variants.end()) {
-        throw std::runtime_error(
+        RPY_THROW(std::runtime_error,
                 "unrecognised variant label for type categorical");
     }
 
     return static_cast<dimn_t>(it - categorical_info.variants.begin());
 }
 
 StreamChannel& StreamChannel::add_variant(string variant_label)
@@ -228,15 +228,15 @@
     if (variant_label.empty()) {
         variant_label = std::to_string(categorical_info.variants.size());
     }
 
     auto found = std::find(categorical_info.variants.begin(),
                            categorical_info.variants.end(), variant_label);
     if (found != categorical_info.variants.end()) {
-        throw std::runtime_error("variant with label " + variant_label
+        RPY_THROW(std::runtime_error,"variant with label " + variant_label
                                  + " already exists");
     }
 
     categorical_info.variants.push_back(std::move(variant_label));
     return *this;
 }
 StreamChannel& StreamChannel::insert_variant(string variant_label)
@@ -390,15 +390,15 @@
     switch (m_type) {
         case StaticChannelType::Value: return 0;
         case StaticChannelType::Categorical: {
             const auto begin = categorical_info.variants.begin();
             const auto end = categorical_info.variants.end();
             const auto found = std::find(begin, end, label);
             if (found == end) {
-                throw std::runtime_error("label " + label
+                RPY_THROW(std::runtime_error,"label " + label
                                          + " not a valid "
                                            "variant of this "
                                            "channel");
             }
             return static_cast<dimn_t>(found - begin);
         }
     }
```

### Comparing `roughpy-0.0.4/streams/src/dyadic_caching_layer.cpp` & `roughpy-0.0.5/streams/src/dyadic_caching_layer.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/dynamically_constructed_stream.cpp` & `roughpy-0.0.5/streams/src/dynamically_constructed_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.cpp` & `roughpy-0.0.5/streams/src/external_data_sources/csv_data_source.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.h` & `roughpy-0.0.5/streams/src/external_data_sources/csv_data_source.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.cpp` & `roughpy-0.0.5/streams/src/external_data_sources/sound_file_data_source.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     auto frame_end = param_to_frame(interval.sup());
 
     RPY_CHECK(frame_begin >= 0 && frame_begin <= frame_end
               && frame_end <= m_handle.frames());
 
     auto frame_count = frame_end - frame_begin;
     auto seek_pos = m_handle.seek(frame_begin, SEEK_SET);
-    if (seek_pos == -1) { throw std::runtime_error("invalid seek"); }
+    if (seek_pos == -1) { RPY_THROW(std::runtime_error, "invalid seek"); }
 
     result.allocate_scalars(frame_count * m_handle.channels());
 
     const auto& sinfo = ctype->info();
 
     if (sinfo.device.device_type == scalars::ScalarDeviceType::CPU) {
         if (sinfo.basic_info.code == scalars::ScalarTypeCode::Float) {
@@ -200,15 +200,15 @@
 
     StreamMetadata meta{0,       intervals::RealInterval(0, 1), nullptr,
                         nullptr, algebra::VectorType::Dense,    10};
 
     if (pl->width) {
         auto width = *pl->width;
         if (width != pl->handle.channels()) {
-            throw std::invalid_argument(
+            RPY_THROW(std::invalid_argument,
                     "requested width does not match number of channels");
         }
         meta.width = width;
     } else {
         meta.width = static_cast<deg_t>(pl->handle.channels());
     }
 
@@ -240,15 +240,15 @@
         // width and channels
         meta.default_context = pl->ctx;
     } else {
         if (meta.width != 0 && pl->depth && meta.data_scalar_type != nullptr) {
             meta.default_context = algebra::get_context(
                     meta.width, *pl->depth, meta.data_scalar_type, {});
         } else {
-            throw std::invalid_argument(
+            RPY_THROW(std::invalid_argument,
                     "insufficient information to get context");
         }
     }
 
     if (pl->vtype) { meta.cached_vector_type = *pl->vtype; }
     if (pl->resolution) { meta.default_resolution = *pl->resolution; }
```

### Comparing `roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.h` & `roughpy-0.0.5/streams/src/external_data_sources/sound_file_data_source.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/external_data_stream.cpp` & `roughpy-0.0.5/streams/src/external_data_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/lie_increment_stream.cpp` & `roughpy-0.0.5/streams/src/lie_increment_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/piecewise_abelian_stream.cpp` & `roughpy-0.0.5/streams/src/piecewise_abelian_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/schema.cpp` & `roughpy-0.0.5/streams/src/schema.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,17 @@
 
 StreamSchema::StreamSchema(dimn_t width)
 {
     reserve(width);
     for (dimn_t i = 0; i < width; ++i) { insert_increment(std::to_string(i)); }
 }
 
-bool StreamSchema::compare_labels(string_view item_label,
-                                  string_view ref_label) noexcept
+bool StreamSchema::compare_labels(
+        string_view item_label, string_view ref_label
+) noexcept
 {
 
     // If the reference label is shorter than item_label it cannot
     // have item_label as a prefix.
     if (ref_label.size() < item_label.size()) { return false; }
 
     if (ref_label.empty()) { return false; }
@@ -85,19 +86,19 @@
 StreamSchema::stream_dim_to_channel_it(dimn_t& stream_dim) const
 {
     for (auto cit = begin(); cit != end(); ++cit) {
         const auto channel_width = channel_it_to_width(cit);
         if (stream_dim < channel_width) { return cit; }
         stream_dim -= channel_width;
     }
-    throw std::runtime_error("stream dimension exceeds width");
+    RPY_THROW(std::runtime_error, "stream dimension exceeds width");
 }
 
-typename StreamSchema::const_iterator
-StreamSchema::find(const string& label) const
+typename StreamSchema::const_iterator StreamSchema::find(const string& label
+) const
 {
     auto it_current = begin();
     const auto it_end = end();
 
     for (; it_current != it_end; ++it_current) {
         if (compare_labels(it_current->first, label)) { return it_current; }
     }
@@ -145,36 +146,38 @@
 dimn_t StreamSchema::width() const { return width_to_iterator(end()); }
 
 dimn_t StreamSchema::channel_to_stream_dim(dimn_t channel_no) const
 {
     RPY_CHECK(channel_no < size());
     return width_to_iterator(nth(channel_no));
 }
-dimn_t StreamSchema::channel_variant_to_stream_dim(dimn_t channel_no,
-                                                   dimn_t variant_no) const
+dimn_t StreamSchema::channel_variant_to_stream_dim(
+        dimn_t channel_no, dimn_t variant_no
+) const
 {
     RPY_CHECK(channel_no < size());
     auto it = nth(channel_no);
 
     auto so_far = width_to_iterator(it);
     RPY_CHECK(variant_no < it->second.num_variants());
     return so_far + variant_no;
 }
 
-std::pair<dimn_t, dimn_t>
-StreamSchema::stream_dim_to_channel(dimn_t stream_dim) const
+std::pair<dimn_t, dimn_t> StreamSchema::stream_dim_to_channel(dimn_t stream_dim
+) const
 {
     std::pair<dimn_t, dimn_t> result(stream_dim, stream_dim);
     const auto channel_it = stream_dim_to_channel_it(result.second);
     result.first = static_cast<dimn_t>(channel_it - begin());
     return result;
 }
 
-string StreamSchema::label_from_channel_it(const_iterator channel_it,
-                                           dimn_t variant_id)
+string StreamSchema::label_from_channel_it(
+        const_iterator channel_it, dimn_t variant_id
+)
 {
     return channel_it->first + channel_it->second.label_suffix(variant_id);
 }
 
 string StreamSchema::label_of_stream_dim(dimn_t stream_dim) const
 {
     auto variant_id = stream_dim;
@@ -182,16 +185,17 @@
     return label_from_channel_it(channel_it, variant_id);
 }
 string_view StreamSchema::label_of_channel_id(dimn_t channel_id) const
 {
     RPY_CHECK(channel_id < size());
     return nth(channel_id)->first;
 }
-string StreamSchema::label_of_channel_variant(dimn_t channel_id,
-                                              dimn_t channel_variant) const
+string StreamSchema::label_of_channel_variant(
+        dimn_t channel_id, dimn_t channel_variant
+) const
 {
     RPY_CHECK(channel_id < size());
     return label_from_channel_it(nth(channel_id), channel_variant);
 }
 
 dimn_t StreamSchema::label_to_stream_dim(const string& label) const
 {
@@ -212,15 +216,16 @@
         default:
             // The find method will not have matched if neither
             // of these cases occurred.
             RPY_UNREACHABLE();
     }
 
     const string_view variant_label(
-            &*variant_begin, static_cast<dimn_t>(label.end() - variant_begin));
+            &*variant_begin, static_cast<dimn_t>(label.end() - variant_begin)
+    );
     result += channel->second.variant_id_of_label(variant_label);
     return result;
 }
 
 StreamChannel& StreamSchema::insert(string label, StreamChannel&& channel_data)
 {
     RPY_CHECK(!m_is_final);
@@ -285,11 +290,17 @@
     if (found != end) { return found->second; }
 
     return m_static_channels
             .insert(end,
                     {std::move(label), StaticChannel(CategoricalChannelInfo())})
             ->second;
 }
+typename StreamSchema::lie_key
+StreamSchema::label_to_lie_key(const string& label)
+{
+    auto idx = label_to_stream_dim(label);
+    return static_cast<lie_key>(idx) + 1;
+}
 
 #define RPY_SERIAL_IMPL_CLASSNAME rpy::streams::StreamSchema
 
 #include <roughpy/platform/serialization_instantiations.inl>
```

### Comparing `roughpy-0.0.4/streams/src/schema_context.cpp` & `roughpy-0.0.5/streams/src/schema_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/stream.cpp` & `roughpy-0.0.5/streams/src/stream.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     const auto& md = metadata();
     return p_impl->log_signature(m_support, resolution, *md.default_context);
 }
 rpy::streams::Stream::Lie rpy::streams::Stream::log_signature(
         rpy::resolution_t resolution, const rpy::streams::Stream::Context& ctx
 ) const
 {
-    const auto& md = metadata();
+//    const auto& md = metadata();
     return p_impl->log_signature(m_support, resolution, ctx);
 }
 rpy::streams::Stream::Lie rpy::streams::Stream::log_signature(
         const rpy::streams::Stream::Interval& interval
 ) const
 {
     const auto& md = metadata();
@@ -294,10 +294,13 @@
     new_md.default_context = &ctx;
 
     return Stream(PiecewiseAbelianStream(
             std::move(pieces), std::move(new_md), p_impl->get_schema()
     ));
 }
 
+
+
+
 #define RPY_SERIAL_IMPL_CLASSNAME rpy::streams::Stream
 
 #include <roughpy/platform/serialization_instantiations.inl>
```

### Comparing `roughpy-0.0.4/streams/src/stream_base.cpp` & `roughpy-0.0.5/streams/src/stream_base.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/stream_construction_helper.cpp` & `roughpy-0.0.5/streams/src/stream_construction_helper.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/test_brownian_stream.cpp` & `roughpy-0.0.5/streams/src/test_brownian_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/test_lie_increment_stream.cpp` & `roughpy-0.0.5/streams/src/test_lie_increment_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/test_schema.cpp` & `roughpy-0.0.5/streams/src/test_schema.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/streams/src/tick_stream.cpp` & `roughpy-0.0.5/streams/src/tick_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/algebra/test_alg_poly_coeffs.py` & `roughpy-0.0.5/tests/algebra/test_alg_poly_coeffs.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/algebra/test_algebra_context.py` & `roughpy-0.0.5/tests/algebra/test_algebra_context.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/algebra/test_free_tensor.py` & `roughpy-0.0.5/tests/algebra/test_free_tensor.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/algebra/test_lie.py` & `roughpy-0.0.5/tests/algebra/test_lie.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/algebra/test_lie_keys.py` & `roughpy-0.0.5/tests/algebra/test_lie_keys.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/algebra/test_tensor_iterator.py` & `roughpy-0.0.5/tests/algebra/test_tensor_iterator.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/algebra/test_tensor_keys.py` & `roughpy-0.0.5/tests/algebra/test_tensor_keys.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/conftest.py` & `roughpy-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/intervals/test_intervals.py` & `roughpy-0.0.5/tests/intervals/test_intervals.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/scalars/test_monomial.py` & `roughpy-0.0.5/tests/scalars/test_monomial.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/audio/test.flac` & `roughpy-0.0.5/tests/streams/audio/test.flac`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/audio/test.mp3` & `roughpy-0.0.5/tests/streams/audio/test.mp3`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/audio/test.wav` & `roughpy-0.0.5/tests/streams/audio/test.wav`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/test_brownian_stream.py` & `roughpy-0.0.5/tests/streams/test_brownian_stream.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/test_function_path.py` & `roughpy-0.0.5/tests/streams/test_function_path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/test_lie_increment_path.py` & `roughpy-0.0.5/tests/streams/test_lie_increment_path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/test_piecewise_lie_path.py` & `roughpy-0.0.5/tests/streams/test_piecewise_lie_path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/test_schema.py` & `roughpy-0.0.5/tests/streams/test_schema.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/test_sound_path.py` & `roughpy-0.0.5/tests/streams/test_sound_path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tests/streams/test_tick_stream.py` & `roughpy-0.0.5/tests/streams/test_tick_stream.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tools/ci/before-all-common.sh` & `roughpy-0.0.5/tools/ci/before-all-common.sh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tools/python-get-binary-obj-path.py` & `roughpy-0.0.5/tools/python-get-binary-obj-path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/tools/version_from_file.py` & `roughpy-0.0.5/tools/version_from_file.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/vcpkg.json` & `roughpy-0.0.5/vcpkg.json`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.4/PKG-INFO` & `roughpy-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roughpy
-Version: 0.0.4
+Version: 0.0.5
 Keywords: data streams rough paths signatures
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: BSD License
@@ -16,15 +16,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 
-![RoughPy Logo](https://github.com/datasig-ac-uk/roughpy/tree/main/branding/logo/logo_square_white.jpg)
+<center>
+  <img src="https://raw.githubusercontent.com/datasig-ac-uk/RoughPy/main/branding/logo/logo_square_white.jpg">
+</center><br>
+
 # RoughPy
 RoughPy is a package for working with streaming data as rough paths, and working with algebraic objects such as free tensors, shuffle tensors, and elements of the free Lie algebra.
 
 This library is currently in an alpha stage, and as such many features are still incomplete or not fully implemented. Please bear this in mind when looking at the source code.
 
 
 ## Installation
@@ -42,17 +45,26 @@
 You will need to make sure that vcpkg is available on your system before attempting to build RoughPy.
 The following commands should be sufficient to set up the environment for building RoughPy:
 ```bash
 git clone https://github.com/Microsoft/vcpkg.git tools/vcpkg
 tools/vcpkg/bootstrap-vcpkg.sh
 export CMAKE_TOOLCHAIN_FILE=$(pwd)/tools/vcpkg/scripts/buildsystems/vcpkg.cmake
 ```
-With this environment variable set, you should now be able to pip install either using the PyPI source distribution (using the `--no-binary :all:` flag), or directly from GitHub:
+With this environment variable set, most of the dependencies will be installed automatically during the build process.
+
+On MacOS with Apple Silicon you will need to install libomp (for example using Homebrew `brew install libomp`).
+This is not necessary on Intel based MacOS where the Intel iomp5 can be used instead. 
+The build system will use `brew --prefix libomp` to try to locate this library.
+(The actual `brew` executable can be customised by setting the `ROUGHPY_BREW_EXECUTABLE` CMake variable 
+or environment variable.)
+
+You should now be able to pip install either using the PyPI source distribution (using the `--no-binary :roughpy:` 
+flag), or directly from GitHub (recommended):
 ```bash
-pip install https://github.com/datasig-ac-uk/RoughPy.git
+pip install git+https://github.com/datasig-ac-uk/RoughPy.git
 ```
 It will take some time to build.
 
 ## Usage
 Following the NumPy (and related) convention, we import RoughPy under the alias `rp` as follows:
 ```python
 import roughpy as rp
@@ -92,14 +104,24 @@
 ## Contributors
 The full list of contributors is listed in `THANKS` alongside this readme. The people mentioned in this document constitute `The RoughPy Developers`.
 
 ## License
 RoughPy is licensed under a BSD-3-Clause license. This was chosen specifically to match the license of NumPy.
 # Changelog
 
+Version 0.0.5:
+  - Added free functions for performing free-tensor, shuffle, half-shuffle
+  multiplication between pairs of tensors (of either kind).
+  - Added free function for applying the adjoint of left free tensor
+  multiplication to arbitrary tensors.
+  - Improved exception usage, messages now include filename, lineno, and
+  function name to help locate c++ exceptions passed through to Python.
+  - Basis objects in Python are now iterable.
+  - Added `split_n` and `to_index` methods to Tensor key.
+
 Version 0.0.4:
   - Overhauled the RPY_CHECK macro so it now gives much better contextual
   information.
   - Readme updated to reflect PyPI installation with wheels.
   - Antipode is now implemented in libalgebra_lite, and exposed to Python for
   Free tensors.
   - Streams now carry a support interval, outside of which the signature will be
```

