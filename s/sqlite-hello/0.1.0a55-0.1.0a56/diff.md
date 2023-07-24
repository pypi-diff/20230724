# Comparing `tmp/sqlite_hello-0.1.0a55-py3-none-win_amd64.whl.zip` & `tmp/sqlite_hello-0.1.0a56-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 33706 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-23 19:43 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-23 19:42 sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat    47925 b- defN 23-Jul-23 19:43 sqlite_hello/hello0.dll
--rw-rw-rw-  2.0 fat    47923 b- defN 23-Jul-23 19:43 sqlite_hello/hola0.dll
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-23 19:42 sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      521 b- defN 23-Jul-23 19:43 sqlite_hello-0.1.0a55.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jul-23 19:43 sqlite_hello-0.1.0a55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-23 19:43 sqlite_hello-0.1.0a55.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      727 b- defN 23-Jul-23 19:43 sqlite_hello-0.1.0a55.dist-info/RECORD
-9 files, 97614 bytes uncompressed, 32448 bytes compressed:  66.8%
+Zip file size: 33705 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-24 00:29 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-24 00:28 sqlite_hello/__init__.py
+-rw-rw-rw-  2.0 fat    47925 b- defN 23-Jul-24 00:29 sqlite_hello/hello0.dll
+-rw-rw-rw-  2.0 fat    47923 b- defN 23-Jul-24 00:29 sqlite_hello/hola0.dll
+-rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:28 sqlite_hello/version.py
+-rw-rw-rw-  2.0 fat      521 b- defN 23-Jul-24 00:29 sqlite_hello-0.1.0a56.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jul-24 00:29 sqlite_hello-0.1.0a56.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-24 00:29 sqlite_hello-0.1.0a56.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      727 b- defN 23-Jul-24 00:29 sqlite_hello-0.1.0a56.dist-info/RECORD
+9 files, 97614 bytes uncompressed, 32447 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_hello/hola0.dll
 Comment: 
 
 Filename: sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_hello-0.1.0a55.dist-info/METADATA
+Filename: sqlite_hello-0.1.0a56.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_hello-0.1.0a55.dist-info/WHEEL
+Filename: sqlite_hello-0.1.0a56.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_hello-0.1.0a55.dist-info/top_level.txt
+Filename: sqlite_hello-0.1.0a56.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_hello-0.1.0a55.dist-info/RECORD
+Filename: sqlite_hello-0.1.0a56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_hello/hello0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Sun Jul 23 19:42:36 2023
+Time/Date		Mon Jul 24 00:29:10 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
 SizeOfCode		0000000000001c00
 SizeOfInitializedData	0000000000003600
 SizeOfUninitializedData	0000000000000a00
 AddressOfEntryPoint	0000000000001330
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00014000
 SizeOfHeaders		00000600
-CheckSum		0001acdc
+CheckSum		00013431
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
@@ -112,15 +112,15 @@
  00009028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x6e408000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		64bd82ac
+Time/Date stamp 		64bdc5d6
 Major/Minor 			0/0
 Name 				0000000000008032 hello0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -3785,15 +3785,15 @@
     6e404004:	outsl  %ds:(%rsi),(%dx)
     6e404005:	sub    $0x20,%al
     6e404007:	and    $0x76002173,%eax
     6e40400c:	xor    %ch,(%rsi)
     6e40400e:	xor    %ebp,(%rsi)
     6e404010:	xor    %ch,0x68706c61(%rip)        # d6b0ac77 <.debug_str+0x686f7c77>
     6e404016:	(bad)
-    6e404017:	cs xor $0x65680035,%eax
+    6e404017:	cs xor $0x65680036,%eax
     6e40401d:	insb   (%dx),%es:(%rdi)
     6e40401e:	insb   (%dx),%es:(%rdi)
     6e40401f:	outsl  %ds:(%rsi),(%dx)
     6e404020:	add    %ch,0x65(%rax)
     6e404023:	insb   (%dx),%es:(%rdi)
     6e404024:	insb   (%dx),%es:(%rdi)
     6e404025:	outsl  %ds:(%rsi),(%dx)
@@ -4605,17 +4605,17 @@
 	...
 
 Disassembly of section .edata:
 
 000000006e408000 <.edata>:
     6e408000:	add    %al,(%rax)
     6e408002:	add    %al,(%rax)
-    6e408004:	lods   %ds:(%rsi),%al
-    6e408005:	(bad)
-    6e408006:	mov    $0x64,%ebp
+    6e408004:	(bad)
+    6e408005:	vpcmpgtb (%rax),%ymm8,%ymm0
+    6e408009:	add    %al,(%rax)
     6e40800b:	add    %dh,(%rdx)
     6e40800d:	addb   $0x0,(%rax)
     6e408010:	add    %eax,(%rax)
     6e408012:	add    %al,(%rax)
     6e408014:	add    %eax,(%rax)
     6e408016:	add    %al,(%rax)
     6e408018:	add    %eax,(%rax)
