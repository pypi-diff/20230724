# Comparing `tmp/sqlite_url-0.1.0a7-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_url-0.1.0a8-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 238980 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15784 b- defN 23-Jun-10 22:14 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      302 b- defN 23-Jun-10 22:13 sqlite_url/__init__.py
--rw-r--r--  2.0 unx   514456 b- defN 23-Jun-10 22:14 sqlite_url/url0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:13 sqlite_url/version.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jun-10 22:14 sqlite_url-0.1.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-10 22:14 sqlite_url-0.1.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-10 22:14 sqlite_url-0.1.0a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-10 22:14 sqlite_url-0.1.0a7.dist-info/RECORD
-8 files, 531881 bytes uncompressed, 237860 bytes compressed:  55.3%
+Zip file size: 238976 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-Jul-24 04:30 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      302 b- defN 23-Jul-24 04:30 sqlite_url/__init__.py
+-rw-r--r--  2.0 unx   514456 b- defN 23-Jul-24 04:30 sqlite_url/url0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-24 04:30 sqlite_url/version.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jul-24 04:30 sqlite_url-0.1.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jul-24 04:30 sqlite_url-0.1.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-24 04:30 sqlite_url-0.1.0a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jul-24 04:30 sqlite_url-0.1.0a8.dist-info/RECORD
+8 files, 531881 bytes uncompressed, 237856 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_url/url0.so
 Comment: 
 
 Filename: sqlite_url/version.py
 Comment: 
 
-Filename: sqlite_url-0.1.0a7.dist-info/METADATA
+Filename: sqlite_url-0.1.0a8.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_url-0.1.0a7.dist-info/WHEEL
+Filename: sqlite_url-0.1.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_url-0.1.0a7.dist-info/top_level.txt
+Filename: sqlite_url-0.1.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_url-0.1.0a7.dist-info/RECORD
+Filename: sqlite_url-0.1.0a8.dist-info/RECORD
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
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 22abf3459c13b13cb4c502c2be97fd489e62d6b3
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 8d04a58d54b3101e9ec9f5971a50b86d73ea0c91
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
 /home/runner/work/sqlite-url/sqlite-url/python/sqlite_url
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

## sqlite_url/url0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 63a36a4b8c31f769fbed3d067909ee439772d906
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 711eb1b80e6690c88130c6e42501363342e77417
```

### strings --all --bytes=8 {}

```diff
@@ -478,17 +478,17 @@
 []A\A]A^A_
 A\A]A^A_
 A\A]A^A_
 AWAVAUATI
 []A\A]A^A_
 []A\A]A^A_
  ]A\A]A^A_
-v0.1.0-alpha.7
-9561f8c6c602cfb22d30377708d509865a24e65d
-2023-06-10T22:13:39Z+0000
+v0.1.0-alpha.8
+d2a04a2b6b250ef451e5b01b464bf9b224a42cb8
+2023-07-24T04:30:40Z+0000
 Version: %s
 Date: %s
 Source: %s
 libcurl: %s
 url() requires odd number of arguments
 Error initializating URL in the first argument
 Invalid 'host' value
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,14 +1,14 @@
 
 Hex dump of section '.rodata':
-  0x00059000 76302e31 2e302d61 6c706861 2e370000 v0.1.0-alpha.7..
-  0x00059010 39353631 66386336 63363032 63666232 9561f8c6c602cfb2
-  0x00059020 32643330 33373737 30386435 30393836 2d30377708d50986
-  0x00059030 35613234 65363564 00323032 332d3036 5a24e65d.2023-06
-  0x00059040 2d313054 32323a31 333a3339 5a2b3030 -10T22:13:39Z+00
+  0x00059000 76302e31 2e302d61 6c706861 2e380000 v0.1.0-alpha.8..
+  0x00059010 64326130 34613262 36623235 30656634 d2a04a2b6b250ef4
+  0x00059020 35316535 62303162 34363462 66396232 51e5b01b464bf9b2
+  0x00059030 32346134 32636238 00323032 332d3037 24a42cb8.2023-07
+  0x00059040 2d323454 30343a33 303a3430 5a2b3030 -24T04:30:40Z+00
   0x00059050 30300000 00000000 56657273 696f6e3a 00......Version:
   0x00059060 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00059070 7263653a 2025730a 6c696263 75726c3a rce: %s.libcurl:
   0x00059080 20257300 00000000 75726c28 29207265  %s.....url() re
   0x00059090 71756972 6573206f 6464206e 756d6265 quires odd numbe
   0x000590a0 72206f66 20617267 756d656e 74730000 r of arguments..
   0x000590b0 4572726f 7220696e 69746961 6c697a61 Error initializa
```

## sqlite_url/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.7"
+__version__ = "0.1.0-alpha.8"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_url-0.1.0a7.dist-info/RECORD` & `sqlite_url-0.1.0a8.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-noop.cpython-311-x86_64-linux-gnu.so,sha256=kAfc9eDElEqFC2BGRJUPi-X2s78FFdmb-Xv3x7jyOaU,15784
+noop.cpython-311-x86_64-linux-gnu.so,sha256=l3DZU-VvJtaYPXEV4B9nS_P_GR9hjcUpslW2cvNP-CI,15784
 sqlite_url/__init__.py,sha256=PdL2nBKNZstu0_AZr97lI-WiLmcfNt3Tf--ULY-ET0s,302
-sqlite_url/url0.so,sha256=QKJmwmd8oe0I_yuijnbXNM4gsDdyXSssk1QQfpCNiZw,514456
-sqlite_url/version.py,sha256=Mbkem2oiUxB1wrX_6_xh56UHlRqc8T9ExOLDZ5mi0qI,79
-sqlite_url-0.1.0a7.dist-info/METADATA,sha256=bIbgjhf1fBucNmShzD6VvCZ9mEchnJWzk2HeFgQnKwg,496
-sqlite_url-0.1.0a7.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_url-0.1.0a7.dist-info/top_level.txt,sha256=UugqZCwj0DKQ1KbtV1KaQH9BIWTZKYaMjlbkw5ecKS0,16
-sqlite_url-0.1.0a7.dist-info/RECORD,,
+sqlite_url/url0.so,sha256=JsMze28szFjXjC6Y0CRk96yWnkfZ7rHz-jr3MfVrkyc,514456
+sqlite_url/version.py,sha256=I0ZUcRKO4eykIcOSGighZnoI2j-WP8IxOzhHnNZBhaw,79
+sqlite_url-0.1.0a8.dist-info/METADATA,sha256=8yWJGx52B470pOJyICFiXuew8fpMciYDEX74-2n6U5c,496
+sqlite_url-0.1.0a8.dist-info/WHEEL,sha256=bc9AIvLXnt_uk1DFAs9A9G48iq3HERrVzvuB4WpotO8,105
+sqlite_url-0.1.0a8.dist-info/top_level.txt,sha256=UugqZCwj0DKQ1KbtV1KaQH9BIWTZKYaMjlbkw5ecKS0,16
+sqlite_url-0.1.0a8.dist-info/RECORD,,
```

