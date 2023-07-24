# Comparing `tmp/libmata-0.84.0.tar.gz` & `tmp/libmata-0.85.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-0.84.0.tar", last modified: Fri Jul 21 07:51:12 2023, max compression
+gzip compressed data, was "libmata-0.85.0.tar", last modified: Mon Jul 24 11:04:57 2023, max compression
```

## Comparing `libmata-0.84.0.tar` & `libmata-0.85.0.tar`

### file list

```diff
@@ -1,502 +1,502 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.697806 libmata-0.84.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-21 07:51:12.697806 libmata-0.84.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.673804 libmata-0.84.0/libmata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   526002 2023-07-21 07:46:05.719702 libmata-0.84.0/libmata/alphabets.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/alphabets.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/alphabets.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.673804 libmata-0.84.0/libmata/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/nfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1690497 2023-07-21 07:46:07.027778 libmata-0.84.0/libmata/nfa/nfa.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/nfa/nfa.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    43671 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/nfa/nfa.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   434183 2023-07-21 07:46:07.955833 libmata-0.84.0/libmata/nfa/strings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/nfa/strings.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/nfa/strings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   249291 2023-07-21 07:46:08.551867 libmata-0.84.0/libmata/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   696499 2023-07-21 07:46:09.395916 libmata-0.84.0/libmata/plotting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/plotting.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   458232 2023-07-21 07:46:09.739936 libmata-0.84.0/libmata/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-21 07:45:06.176207 libmata-0.84.0/libmata/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.673804 libmata-0.84.0/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.673804 libmata-0.84.0/mata/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-07-21 07:45:06.124204 libmata-0.84.0/mata/3rdparty/args.hxx
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-07-21 07:45:06.128204 libmata-0.84.0/mata/3rdparty/catch.hpp.1.9.3
--rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-07-21 07:45:06.128204 libmata-0.84.0/mata/3rdparty/catch.hpp.2.0.1
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/catch.hpp.2.13.9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.673804 libmata-0.84.0/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.681805 libmata-0.84.0/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.685805 libmata-0.84.0/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-21 07:45:06.156206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.685805 libmata-0.84.0/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-21 07:45:06.160206 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.685805 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-21 07:45:06.164207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/composeids.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-21 07:45:06.168207 libmata-0.84.0/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.681805 libmata-0.84.0/mata/3rdparty/cudd-min/
--rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/bnet.c
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/bnet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/chkMterm.c
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/config.h
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-21 07:45:06.132205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-21 07:45:06.136205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-21 07:45:06.140205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/dddmpUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/epdInt.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/3rdparty/cudd-min/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/3rdparty/cudd-min/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.681805 libmata-0.84.0/mata/3rdparty/cudd-min/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-21 07:45:06.144205 libmata-0.84.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/ntr.c
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/ntr.h
--rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/ntrBddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/ntrHeap.c
--rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/ntrMflow.c
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/ntrShort.c
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/ntrZddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/st.h
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/testdddmp.c
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/testmtr.c
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-07-21 07:45:06.148206 libmata-0.84.0/mata/3rdparty/cudd-min/testobj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd-min/testst.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd-min/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd-min/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-21 07:45:06.152206 libmata-0.84.0/mata/3rdparty/cudd-min/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/simlib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-21 07:45:06.172207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.689805 libmata-0.84.0/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-21 07:45:06.176207 libmata-0.84.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-21 07:51:12.489793 libmata-0.84.0/mata/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101164 2023-07-21 07:51:12.489793 libmata-0.84.0/mata/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-21 07:51:12.489793 libmata-0.84.0/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-21 07:51:12.489793 libmata-0.84.0/mata/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-07-21 07:51:12.489793 libmata-0.84.0/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 07:51:12.489793 libmata-0.84.0/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cli/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cli/MATA-CLI-philosophy.md
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cli/interpreter.cc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5882 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cli/mata
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cli/mata-code.cc
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cli/version.cc.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cmake/Modules/Catch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cmake/Modules/CatchAddTests.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cmake/Modules/CodeCoverage.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cmake/Modules/FindValgrind.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cmake/Modules/GetGitRevisionDescription.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-21 07:45:06.180207 libmata-0.84.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.669804 libmata-0.84.0/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/include/mata/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/afa/afa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/alphabet.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/include/mata/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/nfa/algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/nfa/builder.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/nfa/delta.hh
--rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/nfa/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/nfa/plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/nfa/strings.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/nfa/types.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/include/mata/parser/
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/parser/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/parser/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/parser/parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/parser/re2parser.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/include/mata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/utils/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/utils/number-predicate.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/utils/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/utils/sparse-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/utils/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/include/mata/utils/util.hh
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-21 07:51:12.489793 libmata-0.84.0/mata/merge_static_libraries.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/src/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    38800 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/nfa/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-21 07:45:06.184208 libmata-0.84.0/mata/src/nfa/complement.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/nfa/concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/nfa/delta.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/nfa/inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/nfa/intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30427 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32836 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/nfa/operations.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/nfa/universal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-21 07:45:06.188208 libmata-0.84.0/mata/src/strings/nfa-strings.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/tests/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    27575 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)    42818 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/tests/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/nfa/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32066 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/nfa/nfa-concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/nfa/nfa-intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-21 07:45:06.204209 libmata-0.84.0/mata/tests/nfa/nfa-profiling.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/nfa/nfa-util.hh
--rw-r--r--   0 runner    (1001) docker     (123)    83454 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/ord-vector.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/re2parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/sparse-set.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/tests/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/strings/nfa-string-solving.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/tests/synchronized-iterator.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:51:12.693806 libmata-0.84.0/mata/unit-test-data/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/unit-test-data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-21 07:45:06.208209 libmata-0.84.0/mata/unit-test-data/nfa-a.vtf
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 07:45:06.176207 libmata-0.84.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-21 07:45:06.176207 libmata-0.84.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-07-24 11:04:57.673692 libmata-0.85.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/libmata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   526002 2023-07-24 11:01:11.259324 libmata-0.85.0/libmata/alphabets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/alphabets.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/alphabets.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/libmata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/nfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1690497 2023-07-24 11:01:12.211317 libmata-0.85.0/libmata/nfa/nfa.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/nfa/nfa.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    43671 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/nfa/nfa.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   434183 2023-07-24 11:01:12.867312 libmata-0.85.0/libmata/nfa/strings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/nfa/strings.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/nfa/strings.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   249291 2023-07-24 11:01:13.291309 libmata-0.85.0/libmata/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   696499 2023-07-24 11:01:13.931304 libmata-0.85.0/libmata/plotting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/plotting.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   458232 2023-07-24 11:01:14.191302 libmata-0.85.0/libmata/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-24 11:00:22.235678 libmata-0.85.0/libmata/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-07-24 11:00:22.187678 libmata-0.85.0/mata/3rdparty/args.hxx
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-24 11:00:22.195678 libmata-0.85.0/mata/3rdparty/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-07-24 11:00:22.191678 libmata-0.85.0/mata/3rdparty/catch.hpp.1.9.3
+-rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-07-24 11:00:22.195678 libmata-0.85.0/mata/3rdparty/catch.hpp.2.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-24 11:00:22.195678 libmata-0.85.0/mata/3rdparty/catch.hpp.2.13.9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.665692 libmata-0.85.0/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.665692 libmata-0.85.0/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-24 11:00:22.219678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.665692 libmata-0.85.0/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.665692 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-07-24 11:00:22.223678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/composeids.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-24 11:00:22.227678 libmata-0.85.0/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.665692 libmata-0.85.0/mata/3rdparty/cudd-min/
+-rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-07-24 11:00:22.195678 libmata-0.85.0/mata/3rdparty/cudd-min/bnet.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/bnet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/chkMterm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-24 11:00:22.199678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-24 11:00:22.203678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-24 11:00:22.207678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/dddmpUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/epdInt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/cudd-min/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/cudd-min/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.665692 libmata-0.85.0/mata/3rdparty/cudd-min/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/ntr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/ntr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/ntrBddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/ntrHeap.c
+-rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/ntrMflow.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/ntrShort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/ntrZddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/testdddmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-24 11:00:22.211678 libmata-0.85.0/mata/3rdparty/cudd-min/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd-min/testmtr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd-min/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd-min/testobj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd-min/testst.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd-min/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd-min/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-24 11:00:22.215678 libmata-0.85.0/mata/3rdparty/cudd-min/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-07-24 11:00:22.231678 libmata-0.85.0/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-24 11:00:22.235678 libmata-0.85.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-24 11:04:57.541693 libmata-0.85.0/mata/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101164 2023-07-24 11:04:57.541693 libmata-0.85.0/mata/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-24 11:04:57.541693 libmata-0.85.0/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-24 11:04:57.541693 libmata-0.85.0/mata/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-24 11:04:57.541693 libmata-0.85.0/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 11:04:57.541693 libmata-0.85.0/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.669692 libmata-0.85.0/mata/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cli/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cli/MATA-CLI-philosophy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cli/interpreter.cc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5882 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cli/mata
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cli/mata-code.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cli/version.cc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cmake/Modules/Catch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cmake/Modules/CatchAddTests.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cmake/Modules/CodeCoverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cmake/Modules/FindValgrind.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cmake/Modules/GetGitRevisionDescription.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 11:00:22.239678 libmata-0.85.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.657692 libmata-0.85.0/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/include/mata/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/afa/afa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/alphabet.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/include/mata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/nfa/algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/nfa/builder.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/nfa/delta.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/nfa/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/nfa/plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/nfa/strings.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/nfa/types.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/include/mata/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/parser/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/parser/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/parser/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/parser/re2parser.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/include/mata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/utils/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/utils/number-predicate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/utils/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/utils/sparse-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/utils/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/include/mata/utils/util.hh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-24 11:04:57.541693 libmata-0.85.0/mata/merge_static_libraries.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/src/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    38800 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/complement.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/delta.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30427 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32836 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/operations.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/nfa/universal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-24 11:00:22.243678 libmata-0.85.0/mata/src/strings/nfa-strings.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/tests/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    27575 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    42818 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/tests/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32066 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/nfa/nfa-concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/nfa/nfa-intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/nfa/nfa-profiling.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/nfa/nfa-util.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    83454 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/ord-vector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/re2parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/sparse-set.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/tests/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/strings/nfa-string-solving.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/tests/synchronized-iterator.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:04:57.673692 libmata-0.85.0/mata/unit-test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/unit-test-data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 11:00:22.259678 libmata-0.85.0/mata/unit-test-data/nfa-a.vtf
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 11:00:22.235678 libmata-0.85.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-24 11:00:22.235678 libmata-0.85.0/setup.py
```

### Comparing `libmata-0.84.0/PKG-INFO` & `libmata-0.85.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 0.84.0
+Version: 0.85.0
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
@@ -15,14 +15,15 @@
 [![GitHub tag](https://img.shields.io/github/tag/VeriFIT/mata.svg)](https://github.com/VeriFIT/mata)
 
 [![master: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
 [![master: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
 
 [![devel: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
 [![devel: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
+[![codecov](https://codecov.io/gh/VeriFIT/mata/branch/devel/graph/badge.svg?token=9VAVD19N4D)](https://codecov.io/gh/VeriFIT/mata)
 
 Mata is an open source automata library that offers interface for different kinds of automata (NFA,
 AFA, etc.). Currently, Mata offers two interfaces:
 
   1. An efficient library implemented in C/C++
   2. A flexible wrapper implemented in Python that uses the efficient library
```

### Comparing `libmata-0.84.0/libmata/alphabets.cpp` & `libmata-0.85.0/libmata/alphabets.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/alphabets.pxd` & `libmata-0.85.0/libmata/alphabets.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/alphabets.pyx` & `libmata-0.85.0/libmata/alphabets.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/nfa/nfa.cpp` & `libmata-0.85.0/libmata/nfa/nfa.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/nfa/nfa.pxd` & `libmata-0.85.0/libmata/nfa/nfa.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/nfa/nfa.pyx` & `libmata-0.85.0/libmata/nfa/nfa.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/nfa/strings.cpp` & `libmata-0.85.0/libmata/nfa/strings.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/nfa/strings.pxd` & `libmata-0.85.0/libmata/nfa/strings.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/nfa/strings.pyx` & `libmata-0.85.0/libmata/nfa/strings.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/parser.cpp` & `libmata-0.85.0/libmata/parser.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/parser.pyx` & `libmata-0.85.0/libmata/parser.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/plotting.cpp` & `libmata-0.85.0/libmata/plotting.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/plotting.pyx` & `libmata-0.85.0/libmata/plotting.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/utils.cpp` & `libmata-0.85.0/libmata/utils.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/utils.pxd` & `libmata-0.85.0/libmata/utils.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/libmata/utils.pyx` & `libmata-0.85.0/libmata/utils.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/args.hxx` & `libmata-0.85.0/mata/3rdparty/args.hxx`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/catch.hpp` & `libmata-0.85.0/mata/3rdparty/catch.hpp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/catch.hpp.1.9.3` & `libmata-0.85.0/mata/3rdparty/catch.hpp.1.9.3`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/catch.hpp.2.0.1` & `libmata-0.85.0/mata/3rdparty/catch.hpp.2.0.1`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/catch.hpp.2.13.9` & `libmata-0.85.0/mata/3rdparty/catch.hpp.2.13.9`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/CMakeLists.txt` & `libmata-0.85.0/mata/3rdparty/cudd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/Doxyfile.in` & `libmata-0.85.0/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/LICENSE` & `libmata-0.85.0/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/README` & `libmata-0.85.0/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-0.85.0/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-0.85.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-0.85.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-0.85.0/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-0.85.0/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-0.85.0/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-0.85.0/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-0.85.0/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-0.85.0/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-0.85.0/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/epd/epd.c` & `libmata-0.85.0/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/epd/epd.h` & `libmata-0.85.0/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-0.85.0/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/groups.dox` & `libmata-0.85.0/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-0.85.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-0.85.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-0.85.0/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-0.85.0/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-0.85.0/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-0.85.0/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-0.85.0/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-0.85.0/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/st/st.c` & `libmata-0.85.0/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/st/st.h` & `libmata-0.85.0/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/st/testst.c` & `libmata-0.85.0/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-0.85.0/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/datalimit.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/pipefork.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/prtime.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/strsav.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/texpand.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-0.85.0/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd/util/util.h` & `libmata-0.85.0/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/bnet.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/bnet.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/bnet.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/bnet.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/chkMterm.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/chkMterm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/config.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/config.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cpu_stats.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cpu_time.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cstringstream.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cstringstream.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cudd.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAPI.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddAbs.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddApply.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddFind.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddInv.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddIte.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddNeg.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAddWalsh.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAndAbs.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddAnneal.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddApa.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddApprox.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddBddAbs.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddBddCorr.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddBddIte.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddBridge.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddCache.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddCheck.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddClip.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddCof.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddCompose.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddDecomp.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddEssent.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddExact.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddExport.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddGenCof.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddGenetic.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddGroup.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddHarwell.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddInit.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddInt.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddInteract.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddLCache.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddLevelQ.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddLinear.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddLiteral.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddMatMult.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddObj.cc` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddObj.hh` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddPriority.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddRead.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddRef.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddReorder.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddSat.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddSign.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddSolve.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddSplit.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddSubsetHB.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddSubsetSP.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddSymmetry.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddTable.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddUtil.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddWindow.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddCount.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddFuncs.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddGroup.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddIsop.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddLin.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddMisc.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddPort.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddReord.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddSetop.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddSymm.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/cuddZddUtil.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/datalimit.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmp.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpBinary.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpConvert.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpDbg.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpInt.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpLoad.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/dddmpUtil.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/epd.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/epd.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/epdInt.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh` & `libmata-0.85.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/main.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/main.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/mtr.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/mtrBasic.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/mtrGroup.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/mtrInt.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ntr.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/ntr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ntr.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/ntr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ntrBddTest.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/ntrBddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ntrHeap.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/ntrHeap.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ntrMflow.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/ntrMflow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ntrShort.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/ntrShort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ntrZddTest.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/ntrZddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/pathsearch.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/pipefork.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/prtime.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/safe_mem.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/st.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/st.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/strsav.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/testcudd.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/testdddmp.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/testextra.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/testmtr.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/testmulti.cc` & `libmata-0.85.0/mata/3rdparty/cudd-min/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/testobj.cc` & `libmata-0.85.0/mata/3rdparty/cudd-min/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/testst.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/texpand.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/ucbqsort.c` & `libmata-0.85.0/mata/3rdparty/cudd-min/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/cudd-min/util.h` & `libmata-0.85.0/mata/3rdparty/cudd-min/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/CMakeLists.txt` & `libmata-0.85.0/mata/3rdparty/re2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-0.85.0/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/LICENSE` & `libmata-0.85.0/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/compile.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/parse.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/pod_array.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/prog.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/prog.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/re2.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/re2.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/regexp.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/regexp.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/simplify.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/tostring.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-0.85.0/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-0.85.0/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/util/logging.h` & `libmata-0.85.0/mata/3rdparty/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/util/mutex.h` & `libmata-0.85.0/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/util/rune.cc` & `libmata-0.85.0/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/util/strutil.cc` & `libmata-0.85.0/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/util/utf.h` & `libmata-0.85.0/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/re2/util/util.h` & `libmata-0.85.0/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-0.85.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-0.85.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/CMakeLists.txt` & `libmata-0.85.0/mata/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,24 @@
 option(WERROR "WERROR" OFF)
 message("-- Treating warnings as errors: ${WERROR}")
 if (WERROR)
     set(COMMON_WARNINGS "${COMMON_WARNINGS}" -Werror)
 endif ()
 
 ##############################################################################
+#                                COVERAGE
+##############################################################################
+
+# if DEBUG, also test coverage
+if(CMAKE_BUILD_TYPE MATCHES "Coverage")
+    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g -O0 -fprofile-arcs -ftest-coverage")
+    set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -lgcov")
+endif()
+
+##############################################################################
 #                                DEPENDENCIES
 ##############################################################################
 
 # find_package(Valgrind)
 
 # Doxygen - voluntary
 find_package(Doxygen)
```

### Comparing `libmata-0.84.0/mata/Doxyfile.in` & `libmata-0.85.0/mata/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/LICENSE` & `libmata-0.85.0/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/Makefile` & `libmata-0.85.0/mata/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 release:
 	mkdir -p $(BUILD_DIR) && cd $(BUILD_DIR) && cmake -DCMAKE_BUILD_TYPE=Release .. && $(MAKE) $(MAKE_FLAGS)
 
 release-werror:
 	mkdir -p $(BUILD_DIR) && cd $(BUILD_DIR) && cmake -DWERROR:BOOL=ON -DCMAKE_BUILD_TYPE=Release .. && $(MAKE) $(MAKE_FLAGS)
 
-coverage: clean
+coverage:
 	mkdir -p $(BUILD_DIR) && cd $(BUILD_DIR) && cmake -DCMAKE_BUILD_TYPE=Coverage .. && $(MAKE) $(MAKE_FLAGS)
 
 doc:
 	cd $(BUILD_DIR) && $(MAKE) $(MAKE_FLAGS) doc
 
 test:
 	cd $(BUILD_DIR) && ctest $(TEST_FLAGS)
```

### Comparing `libmata-0.84.0/mata/README.md` & `libmata-0.85.0/mata/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![GitHub tag](https://img.shields.io/github/tag/VeriFIT/mata.svg)](https://github.com/VeriFIT/mata)
 
 [![master: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
 [![master: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
 
 [![devel: Ubuntu (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/ubuntu.yml)
 [![devel: MacOS (build-&-test)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml/badge.svg?branch=devel)](https://github.com/VeriFIT/mata/actions/workflows/macos.yml)
+[![codecov](https://codecov.io/gh/VeriFIT/mata/branch/devel/graph/badge.svg?token=9VAVD19N4D)](https://codecov.io/gh/VeriFIT/mata)
 
 Mata is an open source automata library that offers interface for different kinds of automata (NFA,
 AFA, etc.). Currently, Mata offers two interfaces:
 
   1. An efficient library implemented in C/C++
   2. A flexible wrapper implemented in Python that uses the efficient library
```

### Comparing `libmata-0.84.0/mata/cli/CMakeLists.txt` & `libmata-0.85.0/mata/cli/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cli/MATA-CLI-philosophy.md` & `libmata-0.85.0/mata/cli/MATA-CLI-philosophy.md`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cli/mata` & `libmata-0.85.0/mata/cli/mata`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cli/mata-code.cc` & `libmata-0.85.0/mata/cli/mata-code.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cmake/Modules/Catch.cmake` & `libmata-0.85.0/mata/cmake/Modules/Catch.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cmake/Modules/CatchAddTests.cmake` & `libmata-0.85.0/mata/cmake/Modules/CatchAddTests.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cmake/Modules/CodeCoverage.cmake` & `libmata-0.85.0/mata/cmake/Modules/CodeCoverage.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cmake/Modules/FindValgrind.cmake` & `libmata-0.85.0/mata/cmake/Modules/FindValgrind.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cmake/Modules/GetGitRevisionDescription.cmake` & `libmata-0.85.0/mata/cmake/Modules/GetGitRevisionDescription.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in` & `libmata-0.85.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/afa/afa.hh` & `libmata-0.85.0/mata/include/mata/afa/afa.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/alphabet.hh` & `libmata-0.85.0/mata/include/mata/alphabet.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/nfa/algorithms.hh` & `libmata-0.85.0/mata/include/mata/nfa/algorithms.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/nfa/builder.hh` & `libmata-0.85.0/mata/include/mata/nfa/builder.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/nfa/delta.hh` & `libmata-0.85.0/mata/include/mata/nfa/delta.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/nfa/nfa.hh` & `libmata-0.85.0/mata/include/mata/nfa/nfa.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/nfa/plumbing.hh` & `libmata-0.85.0/mata/include/mata/nfa/plumbing.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/nfa/strings.hh` & `libmata-0.85.0/mata/include/mata/nfa/strings.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/nfa/types.hh` & `libmata-0.85.0/mata/include/mata/nfa/types.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/parser/inter-aut.hh` & `libmata-0.85.0/mata/include/mata/parser/inter-aut.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/parser/mintermization.hh` & `libmata-0.85.0/mata/include/mata/parser/mintermization.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/parser/parser.hh` & `libmata-0.85.0/mata/include/mata/parser/parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/parser/re2parser.hh` & `libmata-0.85.0/mata/include/mata/parser/re2parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/utils/closed-set.hh` & `libmata-0.85.0/mata/include/mata/utils/closed-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/utils/number-predicate.hh` & `libmata-0.85.0/mata/include/mata/utils/number-predicate.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/utils/ord-vector.hh` & `libmata-0.85.0/mata/include/mata/utils/ord-vector.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/utils/sparse-set.hh` & `libmata-0.85.0/mata/include/mata/utils/sparse-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/utils/synchronized-iterator.hh` & `libmata-0.85.0/mata/include/mata/utils/synchronized-iterator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/include/mata/utils/util.hh` & `libmata-0.85.0/mata/include/mata/utils/util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/CMakeLists.txt` & `libmata-0.85.0/mata/src/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 #set(CMAKE_VERBOSE_MAKEFILE ON)
 
 project(libmata)
 
 # Export compile commands to be used with YouCompleteMe
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
-# if DEBUG, also test coverage
-if(CMAKE_BUILD_TYPE MATCHES "Coverage")
-	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g -O0 -fprofile-arcs -ftest-coverage")
-endif()
-
 # uncomment for profiling
 #add_definitions(-pg)
 #set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -pg")
 
 include_directories(../include)
 include_directories(../3rdparty/) # this is here since it is clearer to include re2/utils than just utils
 include_directories(../3rdparty/cudd/include)
```

### Comparing `libmata-0.84.0/mata/src/afa/afa.cc` & `libmata-0.85.0/mata/src/afa/afa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/alphabet.cc` & `libmata-0.85.0/mata/src/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/inter-aut.cc` & `libmata-0.85.0/mata/src/inter-aut.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/mintermization.cc` & `libmata-0.85.0/mata/src/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/builder.cc` & `libmata-0.85.0/mata/src/nfa/builder.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/complement.cc` & `libmata-0.85.0/mata/src/nfa/complement.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/concatenation.cc` & `libmata-0.85.0/mata/src/nfa/concatenation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/delta.cc` & `libmata-0.85.0/mata/src/nfa/delta.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/inclusion.cc` & `libmata-0.85.0/mata/src/nfa/inclusion.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/intersection.cc` & `libmata-0.85.0/mata/src/nfa/intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/nfa.cc` & `libmata-0.85.0/mata/src/nfa/nfa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/operations.cc` & `libmata-0.85.0/mata/src/nfa/operations.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/nfa/universal.cc` & `libmata-0.85.0/mata/src/nfa/universal.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/parser.cc` & `libmata-0.85.0/mata/src/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/re2parser.cc` & `libmata-0.85.0/mata/src/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/strings/nfa-noodlification.cc` & `libmata-0.85.0/mata/src/strings/nfa-noodlification.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/strings/nfa-segmentation.cc` & `libmata-0.85.0/mata/src/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/src/strings/nfa-strings.cc` & `libmata-0.85.0/mata/src/strings/nfa-strings.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/CMakeLists.txt` & `libmata-0.85.0/mata/tests/CMakeLists.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 set(CMAKE_COLOR_MAKEFILE ON)
 #set(CMAKE_VERBOSE_MAKEFILE ON)
 
 # Export compile commands to be used with YouCompleteMe
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
-# if DEBUG, also test coverage
-if(CMAKE_BUILD_TYPE MATCHES "Coverage")
-	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g -O0 -fprofile-arcs -ftest-coverage")
-endif()
 
 # uncomment for profiling
 #add_definitions(-pg)
 #set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -pg")
 
 include_directories(../include)
 include_directories(../3rdparty/) # this is here since it is clearer to include re2/utils than just utils
```

### Comparing `libmata-0.84.0/mata/tests/afa/afa.cc` & `libmata-0.85.0/mata/tests/afa/afa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/alphabet.cc` & `libmata-0.85.0/mata/tests/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/main.cc` & `libmata-0.85.0/mata/tests/main.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/mintermization.cc` & `libmata-0.85.0/mata/tests/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/nfa/builder.cc` & `libmata-0.85.0/mata/tests/nfa/builder.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/nfa/nfa-concatenation.cc` & `libmata-0.85.0/mata/tests/nfa/nfa-concatenation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/nfa/nfa-intersection.cc` & `libmata-0.85.0/mata/tests/nfa/nfa-intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/nfa/nfa-profiling.cc` & `libmata-0.85.0/mata/tests/nfa/nfa-profiling.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/nfa/nfa-util.hh` & `libmata-0.85.0/mata/tests/nfa/nfa-util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/nfa/nfa.cc` & `libmata-0.85.0/mata/tests/nfa/nfa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/ord-vector.cc` & `libmata-0.85.0/mata/tests/ord-vector.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/parser.cc` & `libmata-0.85.0/mata/tests/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/re2parser.cc` & `libmata-0.85.0/mata/tests/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/sparse-set.cc` & `libmata-0.85.0/mata/tests/sparse-set.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/strings/nfa-noodlification.cc` & `libmata-0.85.0/mata/tests/strings/nfa-noodlification.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/strings/nfa-segmentation.cc` & `libmata-0.85.0/mata/tests/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/strings/nfa-string-solving.cc` & `libmata-0.85.0/mata/tests/strings/nfa-string-solving.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/mata/tests/synchronized-iterator.cc` & `libmata-0.85.0/mata/tests/synchronized-iterator.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.84.0/setup.py` & `libmata-0.85.0/setup.py`

 * *Files identical despite different names*