```

## sqlite_hello/hola0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Sun Jul 23 19:42:36 2023
+Time/Date		Mon Jul 24 00:29:10 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
 SizeOfCode		0000000000001c00
 SizeOfInitializedData	0000000000003600
 SizeOfUninitializedData	0000000000000a00
 AddressOfEntryPoint	0000000000001330
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00014000
 SizeOfHeaders		00000600
-CheckSum		00012252
+CheckSum		0001a8a7
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
@@ -112,15 +112,15 @@
  00009028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x68748000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		64bd82ac
+Time/Date stamp 		64bdc5d6
 Major/Minor 			0/0
 Name 				0000000000008032 hola0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -3785,15 +3785,15 @@
     68744005:	(bad)
     68744006:	sub    $0x20,%al
     68744008:	and    $0x76002173,%eax
     6874400d:	xor    %ch,(%rsi)
     6874400f:	xor    %ebp,(%rsi)
     68744011:	xor    %ch,0x68706c61(%rip)        # d0e4ac78 <.debug_str+0x686f7c78>
     68744017:	(bad)
-    68744018:	cs xor $0x6f680035,%eax
+    68744018:	cs xor $0x6f680036,%eax
     6874401e:	insb   (%dx),%es:(%rdi)
     6874401f:	(bad)
     68744020:	add    %ch,0x6f(%rax)
     68744023:	insb   (%dx),%es:(%rdi)
     68744024:	(bad)
     68744025:	pop    %rdi
     68744026:	jbe    6874408d <_tls_used+0x2d>
@@ -4596,17 +4596,17 @@
 	...
 
 Disassembly of section .edata:
 
 0000000068748000 <.edata>:
     68748000:	add    %al,(%rax)
     68748002:	add    %al,(%rax)
-    68748004:	lods   %ds:(%rsi),%al
-    68748005:	(bad)
-    68748006:	mov    $0x64,%ebp
+    68748004:	(bad)
+    68748005:	vpcmpgtb (%rax),%ymm8,%ymm0
+    68748009:	add    %al,(%rax)
     6874800b:	add    %dh,(%rdx)
     6874800d:	addb   $0x0,(%rax)
     68748010:	add    %eax,(%rax)
     68748012:	add    %al,(%rax)
     68748014:	add    %eax,(%rax)
     68748016:	add    %al,(%rax)
     68748018:	add    %eax,(%rax)
```

## sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.55"
+__version__ = "0.1.0-alpha.56"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_hello-0.1.0a55.dist-info/METADATA` & `sqlite_hello-0.1.0a56.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-hello
-Version: 0.1.0a55
+Version: 0.1.0a56
 Home-page: https://github.com/asg017/sqlite-hello
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Requires-Python: >=3.6
```

## Comparing `sqlite_hello-0.1.0a55.dist-info/RECORD` & `sqlite_hello-0.1.0a56.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 noop.cp311-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sqlite_hello/__init__.py,sha256=_SH5dbQOWvHZs14Mu6FCjaNhOleuM2Z9mTPoPkZaopE,316
-sqlite_hello/hello0.dll,sha256=SnWjmDKD1qMnY0st8Na54kpRJOF2ECzzsalR272QuVg,47925
-sqlite_hello/hola0.dll,sha256=Tcf4EcnKXetJczji0SpnldnUbdIKUaW9luvoYszxWtA,47923
-sqlite_hello/version.py,sha256=D1ohCmf7mGH5dOtHOjABGeSG_fY-JdpjpeCo734mcEw,82
-sqlite_hello-0.1.0a55.dist-info/METADATA,sha256=c08ZEJomtFw2R3oaobUSobVbMT4XQqMC1vfat138X7k,521
-sqlite_hello-0.1.0a55.dist-info/WHEEL,sha256=_7p9Q7gln4IKfQKAaNeimlWk5nRt3CeHwqN-V03Bs0E,102
-sqlite_hello-0.1.0a55.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
-sqlite_hello-0.1.0a55.dist-info/RECORD,,
+sqlite_hello/hello0.dll,sha256=fko-SOFiswblfU3cugyRqhbOrwuQXCi2Vif-1bZWmdg,47925
+sqlite_hello/hola0.dll,sha256=fJSRNkhhEdykTwM2O-2MMVz-rH8Aj6Q-ic7L9DfUEPg,47923
+sqlite_hello/version.py,sha256=Uwv8aq5HcgAJrdh8JNdLXTtBEkUC32FyRn3uwtczObQ,82
+sqlite_hello-0.1.0a56.dist-info/METADATA,sha256=c3hPYvwjUuWC4I7LD-2bTDIM6bhwXVj2hdCYeEzs80I,521
+sqlite_hello-0.1.0a56.dist-info/WHEEL,sha256=_7p9Q7gln4IKfQKAaNeimlWk5nRt3CeHwqN-V03Bs0E,102
+sqlite_hello-0.1.0a56.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
+sqlite_hello-0.1.0a56.dist-info/RECORD,,
```

