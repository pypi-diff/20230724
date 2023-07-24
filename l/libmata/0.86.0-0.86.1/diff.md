# Comparing `tmp/libmata-0.86.0.tar.gz` & `tmp/libmata-0.86.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-0.86.0.tar", last modified: Mon Jul 24 16:08:49 2023, max compression
+gzip compressed data, was "libmata-0.86.1.tar", last modified: Mon Jul 24 17:43:22 2023, max compression
```

## Comparing `libmata-0.86.0.tar` & `libmata-0.86.1.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.940061 libmata-0.86.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-07-24 16:08:49.940061 libmata-0.86.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.920060 libmata-0.86.0/libmata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   525998 2023-07-24 16:04:56.359338 libmata-0.86.0/libmata/alphabets.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/alphabets.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/alphabets.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.920060 libmata-0.86.0/libmata/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/nfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1690493 2023-07-24 16:04:57.311417 libmata-0.86.0/libmata/nfa/nfa.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/nfa/nfa.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    43671 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/nfa/nfa.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   434179 2023-07-24 16:04:58.023476 libmata-0.86.0/libmata/nfa/strings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/nfa/strings.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/nfa/strings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   249287 2023-07-24 16:04:58.471515 libmata-0.86.0/libmata/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   696495 2023-07-24 16:04:59.103577 libmata-0.86.0/libmata/plotting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/plotting.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   458228 2023-07-24 16:04:59.363603 libmata-0.86.0/libmata/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-24 16:04:00.985938 libmata-0.86.0/libmata/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.920060 libmata-0.86.0/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.920060 libmata-0.86.0/mata/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-07-24 16:04:00.953934 libmata-0.86.0/mata/3rdparty/args.hxx
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-07-24 16:04:00.957934 libmata-0.86.0/mata/3rdparty/catch.hpp.1.9.3
--rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/catch.hpp.2.0.1
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/catch.hpp.2.13.9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.920060 libmata-0.86.0/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.920060 libmata-0.86.0/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-24 16:04:00.961935 libmata-0.86.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.924060 libmata-0.86.0/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-24 16:04:00.965935 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-24 16:04:00.969936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.924060 libmata-0.86.0/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.924060 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 16:04:00.973936 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/composeids.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.916060 libmata-0.86.0/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.916060 libmata-0.86.0/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-24 16:04:00.977937 libmata-0.86.0/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.928061 libmata-0.86.0/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/3rdparty/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 16:04:00.981937 libmata-0.86.0/mata/3rdparty/simlib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.916060 libmata-0.86.0/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.916060 libmata-0.86.0/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-24 16:08:49.808054 libmata-0.86.0/mata/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101164 2023-07-24 16:08:49.808054 libmata-0.86.0/mata/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-24 16:08:49.808054 libmata-0.86.0/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-24 16:08:49.808054 libmata-0.86.0/mata/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-24 16:08:49.808054 libmata-0.86.0/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 16:08:49.808054 libmata-0.86.0/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.916060 libmata-0.86.0/mata/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/cmake/Modules/Catch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/cmake/Modules/CatchAddTests.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/cmake/Modules/CodeCoverage.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/cmake/Modules/FindValgrind.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/cmake/Modules/GetGitRevisionDescription.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 16:04:00.985938 libmata-0.86.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.916060 libmata-0.86.0/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/include/mata/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/afa/afa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/alphabet.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/include/mata/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/nfa/algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/nfa/builder.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/nfa/delta.hh
--rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/nfa/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/nfa/plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/nfa/strings.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/nfa/types.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.932061 libmata-0.86.0/mata/include/mata/parser/
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/parser/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/parser/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/parser/parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/parser/re2parser.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.936061 libmata-0.86.0/mata/include/mata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/utils/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/utils/number-predicate.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/utils/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/utils/sparse-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/utils/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/include/mata/utils/util.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.936061 libmata-0.86.0/mata/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/scripts/merge_static_libraries.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.936061 libmata-0.86.0/mata/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.936061 libmata-0.86.0/mata/src/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    38800 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.940061 libmata-0.86.0/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/nfa/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/nfa/complement.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/nfa/concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/nfa/delta.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/nfa/inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/nfa/intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30427 2023-07-24 16:04:00.989938 libmata-0.86.0/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32836 2023-07-24 16:04:00.993939 libmata-0.86.0/mata/src/nfa/operations.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-24 16:04:00.993939 libmata-0.86.0/mata/src/nfa/universal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-24 16:04:00.993939 libmata-0.86.0/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-07-24 16:04:00.993939 libmata-0.86.0/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.940061 libmata-0.86.0/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-24 16:04:00.993939 libmata-0.86.0/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-24 16:04:00.993939 libmata-0.86.0/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-24 16:04:00.993939 libmata-0.86.0/mata/src/strings/nfa-strings.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.940061 libmata-0.86.0/mata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.940061 libmata-0.86.0/mata/tests/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    27575 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)    42818 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.940061 libmata-0.86.0/mata/tests/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/nfa/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32066 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/nfa/nfa-concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/nfa/nfa-intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/nfa/nfa-profiling.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/nfa/nfa-util.hh
--rw-r--r--   0 runner    (1001) docker     (123)    83454 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/ord-vector.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/re2parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/sparse-set.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:08:49.940061 libmata-0.86.0/mata/tests/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/strings/nfa-string-solving.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-24 16:04:01.005940 libmata-0.86.0/mata/tests/synchronized-iterator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 16:04:00.985938 libmata-0.86.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-24 16:04:00.985938 libmata-0.86.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.893743 libmata-0.86.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-24 17:43:22.893743 libmata-0.86.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.881743 libmata-0.86.1/libmata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   525998 2023-07-24 17:39:34.086904 libmata-0.86.1/libmata/alphabets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/alphabets.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/alphabets.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.881743 libmata-0.86.1/libmata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/nfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1690493 2023-07-24 17:39:35.066901 libmata-0.86.1/libmata/nfa/nfa.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/nfa/nfa.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    43671 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/nfa/nfa.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   434179 2023-07-24 17:39:35.758898 libmata-0.86.1/libmata/nfa/strings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/nfa/strings.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/nfa/strings.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   249287 2023-07-24 17:39:36.194896 libmata-0.86.1/libmata/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   696495 2023-07-24 17:39:36.866895 libmata-0.86.1/libmata/plotting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/plotting.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   458228 2023-07-24 17:39:37.146896 libmata-0.86.1/libmata/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-24 17:38:42.983003 libmata-0.86.1/libmata/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.881743 libmata-0.86.1/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.881743 libmata-0.86.1/mata/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-07-24 17:38:42.947003 libmata-0.86.1/mata/3rdparty/args.hxx
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-07-24 17:38:42.955003 libmata-0.86.1/mata/3rdparty/catch.hpp.1.9.3
+-rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-07-24 17:38:42.955003 libmata-0.86.1/mata/3rdparty/catch.hpp.2.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/catch.hpp.2.13.9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.881743 libmata-0.86.1/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.881743 libmata-0.86.1/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-24 17:38:42.959003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-24 17:38:42.963003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 17:38:42.967003 libmata-0.86.1/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-24 17:38:42.971003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/composeids.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.877743 libmata-0.86.1/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.877743 libmata-0.86.1/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.885743 libmata-0.86.1/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-24 17:38:42.975003 libmata-0.86.1/mata/3rdparty/re2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.877743 libmata-0.86.1/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.877743 libmata-0.86.1/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-24 17:38:42.979003 libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-24 17:38:42.983003 libmata-0.86.1/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-24 17:43:22.773743 libmata-0.86.1/mata/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101164 2023-07-24 17:43:22.773743 libmata-0.86.1/mata/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-24 17:43:22.773743 libmata-0.86.1/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-24 17:43:22.773743 libmata-0.86.1/mata/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-07-24 17:43:22.773743 libmata-0.86.1/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 17:43:22.773743 libmata-0.86.1/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.877743 libmata-0.86.1/mata/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-24 17:38:42.983003 libmata-0.86.1/mata/cmake/Modules/Catch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-24 17:38:42.983003 libmata-0.86.1/mata/cmake/Modules/CatchAddTests.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-24 17:38:42.983003 libmata-0.86.1/mata/cmake/Modules/CodeCoverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 17:38:42.983003 libmata-0.86.1/mata/cmake/Modules/FindValgrind.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-07-24 17:38:42.983003 libmata-0.86.1/mata/cmake/Modules/GetGitRevisionDescription.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 17:38:42.983003 libmata-0.86.1/mata/cmake/Modules/GetGitRevisionDescription.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.881743 libmata-0.86.1/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/include/mata/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/afa/afa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/alphabet.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/include/mata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/nfa/algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/nfa/builder.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/nfa/delta.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/nfa/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/nfa/plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/nfa/strings.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/nfa/types.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/include/mata/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/parser/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/parser/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/parser/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/parser/re2parser.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/include/mata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/utils/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/utils/number-predicate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/utils/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/utils/sparse-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/utils/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/include/mata/utils/util.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/scripts/merge_static_libraries.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/src/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    38800 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/complement.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/delta.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30427 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32836 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/operations.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-24 17:38:42.987002 libmata-0.86.1/mata/src/nfa/universal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-24 17:38:42.991003 libmata-0.86.1/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-07-24 17:38:42.991003 libmata-0.86.1/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.889743 libmata-0.86.1/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-24 17:38:42.991003 libmata-0.86.1/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-24 17:38:42.991003 libmata-0.86.1/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-24 17:38:42.991003 libmata-0.86.1/mata/src/strings/nfa-strings.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.893743 libmata-0.86.1/mata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.893743 libmata-0.86.1/mata/tests/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    27575 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    42818 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.893743 libmata-0.86.1/mata/tests/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32066 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/nfa/nfa-concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/nfa/nfa-intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/nfa/nfa-profiling.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/nfa/nfa-util.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    83454 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/ord-vector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-07-24 17:38:43.003003 libmata-0.86.1/mata/tests/re2parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-24 17:38:43.007002 libmata-0.86.1/mata/tests/sparse-set.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:43:22.893743 libmata-0.86.1/mata/tests/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-07-24 17:38:43.007002 libmata-0.86.1/mata/tests/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-24 17:38:43.007002 libmata-0.86.1/mata/tests/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-24 17:38:43.007002 libmata-0.86.1/mata/tests/strings/nfa-string-solving.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-24 17:38:43.007002 libmata-0.86.1/mata/tests/synchronized-iterator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 17:38:42.983003 libmata-0.86.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-24 17:38:42.983003 libmata-0.86.1/setup.py
```

### Comparing `libmata-0.86.0/PKG-INFO` & `libmata-0.86.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 0.86.0
+Version: 0.86.1
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Mata: The Automata Library
 
 [![GitHub tag](https://img.shields.io/github/tag/VeriFIT/mata.svg)](https://github.com/VeriFIT/mata)
-
-[![master: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
-[![master: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
-
-[![devel: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
-[![devel: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
+[![Quality](https://github.com/VeriFIT/mata/actions/workflows/code-quality.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/code-quality.yml)
+[![Python-Binding (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/python-binding.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/python-binding.yml)
 [![codecov](https://codecov.io/gh/VeriFIT/mata/branch/devel/graph/badge.svg?token=9VAVD19N4D)](https://codecov.io/gh/VeriFIT/mata)
 
 Mata is an open source automata library that offers interface for different kinds of automata (NFA,
 AFA, etc.). Currently, Mata offers two interfaces:
 
   1. An efficient library implemented in C/C++
   2. A flexible wrapper implemented in Python that uses the efficient library
```

### Comparing `libmata-0.86.0/libmata/alphabets.cpp` & `libmata-0.86.1/libmata/alphabets.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/alphabets.pxd` & `libmata-0.86.1/libmata/alphabets.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/alphabets.pyx` & `libmata-0.86.1/libmata/alphabets.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/nfa/nfa.cpp` & `libmata-0.86.1/libmata/nfa/nfa.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/nfa/nfa.pxd` & `libmata-0.86.1/libmata/nfa/nfa.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/nfa/nfa.pyx` & `libmata-0.86.1/libmata/nfa/nfa.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/nfa/strings.cpp` & `libmata-0.86.1/libmata/nfa/strings.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/nfa/strings.pxd` & `libmata-0.86.1/libmata/nfa/strings.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/nfa/strings.pyx` & `libmata-0.86.1/libmata/nfa/strings.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/parser.cpp` & `libmata-0.86.1/libmata/parser.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/parser.pyx` & `libmata-0.86.1/libmata/parser.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/plotting.cpp` & `libmata-0.86.1/libmata/plotting.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/plotting.pyx` & `libmata-0.86.1/libmata/plotting.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/utils.cpp` & `libmata-0.86.1/libmata/utils.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/utils.pxd` & `libmata-0.86.1/libmata/utils.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/libmata/utils.pyx` & `libmata-0.86.1/libmata/utils.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/args.hxx` & `libmata-0.86.1/mata/3rdparty/args.hxx`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/catch.hpp` & `libmata-0.86.1/mata/3rdparty/catch.hpp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/catch.hpp.1.9.3` & `libmata-0.86.1/mata/3rdparty/catch.hpp.1.9.3`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/catch.hpp.2.0.1` & `libmata-0.86.1/mata/3rdparty/catch.hpp.2.0.1`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/catch.hpp.2.13.9` & `libmata-0.86.1/mata/3rdparty/catch.hpp.2.13.9`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/CMakeLists.txt` & `libmata-0.86.1/mata/3rdparty/cudd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/Doxyfile.in` & `libmata-0.86.1/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/LICENSE` & `libmata-0.86.1/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/README` & `libmata-0.86.1/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-0.86.1/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-0.86.1/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-0.86.1/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-0.86.1/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-0.86.1/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-0.86.1/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-0.86.1/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-0.86.1/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-0.86.1/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-0.86.1/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/epd/epd.c` & `libmata-0.86.1/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/epd/epd.h` & `libmata-0.86.1/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-0.86.1/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/groups.dox` & `libmata-0.86.1/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-0.86.1/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-0.86.1/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-0.86.1/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-0.86.1/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-0.86.1/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-0.86.1/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-0.86.1/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-0.86.1/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/st/st.c` & `libmata-0.86.1/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/st/st.h` & `libmata-0.86.1/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/st/testst.c` & `libmata-0.86.1/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-0.86.1/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/datalimit.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/pipefork.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/prtime.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/strsav.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/texpand.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-0.86.1/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/cudd/util/util.h` & `libmata-0.86.1/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/CMakeLists.txt` & `libmata-0.86.1/mata/3rdparty/re2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-0.86.1/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/LICENSE` & `libmata-0.86.1/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/compile.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/parse.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/pod_array.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/prog.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/prog.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/re2.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/re2.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/regexp.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/regexp.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/simplify.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/tostring.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-0.86.1/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-0.86.1/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/util/logging.h` & `libmata-0.86.1/mata/3rdparty/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/util/mutex.h` & `libmata-0.86.1/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/util/rune.cc` & `libmata-0.86.1/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/util/strutil.cc` & `libmata-0.86.1/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/util/utf.h` & `libmata-0.86.1/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/re2/util/util.h` & `libmata-0.86.1/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-0.86.1/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-0.86.1/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/CMakeLists.txt` & `libmata-0.86.1/mata/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/Doxyfile.in` & `libmata-0.86.1/mata/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/LICENSE` & `libmata-0.86.1/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/Makefile` & `libmata-0.86.1/mata/Makefile`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/README.md` & `libmata-0.86.1/mata/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # Mata: The Automata Library
 
 [![GitHub tag](https://img.shields.io/github/tag/VeriFIT/mata.svg)](https://github.com/VeriFIT/mata)
-
-[![master: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
-[![master: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
-
-[![devel: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
-[![devel: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
+[![Quality](https://github.com/VeriFIT/mata/actions/workflows/code-quality.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/code-quality.yml)
+[![Python-Binding (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/python-binding.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/python-binding.yml)
 [![codecov](https://codecov.io/gh/VeriFIT/mata/branch/devel/graph/badge.svg?token=9VAVD19N4D)](https://codecov.io/gh/VeriFIT/mata)
 
 Mata is an open source automata library that offers interface for different kinds of automata (NFA,
 AFA, etc.). Currently, Mata offers two interfaces:
 
   1. An efficient library implemented in C/C++
   2. A flexible wrapper implemented in Python that uses the efficient library
```

### Comparing `libmata-0.86.0/mata/cmake/Modules/Catch.cmake` & `libmata-0.86.1/mata/cmake/Modules/Catch.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/cmake/Modules/CatchAddTests.cmake` & `libmata-0.86.1/mata/cmake/Modules/CatchAddTests.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/cmake/Modules/CodeCoverage.cmake` & `libmata-0.86.1/mata/cmake/Modules/CodeCoverage.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/cmake/Modules/FindValgrind.cmake` & `libmata-0.86.1/mata/cmake/Modules/FindValgrind.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/cmake/Modules/GetGitRevisionDescription.cmake` & `libmata-0.86.1/mata/cmake/Modules/GetGitRevisionDescription.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in` & `libmata-0.86.1/mata/cmake/Modules/GetGitRevisionDescription.cmake.in`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/afa/afa.hh` & `libmata-0.86.1/mata/include/mata/afa/afa.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/alphabet.hh` & `libmata-0.86.1/mata/include/mata/alphabet.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/nfa/algorithms.hh` & `libmata-0.86.1/mata/include/mata/nfa/algorithms.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/nfa/builder.hh` & `libmata-0.86.1/mata/include/mata/nfa/builder.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/nfa/delta.hh` & `libmata-0.86.1/mata/include/mata/nfa/delta.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/nfa/nfa.hh` & `libmata-0.86.1/mata/include/mata/nfa/nfa.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/nfa/plumbing.hh` & `libmata-0.86.1/mata/include/mata/nfa/plumbing.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/nfa/strings.hh` & `libmata-0.86.1/mata/include/mata/nfa/strings.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/nfa/types.hh` & `libmata-0.86.1/mata/include/mata/nfa/types.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/parser/inter-aut.hh` & `libmata-0.86.1/mata/include/mata/parser/inter-aut.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/parser/mintermization.hh` & `libmata-0.86.1/mata/include/mata/parser/mintermization.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/parser/parser.hh` & `libmata-0.86.1/mata/include/mata/parser/parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/parser/re2parser.hh` & `libmata-0.86.1/mata/include/mata/parser/re2parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/utils/closed-set.hh` & `libmata-0.86.1/mata/include/mata/utils/closed-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/utils/number-predicate.hh` & `libmata-0.86.1/mata/include/mata/utils/number-predicate.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/utils/ord-vector.hh` & `libmata-0.86.1/mata/include/mata/utils/ord-vector.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/utils/sparse-set.hh` & `libmata-0.86.1/mata/include/mata/utils/sparse-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/utils/synchronized-iterator.hh` & `libmata-0.86.1/mata/include/mata/utils/synchronized-iterator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/include/mata/utils/util.hh` & `libmata-0.86.1/mata/include/mata/utils/util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/CMakeLists.txt` & `libmata-0.86.1/mata/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/afa/afa.cc` & `libmata-0.86.1/mata/src/afa/afa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/alphabet.cc` & `libmata-0.86.1/mata/src/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/inter-aut.cc` & `libmata-0.86.1/mata/src/inter-aut.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/mintermization.cc` & `libmata-0.86.1/mata/src/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/builder.cc` & `libmata-0.86.1/mata/src/nfa/builder.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/complement.cc` & `libmata-0.86.1/mata/src/nfa/complement.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/concatenation.cc` & `libmata-0.86.1/mata/src/nfa/concatenation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/delta.cc` & `libmata-0.86.1/mata/src/nfa/delta.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/inclusion.cc` & `libmata-0.86.1/mata/src/nfa/inclusion.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/intersection.cc` & `libmata-0.86.1/mata/src/nfa/intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/nfa.cc` & `libmata-0.86.1/mata/src/nfa/nfa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/operations.cc` & `libmata-0.86.1/mata/src/nfa/operations.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/nfa/universal.cc` & `libmata-0.86.1/mata/src/nfa/universal.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/parser.cc` & `libmata-0.86.1/mata/src/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/re2parser.cc` & `libmata-0.86.1/mata/src/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/strings/nfa-noodlification.cc` & `libmata-0.86.1/mata/src/strings/nfa-noodlification.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/strings/nfa-segmentation.cc` & `libmata-0.86.1/mata/src/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/src/strings/nfa-strings.cc` & `libmata-0.86.1/mata/src/strings/nfa-strings.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/CMakeLists.txt` & `libmata-0.86.1/mata/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/afa/afa.cc` & `libmata-0.86.1/mata/tests/afa/afa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/alphabet.cc` & `libmata-0.86.1/mata/tests/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/main.cc` & `libmata-0.86.1/mata/tests/main.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/mintermization.cc` & `libmata-0.86.1/mata/tests/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/nfa/builder.cc` & `libmata-0.86.1/mata/tests/nfa/builder.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/nfa/nfa-concatenation.cc` & `libmata-0.86.1/mata/tests/nfa/nfa-concatenation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/nfa/nfa-intersection.cc` & `libmata-0.86.1/mata/tests/nfa/nfa-intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/nfa/nfa-profiling.cc` & `libmata-0.86.1/mata/tests/nfa/nfa-profiling.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/nfa/nfa-util.hh` & `libmata-0.86.1/mata/tests/nfa/nfa-util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/nfa/nfa.cc` & `libmata-0.86.1/mata/tests/nfa/nfa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/ord-vector.cc` & `libmata-0.86.1/mata/tests/ord-vector.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/parser.cc` & `libmata-0.86.1/mata/tests/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/re2parser.cc` & `libmata-0.86.1/mata/tests/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/sparse-set.cc` & `libmata-0.86.1/mata/tests/sparse-set.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/strings/nfa-noodlification.cc` & `libmata-0.86.1/mata/tests/strings/nfa-noodlification.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/strings/nfa-segmentation.cc` & `libmata-0.86.1/mata/tests/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/strings/nfa-string-solving.cc` & `libmata-0.86.1/mata/tests/strings/nfa-string-solving.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/mata/tests/synchronized-iterator.cc` & `libmata-0.86.1/mata/tests/synchronized-iterator.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.86.0/setup.py` & `libmata-0.86.1/setup.py`

 * *Files identical despite different names*

