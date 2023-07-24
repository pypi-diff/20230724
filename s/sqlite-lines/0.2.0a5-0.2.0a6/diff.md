# Comparing `tmp/sqlite_lines-0.2.0a5-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_lines-0.2.0a6-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9315 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15792 b- defN 23-Jun-10 22:11 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      531 b- defN 23-Jun-10 22:11 sqlite_lines/__init__.py
--rw-r--r--  2.0 unx    21784 b- defN 23-Jun-10 22:11 sqlite_lines/lines0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:11 sqlite_lines/version.py
--rw-r--r--  2.0 unx      506 b- defN 23-Jun-10 22:11 sqlite_lines-0.2.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-10 22:11 sqlite_lines-0.2.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-10 22:11 sqlite_lines-0.2.0a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      658 b- defN 23-Jun-10 22:11 sqlite_lines-0.2.0a5.dist-info/RECORD
-8 files, 39473 bytes uncompressed, 8163 bytes compressed:  79.3%
+Zip file size: 9316 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15792 b- defN 23-Jul-24 04:39 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      531 b- defN 23-Jul-24 04:39 sqlite_lines/__init__.py
+-rw-r--r--  2.0 unx    21784 b- defN 23-Jul-24 04:39 sqlite_lines/lines0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-24 04:39 sqlite_lines/version.py
+-rw-r--r--  2.0 unx      506 b- defN 23-Jul-24 04:39 sqlite_lines-0.2.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jul-24 04:39 sqlite_lines-0.2.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-24 04:39 sqlite_lines-0.2.0a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-Jul-24 04:39 sqlite_lines-0.2.0a6.dist-info/RECORD
+8 files, 39473 bytes uncompressed, 8164 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_lines/lines0.so
 Comment: 
 
 Filename: sqlite_lines/version.py
 Comment: 
 
-Filename: sqlite_lines-0.2.0a5.dist-info/METADATA
+Filename: sqlite_lines-0.2.0a6.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_lines-0.2.0a5.dist-info/WHEEL
+Filename: sqlite_lines-0.2.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_lines-0.2.0a5.dist-info/top_level.txt
+Filename: sqlite_lines-0.2.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_lines-0.2.0a5.dist-info/RECORD
+Filename: sqlite_lines-0.2.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## noop.cpython-311-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --dynamic {}

```diff
@@ -1,11 +1,11 @@
 
 Dynamic section at offset 0x2e80 contains 18 entries:
   Tag        Type                         Name/Value
- 0x000000000000001d (RUNPATH)            Library runpath: [/opt/hostedtoolcache/Python/3.11.3/x64/lib]
+ 0x000000000000001d (RUNPATH)            Library runpath: [/opt/hostedtoolcache/Python/3.11.4/x64/lib]
  0x000000000000000c (INIT)               0x1000
  0x000000000000000d (FINI)               0x10fc
  0x0000000000000019 (INIT_ARRAY)         0x3e70
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x3e78
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2b8
```

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 56a6043bb7afd603205202a2ea53db3b9d9940dc
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 81a591e1454ee6aefa5f9bfbf9a55ae25a237d0b
```

### strings --all --bytes=8 {}

```diff
@@ -1,12 +1,12 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
-/opt/hostedtoolcache/Python/3.11.3/x64/lib
+/opt/hostedtoolcache/Python/3.11.4/x64/lib
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
 /home/runner/work/sqlite-lines/sqlite-lines/python/sqlite_lines
 GNU C17 9.4.0 -mtune=generic -march=x86-64 -g -O3 -fwrapv -fPIC -fasynchronous-unwind-tables -fstack-protector-strong -fstack-clash-protection -fcf-protection
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8061
```

### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -3,9 +3,9 @@
   0x00000350 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
   0x00000360 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
   0x00000370 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
   0x00000380 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
   0x00000390 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
   0x000003a0 6c697a65 002f6f70 742f686f 73746564 lize./opt/hosted
   0x000003b0 746f6f6c 63616368 652f5079 74686f6e toolcache/Python
-  0x000003c0 2f332e31 312e332f 7836342f 6c696200 /3.11.3/x64/lib.
+  0x000003c0 2f332e31 312e342f 7836342f 6c696200 /3.11.4/x64/lib.
```

## sqlite_lines/lines0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: b6ad726eacd0c12d021b8ed5aee5f9149b58b8ee
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 6873637689ce4781b6ded095dcd601d6845a248d
```

### strings --all --bytes=8 {}

```diff
@@ -17,17 +17,17 @@
 unable to allocate memory for idxStr
 path argument is required
 Error reading document, size=%d: %s
 Delimiter must be 1 character long, got %d characters
 path is null
 Error reading %s: %s
 CREATE TABLE x(line text,path hidden, delimiter hidden)
-93097133c3fbd5653d63e1311e27573e19cd78d1
-2023-06-10T22:11:37Z+0000
-v0.2.0-alpha.5
+627f20380fe937f3382165f994aa344ed464a42f
+2023-07-24T04:39:12Z+0000
+v0.2.0-alpha.6
 Version: %s
 Date: %s
 Source: %s
 lines_version
 lines_debug
 lines_read
 Version: %s
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -21,20 +21,20 @@
   0x00003120 25642063 68617261 63746572 73000070 %d characters..p
   0x00003130 61746820 6973206e 756c6c00 4572726f ath is null.Erro
   0x00003140 72207265 6164696e 67202573 3a202573 r reading %s: %s
   0x00003150 00000000 00000000 43524541 54452054 ........CREATE T
   0x00003160 41424c45 2078286c 696e6520 74657874 ABLE x(line text
   0x00003170 2c706174 68206869 6464656e 2c206465 ,path hidden, de
   0x00003180 6c696d69 74657220 68696464 656e2900 limiter hidden).
-  0x00003190 39333039 37313333 63336662 64353635 93097133c3fbd565
-  0x000031a0 33643633 65313331 31653237 35373365 3d63e1311e27573e
-  0x000031b0 31396364 37386431 00323032 332d3036 19cd78d1.2023-06
-  0x000031c0 2d313054 32323a31 313a3337 5a2b3030 -10T22:11:37Z+00
+  0x00003190 36323766 32303338 30666539 33376633 627f20380fe937f3
+  0x000031a0 33383231 36356639 39346161 33343465 382165f994aa344e
+  0x000031b0 64343634 61343266 00323032 332d3037 d464a42f.2023-07
+  0x000031c0 2d323454 30343a33 393a3132 5a2b3030 -24T04:39:12Z+00
   0x000031d0 30300076 302e322e 302d616c 7068612e 00.v0.2.0-alpha.
-  0x000031e0 35000000 00000000 56657273 696f6e3a 5.......Version:
+  0x000031e0 36000000 00000000 56657273 696f6e3a 6.......Version:
   0x000031f0 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003200 7263653a 20257300 6c696e65 735f7665 rce: %s.lines_ve
   0x00003210 7273696f 6e006c69 6e65735f 64656275 rsion.lines_debu
   0x00003220 67006c69 6e657300 6c696e65 735f7265 g.lines.lines_re
   0x00003230 61640000 00000000 56657273 696f6e3a ad......Version:
   0x00003240 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003250 7263653a 2025730a 4e4f2046 494c4553 rce: %s.NO FILES
```

## sqlite_lines/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.5"
+__version__ = "0.2.0-alpha.6"
 __version_info__ = tuple(__version__.split("."))
```

