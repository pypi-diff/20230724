# Comparing `tmp/PyQt6_NetworkAuth_Qt6-6.5.1-py3-none-win_amd64.whl.zip` & `tmp/PyQt6_NetworkAuth_Qt6-6.5.2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 100124 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   198288 b- defN 23-May-21 07:14 PyQt6/Qt6/bin/Qt6NetworkAuth.dll
--rw-rw-rw-  2.0 fat    44738 b- defN 23-May-25 17:40 PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      597 b- defN 23-May-25 17:40 PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       95 b- defN 23-May-25 17:40 PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      446 b- defN 23-May-25 17:40 PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/RECORD
-5 files, 244164 bytes uncompressed, 99302 bytes compressed:  59.3%
+Zip file size: 100115 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   198288 b- defN 23-Jul-07 04:25 PyQt6/Qt6/bin/Qt6NetworkAuth.dll
+-rw-rw-rw-  2.0 fat    44738 b- defN 23-Jul-21 17:43 PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      597 b- defN 23-Jul-21 17:43 PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       95 b- defN 23-Jul-21 17:43 PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      446 b- defN 23-Jul-21 17:43 PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/RECORD
+5 files, 244164 bytes uncompressed, 99293 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: PyQt6/Qt6/bin/Qt6NetworkAuth.dll
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/LICENSE
+Filename: PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/METADATA
+Filename: PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/METADATA
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/WHEEL
+Filename: PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/RECORD
+Filename: PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PyQt6/Qt6/bin/Qt6NetworkAuth.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180019d40
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 21 06:13:57 2023
+Time/Date		Fri Jul  7 03:25:07 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000019a00
 SizeOfInitializedData	0000000000013800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000019d40
@@ -25,15 +25,15 @@
 MajorImageVersion	6
 MinorImageVersion	5
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00032000
 SizeOfHeaders		00000400
-CheckSum		00033195
+CheckSum		000365fd
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00004160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					GUARD_CF
 SizeOfStackReserve	0000000000100000
@@ -46,19 +46,19 @@
 The Data Directory
 Entry 0 0000000000022900 00004544 Export Directory [.edata (or where ever we found it)]
 Entry 1 0000000000026e44 000000c8 Import Directory [parts of .idata]
 Entry 2 0000000000030000 00000570 Resource Directory [.rsrc]
 Entry 3 000000000002e000 00001c14 Exception Directory [.pdata]
 Entry 4 000000000002d600 00003090 Security Directory
 Entry 5 0000000000031000 00000458 Base Relocation Directory [.reloc]
-Entry 6 000000000001f738 00000054 Debug Directory
+Entry 6 000000000001f748 00000054 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
 Entry 9 000000000001f900 00000028 Thread Storage Directory [.tls]
-Entry a 000000000001f790 00000138 Load Configuration Directory
+Entry a 000000000001f7a0 00000138 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
 Entry c 000000000001b000 00000a78 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
 There is an import table in .rdata at 0x180026e44
@@ -68,287 +68,287 @@
                  Table   Stamp     Chain    Name      Thunk
  00026e44	000276d0 00000000 00000000 00028550 0001b7c0
 
 	DLL Name: Qt6Network.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	28502	  739  ?header@QNetworkReply@@QEBA?AVQVariant@@W4KnownHeaders@QNetworkRequest@@@Z
 	284d0	  667  ?error@QNetworkReply@@QEBA?AW4NetworkError@1@XZ
-	2849e	 1561  ?staticMetaObject@QTcpServer@@2UQMetaObject@@B
-	28468	 1537  ?staticMetaObject@QAbstractSocket@@2UQMetaObject@@B
+	2849e	 1560  ?staticMetaObject@QTcpServer@@2UQMetaObject@@B
+	28468	 1536  ?staticMetaObject@QAbstractSocket@@2UQMetaObject@@B
 	28442	  970  ?newConnection@QTcpServer@@QEAAXXZ
-	28420	 1247  ?serverPort@QTcpServer@@QEBAGXZ
+	28420	 1246  ?serverPort@QTcpServer@@QEBAGXZ
 	283fc	  814  ?isListening@QTcpServer@@QEBA_NXZ
 	283de	  523  ?close@QTcpServer@@QEAAXXZ
 	283ac	  875  ?listen@QTcpServer@@QEAA_NAEBVQHostAddress@@G@Z
 	28392	  206  ??1QTcpServer@@UEAA@XZ
 	2836c	  137  ??0QTcpServer@@QEAA@PEAVQObject@@@Z
 	28350	  164  ??1QHostAddress@@QEAA@XZ
 	28322	   39  ??0QHostAddress@@QEAA@W4SpecialAddress@0@@Z
 	282f8	  632  ?disconnected@QAbstractSocket@@QEAAXXZ
-	282bc	 1547  ?staticMetaObject@QNetworkAccessManager@@2UQMetaObject@@B
-	28288	 1387  ?setPassword@QAuthenticator@@QEAAXAEBVQString@@@Z
-	28258	 1485  ?setUser@QAuthenticator@@QEAAXAEBVQString@@@Z
-	28232	 1699  ?url@QNetworkReply@@QEBA?AVQUrl@@XZ
+	282bc	 1546  ?staticMetaObject@QNetworkAccessManager@@2UQMetaObject@@B
+	28288	 1386  ?setPassword@QAuthenticator@@QEAAXAEBVQString@@@Z
+	28258	 1484  ?setUser@QAuthenticator@@QEAAXAEBVQString@@@Z
+	28232	 1698  ?url@QNetworkReply@@QEBA?AVQUrl@@XZ
 	281d2	  462  ?authenticationRequired@QNetworkAccessManager@@QEAAXPEAVQNetworkReply@@PEAVQAuthenticator@@@Z
 	281ac	  830  ?isNull@QSslConfiguration@@QEBA_NXZ
-	28164	 1464  ?setSslConfiguration@QNetworkRequest@@QEAAXAEBVQSslConfiguration@@@Z
-	28112	 1087  ?qRegisterNormalizedMetaType_QNetworkReply__NetworkError@@YAHAEBVQByteArray@@@Z
+	28164	 1463  ?setSslConfiguration@QNetworkRequest@@QEAAXAEBVQSslConfiguration@@@Z
+	28112	 1086  ?qRegisterNormalizedMetaType_QNetworkReply__NetworkError@@YAHAEBVQByteArray@@@Z
 	280d8	  672  ?errorOccurred@QNetworkReply@@QEAAXW4NetworkError@1@@Z
-	27988	 1335  ?setHeader@QNetworkRequest@@QEAAXW4KnownHeaders@1@AEBVQVariant@@@Z
+	27988	 1334  ?setHeader@QNetworkRequest@@QEAAXW4KnownHeaders@1@AEBVQVariant@@@Z
 	28098	  740  ?header@QNetworkRequest@@QEBA?AVQVariant@@W4KnownHeaders@1@@Z
-	28070	 1700  ?url@QNetworkRequest@@QEBA?AVQUrl@@XZ
+	28070	 1699  ?url@QNetworkRequest@@QEBA?AVQUrl@@XZ
 	28048	  100  ??0QNetworkRequest@@QEAA@AEBVQUrl@@@Z
 	279ce	   66  ??0QNetworkAccessManager@@QEAA@PEAVQObject@@@Z
 	27a00	  176  ??1QNetworkAccessManager@@UEAA@XZ
 	27a24	  555  ?createRequest@QNetworkAccessManager@@MEAAPEAVQNetworkReply@@W4Operation@1@AEBVQNetworkRequest@@PEAVQIODevice@@@Z
 	27a98	  929  ?metaObject@QNetworkAccessManager@@UEBAPEBUQMetaObject@@XZ
-	27ad6	 1114  ?qt_metacall@QNetworkAccessManager@@UEAAHW4Call@QMetaObject@@HPEAPEAX@Z
-	27b20	 1138  ?qt_metacast@QNetworkAccessManager@@UEAAPEAXPEBD@Z
-	27b56	 1589  ?supportedSchemes@QNetworkAccessManager@@UEBA?AV?$QList@VQString@@@@XZ
-	27ba0	 1557  ?staticMetaObject@QNetworkReply@@2UQMetaObject@@B
-	27bd4	 1542  ?staticMetaObject@QHttpMultiPart@@2UQMetaObject@@B
+	27ad6	 1113  ?qt_metacall@QNetworkAccessManager@@UEAAHW4Call@QMetaObject@@HPEAPEAX@Z
+	27b20	 1137  ?qt_metacast@QNetworkAccessManager@@UEAAPEAXPEBD@Z
+	27b56	 1588  ?supportedSchemes@QNetworkAccessManager@@UEBA?AV?$QList@VQString@@@@XZ
+	27ba0	 1556  ?staticMetaObject@QNetworkReply@@2UQMetaObject@@B
+	27bd4	 1541  ?staticMetaObject@QHttpMultiPart@@2UQMetaObject@@B
 	27c0a	  101  ??0QNetworkRequest@@QEAA@XZ
 	27c28	  192  ??1QNetworkRequest@@QEAA@XZ
-	27c46	 1483  ?setUrl@QNetworkRequest@@QEAAXAEBVQUrl@@@Z
-	27c74	 1428  ?setRawHeader@QNetworkRequest@@QEAAXAEBVQByteArray@@0@Z
+	27c46	 1482  ?setUrl@QNetworkRequest@@QEAAXAEBVQUrl@@@Z
+	27c74	 1427  ?setRawHeader@QNetworkRequest@@QEAAXAEBVQByteArray@@0@Z
 	27cae	  116  ??0QSslConfiguration@@QEAA@XZ
 	27cce	  115  ??0QSslConfiguration@@QEAA@AEBV0@@Z
 	27cf4	  197  ??1QSslConfiguration@@QEAA@XZ
 	27d14	  274  ??4QSslConfiguration@@QEAAAEAV0@AEBV0@@Z
 	27d40	  318  ??8QSslConfiguration@@QEBA_NAEBV0@@Z
 	27fc2	 1068  ?put@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@PEAVQHttpMultiPart@@@Z
-	27d68	 1093  ?qRegisterNormalizedMetaType_QSslConfiguration@@YAHAEBVQByteArray@@@Z
+	27d68	 1092  ?qRegisterNormalizedMetaType_QSslConfiguration@@YAHAEBVQByteArray@@@Z
 	27db0	  736  ?head@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@@Z
 	27dfe	  710  ?get@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@@Z
 	27e4c	 1029  ?post@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@AEBVQByteArray@@@Z
 	27eaa	 1067  ?put@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@AEBVQByteArray@@@Z
 	27f08	  617  ?deleteResource@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@@Z
 	27f60	 1030  ?post@QNetworkAccessManager@@QEAAPEAVQNetworkReply@@AEBVQNetworkRequest@@PEAVQHttpMultiPart@@@Z
 	28024	  693  ?finished@QNetworkReply@@QEAAXXZ
 
  00026e58	00027000 00000000 00000000 0002a9b6 0001b0f0
 
 	DLL Name: Qt6Core.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	2a988	 3305  ?errorString@QIODevice@@QEBA?AVQString@@XZ
-	2a95c	 5525  ?readAll@QIODevice@@QEAA?AVQByteArray@@XZ
-	2a92c	 4930  ?object@QJsonDocument@@QEBA?AVQJsonObject@@XZ
-	2a908	 4186  ?isObject@QJsonDocument@@QEBA_NXZ
-	2a8be	 3547  ?fromJson@QJsonDocument@@SA?AV1@AEBVQByteArray@@PEAUQJsonParseError@@@Z
-	2a89c	 4055  ?isEmpty@QJsonObject@@QEBA_NXZ
+	2a988	 3306  ?errorString@QIODevice@@QEBA?AVQString@@XZ
+	2a95c	 5526  ?readAll@QIODevice@@QEAA?AVQByteArray@@XZ
+	2a92c	 4931  ?object@QJsonDocument@@QEBA?AVQJsonObject@@XZ
+	2a908	 4187  ?isObject@QJsonDocument@@QEBA_NXZ
+	2a8be	 3548  ?fromJson@QJsonDocument@@SA?AV1@AEBVQByteArray@@PEAUQJsonParseError@@@Z
+	2a89c	 4056  ?isEmpty@QJsonObject@@QEBA_NXZ
 	2a856	 7151  ?toVariantMap@QJsonObject@@QEBA?AV?$QMap@VQString@@VQVariant@@@@XZ
 	2a83c	  813  ??1QJsonObject@@QEAA@XZ
-	2a81e	 4182  ?isNull@QVariant@@QEBA_NXZ
+	2a81e	 4183  ?isNull@QVariant@@QEBA_NXZ
 	2a7ee	 6626  ?staticMetaObject@QIODevice@@2UQMetaObject@@B
-	2a7c4	 3910  ?instance@QCoreApplication@@SAPEAV1@XZ
-	2a78e	 2094  ?applicationName@QCoreApplication@@SA?AVQString@@XZ
-	2a76e	 5561  ?readyRead@QIODevice@@QEAAXXZ
-	2a74a	 3647  ?getChar@QIODevice@@QEAA_NPEAD@Z
+	2a7c4	 3911  ?instance@QCoreApplication@@SAPEAV1@XZ
+	2a78e	 2095  ?applicationName@QCoreApplication@@SA?AVQString@@XZ
+	2a76e	 5562  ?readyRead@QIODevice@@QEAAXXZ
+	2a74a	 3648  ?getChar@QIODevice@@QEAA_NPEAD@Z
 	2a71c	 7506  ?write@QIODevice@@QEAA_JAEBVQByteArray@@@Z
 	2a6f6	 7199  ?tr@QObject@@SA?AVQString@@PEBD0H@Z
-	2a6a6	 5012  ?path@QUrl@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	2a68c	 4375  ?isValid@QUrl@@QEBA_NXZ
-	2a656	 6359  ?setUrl@QUrl@@QEAAXAEBVQString@@W4ParsingMode@1@@Z
+	2a6a6	 5013  ?path@QUrl@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
+	2a68c	 4376  ?isValid@QUrl@@QEBA_NXZ
+	2a656	 6360  ?setUrl@QUrl@@QEAAXAEBVQString@@W4ParsingMode@1@@Z
 	2a628	  528  ??0QString@@QEAA@_JW4Initialization@Qt@@@Z
-	2a608	 4920  ?number@QString@@SA?AV1@HH@Z
-	2a5ca	 6579  ?startsWith@QString@@QEBA_NVQChar@@W4CaseSensitivity@Qt@@@Z
-	2a5aa	 4712  ?mid@QString@@QEBA?AV1@_J0@Z
-	2a582	 2104  ?arg@QString@@QEBA?AV1@GHHVQChar@@@Z
+	2a608	 4921  ?number@QString@@SA?AV1@HH@Z
+	2a5ca	 6580  ?startsWith@QString@@QEBA_NVQChar@@W4CaseSensitivity@Qt@@@Z
+	2a5aa	 4713  ?mid@QString@@QEBA?AV1@_J0@Z
+	2a582	 2105  ?arg@QString@@QEBA?AV1@GHHVQChar@@@Z
 	28560	 6634  ?staticMetaObject@QObject@@2UQMetaObject@@B
-	2858e	 2570  ?compareMemory@QtPrivate@@YAHVQByteArrayView@@0@Z
+	2858e	 2571  ?compareMemory@QtPrivate@@YAHVQByteArrayView@@0@Z
 	285c2	   90  ??0QByteArray@@QEAA@XZ
 	285dc	   88  ??0QByteArray@@QEAA@AEBV0@@Z
 	285fc	  752  ??1QByteArray@@QEAA@XZ
 	28616	   86  ??0QByteArray@@QEAA@$$QEAV0@@Z
-	28638	 5760  ?reserve@QByteArray@@QEAAX_J@Z
-	2865a	 2970  ?data@QByteArray@@QEBAPEBDXZ
-	2867a	 2048  ?append@QByteArray@@QEAAAEAV1@PEBD@Z
-	286a2	 6436  ?size@QByteArray@@QEBA_JXZ
-	286c0	 4161  ?isNull@QByteArray@@QEBA_NXZ
+	28638	 5761  ?reserve@QByteArray@@QEAAX_J@Z
+	2865a	 2971  ?data@QByteArray@@QEBAPEBDXZ
+	2867a	 2049  ?append@QByteArray@@QEAAAEAV1@PEBD@Z
+	286a2	 6437  ?size@QByteArray@@QEBA_JXZ
+	286c0	 4162  ?isNull@QByteArray@@QEBA_NXZ
 	286e0	 1293  ??6@YAAEAVQDataStream@@AEAV0@AEBVQByteArray@@@Z
 	28712	 1176  ??5@YAAEAVQDataStream@@AEAV0@AEAVQByteArray@@@Z
-	28744	 2442  ?className@QMetaObject@@QEBAPEBDXZ
+	28744	 2443  ?className@QMetaObject@@QEBAPEBDXZ
 	2876a	 7196  ?tr@QMetaObject@@QEBA?AVQString@@PEBD0H@Z
-	28796	 1929  ?activate@QMetaObject@@SAXPEAVQObject@@PEBU1@HPEAPEAX@Z
-	287d0	 2577  ?compareStrings@QtPrivate@@YAHVQStringView@@0W4CaseSensitivity@Qt@@@Z
+	28796	 1930  ?activate@QMetaObject@@SAXPEAVQObject@@PEBU1@HPEAPEAX@Z
+	287d0	 2578  ?compareStrings@QtPrivate@@YAHVQStringView@@0W4CaseSensitivity@Qt@@@Z
 	28818	  526  ??0QString@@QEAA@XZ
 	2882e	  520  ??0QString@@QEAA@AEBV0@@Z
 	2884a	  866  ??1QString@@QEAA@XZ
 	28860	  519  ??0QString@@QEAA@$$QEAV0@@Z
 	2887e	 1120  ??4QString@@QEAAAEAV0@$$QEAV0@@Z
-	288a2	 2981  ?data@QString@@QEBAPEBVQChar@@XZ
-	288c6	 4178  ?isNull@QString@@QEBA_NXZ
+	288a2	 2982  ?data@QString@@QEBAPEBVQChar@@XZ
+	288c6	 4179  ?isNull@QString@@QEBA_NXZ
 	288e2	 1315  ??6@YAAEAVQDataStream@@AEAV0@AEBVQString@@@Z
 	28912	 1200  ??5@YAAEAVQDataStream@@AEAV0@AEAVQString@@@Z
 	28942	  598  ??0QUrl@@QEAA@XZ
 	28956	  596  ??0QUrl@@QEAA@AEBV0@@Z
 	28970	 1144  ??4QUrl@@QEAAAEAV0@$$QEAV0@@Z
 	28990	  888  ??1QUrl@@QEAA@XZ
 	289a4	 1593  ??MQUrl@@QEBA_NAEBV0@@Z
 	289be	 1427  ??8QUrl@@QEBA_NAEBV0@@Z
 	289d8	 1318  ??6@YAAEAVQDataStream@@AEAV0@AEBVQUrl@@@Z
 	28a04	 1204  ??5@YAAEAVQDataStream@@AEAV0@AEAVQUrl@@@Z
 	28a30	 1278  ??6@YA?AVQDebug@@V0@AEBVQUrl@@@Z
 	28a54	 6668  ?status@QDataStream@@QEBA?AW4Status@1@XZ
-	28a80	 6324  ?setStatus@QDataStream@@QEAAXW4Status@1@@Z
-	28aae	 5780  ?resetStatus@QDataStream@@QEAAXXZ
+	28a80	 6325  ?setStatus@QDataStream@@QEAAXW4Status@1@@Z
+	28aae	 5781  ?resetStatus@QDataStream@@QEAAXXZ
 	28ad2	 1217  ??5QDataStream@@QEAAAEAV0@AEAH@Z
 	28af6	 1335  ??6QDataStream@@QEAAAEAV0@H@Z
-	28b16	 4034  ?isDeviceTransactionStarted@QDataStream@@QEBA_NXZ
-	28b4a	 5595  ?registerNormalizedTypedef@QMetaType@@SAXAEBVQByteArray@@V1@@Z
-	28b8c	 3773  ?id@QMetaType@@QEBAHH@Z
-	28ba6	 3167  ?dynamicMetaObject@QObjectData@@QEBAPEAUQMetaObject@@XZ
-	28be0	 5391  ?qt_metacast@QObject@@UEAAPEAXPEBD@Z
-	28c08	 5338  ?qt_metacall@QObject@@UEAAHW4Call@QMetaObject@@HPEAPEAX@Z
+	28b16	 4035  ?isDeviceTransactionStarted@QDataStream@@QEBA_NXZ
+	28b4a	 5596  ?registerNormalizedTypedef@QMetaType@@SAXAEBVQByteArray@@V1@@Z
+	28b8c	 3774  ?id@QMetaType@@QEBAHH@Z
+	28ba6	 3168  ?dynamicMetaObject@QObjectData@@QEBAPEAUQMetaObject@@XZ
+	28be0	 5392  ?qt_metacast@QObject@@UEAAPEAXPEBD@Z
+	28c08	 5339  ?qt_metacall@QObject@@UEAAHW4Call@QMetaObject@@HPEAPEAX@Z
 	28c44	  205  ??0QDebug@@QEAA@$$QEAV0@@Z
 	28c62	  774  ??1QDebug@@QEAA@XZ
 	28c78	 1349  ??6QDebug@@QEAAAEAV0@D@Z
 	28c94	 1359  ??6QDebug@@QEAAAEAV0@PEBD@Z
 	28cb2	 1348  ??6QDebug@@QEAAAEAV0@AEBVQString@@@Z
 	28cda	 1347  ??6QDebug@@QEAAAEAV0@AEBVQByteArray@@@Z
 	28d04	  210  ??0QDebugStateSaver@@QEAA@AEAVQDebug@@@Z
 	28d30	  775  ??1QDebugStateSaver@@QEAA@XZ
-	28d50	 5297  ?qt_QMetaEnum_debugOperator@@YA?AVQDebug@@AEAV1@_JPEBUQMetaObject@@PEBD@Z
+	28d50	 5298  ?qt_QMetaEnum_debugOperator@@YA?AVQDebug@@AEAV1@_JPEBUQMetaObject@@PEBD@Z
 	28d9c	  662  ??0QVariant@@QEAA@XZ
 	28db4	  890  ??1QVariant@@QEAA@XZ
 	28dcc	  614  ??0QVariant@@QEAA@AEBV0@@Z
 	28dea	 1153  ??4QVariant@@QEAAAEAV0@AEBV0@@Z
-	28e0c	 5279  ?qdebugHelper@QVariant@@AEBA?AVQDebug@@V2@@Z
-	28e3c	 3282  ?equals@QVariant@@IEBA_NAEBV1@@Z
+	28e0c	 5280  ?qdebugHelper@QVariant@@AEBA?AVQDebug@@V2@@Z
+	28e3c	 3283  ?equals@QVariant@@IEBA_NAEBV1@@Z
 	28e60	 1206  ??5@YAAEAVQDataStream@@AEAV0@AEAVQVariant@@@Z
 	28e90	 1320  ??6@YAAEAVQDataStream@@AEAV0@AEBVQVariant@@@Z
-	28ec0	 3031  ?deallocate@QArrayData@@SAXPEAU1@_J1@Z
+	28ec0	 3032  ?deallocate@QArrayData@@SAXPEAU1@_J1@Z
 	28eea	  949  ??4QByteArray@@QEAAAEAV0@$$QEAV0@@Z
-	28f10	 2047  ?append@QByteArray@@QEAAAEAV1@D@Z
+	28f10	 2048  ?append@QByteArray@@QEAAAEAV1@D@Z
 	28f34	 1121  ??4QString@@QEAAAEAV0@AEBV0@@Z
 	28f56	 7134  ?toUtf8@QString@@QEHAA?AVQByteArray@@XZ
 	28f80	  518  ??0QString@@QEAA@$$QEAU?$QArrayDataPointer@_S@@@Z
 	28fb4	 1145  ??4QUrl@@QEAAAEAV0@AEBV0@@Z
-	28fd2	 6264  ?setQuery@QUrl@@QEAAXAEBVQUrlQuery@@@Z
+	28fd2	 6265  ?setQuery@QUrl@@QEAAXAEBVQUrlQuery@@@Z
 	28ffc	 1466  ??9QUrl@@QEBA_NAEBV0@@Z
 	29016	  831  ??1QObject@@UEAA@XZ
-	2902c	 4990  ?parent@QObject@@QEBAPEAV1@XZ
+	2902c	 4991  ?parent@QObject@@QEBAPEAV1@XZ
 	2904c	  412  ??0QObject@@IEAA@AEAVQObjectPrivate@@PEAV0@@Z
-	2907c	 3645  ?getAndRef@ExternalRefCountData@QtSharedPointer@@SAPEAU12@PEBVQObject@@@Z
+	2907c	 3646  ?getAndRef@ExternalRefCountData@QtSharedPointer@@SAPEAU12@PEBVQObject@@@Z
 	290c8	  618  ??0QVariant@@QEAA@AEBV?$QMap@VQString@@VQVariant@@@@@Z
 	29102	  639  ??0QVariant@@QEAA@AEBVQString@@@Z
 	29126	 7078  ?toString@QVariant@@QEBA?AVQString@@XZ
 	29150	  416  ??0QObjectPrivate@@QEAA@H@Z
 	2916e	  834  ??1QObjectPrivate@@UEAA@XZ
 	2918c	  366  ??0QLoggingCategory@@QEAA@PEBDW4QtMsgType@@@Z
 	291bc	  820  ??1QLoggingCategory@@QEAA@XZ
 	291dc	  772  ??1QDateTime@@QEAA@XZ
 	291f4	 6983  ?toMSecsSinceEpoch@QDateTime@@QEBA_JXZ
-	2921e	 2826  ?currentDateTime@QDateTime@@SA?AV1@XZ
+	2921e	 2827  ?currentDateTime@QDateTime@@SA?AV1@XZ
 	29246	  604  ??0QUrlQuery@@QEAA@XZ
 	2925e	  889  ??1QUrlQuery@@QEAA@XZ
 	29276	 7076  ?toString@QUrlQuery@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	292ce	 1989  ?addQueryItem@QUrlQuery@@QEAAXAEBVQString@@0@Z
+	292ce	 1990  ?addQueryItem@QUrlQuery@@QEAAXAEBVQString@@0@Z
 	29300	  812  ??1QJsonDocument@@QEAA@XZ
-	2931c	 3623  ?fromVariant@QJsonDocument@@SA?AV1@AEBVQVariant@@@Z
+	2931c	 3624  ?fromVariant@QJsonDocument@@SA?AV1@AEBVQVariant@@@Z
 	29352	 6935  ?toJson@QJsonDocument@@QEBA?AVQByteArray@@W4JsonFormat@1@@Z
-	29390	 2424  ?childEvent@QObject@@MEAAXPEAVQChildEvent@@@Z
-	293c0	 2615  ?connectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
-	293f4	 2856  ?customEvent@QObject@@MEAAXPEAVQEvent@@@Z
-	29420	 3125  ?disconnectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
-	29456	 3327  ?event@QObject@@UEAA_NPEAVQEvent@@@Z
-	2947e	 3343  ?eventFilter@QObject@@UEAA_NPEAV1@PEAVQEvent@@@Z
-	294b2	 3511  ?flagsForDumping@QObjectPrivate@@UEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
+	29390	 2425  ?childEvent@QObject@@MEAAXPEAVQChildEvent@@@Z
+	293c0	 2616  ?connectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
+	293f4	 2857  ?customEvent@QObject@@MEAAXPEAVQEvent@@@Z
+	29420	 3126  ?disconnectNotify@QObject@@MEAAXAEBVQMetaMethod@@@Z
+	29456	 3328  ?event@QObject@@UEAA_NPEAVQEvent@@@Z
+	2947e	 3344  ?eventFilter@QObject@@UEAA_NPEAV1@PEAVQEvent@@@Z
+	294b2	 3512  ?flagsForDumping@QObjectPrivate@@UEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
 	2951c	 6820  ?timerEvent@QObject@@MEAAXPEAVQTimerEvent@@@Z
 	2954c	  368  ??0QMessageLogger@@QEAA@PEBDH00@Z
 	29570	 7479  ?warning@QMessageLogger@@QEBAXPEBDZZ
-	29598	 4499  ?lengthHelperCharArray@QByteArrayView@@CA_JPEBD_K@Z
+	29598	 4500  ?lengthHelperCharArray@QByteArrayView@@CA_JPEBD_K@Z
 	295ce	   89  ??0QByteArray@@QEAA@PEBD_J@Z
-	295ee	 2101  ?arg@QString@@QEBA?AV1@AEBV1@HVQChar@@@Z
+	295ee	 2102  ?arg@QString@@QEBA?AV1@AEBV1@HVQChar@@@Z
 	2961a	 7133  ?toUtf8@QString@@QEGBA?AVQByteArray@@XZ
-	29644	 3621  ?fromUtf8@QString@@SA?AV1@VQByteArrayView@@@Z
-	29674	 4890  ?normalizedType@QMetaObject@@SA?AVQByteArray@@PEBD@Z
+	29644	 3622  ?fromUtf8@QString@@SA?AV1@VQByteArrayView@@@Z
+	29674	 4891  ?normalizedType@QMetaObject@@SA?AVQByteArray@@PEBD@Z
 	296ac	  725  ??1Connection@QMetaObject@@QEAA@XZ
-	296d2	 2611  ?connectImpl@QObject@@CA?AVConnection@QMetaObject@@PEBV1@PEAPEAX01PEAVQSlotObjectBase@QtPrivate@@W4ConnectionType@Qt@@PEBHPEBU3@@Z
+	296d2	 2612  ?connectImpl@QObject@@CA?AVConnection@QMetaObject@@PEBV1@PEAPEAX01PEAVQSlotObjectBase@QtPrivate@@W4ConnectionType@Qt@@PEBHPEBU3@@Z
 	29758	  199  ??0QDateTime@@QEAA@XZ
 	29770	  195  ??0QDateTime@@QEAA@AEBV0@@Z
 	2978e	  194  ??0QDateTime@@QEAA@$$QEAV0@@Z
 	297ae	  981  ??4QDateTime@@QEAAAEAV0@$$QEAV0@@Z
-	297d4	 3278  ?equals@QDateTime@@AEBA_NAEBV1@@Z
-	297f8	 5064  ?precedes@QDateTime@@AEBA_NAEBV1@@Z
+	297d4	 3279  ?equals@QDateTime@@AEBA_NAEBV1@@Z
+	297f8	 5065  ?precedes@QDateTime@@AEBA_NAEBV1@@Z
 	2981e	 1297  ??6@YAAEAVQDataStream@@AEAV0@AEBVQDateTime@@@Z
 	29850	 1182  ??5@YAAEAVQDataStream@@AEAV0@AEAVQDateTime@@@Z
 	29882	 1249  ??6@YA?AVQDebug@@V0@AEBVQDateTime@@@Z
-	298aa	 5486  ?query@QUrl@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	298fa	 4386  ?isWarningEnabled@QLoggingCategory@@QEBA_NXZ
+	298aa	 5487  ?query@QUrl@@QEBA?AVQString@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
+	298fa	 4387  ?isWarningEnabled@QLoggingCategory@@QEBA_NXZ
 	2992a	  601  ??0QUrlQuery@@QEAA@AEBVQString@@@Z
 	29950	  413  ??0QObject@@QEAA@PEAV0@@Z
 	2996c	  369  ??0QMessageLogger@@QEAA@PEBDH0@Z
-	29990	 3389  ?fatal@QMessageLogger@@QEBAXPEBDZZ
-	299b6	 2030  ?allocate@QArrayData@@SAPEAXPEAPEAU1@_J11W4AllocationOption@1@@Z
-	299fa	 5572  ?reallocateUnaligned@QArrayData@@SA?AU?$pair@PEAUQArrayData@@PEAX@std@@PEAU1@PEAX_J2W4AllocationOption@1@@Z
-	29a68	 2630  ?constData@QByteArray@@QEBAPEBDXZ
+	29990	 3390  ?fatal@QMessageLogger@@QEBAXPEBDZZ
+	299b6	 2031  ?allocate@QArrayData@@SAPEAXPEAPEAU1@_J11W4AllocationOption@1@@Z
+	299fa	 5573  ?reallocateUnaligned@QArrayData@@SA?AU?$pair@PEAUQArrayData@@PEAX@std@@PEAU1@PEAX_J2W4AllocationOption@1@@Z
+	29a68	 2631  ?constData@QByteArray@@QEBAPEBDXZ
 	29a8c	 6840  ?toBase64@QByteArray@@QEBA?AV1@V?$QFlags@W4Base64Option@QByteArray@@@@@Z
-	29ad8	 2382  ?cast@QMetaObject@@QEBAPEBVQObject@@PEBV2@@Z
+	29ad8	 2383  ?cast@QMetaObject@@QEBAPEBVQObject@@PEBV2@@Z
 	29b08	   29  ??0Connection@QMetaObject@@QEAA@XZ
 	29b2e	  925  ??4Connection@QMetaObject@@QEAAAEAV01@$$QEAV01@@Z
 	29b62	  158  ??0QChar@@QEAA@UQLatin1Char@@@Z
-	29b84	 5788  ?resize@QString@@QEAAX_J@Z
-	29ba2	 2359  ?capacity@QString@@QEBA_JXZ
-	29bc0	 5762  ?reserve@QString@@QEAAX_J@Z
-	29bde	 2980  ?data@QString@@QEAAPEAVQChar@@XZ
-	29c02	 2633  ?constData@QString@@QEBAPEBVQChar@@XZ
-	29c2a	 3088  ?detach@QString@@QEAAXXZ
-	29c46	 2461  ?clear@QString@@QEAAXXZ
-	29c60	 6578  ?startsWith@QString@@QEBA_NAEBV1@W4CaseSensitivity@Qt@@@Z
-	29c9c	 2081  ?append@QString@@QEAAAEAV1@VQLatin1String@@@Z
+	29b84	 5789  ?resize@QString@@QEAAX_J@Z
+	29ba2	 2360  ?capacity@QString@@QEBA_JXZ
+	29bc0	 5763  ?reserve@QString@@QEAAX_J@Z
+	29bde	 2981  ?data@QString@@QEAAPEAVQChar@@XZ
+	29c02	 2634  ?constData@QString@@QEBAPEBVQChar@@XZ
+	29c2a	 3089  ?detach@QString@@QEAAXXZ
+	29c46	 2462  ?clear@QString@@QEAAXXZ
+	29c60	 6579  ?startsWith@QString@@QEBA_NAEBV1@W4CaseSensitivity@Qt@@@Z
+	29c9c	 2082  ?append@QString@@QEAAAEAV1@VQLatin1String@@@Z
 	29ccc	 6955  ?toLocal8Bit@QString@@QEGBA?AVQByteArray@@XZ
-	29cfc	 4925  ?number@QString@@SA?AV1@_JH@Z
-	29d1c	 2087  ?appendLatin1To@QAbstractConcatenable@@KAXVQLatin1String@@PEAVQChar@@@Z
-	29d66	 4064  ?isEmpty@QUrl@@QEBA_NXZ
+	29cfc	 4926  ?number@QString@@SA?AV1@_JH@Z
+	29d1c	 2088  ?appendLatin1To@QAbstractConcatenable@@KAXVQLatin1String@@PEAVQChar@@@Z
+	29d66	 4065  ?isEmpty@QUrl@@QEBA_NXZ
 	29d80	 7000  ?toPercentEncoding@QUrl@@SA?AVQByteArray@@AEBVQString@@AEBV2@1@Z
-	29dc4	 3117  ?disconnect@QObject@@SA_NAEBVConnection@QMetaObject@@@Z
-	29dfe	 3062  ?deleteLater@QObject@@QEAAXXZ
+	29dc4	 3118  ?disconnect@QObject@@SA_NAEBVConnection@QMetaObject@@@Z
+	29dfe	 3063  ?deleteLater@QObject@@QEAAXXZ
 	29e1e	  665  ??0QVariant@@QEAA@_N@Z
 	29e38	  620  ??0QVariant@@QEAA@AEBVQByteArray@@@Z
 	29e60	  613  ??0QVariant@@QEAA@$$QEAV0@@Z
 	29e80	 6847  ?toBool@QVariant@@QEBA_NXZ
 	29e9e	 6852  ?toByteArray@QVariant@@QEBA?AVQByteArray@@XZ
 	29ece	 7015  ?toSecsSinceEpoch@QDateTime@@QEBA_JXZ
-	29ef6	 2827  ?currentDateTimeUtc@QDateTime@@SA?AV1@XZ
-	29f22	 3640  ?get@QObjectPrivate@@SAPEAV1@PEAVQObject@@@Z
-	29f52	 5489  ?queryItems@QUrlQuery@@QEBA?AV?$QList@U?$pair@VQString@@V1@@std@@@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
-	29fc8	 2813  ?critical@QMessageLogger@@QEBAXPEBDZZ
+	29ef6	 2828  ?currentDateTimeUtc@QDateTime@@SA?AV1@XZ
+	29f22	 3641  ?get@QObjectPrivate@@SAPEAV1@PEAVQObject@@@Z
+	29f52	 5490  ?queryItems@QUrlQuery@@QEBA?AV?$QList@U?$pair@VQString@@V1@@std@@@@V?$QFlags@W4ComponentFormattingOption@QUrl@@@@@Z
+	29fc8	 2814  ?critical@QMessageLogger@@QEBAXPEBDZZ
 	29ff0	   92  ??0QByteArray@@QEAA@_JW4Initialization@Qt@@@Z
 	2a020	  950  ??4QByteArray@@QEAAAEAV0@AEBV0@@Z
-	2a044	 4047  ?isEmpty@QByteArray@@QEBA_NXZ
-	2a064	 5783  ?resize@QByteArray@@QEAAX_J@Z
-	2a084	 2358  ?capacity@QByteArray@@QEBA_JXZ
-	2a0a6	 2969  ?data@QByteArray@@QEAAPEADXZ
-	2a0c6	 3079  ?detach@QByteArray@@QEAAXXZ
-	2a0e4	 2046  ?append@QByteArray@@QEAAAEAV1@AEBV1@@Z
-	2a10e	 3196  ?end@QByteArray@@QEBAPEBDXZ
-	2a12c	 5742  ?replace@QString@@QEAAAEAV1@VQChar@@0W4CaseSensitivity@Qt@@@Z
-	2a16c	 3556  ?fromLatin1@QString@@SA?AV1@VQByteArrayView@@@Z
+	2a044	 4048  ?isEmpty@QByteArray@@QEBA_NXZ
+	2a064	 5784  ?resize@QByteArray@@QEAAX_J@Z
+	2a084	 2359  ?capacity@QByteArray@@QEBA_JXZ
+	2a0a6	 2970  ?data@QByteArray@@QEAAPEADXZ
+	2a0c6	 3080  ?detach@QByteArray@@QEAAXXZ
+	2a0e4	 2047  ?append@QByteArray@@QEAAAEAV1@AEBV1@@Z
+	2a10e	 3197  ?end@QByteArray@@QEBAPEBDXZ
+	2a12c	 5743  ?replace@QString@@QEAAAEAV1@VQChar@@0W4CaseSensitivity@Qt@@@Z
+	2a16c	 3557  ?fromLatin1@QString@@SA?AV1@VQByteArrayView@@@Z
 	2a19e	 7075  ?toString@QUrl@@QEBA?AVQString@@V?$QUrlTwoFlags@W4UrlFormattingOption@QUrl@@W4ComponentFormattingOption@2@@@@Z
-	2a210	 4009  ?isCriticalEnabled@QLoggingCategory@@QEBA_NXZ
-	2a240	 3745  ?hash@QMessageAuthenticationCode@@SA?AVQByteArray@@AEBV2@0W4Algorithm@QCryptographicHash@@@Z
-	2a2a0	 3037  ?debug@QMessageLogger@@QEBAXPEBDZZ
+	2a210	 4010  ?isCriticalEnabled@QLoggingCategory@@QEBA_NXZ
+	2a240	 3746  ?hash@QMessageAuthenticationCode@@SA?AVQByteArray@@AEBV2@0W4Algorithm@QCryptographicHash@@@Z
+	2a2a0	 3038  ?debug@QMessageLogger@@QEBAXPEBDZZ
 	2a2c6	 6956  ?toLocal8Bit@QString@@QEHAA?AVQByteArray@@XZ
-	2a2f6	 4376  ?isValid@QVariant@@QEBA_NXZ
+	2a2f6	 4377  ?isValid@QVariant@@QEBA_NXZ
 	2a314	 6927  ?toInt@QVariant@@QEBAHPEA_N@Z
-	2a334	 1994  ?addSecs@QDateTime@@QEBA?AV1@_J@Z
-	2a358	 5902  ?secsTo@QDateTime@@QEBA_JAEBV1@@Z
+	2a334	 1995  ?addSecs@QDateTime@@QEBA?AV1@_J@Z
+	2a358	 5903  ?secsTo@QDateTime@@QEBA_JAEBV1@@Z
 	2a37c	  597  ??0QUrl@@QEAA@AEBVQString@@W4ParsingMode@0@@Z
-	2a3ac	 4018  ?isDebugEnabled@QLoggingCategory@@QEBA_NXZ
+	2a3ac	 4019  ?isDebugEnabled@QLoggingCategory@@QEBA_NXZ
 	2a3da	 1147  ??4QUrlQuery@@QEAAAEAV0@$$QEAV0@@Z
-	2a400	 2450  ?clear@QByteArray@@QEAAXXZ
-	2a41e	 2128  ?at@QByteArray@@QEBAD_J@Z
-	2a43a	 3802  ?indexOf@QByteArray@@QEBA_JD_J@Z
-	2a45e	 4709  ?mid@QByteArray@@QEBA?AV1@_J0@Z
-	2a480	 6575  ?startsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
-	2a4b4	 3232  ?endsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
-	2a4e6	 2429  ?chop@QByteArray@@QEAAX_J@Z
+	2a400	 2451  ?clear@QByteArray@@QEAAXXZ
+	2a41e	 2129  ?at@QByteArray@@QEBAD_J@Z
+	2a43a	 3803  ?indexOf@QByteArray@@QEBA_JD_J@Z
+	2a45e	 4710  ?mid@QByteArray@@QEBA?AV1@_J0@Z
+	2a480	 6576  ?startsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
+	2a4b4	 3233  ?endsWith@QByteArray@@QEBA_NVQByteArrayView@@@Z
+	2a4e6	 2430  ?chop@QByteArray@@QEAAX_J@Z
 	2a504	 7253  ?trimmed@QByteArray@@QEHAA?AV1@XZ
-	2a528	 4918  ?number@QByteArray@@SA?AV1@_JH@Z
+	2a528	 4919  ?number@QByteArray@@SA?AV1@_JH@Z
 	2a54c	   85  ??0QByteArray@@QEAA@$$QEAU?$QArrayDataPointer@D@@@Z
 
  00026e6c	00026fe8 00000000 00000000 0002aa06 0001b0d8
 
 	DLL Name: MSVCP140.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	2a9e4	  652  ?_Xbad_function_call@std@@YAXXZ
@@ -485,21 +485,21 @@
 	[  25] +base[  26] 33a0 Export RVA
 	[  26] +base[  27] e6b0 Export RVA
 	[  27] +base[  28] 11660 Export RVA
 	[  28] +base[  29] 15490 Export RVA
 	[  29] +base[  30] 4740 Export RVA
 	[  30] +base[  31] e6c0 Export RVA
 	[  31] +base[  32] e700 Export RVA
-	[  32] +base[  33] 1e4a0 Export RVA
+	[  32] +base[  33] 1e4a8 Export RVA
 	[  33] +base[  34] 1d6a0 Export RVA
-	[  34] +base[  35] 1e638 Export RVA
-	[  35] +base[  36] 1e850 Export RVA
-	[  36] +base[  37] 1ee78 Export RVA
-	[  37] +base[  38] 1f1e8 Export RVA
-	[  38] +base[  39] 1f4e8 Export RVA
+	[  34] +base[  35] 1e648 Export RVA
+	[  35] +base[  36] 1e860 Export RVA
+	[  36] +base[  37] 1ee88 Export RVA
+	[  37] +base[  38] 1f1f8 Export RVA
+	[  38] +base[  39] 1f4f8 Export RVA
 	[  39] +base[  40] 6c50 Export RVA
 	[  40] +base[  41] 37e0 Export RVA
 	[  41] +base[  42] 37f0 Export RVA
 	[  42] +base[  43] 9530 Export RVA
 	[  43] +base[  44] 117c0 Export RVA
 	[  44] +base[  45] 95d0 Export RVA
 	[  45] +base[  46] 4b30 Export RVA
@@ -605,15 +605,15 @@
 	[ 145] +base[ 146] 135c0 Export RVA
 	[ 146] +base[ 147] 17370 Export RVA
 	[ 147] +base[ 148] 191d0 Export RVA
 	[ 148] +base[ 149] 5c50 Export RVA
 	[ 149] +base[ 150] 22e0 Export RVA
 	[ 150] +base[ 151] 1e00 Export RVA
 	[ 151] +base[ 152] 2940 Export RVA
-	[ 152] +base[ 153] 10f20 Export RVA
+	[ 152] +base[ 153] 10f60 Export RVA
 	[ 153] +base[ 154] 14ac0 Export RVA
 	[ 154] +base[ 155] 14ac0 Export RVA
 	[ 155] +base[ 156] 13610 Export RVA
 	[ 156] +base[ 157] 7d70 Export RVA
 	[ 157] +base[ 158] 7da0 Export RVA
 	[ 158] +base[ 159] 4230 Export RVA
 	[ 159] +base[ 160] 4260 Export RVA
@@ -666,21 +666,21 @@
 	[ 206] +base[ 207] da30 Export RVA
 	[ 207] +base[ 208] dda0 Export RVA
 	[ 208] +base[ 209] 42d0 Export RVA
 	[ 209] +base[ 210] 8220 Export RVA
 	[ 210] +base[ 211] 8280 Export RVA
 	[ 211] +base[ 212] 82b0 Export RVA
 	[ 212] +base[ 213] 82e0 Export RVA
-	[ 213] +base[ 214] 1da70 Export RVA
+	[ 213] +base[ 214] 1e170 Export RVA
 	[ 214] +base[ 215] 1c6f0 Export RVA
 	[ 215] +base[ 216] 1c420 Export RVA
 	[ 216] +base[ 217] 1d240 Export RVA
-	[ 217] +base[ 218] 1ee30 Export RVA
-	[ 218] +base[ 219] 1f1a0 Export RVA
-	[ 219] +base[ 220] 1f420 Export RVA
+	[ 217] +base[ 218] 1ee40 Export RVA
+	[ 218] +base[ 219] 1f1b0 Export RVA
+	[ 219] +base[ 220] 1f430 Export RVA
 	[ 220] +base[ 221] 5a90 Export RVA
 	[ 221] +base[ 222] 4310 Export RVA
 	[ 222] +base[ 223] 108d0 Export RVA
 	[ 223] +base[ 224] 108e0 Export RVA
 	[ 224] +base[ 225] deb0 Export RVA
 	[ 225] +base[ 226] 4350 Export RVA
 	[ 226] +base[ 227] 5aa0 Export RVA
@@ -1346,18 +1346,18 @@
  000000018002f23c:	0000000180010ba0 0000000180010c65 0000000180021bd4
  000000018002f248:	0000000180010c65 0000000180010ccd 0000000180021bec
  000000018002f254:	0000000180010ccd 0000000180010e1b 0000000180021c00
  000000018002f260:	0000000180010e20 0000000180010e42 0000000180020b10
  000000018002f26c:	0000000180010e50 0000000180010e82 0000000180021afc
  000000018002f278:	0000000180010e82 0000000180010ebe 0000000180021b14
  000000018002f284:	0000000180010ebe 0000000180010f09 0000000180021b28
- 000000018002f290:	0000000180010f20 0000000180010faf 0000000180020d18
- 000000018002f29c:	0000000180010faf 0000000180010ff0 0000000180021e9c
- 000000018002f2a8:	0000000180010ff0 000000018001100b 0000000180021eb0
- 000000018002f2b4:	0000000180011010 0000000180011050 0000000180021fbc
+ 000000018002f290:	0000000180010f10 0000000180010f50 0000000180021fbc
+ 000000018002f29c:	0000000180010f60 0000000180010fef 0000000180020d18
+ 000000018002f2a8:	0000000180010fef 0000000180011030 0000000180021e9c
+ 000000018002f2b4:	0000000180011030 000000018001104b 0000000180021eb0
  000000018002f2c0:	0000000180011050 0000000180011248 00000001800220d4
  000000018002f2cc:	0000000180011250 000000018001128b 0000000180020b10
  000000018002f2d8:	0000000180011290 0000000180011309 0000000180021a60
  000000018002f2e4:	0000000180011310 00000001800113aa 0000000180021ec0
  000000018002f2f0:	00000001800113b0 000000018001144a 0000000180021ed4
  000000018002f2fc:	0000000180011450 00000001800114ac 0000000180020f38
  000000018002f308:	00000001800114b0 00000001800114ff 0000000180020d70
@@ -3813,34 +3813,34 @@
 	Chain: start: 0000000000010e50, end: 0000000000010e82
 	 unwind data: 0000000000021afc.
  0000000180021b28 (rva: 00021b28): 0000000180010ebe - 0000000180010f09
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	Chain: start: 0000000000010e50, end: 0000000000010e82
 	 unwind data: 0000000000021afc.
- 0000000180020d18 (rva: 00020d18): 0000000180010f20 - 0000000180010faf
+ 0000000180021fbc (rva: 00021fbc): 0000000180010f10 - 0000000180010f50
+	Version: 1, Flags: none
+	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
+	  pc+0x06: alloc small area: rsp = rsp - 0x40
+	  pc+0x02: push rbx
+ 0000000180020d18 (rva: 00020d18): 0000000180010f60 - 0000000180010fef
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x38
- 0000000180021e9c (rva: 00021e9c): 0000000180010faf - 0000000180010ff0
+ 0000000180021e9c (rva: 00021e9c): 0000000180010fef - 0000000180011030
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: save rbx at rsp + 0x30
-	Chain: start: 0000000000010f20, end: 0000000000010faf
+	Chain: start: 0000000000010f60, end: 0000000000010fef
 	 unwind data: 0000000000020d18.
- 0000000180021eb0 (rva: 00021eb0): 0000000180010ff0 - 000000018001100b
+ 0000000180021eb0 (rva: 00021eb0): 0000000180011030 - 000000018001104b
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 0000000000010f20, end: 0000000000010faf
+	Chain: start: 0000000000010f60, end: 0000000000010fef
 	 unwind data: 0000000000020d18.
- 0000000180021fbc (rva: 00021fbc): 0000000180011010 - 0000000180011050
-	Version: 1, Flags: none
-	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
-	  pc+0x06: alloc small area: rsp = rsp - 0x40
-	  pc+0x02: push rbx
  00000001800220d4 (rva: 000220d4): 0000000180011050 - 0000000180011248
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x18, Frame offset: 0x0, Frame reg: none
 	  pc+0x18: save rsi at rsp + 0x78
 	  pc+0x18: save rbp at rsp + 0x70
 	  pc+0x18: save rbx at rsp + 0x68
 	  pc+0x18: alloc small area: rsp = rsp - 0x40
@@ -5034,16 +5034,16 @@
 	  130: a0 83 00 00 d0 83 00 00 90 8e 00 00 80 90 00 00
 	  140: 10 91 00 00 40 e4 00 00 60 e4 00 00 80 e4 00 00
 	  150: 00 e5 00 00 90 12 01 00 10 13 01 00 b0 13 01 00
 	  160: 50 14 01 00 b0 14 01 00 40 51 01 00 70 52 01 00
 	  170: e0 52 01 00 00 82 01 00 40 67 00 00 10 46 00 00
 	  180: 00 84 00 00 a0 33 00 00 b0 e6 00 00 60 16 01 00
 	  190: 90 54 01 00 40 47 00 00 c0 e6 00 00 00 e7 00 00
-	  1a0: a0 e4 01 00 a0 d6 01 00 38 e6 01 00 50 e8 01 00
-	  1b0: 78 ee 01 00 e8 f1 01 00 e8 f4 01 00 50 6c 00 00
+	  1a0: a8 e4 01 00 a0 d6 01 00 48 e6 01 00 60 e8 01 00
+	  1b0: 88 ee 01 00 f8 f1 01 00 f8 f4 01 00 50 6c 00 00
 	  1c0: e0 37 00 00 f0 37 00 00 30 95 00 00 c0 17 01 00
 	  1d0: d0 95 00 00 30 4b 00 00 b0 28 01 00 e0 28 01 00
 	  1e0: 50 e8 00 00 40 6d 00 00 10 4f 00 00 b0 3a 00 00
 	  1f0: e0 3a 00 00 10 29 01 00 40 4f 00 00 60 67 01 00
 	  200: f0 82 01 00 10 3b 00 00 80 68 01 00 40 3b 00 00
 	  210: b0 68 01 00 a0 a0 00 00 00 50 00 00 40 3c 00 00
 	  220: 70 6d 00 00 a0 6d 00 00 00 ee 00 00 70 6d 00 00
@@ -5064,31 +5064,31 @@
 	  310: 40 76 00 00 a0 76 00 00 c0 77 00 00 e0 ba 00 00
 	  320: e0 78 00 00 90 bc 00 00 e0 79 00 00 40 7a 00 00
 	  330: 60 7b 00 00 10 c3 00 00 80 7c 00 00 80 3f 00 00
 	  340: 20 40 00 00 a0 40 00 00 20 35 01 00 60 73 01 00
 	  350: c0 91 01 00 20 7d 00 00 10 41 00 00 60 41 00 00
 	  360: b0 41 00 00 c0 35 01 00 70 73 01 00 d0 91 01 00
 	  370: 50 5c 00 00 e0 22 00 00 00 1e 00 00 40 29 00 00
-	  380: 20 0f 01 00 c0 4a 01 00 c0 4a 01 00 10 36 01 00
+	  380: 60 0f 01 00 c0 4a 01 00 c0 4a 01 00 10 36 01 00
 	  390: 70 7d 00 00 a0 7d 00 00 30 42 00 00 60 42 00 00
 	  3a0: a0 55 00 00 60 40 01 00 90 42 00 00 e0 c7 00 00
 	  3b0: 10 d5 00 00 f0 55 00 00 10 48 01 00 d0 7d 00 00
 	  3c0: 00 7e 00 00 90 fc 00 00 30 7e 00 00 60 7e 00 00
 	  3d0: b0 49 01 00 d0 56 00 00 90 80 01 00 50 81 01 00
 	  3e0: 20 d5 00 00 80 d5 00 00 30 57 00 00 90 7e 00 00
 	  3f0: 00 fd 00 00 e0 d5 00 00 90 57 00 00 30 fd 00 00
 	  400: 70 fd 00 00 b0 57 00 00 40 58 00 00 90 fd 00 00
 	  410: 10 7f 00 00 60 59 00 00 90 7f 00 00 10 80 00 00
 	  420: 40 d6 00 00 80 80 00 00 20 81 00 00 c0 59 00 00
 	  430: 60 d6 00 00 30 5a 00 00 c0 d6 00 00 20 d7 00 00
 	  440: 80 d7 00 00 e0 d7 00 00 90 01 01 00 c0 01 01 00
 	  450: a0 81 00 00 40 d8 00 00 30 da 00 00 a0 dd 00 00
 	  460: d0 42 00 00 20 82 00 00 80 82 00 00 b0 82 00 00
-	  470: e0 82 00 00 70 da 01 00 f0 c6 01 00 20 c4 01 00
-	  480: 40 d2 01 00 30 ee 01 00 a0 f1 01 00 20 f4 01 00
+	  470: e0 82 00 00 70 e1 01 00 f0 c6 01 00 20 c4 01 00
+	  480: 40 d2 01 00 40 ee 01 00 b0 f1 01 00 30 f4 01 00
 	  490: 90 5a 00 00 10 43 00 00 d0 08 01 00 e0 08 01 00
 	  4a0: b0 de 00 00 50 43 00 00 a0 5a 00 00 80 43 00 00
 	  4b0: e0 de 00 00 20 df 00 00 b0 43 00 00 30 7e 00 00
 	  4c0: 20 0a 01 00 e0 43 00 00 10 44 00 00 10 83 00 00
 	  4d0: 40 44 00 00 70 44 00 00 a0 44 00 00 20 4a 01 00
 	  4e0: 50 df 00 00 d0 5a 00 00 20 0e 01 00 40 83 00 00
 	  4f0: 70 83 00 00 50 0e 01 00 d7 32 02 00 1c 33 02 00
@@ -6312,15 +6312,15 @@
 	  5110: 52 ab 02 00 00 00 00 00 6c ab 02 00 00 00 00 00
 	  5120: 8e ab 02 00 00 00 00 00 aa ab 02 00 00 00 00 00
 	  5130: de ab 02 00 00 00 00 00 c6 ab 02 00 00 00 00 00
 	  5140: ec ab 02 00 00 00 00 00 02 ac 02 00 00 00 00 00
 	  5150: f6 ab 02 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  5160: 0e ab 02 00 00 00 00 00 04 ab 02 00 00 00 00 00
 	  5170: 18 ab 02 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  5180: 37 05 3f 73 65 74 48 65 61 64 65 72 40 51 4e 65
+	  5180: 36 05 3f 73 65 74 48 65 61 64 65 72 40 51 4e 65
 	  5190: 74 77 6f 72 6b 52 65 71 75 65 73 74 40 40 51 45
 	  51a0: 41 41 58 57 34 4b 6e 6f 77 6e 48 65 61 64 65 72
 	  51b0: 73 40 31 40 41 45 42 56 51 56 61 72 69 61 6e 74
 	  51c0: 40 40 40 5a 00 00 42 00 3f 3f 30 51 4e 65 74 77
 	  51d0: 6f 72 6b 41 63 63 65 73 73 4d 61 6e 61 67 65 72
 	  51e0: 40 40 51 45 41 41 40 50 45 41 56 51 4f 62 6a 65
 	  51f0: 63 74 40 40 40 5a 00 00 b0 00 3f 3f 31 51 4e 65
@@ -6332,41 +6332,41 @@
 	  5250: 77 6f 72 6b 52 65 70 6c 79 40 40 57 34 4f 70 65
 	  5260: 72 61 74 69 6f 6e 40 31 40 41 45 42 56 51 4e 65
 	  5270: 74 77 6f 72 6b 52 65 71 75 65 73 74 40 40 50 45
 	  5280: 41 56 51 49 4f 44 65 76 69 63 65 40 40 40 5a 00
 	  5290: a1 03 3f 6d 65 74 61 4f 62 6a 65 63 74 40 51 4e
 	  52a0: 65 74 77 6f 72 6b 41 63 63 65 73 73 4d 61 6e 61
 	  52b0: 67 65 72 40 40 55 45 42 41 50 45 42 55 51 4d 65
-	  52c0: 74 61 4f 62 6a 65 63 74 40 40 58 5a 00 00 5a 04
+	  52c0: 74 61 4f 62 6a 65 63 74 40 40 58 5a 00 00 59 04
 	  52d0: 3f 71 74 5f 6d 65 74 61 63 61 6c 6c 40 51 4e 65
 	  52e0: 74 77 6f 72 6b 41 63 63 65 73 73 4d 61 6e 61 67
 	  52f0: 65 72 40 40 55 45 41 41 48 57 34 43 61 6c 6c 40
 	  5300: 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 48 50 45
-	  5310: 41 50 45 41 58 40 5a 00 72 04 3f 71 74 5f 6d 65
+	  5310: 41 50 45 41 58 40 5a 00 71 04 3f 71 74 5f 6d 65
 	  5320: 74 61 63 61 73 74 40 51 4e 65 74 77 6f 72 6b 41
 	  5330: 63 63 65 73 73 4d 61 6e 61 67 65 72 40 40 55 45
-	  5340: 41 41 50 45 41 58 50 45 42 44 40 5a 00 00 35 06
+	  5340: 41 41 50 45 41 58 50 45 42 44 40 5a 00 00 34 06
 	  5350: 3f 73 75 70 70 6f 72 74 65 64 53 63 68 65 6d 65
 	  5360: 73 40 51 4e 65 74 77 6f 72 6b 41 63 63 65 73 73
 	  5370: 4d 61 6e 61 67 65 72 40 40 55 45 42 41 3f 41 56
 	  5380: 3f 24 51 4c 69 73 74 40 56 51 53 74 72 69 6e 67
-	  5390: 40 40 40 40 58 5a 00 00 15 06 3f 73 74 61 74 69
+	  5390: 40 40 40 40 58 5a 00 00 14 06 3f 73 74 61 74 69
 	  53a0: 63 4d 65 74 61 4f 62 6a 65 63 74 40 51 4e 65 74
 	  53b0: 77 6f 72 6b 52 65 70 6c 79 40 40 32 55 51 4d 65
-	  53c0: 74 61 4f 62 6a 65 63 74 40 40 42 00 06 06 3f 73
+	  53c0: 74 61 4f 62 6a 65 63 74 40 40 42 00 05 06 3f 73
 	  53d0: 74 61 74 69 63 4d 65 74 61 4f 62 6a 65 63 74 40
 	  53e0: 51 48 74 74 70 4d 75 6c 74 69 50 61 72 74 40 40
 	  53f0: 32 55 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 42
 	  5400: 00 00 65 00 3f 3f 30 51 4e 65 74 77 6f 72 6b 52
 	  5410: 65 71 75 65 73 74 40 40 51 45 41 41 40 58 5a 00
 	  5420: c0 00 3f 3f 31 51 4e 65 74 77 6f 72 6b 52 65 71
-	  5430: 75 65 73 74 40 40 51 45 41 41 40 58 5a 00 cb 05
+	  5430: 75 65 73 74 40 40 51 45 41 41 40 58 5a 00 ca 05
 	  5440: 3f 73 65 74 55 72 6c 40 51 4e 65 74 77 6f 72 6b
 	  5450: 52 65 71 75 65 73 74 40 40 51 45 41 41 58 41 45
-	  5460: 42 56 51 55 72 6c 40 40 40 5a 00 00 94 05 3f 73
+	  5460: 42 56 51 55 72 6c 40 40 40 5a 00 00 93 05 3f 73
 	  5470: 65 74 52 61 77 48 65 61 64 65 72 40 51 4e 65 74
 	  5480: 77 6f 72 6b 52 65 71 75 65 73 74 40 40 51 45 41
 	  5490: 41 58 41 45 42 56 51 42 79 74 65 41 72 72 61 79
 	  54a0: 40 40 30 40 5a 00 74 00 3f 3f 30 51 53 73 6c 43
 	  54b0: 6f 6e 66 69 67 75 72 61 74 69 6f 6e 40 40 51 45
 	  54c0: 41 41 40 58 5a 00 73 00 3f 3f 30 51 53 73 6c 43
 	  54d0: 6f 6e 66 69 67 75 72 61 74 69 6f 6e 40 40 51 45
@@ -6374,15 +6374,15 @@
 	  54f0: 31 51 53 73 6c 43 6f 6e 66 69 67 75 72 61 74 69
 	  5500: 6f 6e 40 40 51 45 41 41 40 58 5a 00 12 01 3f 3f
 	  5510: 34 51 53 73 6c 43 6f 6e 66 69 67 75 72 61 74 69
 	  5520: 6f 6e 40 40 51 45 41 41 41 45 41 56 30 40 41 45
 	  5530: 42 56 30 40 40 5a 00 00 3e 01 3f 3f 38 51 53 73
 	  5540: 6c 43 6f 6e 66 69 67 75 72 61 74 69 6f 6e 40 40
 	  5550: 51 45 42 41 5f 4e 41 45 42 56 30 40 40 5a 00 00
-	  5560: 45 04 3f 71 52 65 67 69 73 74 65 72 4e 6f 72 6d
+	  5560: 44 04 3f 71 52 65 67 69 73 74 65 72 4e 6f 72 6d
 	  5570: 61 6c 69 7a 65 64 4d 65 74 61 54 79 70 65 5f 51
 	  5580: 53 73 6c 43 6f 6e 66 69 67 75 72 61 74 69 6f 6e
 	  5590: 40 40 59 41 48 41 45 42 56 51 42 79 74 65 41 72
 	  55a0: 72 61 79 40 40 40 5a 00 e0 02 3f 68 65 61 64 40
 	  55b0: 51 4e 65 74 77 6f 72 6b 41 63 63 65 73 73 4d 61
 	  55c0: 6e 61 67 65 72 40 40 51 45 41 41 50 45 41 56 51
 	  55d0: 4e 65 74 77 6f 72 6b 52 65 70 6c 79 40 40 41 45
@@ -6422,52 +6422,52 @@
 	  57f0: 45 42 56 51 4e 65 74 77 6f 72 6b 52 65 71 75 65
 	  5800: 73 74 40 40 50 45 41 56 51 48 74 74 70 4d 75 6c
 	  5810: 74 69 50 61 72 74 40 40 40 5a 00 00 b5 02 3f 66
 	  5820: 69 6e 69 73 68 65 64 40 51 4e 65 74 77 6f 72 6b
 	  5830: 52 65 70 6c 79 40 40 51 45 41 41 58 58 5a 00 00
 	  5840: 64 00 3f 3f 30 51 4e 65 74 77 6f 72 6b 52 65 71
 	  5850: 75 65 73 74 40 40 51 45 41 41 40 41 45 42 56 51
-	  5860: 55 72 6c 40 40 40 5a 00 a4 06 3f 75 72 6c 40 51
+	  5860: 55 72 6c 40 40 40 5a 00 a3 06 3f 75 72 6c 40 51
 	  5870: 4e 65 74 77 6f 72 6b 52 65 71 75 65 73 74 40 40
 	  5880: 51 45 42 41 3f 41 56 51 55 72 6c 40 40 58 5a 00
 	  5890: e4 02 3f 68 65 61 64 65 72 40 51 4e 65 74 77 6f
 	  58a0: 72 6b 52 65 71 75 65 73 74 40 40 51 45 42 41 3f
 	  58b0: 41 56 51 56 61 72 69 61 6e 74 40 40 57 34 4b 6e
 	  58c0: 6f 77 6e 48 65 61 64 65 72 73 40 31 40 40 5a 00
 	  58d0: a0 02 3f 65 72 72 6f 72 4f 63 63 75 72 72 65 64
 	  58e0: 40 51 4e 65 74 77 6f 72 6b 52 65 70 6c 79 40 40
 	  58f0: 51 45 41 41 58 57 34 4e 65 74 77 6f 72 6b 45 72
-	  5900: 72 6f 72 40 31 40 40 5a 00 00 3f 04 3f 71 52 65
+	  5900: 72 6f 72 40 31 40 40 5a 00 00 3e 04 3f 71 52 65
 	  5910: 67 69 73 74 65 72 4e 6f 72 6d 61 6c 69 7a 65 64
 	  5920: 4d 65 74 61 54 79 70 65 5f 51 4e 65 74 77 6f 72
 	  5930: 6b 52 65 70 6c 79 5f 5f 4e 65 74 77 6f 72 6b 45
 	  5940: 72 72 6f 72 40 40 59 41 48 41 45 42 56 51 42 79
-	  5950: 74 65 41 72 72 61 79 40 40 40 5a 00 b8 05 3f 73
+	  5950: 74 65 41 72 72 61 79 40 40 40 5a 00 b7 05 3f 73
 	  5960: 65 74 53 73 6c 43 6f 6e 66 69 67 75 72 61 74 69
 	  5970: 6f 6e 40 51 4e 65 74 77 6f 72 6b 52 65 71 75 65
 	  5980: 73 74 40 40 51 45 41 41 58 41 45 42 56 51 53 73
 	  5990: 6c 43 6f 6e 66 69 67 75 72 61 74 69 6f 6e 40 40
 	  59a0: 40 5a 00 00 3e 03 3f 69 73 4e 75 6c 6c 40 51 53
 	  59b0: 73 6c 43 6f 6e 66 69 67 75 72 61 74 69 6f 6e 40
 	  59c0: 40 51 45 42 41 5f 4e 58 5a 00 ce 01 3f 61 75 74
 	  59d0: 68 65 6e 74 69 63 61 74 69 6f 6e 52 65 71 75 69
 	  59e0: 72 65 64 40 51 4e 65 74 77 6f 72 6b 41 63 63 65
 	  59f0: 73 73 4d 61 6e 61 67 65 72 40 40 51 45 41 41 58
 	  5a00: 50 45 41 56 51 4e 65 74 77 6f 72 6b 52 65 70 6c
 	  5a10: 79 40 40 50 45 41 56 51 41 75 74 68 65 6e 74 69
-	  5a20: 63 61 74 6f 72 40 40 40 5a 00 a3 06 3f 75 72 6c
+	  5a20: 63 61 74 6f 72 40 40 40 5a 00 a2 06 3f 75 72 6c
 	  5a30: 40 51 4e 65 74 77 6f 72 6b 52 65 70 6c 79 40 40
 	  5a40: 51 45 42 41 3f 41 56 51 55 72 6c 40 40 58 5a 00
-	  5a50: cd 05 3f 73 65 74 55 73 65 72 40 51 41 75 74 68
+	  5a50: cc 05 3f 73 65 74 55 73 65 72 40 51 41 75 74 68
 	  5a60: 65 6e 74 69 63 61 74 6f 72 40 40 51 45 41 41 58
 	  5a70: 41 45 42 56 51 53 74 72 69 6e 67 40 40 40 5a 00
-	  5a80: 6b 05 3f 73 65 74 50 61 73 73 77 6f 72 64 40 51
+	  5a80: 6a 05 3f 73 65 74 50 61 73 73 77 6f 72 64 40 51
 	  5a90: 41 75 74 68 65 6e 74 69 63 61 74 6f 72 40 40 51
 	  5aa0: 45 41 41 58 41 45 42 56 51 53 74 72 69 6e 67 40
-	  5ab0: 40 40 5a 00 0b 06 3f 73 74 61 74 69 63 4d 65 74
+	  5ab0: 40 40 5a 00 0a 06 3f 73 74 61 74 69 63 4d 65 74
 	  5ac0: 61 4f 62 6a 65 63 74 40 51 4e 65 74 77 6f 72 6b
 	  5ad0: 41 63 63 65 73 73 4d 61 6e 61 67 65 72 40 40 32
 	  5ae0: 55 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 42 00
 	  5af0: 78 02 3f 64 69 73 63 6f 6e 6e 65 63 74 65 64 40
 	  5b00: 51 41 62 73 74 72 61 63 74 53 6f 63 6b 65 74 40
 	  5b10: 40 51 45 41 41 58 58 5a 00 00 27 00 3f 3f 30 51
 	  5b20: 48 6f 73 74 41 64 64 72 65 73 73 40 40 51 45 41
@@ -6481,89 +6481,89 @@
 	  5ba0: 58 5a 00 00 6b 03 3f 6c 69 73 74 65 6e 40 51 54
 	  5bb0: 63 70 53 65 72 76 65 72 40 40 51 45 41 41 5f 4e
 	  5bc0: 41 45 42 56 51 48 6f 73 74 41 64 64 72 65 73 73
 	  5bd0: 40 40 47 40 5a 00 0b 02 3f 63 6c 6f 73 65 40 51
 	  5be0: 54 63 70 53 65 72 76 65 72 40 40 51 45 41 41 58
 	  5bf0: 58 5a 00 00 2e 03 3f 69 73 4c 69 73 74 65 6e 69
 	  5c00: 6e 67 40 51 54 63 70 53 65 72 76 65 72 40 40 51
-	  5c10: 45 42 41 5f 4e 58 5a 00 df 04 3f 73 65 72 76 65
+	  5c10: 45 42 41 5f 4e 58 5a 00 de 04 3f 73 65 72 76 65
 	  5c20: 72 50 6f 72 74 40 51 54 63 70 53 65 72 76 65 72
 	  5c30: 40 40 51 45 42 41 47 58 5a 00 ca 03 3f 6e 65 77
 	  5c40: 43 6f 6e 6e 65 63 74 69 6f 6e 40 51 54 63 70 53
 	  5c50: 65 72 76 65 72 40 40 51 45 41 41 58 58 5a 00 00
-	  5c60: 01 06 3f 73 74 61 74 69 63 4d 65 74 61 4f 62 6a
+	  5c60: 00 06 3f 73 74 61 74 69 63 4d 65 74 61 4f 62 6a
 	  5c70: 65 63 74 40 51 41 62 73 74 72 61 63 74 53 6f 63
 	  5c80: 6b 65 74 40 40 32 55 51 4d 65 74 61 4f 62 6a 65
-	  5c90: 63 74 40 40 42 00 19 06 3f 73 74 61 74 69 63 4d
+	  5c90: 63 74 40 40 42 00 18 06 3f 73 74 61 74 69 63 4d
 	  5ca0: 65 74 61 4f 62 6a 65 63 74 40 51 54 63 70 53 65
 	  5cb0: 72 76 65 72 40 40 32 55 51 4d 65 74 61 4f 62 6a
 	  5cc0: 65 63 74 40 40 42 00 00 9b 02 3f 65 72 72 6f 72
 	  5cd0: 40 51 4e 65 74 77 6f 72 6b 52 65 70 6c 79 40 40
 	  5ce0: 51 45 42 41 3f 41 57 34 4e 65 74 77 6f 72 6b 45
 	  5cf0: 72 72 6f 72 40 31 40 58 5a 00 e3 02 3f 68 65 61
 	  5d00: 64 65 72 40 51 4e 65 74 77 6f 72 6b 52 65 70 6c
 	  5d10: 79 40 40 51 45 42 41 3f 41 56 51 56 61 72 69 61
 	  5d20: 6e 74 40 40 57 34 4b 6e 6f 77 6e 48 65 61 64 65
 	  5d30: 72 73 40 51 4e 65 74 77 6f 72 6b 52 65 71 75 65
 	  5d40: 73 74 40 40 40 5a 00 00 51 74 36 4e 65 74 77 6f
 	  5d50: 72 6b 2e 64 6c 6c 00 00 ea 19 3f 73 74 61 74 69
 	  5d60: 63 4d 65 74 61 4f 62 6a 65 63 74 40 51 4f 62 6a
 	  5d70: 65 63 74 40 40 32 55 51 4d 65 74 61 4f 62 6a 65
-	  5d80: 63 74 40 40 42 00 0a 0a 3f 63 6f 6d 70 61 72 65
+	  5d80: 63 74 40 40 42 00 0b 0a 3f 63 6f 6d 70 61 72 65
 	  5d90: 4d 65 6d 6f 72 79 40 51 74 50 72 69 76 61 74 65
 	  5da0: 40 40 59 41 48 56 51 42 79 74 65 41 72 72 61 79
 	  5db0: 56 69 65 77 40 40 30 40 5a 00 5a 00 3f 3f 30 51
 	  5dc0: 42 79 74 65 41 72 72 61 79 40 40 51 45 41 41 40
 	  5dd0: 58 5a 00 00 58 00 3f 3f 30 51 42 79 74 65 41 72
 	  5de0: 72 61 79 40 40 51 45 41 41 40 41 45 42 56 30 40
 	  5df0: 40 5a 00 00 f0 02 3f 3f 31 51 42 79 74 65 41 72
 	  5e00: 72 61 79 40 40 51 45 41 41 40 58 5a 00 00 56 00
 	  5e10: 3f 3f 30 51 42 79 74 65 41 72 72 61 79 40 40 51
 	  5e20: 45 41 41 40 24 24 51 45 41 56 30 40 40 5a 00 00
-	  5e30: 80 16 3f 72 65 73 65 72 76 65 40 51 42 79 74 65
+	  5e30: 81 16 3f 72 65 73 65 72 76 65 40 51 42 79 74 65
 	  5e40: 41 72 72 61 79 40 40 51 45 41 41 58 5f 4a 40 5a
-	  5e50: 00 00 9a 0b 3f 64 61 74 61 40 51 42 79 74 65 41
+	  5e50: 00 00 9b 0b 3f 64 61 74 61 40 51 42 79 74 65 41
 	  5e60: 72 72 61 79 40 40 51 45 42 41 50 45 42 44 58 5a
-	  5e70: 00 00 00 08 3f 61 70 70 65 6e 64 40 51 42 79 74
+	  5e70: 00 00 01 08 3f 61 70 70 65 6e 64 40 51 42 79 74
 	  5e80: 65 41 72 72 61 79 40 40 51 45 41 41 41 45 41 56
-	  5e90: 31 40 50 45 42 44 40 5a 00 00 24 19 3f 73 69 7a
+	  5e90: 31 40 50 45 42 44 40 5a 00 00 25 19 3f 73 69 7a
 	  5ea0: 65 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45
-	  5eb0: 42 41 5f 4a 58 5a 00 00 41 10 3f 69 73 4e 75 6c
+	  5eb0: 42 41 5f 4a 58 5a 00 00 42 10 3f 69 73 4e 75 6c
 	  5ec0: 6c 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45
 	  5ed0: 42 41 5f 4e 58 5a 00 00 0d 05 3f 3f 36 40 59 41
 	  5ee0: 41 45 41 56 51 44 61 74 61 53 74 72 65 61 6d 40
 	  5ef0: 40 41 45 41 56 30 40 41 45 42 56 51 42 79 74 65
 	  5f00: 41 72 72 61 79 40 40 40 5a 00 98 04 3f 3f 35 40
 	  5f10: 59 41 41 45 41 56 51 44 61 74 61 53 74 72 65 61
 	  5f20: 6d 40 40 41 45 41 56 30 40 41 45 41 56 51 42 79
-	  5f30: 74 65 41 72 72 61 79 40 40 40 5a 00 8a 09 3f 63
+	  5f30: 74 65 41 72 72 61 79 40 40 40 5a 00 8b 09 3f 63
 	  5f40: 6c 61 73 73 4e 61 6d 65 40 51 4d 65 74 61 4f 62
 	  5f50: 6a 65 63 74 40 40 51 45 42 41 50 45 42 44 58 5a
 	  5f60: 00 00 1c 1c 3f 74 72 40 51 4d 65 74 61 4f 62 6a
 	  5f70: 65 63 74 40 40 51 45 42 41 3f 41 56 51 53 74 72
-	  5f80: 69 6e 67 40 40 50 45 42 44 30 48 40 5a 00 89 07
+	  5f80: 69 6e 67 40 40 50 45 42 44 30 48 40 5a 00 8a 07
 	  5f90: 3f 61 63 74 69 76 61 74 65 40 51 4d 65 74 61 4f
 	  5fa0: 62 6a 65 63 74 40 40 53 41 58 50 45 41 56 51 4f
 	  5fb0: 62 6a 65 63 74 40 40 50 45 42 55 31 40 48 50 45
-	  5fc0: 41 50 45 41 58 40 5a 00 11 0a 3f 63 6f 6d 70 61
+	  5fc0: 41 50 45 41 58 40 5a 00 12 0a 3f 63 6f 6d 70 61
 	  5fd0: 72 65 53 74 72 69 6e 67 73 40 51 74 50 72 69 76
 	  5fe0: 61 74 65 40 40 59 41 48 56 51 53 74 72 69 6e 67
 	  5ff0: 56 69 65 77 40 40 30 57 34 43 61 73 65 53 65 6e
 	  6000: 73 69 74 69 76 69 74 79 40 51 74 40 40 40 5a 00
 	  6010: 0e 02 3f 3f 30 51 53 74 72 69 6e 67 40 40 51 45
 	  6020: 41 41 40 58 5a 00 08 02 3f 3f 30 51 53 74 72 69
 	  6030: 6e 67 40 40 51 45 41 41 40 41 45 42 56 30 40 40
 	  6040: 5a 00 62 03 3f 3f 31 51 53 74 72 69 6e 67 40 40
 	  6050: 51 45 41 41 40 58 5a 00 07 02 3f 3f 30 51 53 74
 	  6060: 72 69 6e 67 40 40 51 45 41 41 40 24 24 51 45 41
 	  6070: 56 30 40 40 5a 00 60 04 3f 3f 34 51 53 74 72 69
 	  6080: 6e 67 40 40 51 45 41 41 41 45 41 56 30 40 24 24
-	  6090: 51 45 41 56 30 40 40 5a 00 00 a5 0b 3f 64 61 74
+	  6090: 51 45 41 56 30 40 40 5a 00 00 a6 0b 3f 64 61 74
 	  60a0: 61 40 51 53 74 72 69 6e 67 40 40 51 45 42 41 50
-	  60b0: 45 42 56 51 43 68 61 72 40 40 58 5a 00 00 52 10
+	  60b0: 45 42 56 51 43 68 61 72 40 40 58 5a 00 00 53 10
 	  60c0: 3f 69 73 4e 75 6c 6c 40 51 53 74 72 69 6e 67 40
 	  60d0: 40 51 45 42 41 5f 4e 58 5a 00 23 05 3f 3f 36 40
 	  60e0: 59 41 41 45 41 56 51 44 61 74 61 53 74 72 65 61
 	  60f0: 6d 40 40 41 45 41 56 30 40 41 45 42 56 51 53 74
 	  6100: 72 69 6e 67 40 40 40 5a 00 00 b0 04 3f 3f 35 40
 	  6110: 59 41 41 45 41 56 51 44 61 74 61 53 74 72 65 61
 	  6120: 6d 40 40 41 45 41 56 30 40 41 45 41 56 51 53 74
@@ -6583,40 +6583,40 @@
 	  6200: 35 40 59 41 41 45 41 56 51 44 61 74 61 53 74 72
 	  6210: 65 61 6d 40 40 41 45 41 56 30 40 41 45 41 56 51
 	  6220: 55 72 6c 40 40 40 5a 00 fe 04 3f 3f 36 40 59 41
 	  6230: 3f 41 56 51 44 65 62 75 67 40 40 56 30 40 41 45
 	  6240: 42 56 51 55 72 6c 40 40 40 5a 00 00 0c 1a 3f 73
 	  6250: 74 61 74 75 73 40 51 44 61 74 61 53 74 72 65 61
 	  6260: 6d 40 40 51 45 42 41 3f 41 57 34 53 74 61 74 75
-	  6270: 73 40 31 40 58 5a 00 00 b4 18 3f 73 65 74 53 74
+	  6270: 73 40 31 40 58 5a 00 00 b5 18 3f 73 65 74 53 74
 	  6280: 61 74 75 73 40 51 44 61 74 61 53 74 72 65 61 6d
 	  6290: 40 40 51 45 41 41 58 57 34 53 74 61 74 75 73 40
-	  62a0: 31 40 40 5a 00 00 94 16 3f 72 65 73 65 74 53 74
+	  62a0: 31 40 40 5a 00 00 95 16 3f 72 65 73 65 74 53 74
 	  62b0: 61 74 75 73 40 51 44 61 74 61 53 74 72 65 61 6d
 	  62c0: 40 40 51 45 41 41 58 58 5a 00 c1 04 3f 3f 35 51
 	  62d0: 44 61 74 61 53 74 72 65 61 6d 40 40 51 45 41 41
 	  62e0: 41 45 41 56 30 40 41 45 41 48 40 5a 00 00 37 05
 	  62f0: 3f 3f 36 51 44 61 74 61 53 74 72 65 61 6d 40 40
-	  6300: 51 45 41 41 41 45 41 56 30 40 48 40 5a 00 c2 0f
+	  6300: 51 45 41 41 41 45 41 56 30 40 48 40 5a 00 c3 0f
 	  6310: 3f 69 73 44 65 76 69 63 65 54 72 61 6e 73 61 63
 	  6320: 74 69 6f 6e 53 74 61 72 74 65 64 40 51 44 61 74
 	  6330: 61 53 74 72 65 61 6d 40 40 51 45 42 41 5f 4e 58
-	  6340: 5a 00 db 15 3f 72 65 67 69 73 74 65 72 4e 6f 72
+	  6340: 5a 00 dc 15 3f 72 65 67 69 73 74 65 72 4e 6f 72
 	  6350: 6d 61 6c 69 7a 65 64 54 79 70 65 64 65 66 40 51
 	  6360: 4d 65 74 61 54 79 70 65 40 40 53 41 58 41 45 42
 	  6370: 56 51 42 79 74 65 41 72 72 61 79 40 40 56 31 40
-	  6380: 40 5a 00 00 bd 0e 3f 69 64 40 51 4d 65 74 61 54
-	  6390: 79 70 65 40 40 51 45 42 41 48 48 40 5a 00 5f 0c
+	  6380: 40 5a 00 00 be 0e 3f 69 64 40 51 4d 65 74 61 54
+	  6390: 79 70 65 40 40 51 45 42 41 48 48 40 5a 00 60 0c
 	  63a0: 3f 64 79 6e 61 6d 69 63 4d 65 74 61 4f 62 6a 65
 	  63b0: 63 74 40 51 4f 62 6a 65 63 74 44 61 74 61 40 40
 	  63c0: 51 45 42 41 50 45 41 55 51 4d 65 74 61 4f 62 6a
-	  63d0: 65 63 74 40 40 58 5a 00 0f 15 3f 71 74 5f 6d 65
+	  63d0: 65 63 74 40 40 58 5a 00 10 15 3f 71 74 5f 6d 65
 	  63e0: 74 61 63 61 73 74 40 51 4f 62 6a 65 63 74 40 40
 	  63f0: 55 45 41 41 50 45 41 58 50 45 42 44 40 5a 00 00
-	  6400: da 14 3f 71 74 5f 6d 65 74 61 63 61 6c 6c 40 51
+	  6400: db 14 3f 71 74 5f 6d 65 74 61 63 61 6c 6c 40 51
 	  6410: 4f 62 6a 65 63 74 40 40 55 45 41 41 48 57 34 43
 	  6420: 61 6c 6c 40 51 4d 65 74 61 4f 62 6a 65 63 74 40
 	  6430: 40 48 50 45 41 50 45 41 58 40 5a 00 cd 00 3f 3f
 	  6440: 30 51 44 65 62 75 67 40 40 51 45 41 41 40 24 24
 	  6450: 51 45 41 56 30 40 40 5a 00 00 06 03 3f 3f 31 51
 	  6460: 44 65 62 75 67 40 40 51 45 41 41 40 58 5a 00 00
 	  6470: 45 05 3f 3f 36 51 44 65 62 75 67 40 40 51 45 41
@@ -6628,66 +6628,66 @@
 	  64d0: 00 00 43 05 3f 3f 36 51 44 65 62 75 67 40 40 51
 	  64e0: 45 41 41 41 45 41 56 30 40 41 45 42 56 51 42 79
 	  64f0: 74 65 41 72 72 61 79 40 40 40 5a 00 d2 00 3f 3f
 	  6500: 30 51 44 65 62 75 67 53 74 61 74 65 53 61 76 65
 	  6510: 72 40 40 51 45 41 41 40 41 45 41 56 51 44 65 62
 	  6520: 75 67 40 40 40 5a 00 00 07 03 3f 3f 31 51 44 65
 	  6530: 62 75 67 53 74 61 74 65 53 61 76 65 72 40 40 51
-	  6540: 45 41 41 40 58 5a 00 00 b1 14 3f 71 74 5f 51 4d
+	  6540: 45 41 41 40 58 5a 00 00 b2 14 3f 71 74 5f 51 4d
 	  6550: 65 74 61 45 6e 75 6d 5f 64 65 62 75 67 4f 70 65
 	  6560: 72 61 74 6f 72 40 40 59 41 3f 41 56 51 44 65 62
 	  6570: 75 67 40 40 41 45 41 56 31 40 5f 4a 50 45 42 55
 	  6580: 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 50 45 42
 	  6590: 44 40 5a 00 96 02 3f 3f 30 51 56 61 72 69 61 6e
 	  65a0: 74 40 40 51 45 41 41 40 58 5a 00 00 7a 03 3f 3f
 	  65b0: 31 51 56 61 72 69 61 6e 74 40 40 51 45 41 41 40
 	  65c0: 58 5a 00 00 66 02 3f 3f 30 51 56 61 72 69 61 6e
 	  65d0: 74 40 40 51 45 41 41 40 41 45 42 56 30 40 40 5a
 	  65e0: 00 00 81 04 3f 3f 34 51 56 61 72 69 61 6e 74 40
 	  65f0: 40 51 45 41 41 41 45 41 56 30 40 41 45 42 56 30
-	  6600: 40 40 5a 00 9f 14 3f 71 64 65 62 75 67 48 65 6c
+	  6600: 40 40 5a 00 a0 14 3f 71 64 65 62 75 67 48 65 6c
 	  6610: 70 65 72 40 51 56 61 72 69 61 6e 74 40 40 41 45
 	  6620: 42 41 3f 41 56 51 44 65 62 75 67 40 40 56 32 40
-	  6630: 40 5a 00 00 d2 0c 3f 65 71 75 61 6c 73 40 51 56
+	  6630: 40 5a 00 00 d3 0c 3f 65 71 75 61 6c 73 40 51 56
 	  6640: 61 72 69 61 6e 74 40 40 49 45 42 41 5f 4e 41 45
 	  6650: 42 56 31 40 40 5a 00 00 b6 04 3f 3f 35 40 59 41
 	  6660: 41 45 41 56 51 44 61 74 61 53 74 72 65 61 6d 40
 	  6670: 40 41 45 41 56 30 40 41 45 41 56 51 56 61 72 69
 	  6680: 61 6e 74 40 40 40 5a 00 28 05 3f 3f 36 40 59 41
 	  6690: 41 45 41 56 51 44 61 74 61 53 74 72 65 61 6d 40
 	  66a0: 40 41 45 41 56 30 40 41 45 42 56 51 56 61 72 69
-	  66b0: 61 6e 74 40 40 40 5a 00 d7 0b 3f 64 65 61 6c 6c
+	  66b0: 61 6e 74 40 40 40 5a 00 d8 0b 3f 64 65 61 6c 6c
 	  66c0: 6f 63 61 74 65 40 51 41 72 72 61 79 44 61 74 61
 	  66d0: 40 40 53 41 58 50 45 41 55 31 40 5f 4a 31 40 5a
 	  66e0: 00 00 b5 03 3f 3f 34 51 42 79 74 65 41 72 72 61
 	  66f0: 79 40 40 51 45 41 41 41 45 41 56 30 40 24 24 51
-	  6700: 45 41 56 30 40 40 5a 00 ff 07 3f 61 70 70 65 6e
+	  6700: 45 41 56 30 40 40 5a 00 00 08 3f 61 70 70 65 6e
 	  6710: 64 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45
 	  6720: 41 41 41 45 41 56 31 40 44 40 5a 00 61 04 3f 3f
 	  6730: 34 51 53 74 72 69 6e 67 40 40 51 45 41 41 41 45
 	  6740: 41 56 30 40 41 45 42 56 30 40 40 5a 00 00 de 1b
 	  6750: 3f 74 6f 55 74 66 38 40 51 53 74 72 69 6e 67 40
 	  6760: 40 51 45 48 41 41 3f 41 56 51 42 79 74 65 41 72
 	  6770: 72 61 79 40 40 58 5a 00 06 02 3f 3f 30 51 53 74
 	  6780: 72 69 6e 67 40 40 51 45 41 41 40 24 24 51 45 41
 	  6790: 55 3f 24 51 41 72 72 61 79 44 61 74 61 50 6f 69
 	  67a0: 6e 74 65 72 40 5f 53 40 40 40 5a 00 79 04 3f 3f
 	  67b0: 34 51 55 72 6c 40 40 51 45 41 41 41 45 41 56 30
-	  67c0: 40 41 45 42 56 30 40 40 5a 00 78 18 3f 73 65 74
+	  67c0: 40 41 45 42 56 30 40 40 5a 00 79 18 3f 73 65 74
 	  67d0: 51 75 65 72 79 40 51 55 72 6c 40 40 51 45 41 41
 	  67e0: 58 41 45 42 56 51 55 72 6c 51 75 65 72 79 40 40
 	  67f0: 40 5a 00 00 ba 05 3f 3f 39 51 55 72 6c 40 40 51
 	  6800: 45 42 41 5f 4e 41 45 42 56 30 40 40 5a 00 3f 03
 	  6810: 3f 3f 31 51 4f 62 6a 65 63 74 40 40 55 45 41 41
-	  6820: 40 58 5a 00 7e 13 3f 70 61 72 65 6e 74 40 51 4f
+	  6820: 40 58 5a 00 7f 13 3f 70 61 72 65 6e 74 40 51 4f
 	  6830: 62 6a 65 63 74 40 40 51 45 42 41 50 45 41 56 31
 	  6840: 40 58 5a 00 9c 01 3f 3f 30 51 4f 62 6a 65 63 74
 	  6850: 40 40 49 45 41 41 40 41 45 41 56 51 4f 62 6a 65
 	  6860: 63 74 50 72 69 76 61 74 65 40 40 50 45 41 56 30
-	  6870: 40 40 5a 00 3d 0e 3f 67 65 74 41 6e 64 52 65 66
+	  6870: 40 40 5a 00 3e 0e 3f 67 65 74 41 6e 64 52 65 66
 	  6880: 40 45 78 74 65 72 6e 61 6c 52 65 66 43 6f 75 6e
 	  6890: 74 44 61 74 61 40 51 74 53 68 61 72 65 64 50 6f
 	  68a0: 69 6e 74 65 72 40 40 53 41 50 45 41 55 31 32 40
 	  68b0: 50 45 42 56 51 4f 62 6a 65 63 74 40 40 40 5a 00
 	  68c0: 6a 02 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51
 	  68d0: 45 41 41 40 41 45 42 56 3f 24 51 4d 61 70 40 56
 	  68e0: 51 53 74 72 69 6e 67 40 40 56 51 56 61 72 69 61
@@ -6705,90 +6705,90 @@
 	  69a0: 50 45 42 44 57 34 51 74 4d 73 67 54 79 70 65 40
 	  69b0: 40 40 5a 00 34 03 3f 3f 31 51 4c 6f 67 67 69 6e
 	  69c0: 67 43 61 74 65 67 6f 72 79 40 40 51 45 41 41 40
 	  69d0: 58 5a 00 00 04 03 3f 3f 31 51 44 61 74 65 54 69
 	  69e0: 6d 65 40 40 51 45 41 41 40 58 5a 00 47 1b 3f 74
 	  69f0: 6f 4d 53 65 63 73 53 69 6e 63 65 45 70 6f 63 68
 	  6a00: 40 51 44 61 74 65 54 69 6d 65 40 40 51 45 42 41
-	  6a10: 5f 4a 58 5a 00 00 0a 0b 3f 63 75 72 72 65 6e 74
+	  6a10: 5f 4a 58 5a 00 00 0b 0b 3f 63 75 72 72 65 6e 74
 	  6a20: 44 61 74 65 54 69 6d 65 40 51 44 61 74 65 54 69
 	  6a30: 6d 65 40 40 53 41 3f 41 56 31 40 58 5a 00 5c 02
 	  6a40: 3f 3f 30 51 55 72 6c 51 75 65 72 79 40 40 51 45
 	  6a50: 41 41 40 58 5a 00 79 03 3f 3f 31 51 55 72 6c 51
 	  6a60: 75 65 72 79 40 40 51 45 41 41 40 58 5a 00 a4 1b
 	  6a70: 3f 74 6f 53 74 72 69 6e 67 40 51 55 72 6c 51 75
 	  6a80: 65 72 79 40 40 51 45 42 41 3f 41 56 51 53 74 72
 	  6a90: 69 6e 67 40 40 56 3f 24 51 46 6c 61 67 73 40 57
 	  6aa0: 34 43 6f 6d 70 6f 6e 65 6e 74 46 6f 72 6d 61 74
 	  6ab0: 74 69 6e 67 4f 70 74 69 6f 6e 40 51 55 72 6c 40
-	  6ac0: 40 40 40 40 5a 00 c5 07 3f 61 64 64 51 75 65 72
+	  6ac0: 40 40 40 40 5a 00 c6 07 3f 61 64 64 51 75 65 72
 	  6ad0: 79 49 74 65 6d 40 51 55 72 6c 51 75 65 72 79 40
 	  6ae0: 40 51 45 41 41 58 41 45 42 56 51 53 74 72 69 6e
 	  6af0: 67 40 40 30 40 5a 00 00 2c 03 3f 3f 31 51 4a 73
 	  6b00: 6f 6e 44 6f 63 75 6d 65 6e 74 40 40 51 45 41 41
-	  6b10: 40 58 5a 00 27 0e 3f 66 72 6f 6d 56 61 72 69 61
+	  6b10: 40 58 5a 00 28 0e 3f 66 72 6f 6d 56 61 72 69 61
 	  6b20: 6e 74 40 51 4a 73 6f 6e 44 6f 63 75 6d 65 6e 74
 	  6b30: 40 40 53 41 3f 41 56 31 40 41 45 42 56 51 56 61
 	  6b40: 72 69 61 6e 74 40 40 40 5a 00 17 1b 3f 74 6f 4a
 	  6b50: 73 6f 6e 40 51 4a 73 6f 6e 44 6f 63 75 6d 65 6e
 	  6b60: 74 40 40 51 45 42 41 3f 41 56 51 42 79 74 65 41
 	  6b70: 72 72 61 79 40 40 57 34 4a 73 6f 6e 46 6f 72 6d
-	  6b80: 61 74 40 31 40 40 5a 00 78 09 3f 63 68 69 6c 64
+	  6b80: 61 74 40 31 40 40 5a 00 79 09 3f 63 68 69 6c 64
 	  6b90: 45 76 65 6e 74 40 51 4f 62 6a 65 63 74 40 40 4d
 	  6ba0: 45 41 41 58 50 45 41 56 51 43 68 69 6c 64 45 76
-	  6bb0: 65 6e 74 40 40 40 5a 00 37 0a 3f 63 6f 6e 6e 65
+	  6bb0: 65 6e 74 40 40 40 5a 00 38 0a 3f 63 6f 6e 6e 65
 	  6bc0: 63 74 4e 6f 74 69 66 79 40 51 4f 62 6a 65 63 74
 	  6bd0: 40 40 4d 45 41 41 58 41 45 42 56 51 4d 65 74 61
-	  6be0: 4d 65 74 68 6f 64 40 40 40 5a 00 00 28 0b 3f 63
+	  6be0: 4d 65 74 68 6f 64 40 40 40 5a 00 00 29 0b 3f 63
 	  6bf0: 75 73 74 6f 6d 45 76 65 6e 74 40 51 4f 62 6a 65
 	  6c00: 63 74 40 40 4d 45 41 41 58 50 45 41 56 51 45 76
-	  6c10: 65 6e 74 40 40 40 5a 00 35 0c 3f 64 69 73 63 6f
+	  6c10: 65 6e 74 40 40 40 5a 00 36 0c 3f 64 69 73 63 6f
 	  6c20: 6e 6e 65 63 74 4e 6f 74 69 66 79 40 51 4f 62 6a
 	  6c30: 65 63 74 40 40 4d 45 41 41 58 41 45 42 56 51 4d
-	  6c40: 65 74 61 4d 65 74 68 6f 64 40 40 40 5a 00 ff 0c
+	  6c40: 65 74 61 4d 65 74 68 6f 64 40 40 40 5a 00 00 0d
 	  6c50: 3f 65 76 65 6e 74 40 51 4f 62 6a 65 63 74 40 40
 	  6c60: 55 45 41 41 5f 4e 50 45 41 56 51 45 76 65 6e 74
-	  6c70: 40 40 40 5a 00 00 0f 0d 3f 65 76 65 6e 74 46 69
+	  6c70: 40 40 40 5a 00 00 10 0d 3f 65 76 65 6e 74 46 69
 	  6c80: 6c 74 65 72 40 51 4f 62 6a 65 63 74 40 40 55 45
 	  6c90: 41 41 5f 4e 50 45 41 56 31 40 50 45 41 56 51 45
-	  6ca0: 76 65 6e 74 40 40 40 5a 00 00 b7 0d 3f 66 6c 61
+	  6ca0: 76 65 6e 74 40 40 40 5a 00 00 b8 0d 3f 66 6c 61
 	  6cb0: 67 73 46 6f 72 44 75 6d 70 69 6e 67 40 51 4f 62
 	  6cc0: 6a 65 63 74 50 72 69 76 61 74 65 40 40 55 45 42
 	  6cd0: 41 3f 41 56 3f 24 62 61 73 69 63 5f 73 74 72 69
 	  6ce0: 6e 67 40 44 55 3f 24 63 68 61 72 5f 74 72 61 69
 	  6cf0: 74 73 40 44 40 73 74 64 40 40 56 3f 24 61 6c 6c
 	  6d00: 6f 63 61 74 6f 72 40 44 40 32 40 40 73 74 64 40
 	  6d10: 40 58 5a 00 a4 1a 3f 74 69 6d 65 72 45 76 65 6e
 	  6d20: 74 40 51 4f 62 6a 65 63 74 40 40 4d 45 41 41 58
 	  6d30: 50 45 41 56 51 54 69 6d 65 72 45 76 65 6e 74 40
 	  6d40: 40 40 5a 00 70 01 3f 3f 30 51 4d 65 73 73 61 67
 	  6d50: 65 4c 6f 67 67 65 72 40 40 51 45 41 41 40 50 45
 	  6d60: 42 44 48 30 30 40 5a 00 37 1d 3f 77 61 72 6e 69
 	  6d70: 6e 67 40 51 4d 65 73 73 61 67 65 4c 6f 67 67 65
 	  6d80: 72 40 40 51 45 42 41 58 50 45 42 44 5a 5a 00 00
-	  6d90: 93 11 3f 6c 65 6e 67 74 68 48 65 6c 70 65 72 43
+	  6d90: 94 11 3f 6c 65 6e 67 74 68 48 65 6c 70 65 72 43
 	  6da0: 68 61 72 41 72 72 61 79 40 51 42 79 74 65 41 72
 	  6db0: 72 61 79 56 69 65 77 40 40 43 41 5f 4a 50 45 42
 	  6dc0: 44 5f 4b 40 5a 00 59 00 3f 3f 30 51 42 79 74 65
 	  6dd0: 41 72 72 61 79 40 40 51 45 41 41 40 50 45 42 44
-	  6de0: 5f 4a 40 5a 00 00 35 08 3f 61 72 67 40 51 53 74
+	  6de0: 5f 4a 40 5a 00 00 36 08 3f 61 72 67 40 51 53 74
 	  6df0: 72 69 6e 67 40 40 51 45 42 41 3f 41 56 31 40 41
 	  6e00: 45 42 56 31 40 48 56 51 43 68 61 72 40 40 40 5a
 	  6e10: 00 00 dd 1b 3f 74 6f 55 74 66 38 40 51 53 74 72
 	  6e20: 69 6e 67 40 40 51 45 47 42 41 3f 41 56 51 42 79
-	  6e30: 74 65 41 72 72 61 79 40 40 58 5a 00 25 0e 3f 66
+	  6e30: 74 65 41 72 72 61 79 40 40 58 5a 00 26 0e 3f 66
 	  6e40: 72 6f 6d 55 74 66 38 40 51 53 74 72 69 6e 67 40
 	  6e50: 40 53 41 3f 41 56 31 40 56 51 42 79 74 65 41 72
-	  6e60: 72 61 79 56 69 65 77 40 40 40 5a 00 1a 13 3f 6e
+	  6e60: 72 61 79 56 69 65 77 40 40 40 5a 00 1b 13 3f 6e
 	  6e70: 6f 72 6d 61 6c 69 7a 65 64 54 79 70 65 40 51 4d
 	  6e80: 65 74 61 4f 62 6a 65 63 74 40 40 53 41 3f 41 56
 	  6e90: 51 42 79 74 65 41 72 72 61 79 40 40 50 45 42 44
 	  6ea0: 40 5a 00 00 d5 02 3f 3f 31 43 6f 6e 6e 65 63 74
 	  6eb0: 69 6f 6e 40 51 4d 65 74 61 4f 62 6a 65 63 74 40
-	  6ec0: 40 51 45 41 41 40 58 5a 00 00 33 0a 3f 63 6f 6e
+	  6ec0: 40 51 45 41 41 40 58 5a 00 00 34 0a 3f 63 6f 6e
 	  6ed0: 6e 65 63 74 49 6d 70 6c 40 51 4f 62 6a 65 63 74
 	  6ee0: 40 40 43 41 3f 41 56 43 6f 6e 6e 65 63 74 69 6f
 	  6ef0: 6e 40 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 50
 	  6f00: 45 42 56 31 40 50 45 41 50 45 41 58 30 31 50 45
 	  6f10: 41 56 51 53 6c 6f 74 4f 62 6a 65 63 74 42 61 73
 	  6f20: 65 40 51 74 50 72 69 76 61 74 65 40 40 57 34 43
 	  6f30: 6f 6e 6e 65 63 74 69 6f 6e 54 79 70 65 40 51 74
@@ -6796,299 +6796,299 @@
 	  6f50: c7 00 3f 3f 30 51 44 61 74 65 54 69 6d 65 40 40
 	  6f60: 51 45 41 41 40 58 5a 00 c3 00 3f 3f 30 51 44 61
 	  6f70: 74 65 54 69 6d 65 40 40 51 45 41 41 40 41 45 42
 	  6f80: 56 30 40 40 5a 00 c2 00 3f 3f 30 51 44 61 74 65
 	  6f90: 54 69 6d 65 40 40 51 45 41 41 40 24 24 51 45 41
 	  6fa0: 56 30 40 40 5a 00 d5 03 3f 3f 34 51 44 61 74 65
 	  6fb0: 54 69 6d 65 40 40 51 45 41 41 41 45 41 56 30 40
-	  6fc0: 24 24 51 45 41 56 30 40 40 5a 00 00 ce 0c 3f 65
+	  6fc0: 24 24 51 45 41 56 30 40 40 5a 00 00 cf 0c 3f 65
 	  6fd0: 71 75 61 6c 73 40 51 44 61 74 65 54 69 6d 65 40
 	  6fe0: 40 41 45 42 41 5f 4e 41 45 42 56 31 40 40 5a 00
-	  6ff0: c8 13 3f 70 72 65 63 65 64 65 73 40 51 44 61 74
+	  6ff0: c9 13 3f 70 72 65 63 65 64 65 73 40 51 44 61 74
 	  7000: 65 54 69 6d 65 40 40 41 45 42 41 5f 4e 41 45 42
 	  7010: 56 31 40 40 5a 00 11 05 3f 3f 36 40 59 41 41 45
 	  7020: 41 56 51 44 61 74 61 53 74 72 65 61 6d 40 40 41
 	  7030: 45 41 56 30 40 41 45 42 56 51 44 61 74 65 54 69
 	  7040: 6d 65 40 40 40 5a 00 00 9e 04 3f 3f 35 40 59 41
 	  7050: 41 45 41 56 51 44 61 74 61 53 74 72 65 61 6d 40
 	  7060: 40 41 45 41 56 30 40 41 45 41 56 51 44 61 74 65
 	  7070: 54 69 6d 65 40 40 40 5a 00 00 e1 04 3f 3f 36 40
 	  7080: 59 41 3f 41 56 51 44 65 62 75 67 40 40 56 30 40
 	  7090: 41 45 42 56 51 44 61 74 65 54 69 6d 65 40 40 40
-	  70a0: 5a 00 6e 15 3f 71 75 65 72 79 40 51 55 72 6c 40
+	  70a0: 5a 00 6f 15 3f 71 75 65 72 79 40 51 55 72 6c 40
 	  70b0: 40 51 45 42 41 3f 41 56 51 53 74 72 69 6e 67 40
 	  70c0: 40 56 3f 24 51 46 6c 61 67 73 40 57 34 43 6f 6d
 	  70d0: 70 6f 6e 65 6e 74 46 6f 72 6d 61 74 74 69 6e 67
 	  70e0: 4f 70 74 69 6f 6e 40 51 55 72 6c 40 40 40 40 40
-	  70f0: 5a 00 22 11 3f 69 73 57 61 72 6e 69 6e 67 45 6e
+	  70f0: 5a 00 23 11 3f 69 73 57 61 72 6e 69 6e 67 45 6e
 	  7100: 61 62 6c 65 64 40 51 4c 6f 67 67 69 6e 67 43 61
 	  7110: 74 65 67 6f 72 79 40 40 51 45 42 41 5f 4e 58 5a
 	  7120: 00 00 59 02 3f 3f 30 51 55 72 6c 51 75 65 72 79
 	  7130: 40 40 51 45 41 41 40 41 45 42 56 51 53 74 72 69
 	  7140: 6e 67 40 40 40 5a 00 00 9d 01 3f 3f 30 51 4f 62
 	  7150: 6a 65 63 74 40 40 51 45 41 41 40 50 45 41 56 30
 	  7160: 40 40 5a 00 71 01 3f 3f 30 51 4d 65 73 73 61 67
 	  7170: 65 4c 6f 67 67 65 72 40 40 51 45 41 41 40 50 45
-	  7180: 42 44 48 30 40 5a 00 00 3d 0d 3f 66 61 74 61 6c
+	  7180: 42 44 48 30 40 5a 00 00 3e 0d 3f 66 61 74 61 6c
 	  7190: 40 51 4d 65 73 73 61 67 65 4c 6f 67 67 65 72 40
-	  71a0: 40 51 45 42 41 58 50 45 42 44 5a 5a 00 00 ee 07
+	  71a0: 40 51 45 42 41 58 50 45 42 44 5a 5a 00 00 ef 07
 	  71b0: 3f 61 6c 6c 6f 63 61 74 65 40 51 41 72 72 61 79
 	  71c0: 44 61 74 61 40 40 53 41 50 45 41 58 50 45 41 50
 	  71d0: 45 41 55 31 40 5f 4a 31 31 57 34 41 6c 6c 6f 63
 	  71e0: 61 74 69 6f 6e 4f 70 74 69 6f 6e 40 31 40 40 5a
-	  71f0: 00 00 c4 15 3f 72 65 61 6c 6c 6f 63 61 74 65 55
+	  71f0: 00 00 c5 15 3f 72 65 61 6c 6c 6f 63 61 74 65 55
 	  7200: 6e 61 6c 69 67 6e 65 64 40 51 41 72 72 61 79 44
 	  7210: 61 74 61 40 40 53 41 3f 41 55 3f 24 70 61 69 72
 	  7220: 40 50 45 41 55 51 41 72 72 61 79 44 61 74 61 40
 	  7230: 40 50 45 41 58 40 73 74 64 40 40 50 45 41 55 31
 	  7240: 40 50 45 41 58 5f 4a 32 57 34 41 6c 6c 6f 63 61
 	  7250: 74 69 6f 6e 4f 70 74 69 6f 6e 40 31 40 40 5a 00
-	  7260: 46 0a 3f 63 6f 6e 73 74 44 61 74 61 40 51 42 79
+	  7260: 47 0a 3f 63 6f 6e 73 74 44 61 74 61 40 51 42 79
 	  7270: 74 65 41 72 72 61 79 40 40 51 45 42 41 50 45 42
 	  7280: 44 58 5a 00 b8 1a 3f 74 6f 42 61 73 65 36 34 40
 	  7290: 51 42 79 74 65 41 72 72 61 79 40 40 51 45 42 41
 	  72a0: 3f 41 56 31 40 56 3f 24 51 46 6c 61 67 73 40 57
 	  72b0: 34 42 61 73 65 36 34 4f 70 74 69 6f 6e 40 51 42
 	  72c0: 79 74 65 41 72 72 61 79 40 40 40 40 40 5a 00 00
-	  72d0: 4e 09 3f 63 61 73 74 40 51 4d 65 74 61 4f 62 6a
+	  72d0: 4f 09 3f 63 61 73 74 40 51 4d 65 74 61 4f 62 6a
 	  72e0: 65 63 74 40 40 51 45 42 41 50 45 42 56 51 4f 62
 	  72f0: 6a 65 63 74 40 40 50 45 42 56 32 40 40 5a 00 00
 	  7300: 1d 00 3f 3f 30 43 6f 6e 6e 65 63 74 69 6f 6e 40
 	  7310: 51 4d 65 74 61 4f 62 6a 65 63 74 40 40 51 45 41
 	  7320: 41 40 58 5a 00 00 9d 03 3f 3f 34 43 6f 6e 6e 65
 	  7330: 63 74 69 6f 6e 40 51 4d 65 74 61 4f 62 6a 65 63
 	  7340: 74 40 40 51 45 41 41 41 45 41 56 30 31 40 24 24
 	  7350: 51 45 41 56 30 31 40 40 5a 00 9e 00 3f 3f 30 51
 	  7360: 43 68 61 72 40 40 51 45 41 41 40 55 51 4c 61 74
-	  7370: 69 6e 31 43 68 61 72 40 40 40 5a 00 9c 16 3f 72
+	  7370: 69 6e 31 43 68 61 72 40 40 40 5a 00 9d 16 3f 72
 	  7380: 65 73 69 7a 65 40 51 53 74 72 69 6e 67 40 40 51
-	  7390: 45 41 41 58 5f 4a 40 5a 00 00 37 09 3f 63 61 70
+	  7390: 45 41 41 58 5f 4a 40 5a 00 00 38 09 3f 63 61 70
 	  73a0: 61 63 69 74 79 40 51 53 74 72 69 6e 67 40 40 51
-	  73b0: 45 42 41 5f 4a 58 5a 00 82 16 3f 72 65 73 65 72
+	  73b0: 45 42 41 5f 4a 58 5a 00 83 16 3f 72 65 73 65 72
 	  73c0: 76 65 40 51 53 74 72 69 6e 67 40 40 51 45 41 41
-	  73d0: 58 5f 4a 40 5a 00 a4 0b 3f 64 61 74 61 40 51 53
+	  73d0: 58 5f 4a 40 5a 00 a5 0b 3f 64 61 74 61 40 51 53
 	  73e0: 74 72 69 6e 67 40 40 51 45 41 41 50 45 41 56 51
-	  73f0: 43 68 61 72 40 40 58 5a 00 00 49 0a 3f 63 6f 6e
+	  73f0: 43 68 61 72 40 40 58 5a 00 00 4a 0a 3f 63 6f 6e
 	  7400: 73 74 44 61 74 61 40 51 53 74 72 69 6e 67 40 40
 	  7410: 51 45 42 41 50 45 42 56 51 43 68 61 72 40 40 58
-	  7420: 5a 00 10 0c 3f 64 65 74 61 63 68 40 51 53 74 72
-	  7430: 69 6e 67 40 40 51 45 41 41 58 58 5a 00 00 9d 09
+	  7420: 5a 00 11 0c 3f 64 65 74 61 63 68 40 51 53 74 72
+	  7430: 69 6e 67 40 40 51 45 41 41 58 58 5a 00 00 9e 09
 	  7440: 3f 63 6c 65 61 72 40 51 53 74 72 69 6e 67 40 40
-	  7450: 51 45 41 41 58 58 5a 00 b2 19 3f 73 74 61 72 74
+	  7450: 51 45 41 41 58 58 5a 00 b3 19 3f 73 74 61 72 74
 	  7460: 73 57 69 74 68 40 51 53 74 72 69 6e 67 40 40 51
 	  7470: 45 42 41 5f 4e 41 45 42 56 31 40 57 34 43 61 73
 	  7480: 65 53 65 6e 73 69 74 69 76 69 74 79 40 51 74 40
-	  7490: 40 40 5a 00 21 08 3f 61 70 70 65 6e 64 40 51 53
+	  7490: 40 40 5a 00 22 08 3f 61 70 70 65 6e 64 40 51 53
 	  74a0: 74 72 69 6e 67 40 40 51 45 41 41 41 45 41 56 31
 	  74b0: 40 56 51 4c 61 74 69 6e 31 53 74 72 69 6e 67 40
 	  74c0: 40 40 5a 00 2b 1b 3f 74 6f 4c 6f 63 61 6c 38 42
 	  74d0: 69 74 40 51 53 74 72 69 6e 67 40 40 51 45 47 42
 	  74e0: 41 3f 41 56 51 42 79 74 65 41 72 72 61 79 40 40
-	  74f0: 58 5a 00 00 3d 13 3f 6e 75 6d 62 65 72 40 51 53
+	  74f0: 58 5a 00 00 3e 13 3f 6e 75 6d 62 65 72 40 51 53
 	  7500: 74 72 69 6e 67 40 40 53 41 3f 41 56 31 40 5f 4a
-	  7510: 48 40 5a 00 27 08 3f 61 70 70 65 6e 64 4c 61 74
+	  7510: 48 40 5a 00 28 08 3f 61 70 70 65 6e 64 4c 61 74
 	  7520: 69 6e 31 54 6f 40 51 41 62 73 74 72 61 63 74 43
 	  7530: 6f 6e 63 61 74 65 6e 61 62 6c 65 40 40 4b 41 58
 	  7540: 56 51 4c 61 74 69 6e 31 53 74 72 69 6e 67 40 40
-	  7550: 50 45 41 56 51 43 68 61 72 40 40 40 5a 00 e0 0f
+	  7550: 50 45 41 56 51 43 68 61 72 40 40 40 5a 00 e1 0f
 	  7560: 3f 69 73 45 6d 70 74 79 40 51 55 72 6c 40 40 51
 	  7570: 45 42 41 5f 4e 58 5a 00 58 1b 3f 74 6f 50 65 72
 	  7580: 63 65 6e 74 45 6e 63 6f 64 69 6e 67 40 51 55 72
 	  7590: 6c 40 40 53 41 3f 41 56 51 42 79 74 65 41 72 72
 	  75a0: 61 79 40 40 41 45 42 56 51 53 74 72 69 6e 67 40
-	  75b0: 40 41 45 42 56 32 40 31 40 5a 00 00 2d 0c 3f 64
+	  75b0: 40 41 45 42 56 32 40 31 40 5a 00 00 2e 0c 3f 64
 	  75c0: 69 73 63 6f 6e 6e 65 63 74 40 51 4f 62 6a 65 63
 	  75d0: 74 40 40 53 41 5f 4e 41 45 42 56 43 6f 6e 6e 65
 	  75e0: 63 74 69 6f 6e 40 51 4d 65 74 61 4f 62 6a 65 63
-	  75f0: 74 40 40 40 5a 00 f6 0b 3f 64 65 6c 65 74 65 4c
+	  75f0: 74 40 40 40 5a 00 f7 0b 3f 64 65 6c 65 74 65 4c
 	  7600: 61 74 65 72 40 51 4f 62 6a 65 63 74 40 40 51 45
 	  7610: 41 41 58 58 5a 00 99 02 3f 3f 30 51 56 61 72 69
 	  7620: 61 6e 74 40 40 51 45 41 41 40 5f 4e 40 5a 00 00
 	  7630: 6c 02 3f 3f 30 51 56 61 72 69 61 6e 74 40 40 51
 	  7640: 45 41 41 40 41 45 42 56 51 42 79 74 65 41 72 72
 	  7650: 61 79 40 40 40 5a 00 00 65 02 3f 3f 30 51 56 61
 	  7660: 72 69 61 6e 74 40 40 51 45 41 41 40 24 24 51 45
 	  7670: 41 56 30 40 40 5a 00 00 bf 1a 3f 74 6f 42 6f 6f
 	  7680: 6c 40 51 56 61 72 69 61 6e 74 40 40 51 45 42 41
 	  7690: 5f 4e 58 5a 00 00 c4 1a 3f 74 6f 42 79 74 65 41
 	  76a0: 72 72 61 79 40 51 56 61 72 69 61 6e 74 40 40 51
 	  76b0: 45 42 41 3f 41 56 51 42 79 74 65 41 72 72 61 79
 	  76c0: 40 40 58 5a 00 00 67 1b 3f 74 6f 53 65 63 73 53
 	  76d0: 69 6e 63 65 45 70 6f 63 68 40 51 44 61 74 65 54
-	  76e0: 69 6d 65 40 40 51 45 42 41 5f 4a 58 5a 00 0b 0b
+	  76e0: 69 6d 65 40 40 51 45 42 41 5f 4a 58 5a 00 0c 0b
 	  76f0: 3f 63 75 72 72 65 6e 74 44 61 74 65 54 69 6d 65
 	  7700: 55 74 63 40 51 44 61 74 65 54 69 6d 65 40 40 53
-	  7710: 41 3f 41 56 31 40 58 5a 00 00 38 0e 3f 67 65 74
+	  7710: 41 3f 41 56 31 40 58 5a 00 00 39 0e 3f 67 65 74
 	  7720: 40 51 4f 62 6a 65 63 74 50 72 69 76 61 74 65 40
 	  7730: 40 53 41 50 45 41 56 31 40 50 45 41 56 51 4f 62
-	  7740: 6a 65 63 74 40 40 40 5a 00 00 71 15 3f 71 75 65
+	  7740: 6a 65 63 74 40 40 40 5a 00 00 72 15 3f 71 75 65
 	  7750: 72 79 49 74 65 6d 73 40 51 55 72 6c 51 75 65 72
 	  7760: 79 40 40 51 45 42 41 3f 41 56 3f 24 51 4c 69 73
 	  7770: 74 40 55 3f 24 70 61 69 72 40 56 51 53 74 72 69
 	  7780: 6e 67 40 40 56 31 40 40 73 74 64 40 40 40 40 56
 	  7790: 3f 24 51 46 6c 61 67 73 40 57 34 43 6f 6d 70 6f
 	  77a0: 6e 65 6e 74 46 6f 72 6d 61 74 74 69 6e 67 4f 70
 	  77b0: 74 69 6f 6e 40 51 55 72 6c 40 40 40 40 40 5a 00
-	  77c0: fd 0a 3f 63 72 69 74 69 63 61 6c 40 51 4d 65 73
+	  77c0: fe 0a 3f 63 72 69 74 69 63 61 6c 40 51 4d 65 73
 	  77d0: 73 61 67 65 4c 6f 67 67 65 72 40 40 51 45 42 41
 	  77e0: 58 50 45 42 44 5a 5a 00 5c 00 3f 3f 30 51 42 79
 	  77f0: 74 65 41 72 72 61 79 40 40 51 45 41 41 40 5f 4a
 	  7800: 57 34 49 6e 69 74 69 61 6c 69 7a 61 74 69 6f 6e
 	  7810: 40 51 74 40 40 40 5a 00 b6 03 3f 3f 34 51 42 79
 	  7820: 74 65 41 72 72 61 79 40 40 51 45 41 41 41 45 41
-	  7830: 56 30 40 41 45 42 56 30 40 40 5a 00 cf 0f 3f 69
+	  7830: 56 30 40 41 45 42 56 30 40 40 5a 00 d0 0f 3f 69
 	  7840: 73 45 6d 70 74 79 40 51 42 79 74 65 41 72 72 61
-	  7850: 79 40 40 51 45 42 41 5f 4e 58 5a 00 97 16 3f 72
+	  7850: 79 40 40 51 45 42 41 5f 4e 58 5a 00 98 16 3f 72
 	  7860: 65 73 69 7a 65 40 51 42 79 74 65 41 72 72 61 79
-	  7870: 40 40 51 45 41 41 58 5f 4a 40 5a 00 36 09 3f 63
+	  7870: 40 40 51 45 41 41 58 5f 4a 40 5a 00 37 09 3f 63
 	  7880: 61 70 61 63 69 74 79 40 51 42 79 74 65 41 72 72
-	  7890: 61 79 40 40 51 45 42 41 5f 4a 58 5a 00 00 99 0b
+	  7890: 61 79 40 40 51 45 42 41 5f 4a 58 5a 00 00 9a 0b
 	  78a0: 3f 64 61 74 61 40 51 42 79 74 65 41 72 72 61 79
-	  78b0: 40 40 51 45 41 41 50 45 41 44 58 5a 00 00 07 0c
+	  78b0: 40 40 51 45 41 41 50 45 41 44 58 5a 00 00 08 0c
 	  78c0: 3f 64 65 74 61 63 68 40 51 42 79 74 65 41 72 72
-	  78d0: 61 79 40 40 51 45 41 41 58 58 5a 00 fe 07 3f 61
+	  78d0: 61 79 40 40 51 45 41 41 58 58 5a 00 ff 07 3f 61
 	  78e0: 70 70 65 6e 64 40 51 42 79 74 65 41 72 72 61 79
 	  78f0: 40 40 51 45 41 41 41 45 41 56 31 40 41 45 42 56
-	  7900: 31 40 40 5a 00 00 7c 0c 3f 65 6e 64 40 51 42 79
+	  7900: 31 40 40 5a 00 00 7d 0c 3f 65 6e 64 40 51 42 79
 	  7910: 74 65 41 72 72 61 79 40 40 51 45 42 41 50 45 42
-	  7920: 44 58 5a 00 6e 16 3f 72 65 70 6c 61 63 65 40 51
+	  7920: 44 58 5a 00 6f 16 3f 72 65 70 6c 61 63 65 40 51
 	  7930: 53 74 72 69 6e 67 40 40 51 45 41 41 41 45 41 56
 	  7940: 31 40 56 51 43 68 61 72 40 40 30 57 34 43 61 73
 	  7950: 65 53 65 6e 73 69 74 69 76 69 74 79 40 51 74 40
-	  7960: 40 40 5a 00 e4 0d 3f 66 72 6f 6d 4c 61 74 69 6e
+	  7960: 40 40 5a 00 e5 0d 3f 66 72 6f 6d 4c 61 74 69 6e
 	  7970: 31 40 51 53 74 72 69 6e 67 40 40 53 41 3f 41 56
 	  7980: 31 40 56 51 42 79 74 65 41 72 72 61 79 56 69 65
 	  7990: 77 40 40 40 5a 00 a3 1b 3f 74 6f 53 74 72 69 6e
 	  79a0: 67 40 51 55 72 6c 40 40 51 45 42 41 3f 41 56 51
 	  79b0: 53 74 72 69 6e 67 40 40 56 3f 24 51 55 72 6c 54
 	  79c0: 77 6f 46 6c 61 67 73 40 57 34 55 72 6c 46 6f 72
 	  79d0: 6d 61 74 74 69 6e 67 4f 70 74 69 6f 6e 40 51 55
 	  79e0: 72 6c 40 40 57 34 43 6f 6d 70 6f 6e 65 6e 74 46
 	  79f0: 6f 72 6d 61 74 74 69 6e 67 4f 70 74 69 6f 6e 40
-	  7a00: 32 40 40 40 40 5a 00 00 a9 0f 3f 69 73 43 72 69
+	  7a00: 32 40 40 40 40 5a 00 00 aa 0f 3f 69 73 43 72 69
 	  7a10: 74 69 63 61 6c 45 6e 61 62 6c 65 64 40 51 4c 6f
 	  7a20: 67 67 69 6e 67 43 61 74 65 67 6f 72 79 40 40 51
-	  7a30: 45 42 41 5f 4e 58 5a 00 a1 0e 3f 68 61 73 68 40
+	  7a30: 45 42 41 5f 4e 58 5a 00 a2 0e 3f 68 61 73 68 40
 	  7a40: 51 4d 65 73 73 61 67 65 41 75 74 68 65 6e 74 69
 	  7a50: 63 61 74 69 6f 6e 43 6f 64 65 40 40 53 41 3f 41
 	  7a60: 56 51 42 79 74 65 41 72 72 61 79 40 40 41 45 42
 	  7a70: 56 32 40 30 57 34 41 6c 67 6f 72 69 74 68 6d 40
 	  7a80: 51 43 72 79 70 74 6f 67 72 61 70 68 69 63 48 61
-	  7a90: 73 68 40 40 40 5a 00 00 dd 0b 3f 64 65 62 75 67
+	  7a90: 73 68 40 40 40 5a 00 00 de 0b 3f 64 65 62 75 67
 	  7aa0: 40 51 4d 65 73 73 61 67 65 4c 6f 67 67 65 72 40
 	  7ab0: 40 51 45 42 41 58 50 45 42 44 5a 5a 00 00 2c 1b
 	  7ac0: 3f 74 6f 4c 6f 63 61 6c 38 42 69 74 40 51 53 74
 	  7ad0: 72 69 6e 67 40 40 51 45 48 41 41 3f 41 56 51 42
-	  7ae0: 79 74 65 41 72 72 61 79 40 40 58 5a 00 00 18 11
+	  7ae0: 79 74 65 41 72 72 61 79 40 40 58 5a 00 00 19 11
 	  7af0: 3f 69 73 56 61 6c 69 64 40 51 56 61 72 69 61 6e
 	  7b00: 74 40 40 51 45 42 41 5f 4e 58 5a 00 0f 1b 3f 74
 	  7b10: 6f 49 6e 74 40 51 56 61 72 69 61 6e 74 40 40 51
-	  7b20: 45 42 41 48 50 45 41 5f 4e 40 5a 00 ca 07 3f 61
+	  7b20: 45 42 41 48 50 45 41 5f 4e 40 5a 00 cb 07 3f 61
 	  7b30: 64 64 53 65 63 73 40 51 44 61 74 65 54 69 6d 65
 	  7b40: 40 40 51 45 42 41 3f 41 56 31 40 5f 4a 40 5a 00
-	  7b50: 0e 17 3f 73 65 63 73 54 6f 40 51 44 61 74 65 54
+	  7b50: 0f 17 3f 73 65 63 73 54 6f 40 51 44 61 74 65 54
 	  7b60: 69 6d 65 40 40 51 45 42 41 5f 4a 41 45 42 56 31
 	  7b70: 40 40 5a 00 55 02 3f 3f 30 51 55 72 6c 40 40 51
 	  7b80: 45 41 41 40 41 45 42 56 51 53 74 72 69 6e 67 40
 	  7b90: 40 57 34 50 61 72 73 69 6e 67 4d 6f 64 65 40 30
-	  7ba0: 40 40 5a 00 b2 0f 3f 69 73 44 65 62 75 67 45 6e
+	  7ba0: 40 40 5a 00 b3 0f 3f 69 73 44 65 62 75 67 45 6e
 	  7bb0: 61 62 6c 65 64 40 51 4c 6f 67 67 69 6e 67 43 61
 	  7bc0: 74 65 67 6f 72 79 40 40 51 45 42 41 5f 4e 58 5a
 	  7bd0: 00 00 7b 04 3f 3f 34 51 55 72 6c 51 75 65 72 79
 	  7be0: 40 40 51 45 41 41 41 45 41 56 30 40 24 24 51 45
-	  7bf0: 41 56 30 40 40 5a 00 00 92 09 3f 63 6c 65 61 72
+	  7bf0: 41 56 30 40 40 5a 00 00 93 09 3f 63 6c 65 61 72
 	  7c00: 40 51 42 79 74 65 41 72 72 61 79 40 40 51 45 41
-	  7c10: 41 58 58 5a 00 00 50 08 3f 61 74 40 51 42 79 74
+	  7c10: 41 58 58 5a 00 00 51 08 3f 61 74 40 51 42 79 74
 	  7c20: 65 41 72 72 61 79 40 40 51 45 42 41 44 5f 4a 40
-	  7c30: 5a 00 da 0e 3f 69 6e 64 65 78 4f 66 40 51 42 79
+	  7c30: 5a 00 db 0e 3f 69 6e 64 65 78 4f 66 40 51 42 79
 	  7c40: 74 65 41 72 72 61 79 40 40 51 45 42 41 5f 4a 44
-	  7c50: 5f 4a 40 5a 00 00 65 12 3f 6d 69 64 40 51 42 79
+	  7c50: 5f 4a 40 5a 00 00 66 12 3f 6d 69 64 40 51 42 79
 	  7c60: 74 65 41 72 72 61 79 40 40 51 45 42 41 3f 41 56
-	  7c70: 31 40 5f 4a 30 40 5a 00 af 19 3f 73 74 61 72 74
+	  7c70: 31 40 5f 4a 30 40 5a 00 b0 19 3f 73 74 61 72 74
 	  7c80: 73 57 69 74 68 40 51 42 79 74 65 41 72 72 61 79
 	  7c90: 40 40 51 45 42 41 5f 4e 56 51 42 79 74 65 41 72
-	  7ca0: 72 61 79 56 69 65 77 40 40 40 5a 00 a0 0c 3f 65
+	  7ca0: 72 61 79 56 69 65 77 40 40 40 5a 00 a1 0c 3f 65
 	  7cb0: 6e 64 73 57 69 74 68 40 51 42 79 74 65 41 72 72
 	  7cc0: 61 79 40 40 51 45 42 41 5f 4e 56 51 42 79 74 65
-	  7cd0: 41 72 72 61 79 56 69 65 77 40 40 40 5a 00 7d 09
+	  7cd0: 41 72 72 61 79 56 69 65 77 40 40 40 5a 00 7e 09
 	  7ce0: 3f 63 68 6f 70 40 51 42 79 74 65 41 72 72 61 79
 	  7cf0: 40 40 51 45 41 41 58 5f 4a 40 5a 00 55 1c 3f 74
 	  7d00: 72 69 6d 6d 65 64 40 51 42 79 74 65 41 72 72 61
 	  7d10: 79 40 40 51 45 48 41 41 3f 41 56 31 40 58 5a 00
-	  7d20: 36 13 3f 6e 75 6d 62 65 72 40 51 42 79 74 65 41
+	  7d20: 37 13 3f 6e 75 6d 62 65 72 40 51 42 79 74 65 41
 	  7d30: 72 72 61 79 40 40 53 41 3f 41 56 31 40 5f 4a 48
 	  7d40: 40 5a 00 00 55 00 3f 3f 30 51 42 79 74 65 41 72
 	  7d50: 72 61 79 40 40 51 45 41 41 40 24 24 51 45 41 55
 	  7d60: 3f 24 51 41 72 72 61 79 44 61 74 61 50 6f 69 6e
-	  7d70: 74 65 72 40 44 40 40 40 5a 00 38 08 3f 61 72 67
+	  7d70: 74 65 72 40 44 40 40 40 5a 00 39 08 3f 61 72 67
 	  7d80: 40 51 53 74 72 69 6e 67 40 40 51 45 42 41 3f 41
 	  7d90: 56 31 40 47 48 48 56 51 43 68 61 72 40 40 40 5a
-	  7da0: 00 00 68 12 3f 6d 69 64 40 51 53 74 72 69 6e 67
+	  7da0: 00 00 69 12 3f 6d 69 64 40 51 53 74 72 69 6e 67
 	  7db0: 40 40 51 45 42 41 3f 41 56 31 40 5f 4a 30 40 5a
-	  7dc0: 00 00 b3 19 3f 73 74 61 72 74 73 57 69 74 68 40
+	  7dc0: 00 00 b4 19 3f 73 74 61 72 74 73 57 69 74 68 40
 	  7dd0: 51 53 74 72 69 6e 67 40 40 51 45 42 41 5f 4e 56
 	  7de0: 51 43 68 61 72 40 40 57 34 43 61 73 65 53 65 6e
 	  7df0: 73 69 74 69 76 69 74 79 40 51 74 40 40 40 5a 00
-	  7e00: 38 13 3f 6e 75 6d 62 65 72 40 51 53 74 72 69 6e
+	  7e00: 39 13 3f 6e 75 6d 62 65 72 40 51 53 74 72 69 6e
 	  7e10: 67 40 40 53 41 3f 41 56 31 40 48 48 40 5a 00 00
 	  7e20: 10 02 3f 3f 30 51 53 74 72 69 6e 67 40 40 51 45
 	  7e30: 41 41 40 5f 4a 57 34 49 6e 69 74 69 61 6c 69 7a
-	  7e40: 61 74 69 6f 6e 40 51 74 40 40 40 5a 00 00 d7 18
+	  7e40: 61 74 69 6f 6e 40 51 74 40 40 40 5a 00 00 d8 18
 	  7e50: 3f 73 65 74 55 72 6c 40 51 55 72 6c 40 40 51 45
 	  7e60: 41 41 58 41 45 42 56 51 53 74 72 69 6e 67 40 40
 	  7e70: 57 34 50 61 72 73 69 6e 67 4d 6f 64 65 40 31 40
-	  7e80: 40 5a 00 00 17 11 3f 69 73 56 61 6c 69 64 40 51
-	  7e90: 55 72 6c 40 40 51 45 42 41 5f 4e 58 5a 00 94 13
+	  7e80: 40 5a 00 00 18 11 3f 69 73 56 61 6c 69 64 40 51
+	  7e90: 55 72 6c 40 40 51 45 42 41 5f 4e 58 5a 00 95 13
 	  7ea0: 3f 70 61 74 68 40 51 55 72 6c 40 40 51 45 42 41
 	  7eb0: 3f 41 56 51 53 74 72 69 6e 67 40 40 56 3f 24 51
 	  7ec0: 46 6c 61 67 73 40 57 34 43 6f 6d 70 6f 6e 65 6e
 	  7ed0: 74 46 6f 72 6d 61 74 74 69 6e 67 4f 70 74 69 6f
 	  7ee0: 6e 40 51 55 72 6c 40 40 40 40 40 5a 00 00 1f 1c
 	  7ef0: 3f 74 72 40 51 4f 62 6a 65 63 74 40 40 53 41 3f
 	  7f00: 41 56 51 53 74 72 69 6e 67 40 40 50 45 42 44 30
 	  7f10: 48 40 5a 00 52 1d 3f 77 72 69 74 65 40 51 49 4f
 	  7f20: 44 65 76 69 63 65 40 40 51 45 41 41 5f 4a 41 45
 	  7f30: 42 56 51 42 79 74 65 41 72 72 61 79 40 40 40 5a
-	  7f40: 00 00 3f 0e 3f 67 65 74 43 68 61 72 40 51 49 4f
+	  7f40: 00 00 40 0e 3f 67 65 74 43 68 61 72 40 51 49 4f
 	  7f50: 44 65 76 69 63 65 40 40 51 45 41 41 5f 4e 50 45
-	  7f60: 41 44 40 5a 00 00 b9 15 3f 72 65 61 64 79 52 65
+	  7f60: 41 44 40 5a 00 00 ba 15 3f 72 65 61 64 79 52 65
 	  7f70: 61 64 40 51 49 4f 44 65 76 69 63 65 40 40 51 45
-	  7f80: 41 41 58 58 5a 00 2e 08 3f 61 70 70 6c 69 63 61
+	  7f80: 41 41 58 58 5a 00 2f 08 3f 61 70 70 6c 69 63 61
 	  7f90: 74 69 6f 6e 4e 61 6d 65 40 51 43 6f 72 65 41 70
 	  7fa0: 70 6c 69 63 61 74 69 6f 6e 40 40 53 41 3f 41 56
-	  7fb0: 51 53 74 72 69 6e 67 40 40 58 5a 00 46 0f 3f 69
+	  7fb0: 51 53 74 72 69 6e 67 40 40 58 5a 00 47 0f 3f 69
 	  7fc0: 6e 73 74 61 6e 63 65 40 51 43 6f 72 65 41 70 70
 	  7fd0: 6c 69 63 61 74 69 6f 6e 40 40 53 41 50 45 41 56
 	  7fe0: 31 40 58 5a 00 00 e2 19 3f 73 74 61 74 69 63 4d
 	  7ff0: 65 74 61 4f 62 6a 65 63 74 40 51 49 4f 44 65 76
 	  8000: 69 63 65 40 40 32 55 51 4d 65 74 61 4f 62 6a 65
-	  8010: 63 74 40 40 42 00 56 10 3f 69 73 4e 75 6c 6c 40
+	  8010: 63 74 40 40 42 00 57 10 3f 69 73 4e 75 6c 6c 40
 	  8020: 51 56 61 72 69 61 6e 74 40 40 51 45 42 41 5f 4e
 	  8030: 58 5a 00 00 2d 03 3f 3f 31 51 4a 73 6f 6e 4f 62
 	  8040: 6a 65 63 74 40 40 51 45 41 41 40 58 5a 00 ef 1b
 	  8050: 3f 74 6f 56 61 72 69 61 6e 74 4d 61 70 40 51 4a
 	  8060: 73 6f 6e 4f 62 6a 65 63 74 40 40 51 45 42 41 3f
 	  8070: 41 56 3f 24 51 4d 61 70 40 56 51 53 74 72 69 6e
 	  8080: 67 40 40 56 51 56 61 72 69 61 6e 74 40 40 40 40
-	  8090: 58 5a 00 00 d7 0f 3f 69 73 45 6d 70 74 79 40 51
+	  8090: 58 5a 00 00 d8 0f 3f 69 73 45 6d 70 74 79 40 51
 	  80a0: 4a 73 6f 6e 4f 62 6a 65 63 74 40 40 51 45 42 41
-	  80b0: 5f 4e 58 5a 00 00 db 0d 3f 66 72 6f 6d 4a 73 6f
+	  80b0: 5f 4e 58 5a 00 00 dc 0d 3f 66 72 6f 6d 4a 73 6f
 	  80c0: 6e 40 51 4a 73 6f 6e 44 6f 63 75 6d 65 6e 74 40
 	  80d0: 40 53 41 3f 41 56 31 40 41 45 42 56 51 42 79 74
 	  80e0: 65 41 72 72 61 79 40 40 50 45 41 55 51 4a 73 6f
 	  80f0: 6e 50 61 72 73 65 45 72 72 6f 72 40 40 40 5a 00
-	  8100: 5a 10 3f 69 73 4f 62 6a 65 63 74 40 51 4a 73 6f
+	  8100: 5b 10 3f 69 73 4f 62 6a 65 63 74 40 51 4a 73 6f
 	  8110: 6e 44 6f 63 75 6d 65 6e 74 40 40 51 45 42 41 5f
-	  8120: 4e 58 5a 00 42 13 3f 6f 62 6a 65 63 74 40 51 4a
+	  8120: 4e 58 5a 00 43 13 3f 6f 62 6a 65 63 74 40 51 4a
 	  8130: 73 6f 6e 44 6f 63 75 6d 65 6e 74 40 40 51 45 42
 	  8140: 41 3f 41 56 51 4a 73 6f 6e 4f 62 6a 65 63 74 40
-	  8150: 40 58 5a 00 95 15 3f 72 65 61 64 41 6c 6c 40 51
+	  8150: 40 58 5a 00 96 15 3f 72 65 61 64 41 6c 6c 40 51
 	  8160: 49 4f 44 65 76 69 63 65 40 40 51 45 41 41 3f 41
 	  8170: 56 51 42 79 74 65 41 72 72 61 79 40 40 58 5a 00
-	  8180: e9 0c 3f 65 72 72 6f 72 53 74 72 69 6e 67 40 51
+	  8180: ea 0c 3f 65 72 72 6f 72 53 74 72 69 6e 67 40 51
 	  8190: 49 4f 44 65 76 69 63 65 40 40 51 45 42 41 3f 41
 	  81a0: 56 51 53 74 72 69 6e 67 40 40 58 5a 00 00 51 74
 	  81b0: 36 43 6f 72 65 2e 64 6c 6c 00 8e 02 3f 5f 58 6c
 	  81c0: 65 6e 67 74 68 5f 65 72 72 6f 72 40 73 74 64 40
 	  81d0: 40 59 41 58 50 45 42 44 40 5a 00 00 8c 02 3f 5f
 	  81e0: 58 62 61 64 5f 66 75 6e 63 74 69 6f 6e 5f 63 61
 	  81f0: 6c 6c 40 73 74 64 40 40 59 41 58 58 5a 00 4d 53
@@ -7275,15 +7275,15 @@
 	reloc   14 offset  698 [1c698] DIR64
 	reloc   15 offset  6f8 [1c6f8] DIR64
 	reloc   16 offset  700 [1c700] DIR64
 	reloc   17 offset  708 [1c708] DIR64
 	reloc   18 offset  710 [1c710] DIR64
 	reloc   19 offset  720 [1c720] DIR64
 
-Virtual Address: 0001d000 Chunk size 236 (0xec) Number of fixups 114
+Virtual Address: 0001d000 Chunk size 368 (0x170) Number of fixups 180
 	reloc    0 offset   20 [1d020] DIR64
 	reloc    1 offset   28 [1d028] DIR64
 	reloc    2 offset   30 [1d030] DIR64
 	reloc    3 offset   38 [1d038] DIR64
 	reloc    4 offset   40 [1d040] DIR64
 	reloc    5 offset   48 [1d048] DIR64
 	reloc    6 offset   50 [1d050] DIR64
@@ -7384,254 +7384,254 @@
 	reloc  101 offset  788 [1d788] DIR64
 	reloc  102 offset  790 [1d790] DIR64
 	reloc  103 offset  798 [1d798] DIR64
 	reloc  104 offset  7a0 [1d7a0] DIR64
 	reloc  105 offset  7a8 [1d7a8] DIR64
 	reloc  106 offset  7b0 [1d7b0] DIR64
 	reloc  107 offset  7b8 [1d7b8] DIR64
-	reloc  108 offset  a78 [1da78] DIR64
-	reloc  109 offset  a80 [1da80] DIR64
-	reloc  110 offset  a88 [1da88] DIR64
-	reloc  111 offset  a90 [1da90] DIR64
-	reloc  112 offset  aa0 [1daa0] DIR64
-	reloc  113 offset    0 [1d000] ABSOLUTE
+	reloc  108 offset  d30 [1dd30] DIR64
+	reloc  109 offset  d38 [1dd38] DIR64
+	reloc  110 offset  d40 [1dd40] DIR64
+	reloc  111 offset  d48 [1dd48] DIR64
+	reloc  112 offset  d50 [1dd50] DIR64
+	reloc  113 offset  d58 [1dd58] DIR64
+	reloc  114 offset  d60 [1dd60] DIR64
+	reloc  115 offset  d68 [1dd68] DIR64
+	reloc  116 offset  d70 [1dd70] DIR64
+	reloc  117 offset  d78 [1dd78] DIR64
+	reloc  118 offset  d80 [1dd80] DIR64
+	reloc  119 offset  d88 [1dd88] DIR64
+	reloc  120 offset  d90 [1dd90] DIR64
+	reloc  121 offset  d98 [1dd98] DIR64
+	reloc  122 offset  da0 [1dda0] DIR64
+	reloc  123 offset  da8 [1dda8] DIR64
+	reloc  124 offset  db0 [1ddb0] DIR64
+	reloc  125 offset  db8 [1ddb8] DIR64
+	reloc  126 offset  dc0 [1ddc0] DIR64
+	reloc  127 offset  dc8 [1ddc8] DIR64
+	reloc  128 offset  dd0 [1ddd0] DIR64
+	reloc  129 offset  dd8 [1ddd8] DIR64
+	reloc  130 offset  de0 [1dde0] DIR64
+	reloc  131 offset  de8 [1dde8] DIR64
+	reloc  132 offset  df0 [1ddf0] DIR64
+	reloc  133 offset  df8 [1ddf8] DIR64
+	reloc  134 offset  e00 [1de00] DIR64
+	reloc  135 offset  e08 [1de08] DIR64
+	reloc  136 offset  e10 [1de10] DIR64
+	reloc  137 offset  e18 [1de18] DIR64
+	reloc  138 offset  e20 [1de20] DIR64
+	reloc  139 offset  e28 [1de28] DIR64
+	reloc  140 offset  e30 [1de30] DIR64
+	reloc  141 offset  e38 [1de38] DIR64
+	reloc  142 offset  e40 [1de40] DIR64
+	reloc  143 offset  e48 [1de48] DIR64
+	reloc  144 offset  e50 [1de50] DIR64
+	reloc  145 offset  e58 [1de58] DIR64
+	reloc  146 offset  e60 [1de60] DIR64
+	reloc  147 offset  e68 [1de68] DIR64
+	reloc  148 offset  e70 [1de70] DIR64
+	reloc  149 offset  e78 [1de78] DIR64
+	reloc  150 offset  e80 [1de80] DIR64
+	reloc  151 offset  e88 [1de88] DIR64
+	reloc  152 offset  e90 [1de90] DIR64
+	reloc  153 offset  e98 [1de98] DIR64
+	reloc  154 offset  ea0 [1dea0] DIR64
+	reloc  155 offset  ea8 [1dea8] DIR64
+	reloc  156 offset  eb0 [1deb0] DIR64
+	reloc  157 offset  eb8 [1deb8] DIR64
+	reloc  158 offset  ec0 [1dec0] DIR64
+	reloc  159 offset  ec8 [1dec8] DIR64
+	reloc  160 offset  ed0 [1ded0] DIR64
+	reloc  161 offset  ed8 [1ded8] DIR64
+	reloc  162 offset  ee0 [1dee0] DIR64
+	reloc  163 offset  ee8 [1dee8] DIR64
+	reloc  164 offset  ef0 [1def0] DIR64
+	reloc  165 offset  ef8 [1def8] DIR64
+	reloc  166 offset  f00 [1df00] DIR64
+	reloc  167 offset  f08 [1df08] DIR64
+	reloc  168 offset  f10 [1df10] DIR64
+	reloc  169 offset  f18 [1df18] DIR64
+	reloc  170 offset  f20 [1df20] DIR64
+	reloc  171 offset  f28 [1df28] DIR64
+	reloc  172 offset  f30 [1df30] DIR64
+	reloc  173 offset  f38 [1df38] DIR64
+	reloc  174 offset  f40 [1df40] DIR64
+	reloc  175 offset  f48 [1df48] DIR64
+	reloc  176 offset  f50 [1df50] DIR64
+	reloc  177 offset  f58 [1df58] DIR64
+	reloc  178 offset  f60 [1df60] DIR64
+	reloc  179 offset    0 [1d000] ABSOLUTE
 
-Virtual Address: 0001e000 Chunk size 360 (0x168) Number of fixups 176
-	reloc    0 offset  260 [1e260] DIR64
-	reloc    1 offset  268 [1e268] DIR64
-	reloc    2 offset  270 [1e270] DIR64
-	reloc    3 offset  278 [1e278] DIR64
-	reloc    4 offset  280 [1e280] DIR64
-	reloc    5 offset  288 [1e288] DIR64
-	reloc    6 offset  290 [1e290] DIR64
-	reloc    7 offset  298 [1e298] DIR64
-	reloc    8 offset  2a0 [1e2a0] DIR64
-	reloc    9 offset  2a8 [1e2a8] DIR64
-	reloc   10 offset  2b0 [1e2b0] DIR64
-	reloc   11 offset  2b8 [1e2b8] DIR64
-	reloc   12 offset  2c0 [1e2c0] DIR64
-	reloc   13 offset  2c8 [1e2c8] DIR64
-	reloc   14 offset  2d0 [1e2d0] DIR64
-	reloc   15 offset  2d8 [1e2d8] DIR64
-	reloc   16 offset  2e0 [1e2e0] DIR64
-	reloc   17 offset  2e8 [1e2e8] DIR64
-	reloc   18 offset  2f0 [1e2f0] DIR64
-	reloc   19 offset  2f8 [1e2f8] DIR64
-	reloc   20 offset  300 [1e300] DIR64
-	reloc   21 offset  308 [1e308] DIR64
-	reloc   22 offset  310 [1e310] DIR64
-	reloc   23 offset  318 [1e318] DIR64
-	reloc   24 offset  320 [1e320] DIR64
-	reloc   25 offset  328 [1e328] DIR64
-	reloc   26 offset  330 [1e330] DIR64
-	reloc   27 offset  338 [1e338] DIR64
-	reloc   28 offset  340 [1e340] DIR64
-	reloc   29 offset  348 [1e348] DIR64
-	reloc   30 offset  350 [1e350] DIR64
-	reloc   31 offset  358 [1e358] DIR64
-	reloc   32 offset  360 [1e360] DIR64
-	reloc   33 offset  368 [1e368] DIR64
-	reloc   34 offset  370 [1e370] DIR64
-	reloc   35 offset  378 [1e378] DIR64
-	reloc   36 offset  380 [1e380] DIR64
-	reloc   37 offset  388 [1e388] DIR64
-	reloc   38 offset  390 [1e390] DIR64
-	reloc   39 offset  398 [1e398] DIR64
-	reloc   40 offset  3a0 [1e3a0] DIR64
-	reloc   41 offset  3a8 [1e3a8] DIR64
-	reloc   42 offset  3b0 [1e3b0] DIR64
-	reloc   43 offset  3b8 [1e3b8] DIR64
-	reloc   44 offset  3c0 [1e3c0] DIR64
-	reloc   45 offset  3c8 [1e3c8] DIR64
-	reloc   46 offset  3d0 [1e3d0] DIR64
-	reloc   47 offset  3d8 [1e3d8] DIR64
-	reloc   48 offset  3e0 [1e3e0] DIR64
-	reloc   49 offset  3e8 [1e3e8] DIR64
-	reloc   50 offset  3f0 [1e3f0] DIR64
-	reloc   51 offset  3f8 [1e3f8] DIR64
-	reloc   52 offset  400 [1e400] DIR64
-	reloc   53 offset  408 [1e408] DIR64
-	reloc   54 offset  410 [1e410] DIR64
-	reloc   55 offset  418 [1e418] DIR64
-	reloc   56 offset  420 [1e420] DIR64
-	reloc   57 offset  428 [1e428] DIR64
-	reloc   58 offset  430 [1e430] DIR64
-	reloc   59 offset  438 [1e438] DIR64
-	reloc   60 offset  440 [1e440] DIR64
-	reloc   61 offset  448 [1e448] DIR64
-	reloc   62 offset  450 [1e450] DIR64
-	reloc   63 offset  458 [1e458] DIR64
-	reloc   64 offset  460 [1e460] DIR64
-	reloc   65 offset  468 [1e468] DIR64
-	reloc   66 offset  470 [1e470] DIR64
-	reloc   67 offset  478 [1e478] DIR64
-	reloc   68 offset  480 [1e480] DIR64
-	reloc   69 offset  488 [1e488] DIR64
-	reloc   70 offset  490 [1e490] DIR64
-	reloc   71 offset  498 [1e498] DIR64
-	reloc   72 offset  4a0 [1e4a0] DIR64
-	reloc   73 offset  4a8 [1e4a8] DIR64
-	reloc   74 offset  4b0 [1e4b0] DIR64
-	reloc   75 offset  4b8 [1e4b8] DIR64
-	reloc   76 offset  4c0 [1e4c0] DIR64
-	reloc   77 offset  4c8 [1e4c8] DIR64
-	reloc   78 offset  4d0 [1e4d0] DIR64
-	reloc   79 offset  4d8 [1e4d8] DIR64
-	reloc   80 offset  4e0 [1e4e0] DIR64
-	reloc   81 offset  4e8 [1e4e8] DIR64
-	reloc   82 offset  4f0 [1e4f0] DIR64
-	reloc   83 offset  4f8 [1e4f8] DIR64
-	reloc   84 offset  500 [1e500] DIR64
-	reloc   85 offset  508 [1e508] DIR64
-	reloc   86 offset  510 [1e510] DIR64
-	reloc   87 offset  518 [1e518] DIR64
-	reloc   88 offset  520 [1e520] DIR64
-	reloc   89 offset  528 [1e528] DIR64
-	reloc   90 offset  530 [1e530] DIR64
-	reloc   91 offset  538 [1e538] DIR64
-	reloc   92 offset  540 [1e540] DIR64
-	reloc   93 offset  548 [1e548] DIR64
-	reloc   94 offset  550 [1e550] DIR64
-	reloc   95 offset  558 [1e558] DIR64
-	reloc   96 offset  560 [1e560] DIR64
-	reloc   97 offset  568 [1e568] DIR64
-	reloc   98 offset  570 [1e570] DIR64
-	reloc   99 offset  630 [1e630] DIR64
-	reloc  100 offset  638 [1e638] DIR64
-	reloc  101 offset  640 [1e640] DIR64
-	reloc  102 offset  648 [1e648] DIR64
-	reloc  103 offset  650 [1e650] DIR64
-	reloc  104 offset  658 [1e658] DIR64
-	reloc  105 offset  660 [1e660] DIR64
-	reloc  106 offset  668 [1e668] DIR64
-	reloc  107 offset  670 [1e670] DIR64
-	reloc  108 offset  678 [1e678] DIR64
-	reloc  109 offset  680 [1e680] DIR64
-	reloc  110 offset  688 [1e688] DIR64
-	reloc  111 offset  690 [1e690] DIR64
-	reloc  112 offset  698 [1e698] DIR64
-	reloc  113 offset  848 [1e848] DIR64
-	reloc  114 offset  850 [1e850] DIR64
-	reloc  115 offset  858 [1e858] DIR64
-	reloc  116 offset  860 [1e860] DIR64
-	reloc  117 offset  868 [1e868] DIR64
-	reloc  118 offset  870 [1e870] DIR64
-	reloc  119 offset  878 [1e878] DIR64
-	reloc  120 offset  880 [1e880] DIR64
-	reloc  121 offset  888 [1e888] DIR64
-	reloc  122 offset  890 [1e890] DIR64
-	reloc  123 offset  898 [1e898] DIR64
-	reloc  124 offset  8a0 [1e8a0] DIR64
-	reloc  125 offset  8a8 [1e8a8] DIR64
-	reloc  126 offset  8b0 [1e8b0] DIR64
-	reloc  127 offset  8b8 [1e8b8] DIR64
-	reloc  128 offset  8c0 [1e8c0] DIR64
-	reloc  129 offset  8c8 [1e8c8] DIR64
-	reloc  130 offset  8d0 [1e8d0] DIR64
-	reloc  131 offset  8d8 [1e8d8] DIR64
-	reloc  132 offset  8e0 [1e8e0] DIR64
-	reloc  133 offset  908 [1e908] DIR64
-	reloc  134 offset  910 [1e910] DIR64
-	reloc  135 offset  918 [1e918] DIR64
-	reloc  136 offset  de0 [1ede0] DIR64
-	reloc  137 offset  de8 [1ede8] DIR64
-	reloc  138 offset  df0 [1edf0] DIR64
-	reloc  139 offset  df8 [1edf8] DIR64
-	reloc  140 offset  e00 [1ee00] DIR64
-	reloc  141 offset  e08 [1ee08] DIR64
-	reloc  142 offset  e38 [1ee38] DIR64
-	reloc  143 offset  e40 [1ee40] DIR64
-	reloc  144 offset  e48 [1ee48] DIR64
-	reloc  145 offset  e50 [1ee50] DIR64
-	reloc  146 offset  e60 [1ee60] DIR64
-	reloc  147 offset  e70 [1ee70] DIR64
-	reloc  148 offset  e78 [1ee78] DIR64
-	reloc  149 offset  e80 [1ee80] DIR64
-	reloc  150 offset  e88 [1ee88] DIR64
-	reloc  151 offset  e90 [1ee90] DIR64
-	reloc  152 offset  e98 [1ee98] DIR64
-	reloc  153 offset  ea0 [1eea0] DIR64
-	reloc  154 offset  ea8 [1eea8] DIR64
-	reloc  155 offset  eb0 [1eeb0] DIR64
-	reloc  156 offset  eb8 [1eeb8] DIR64
-	reloc  157 offset  ec0 [1eec0] DIR64
-	reloc  158 offset  ec8 [1eec8] DIR64
-	reloc  159 offset  ed0 [1eed0] DIR64
-	reloc  160 offset  ed8 [1eed8] DIR64
-	reloc  161 offset  ee0 [1eee0] DIR64
-	reloc  162 offset  ee8 [1eee8] DIR64
-	reloc  163 offset  ef0 [1eef0] DIR64
-	reloc  164 offset  ef8 [1eef8] DIR64
-	reloc  165 offset  f00 [1ef00] DIR64
-	reloc  166 offset  f08 [1ef08] DIR64
-	reloc  167 offset  f10 [1ef10] DIR64
-	reloc  168 offset  f18 [1ef18] DIR64
-	reloc  169 offset  f20 [1ef20] DIR64
-	reloc  170 offset  f28 [1ef28] DIR64
-	reloc  171 offset  f30 [1ef30] DIR64
-	reloc  172 offset  f38 [1ef38] DIR64
-	reloc  173 offset  f40 [1ef40] DIR64
-	reloc  174 offset  f48 [1ef48] DIR64
-	reloc  175 offset    0 [1e000] ABSOLUTE
+Virtual Address: 0001e000 Chunk size 228 (0xe4) Number of fixups 110
+	reloc    0 offset  178 [1e178] DIR64
+	reloc    1 offset  180 [1e180] DIR64
+	reloc    2 offset  188 [1e188] DIR64
+	reloc    3 offset  190 [1e190] DIR64
+	reloc    4 offset  1a0 [1e1a0] DIR64
+	reloc    5 offset  4a0 [1e4a0] DIR64
+	reloc    6 offset  4a8 [1e4a8] DIR64
+	reloc    7 offset  4b0 [1e4b0] DIR64
+	reloc    8 offset  4b8 [1e4b8] DIR64
+	reloc    9 offset  4c0 [1e4c0] DIR64
+	reloc   10 offset  4c8 [1e4c8] DIR64
+	reloc   11 offset  4d0 [1e4d0] DIR64
+	reloc   12 offset  4d8 [1e4d8] DIR64
+	reloc   13 offset  4e0 [1e4e0] DIR64
+	reloc   14 offset  4e8 [1e4e8] DIR64
+	reloc   15 offset  4f0 [1e4f0] DIR64
+	reloc   16 offset  4f8 [1e4f8] DIR64
+	reloc   17 offset  500 [1e500] DIR64
+	reloc   18 offset  508 [1e508] DIR64
+	reloc   19 offset  510 [1e510] DIR64
+	reloc   20 offset  518 [1e518] DIR64
+	reloc   21 offset  520 [1e520] DIR64
+	reloc   22 offset  528 [1e528] DIR64
+	reloc   23 offset  530 [1e530] DIR64
+	reloc   24 offset  538 [1e538] DIR64
+	reloc   25 offset  540 [1e540] DIR64
+	reloc   26 offset  548 [1e548] DIR64
+	reloc   27 offset  550 [1e550] DIR64
+	reloc   28 offset  558 [1e558] DIR64
+	reloc   29 offset  560 [1e560] DIR64
+	reloc   30 offset  568 [1e568] DIR64
+	reloc   31 offset  570 [1e570] DIR64
+	reloc   32 offset  578 [1e578] DIR64
+	reloc   33 offset  640 [1e640] DIR64
+	reloc   34 offset  648 [1e648] DIR64
+	reloc   35 offset  650 [1e650] DIR64
+	reloc   36 offset  658 [1e658] DIR64
+	reloc   37 offset  660 [1e660] DIR64
+	reloc   38 offset  668 [1e668] DIR64
+	reloc   39 offset  670 [1e670] DIR64
+	reloc   40 offset  678 [1e678] DIR64
+	reloc   41 offset  680 [1e680] DIR64
+	reloc   42 offset  688 [1e688] DIR64
+	reloc   43 offset  690 [1e690] DIR64
+	reloc   44 offset  698 [1e698] DIR64
+	reloc   45 offset  6a0 [1e6a0] DIR64
+	reloc   46 offset  6a8 [1e6a8] DIR64
+	reloc   47 offset  858 [1e858] DIR64
+	reloc   48 offset  860 [1e860] DIR64
+	reloc   49 offset  868 [1e868] DIR64
+	reloc   50 offset  870 [1e870] DIR64
+	reloc   51 offset  878 [1e878] DIR64
+	reloc   52 offset  880 [1e880] DIR64
+	reloc   53 offset  888 [1e888] DIR64
+	reloc   54 offset  890 [1e890] DIR64
+	reloc   55 offset  898 [1e898] DIR64
+	reloc   56 offset  8a0 [1e8a0] DIR64
+	reloc   57 offset  8a8 [1e8a8] DIR64
+	reloc   58 offset  8b0 [1e8b0] DIR64
+	reloc   59 offset  8b8 [1e8b8] DIR64
+	reloc   60 offset  8c0 [1e8c0] DIR64
+	reloc   61 offset  8c8 [1e8c8] DIR64
+	reloc   62 offset  8d0 [1e8d0] DIR64
+	reloc   63 offset  8d8 [1e8d8] DIR64
+	reloc   64 offset  8e0 [1e8e0] DIR64
+	reloc   65 offset  8e8 [1e8e8] DIR64
+	reloc   66 offset  8f0 [1e8f0] DIR64
+	reloc   67 offset  918 [1e918] DIR64
+	reloc   68 offset  920 [1e920] DIR64
+	reloc   69 offset  928 [1e928] DIR64
+	reloc   70 offset  df0 [1edf0] DIR64
+	reloc   71 offset  df8 [1edf8] DIR64
+	reloc   72 offset  e00 [1ee00] DIR64
+	reloc   73 offset  e08 [1ee08] DIR64
+	reloc   74 offset  e10 [1ee10] DIR64
+	reloc   75 offset  e18 [1ee18] DIR64
+	reloc   76 offset  e48 [1ee48] DIR64
+	reloc   77 offset  e50 [1ee50] DIR64
+	reloc   78 offset  e58 [1ee58] DIR64
+	reloc   79 offset  e60 [1ee60] DIR64
+	reloc   80 offset  e70 [1ee70] DIR64
+	reloc   81 offset  e80 [1ee80] DIR64
+	reloc   82 offset  e88 [1ee88] DIR64
+	reloc   83 offset  e90 [1ee90] DIR64
+	reloc   84 offset  e98 [1ee98] DIR64
+	reloc   85 offset  ea0 [1eea0] DIR64
+	reloc   86 offset  ea8 [1eea8] DIR64
+	reloc   87 offset  eb0 [1eeb0] DIR64
+	reloc   88 offset  eb8 [1eeb8] DIR64
+	reloc   89 offset  ec0 [1eec0] DIR64
+	reloc   90 offset  ec8 [1eec8] DIR64
+	reloc   91 offset  ed0 [1eed0] DIR64
+	reloc   92 offset  ed8 [1eed8] DIR64
+	reloc   93 offset  ee0 [1eee0] DIR64
+	reloc   94 offset  ee8 [1eee8] DIR64
+	reloc   95 offset  ef0 [1eef0] DIR64
+	reloc   96 offset  ef8 [1eef8] DIR64
+	reloc   97 offset  f00 [1ef00] DIR64
+	reloc   98 offset  f08 [1ef08] DIR64
+	reloc   99 offset  f10 [1ef10] DIR64
+	reloc  100 offset  f18 [1ef18] DIR64
+	reloc  101 offset  f20 [1ef20] DIR64
+	reloc  102 offset  f28 [1ef28] DIR64
+	reloc  103 offset  f30 [1ef30] DIR64
+	reloc  104 offset  f38 [1ef38] DIR64
+	reloc  105 offset  f40 [1ef40] DIR64
+	reloc  106 offset  f48 [1ef48] DIR64
+	reloc  107 offset  f50 [1ef50] DIR64
+	reloc  108 offset  f58 [1ef58] DIR64
+	reloc  109 offset    0 [1e000] ABSOLUTE
 
 Virtual Address: 0001f000 Chunk size 124 (0x7c) Number of fixups 58
-	reloc    0 offset  178 [1f178] DIR64
-	reloc    1 offset  1a8 [1f1a8] DIR64
-	reloc    2 offset  1b0 [1f1b0] DIR64
-	reloc    3 offset  1b8 [1f1b8] DIR64
-	reloc    4 offset  1c0 [1f1c0] DIR64
-	reloc    5 offset  1d0 [1f1d0] DIR64
-	reloc    6 offset  1e0 [1f1e0] DIR64
-	reloc    7 offset  1e8 [1f1e8] DIR64
-	reloc    8 offset  1f0 [1f1f0] DIR64
-	reloc    9 offset  1f8 [1f1f8] DIR64
-	reloc   10 offset  200 [1f200] DIR64
-	reloc   11 offset  208 [1f208] DIR64
-	reloc   12 offset  210 [1f210] DIR64
-	reloc   13 offset  218 [1f218] DIR64
-	reloc   14 offset  220 [1f220] DIR64
-	reloc   15 offset  228 [1f228] DIR64
-	reloc   16 offset  230 [1f230] DIR64
-	reloc   17 offset  238 [1f238] DIR64
-	reloc   18 offset  240 [1f240] DIR64
-	reloc   19 offset  248 [1f248] DIR64
-	reloc   20 offset  428 [1f428] DIR64
-	reloc   21 offset  430 [1f430] DIR64
-	reloc   22 offset  438 [1f438] DIR64
-	reloc   23 offset  440 [1f440] DIR64
-	reloc   24 offset  450 [1f450] DIR64
-	reloc   25 offset  4c0 [1f4c0] DIR64
-	reloc   26 offset  4e0 [1f4e0] DIR64
-	reloc   27 offset  4e8 [1f4e8] DIR64
-	reloc   28 offset  4f0 [1f4f0] DIR64
-	reloc   29 offset  4f8 [1f4f8] DIR64
-	reloc   30 offset  500 [1f500] DIR64
-	reloc   31 offset  508 [1f508] DIR64
-	reloc   32 offset  510 [1f510] DIR64
-	reloc   33 offset  518 [1f518] DIR64
-	reloc   34 offset  520 [1f520] DIR64
-	reloc   35 offset  528 [1f528] DIR64
-	reloc   36 offset  530 [1f530] DIR64
-	reloc   37 offset  538 [1f538] DIR64
-	reloc   38 offset  540 [1f540] DIR64
-	reloc   39 offset  548 [1f548] DIR64
-	reloc   40 offset  638 [1f638] DIR64
-	reloc   41 offset  640 [1f640] DIR64
-	reloc   42 offset  728 [1f728] DIR64
-	reloc   43 offset  730 [1f730] DIR64
-	reloc   44 offset  7e8 [1f7e8] DIR64
-	reloc   45 offset  800 [1f800] DIR64
-	reloc   46 offset  808 [1f808] DIR64
-	reloc   47 offset  810 [1f810] DIR64
-	reloc   48 offset  830 [1f830] DIR64
-	reloc   49 offset  890 [1f890] DIR64
-	reloc   50 offset  8a8 [1f8a8] DIR64
-	reloc   51 offset  8b0 [1f8b0] DIR64
-	reloc   52 offset  8b8 [1f8b8] DIR64
-	reloc   53 offset  8c0 [1f8c0] DIR64
+	reloc    0 offset  188 [1f188] DIR64
+	reloc    1 offset  1b8 [1f1b8] DIR64
+	reloc    2 offset  1c0 [1f1c0] DIR64
+	reloc    3 offset  1c8 [1f1c8] DIR64
+	reloc    4 offset  1d0 [1f1d0] DIR64
+	reloc    5 offset  1e0 [1f1e0] DIR64
+	reloc    6 offset  1f0 [1f1f0] DIR64
+	reloc    7 offset  1f8 [1f1f8] DIR64
+	reloc    8 offset  200 [1f200] DIR64
+	reloc    9 offset  208 [1f208] DIR64
+	reloc   10 offset  210 [1f210] DIR64
+	reloc   11 offset  218 [1f218] DIR64
+	reloc   12 offset  220 [1f220] DIR64
+	reloc   13 offset  228 [1f228] DIR64
+	reloc   14 offset  230 [1f230] DIR64
+	reloc   15 offset  238 [1f238] DIR64
+	reloc   16 offset  240 [1f240] DIR64
+	reloc   17 offset  248 [1f248] DIR64
+	reloc   18 offset  250 [1f250] DIR64
+	reloc   19 offset  258 [1f258] DIR64
+	reloc   20 offset  438 [1f438] DIR64
+	reloc   21 offset  440 [1f440] DIR64
+	reloc   22 offset  448 [1f448] DIR64
+	reloc   23 offset  450 [1f450] DIR64
+	reloc   24 offset  460 [1f460] DIR64
+	reloc   25 offset  4d0 [1f4d0] DIR64
+	reloc   26 offset  4f0 [1f4f0] DIR64
+	reloc   27 offset  4f8 [1f4f8] DIR64
+	reloc   28 offset  500 [1f500] DIR64
+	reloc   29 offset  508 [1f508] DIR64
+	reloc   30 offset  510 [1f510] DIR64
+	reloc   31 offset  518 [1f518] DIR64
+	reloc   32 offset  520 [1f520] DIR64
+	reloc   33 offset  528 [1f528] DIR64
+	reloc   34 offset  530 [1f530] DIR64
+	reloc   35 offset  538 [1f538] DIR64
+	reloc   36 offset  540 [1f540] DIR64
+	reloc   37 offset  548 [1f548] DIR64
+	reloc   38 offset  550 [1f550] DIR64
+	reloc   39 offset  558 [1f558] DIR64
+	reloc   40 offset  648 [1f648] DIR64
+	reloc   41 offset  650 [1f650] DIR64
+	reloc   42 offset  738 [1f738] DIR64
+	reloc   43 offset  740 [1f740] DIR64
+	reloc   44 offset  7f8 [1f7f8] DIR64
+	reloc   45 offset  810 [1f810] DIR64
+	reloc   46 offset  818 [1f818] DIR64
+	reloc   47 offset  820 [1f820] DIR64
+	reloc   48 offset  840 [1f840] DIR64
+	reloc   49 offset  8a0 [1f8a0] DIR64
+	reloc   50 offset  8b8 [1f8b8] DIR64
+	reloc   51 offset  8c0 [1f8c0] DIR64
+	reloc   52 offset  8c8 [1f8c8] DIR64
+	reloc   53 offset  8d0 [1f8d0] DIR64
 	reloc   54 offset  900 [1f900] DIR64
 	reloc   55 offset  908 [1f908] DIR64
 	reloc   56 offset  910 [1f910] DIR64
 	reloc   57 offset  918 [1f918] DIR64
 
 Virtual Address: 0002b000 Chunk size 268 (0x10c) Number of fixups 130
 	reloc    0 offset   18 [2b018] DIR64
@@ -7761,19 +7761,19 @@
 	reloc  124 offset  b88 [2bb88] DIR64
 	reloc  125 offset  bc0 [2bbc0] DIR64
 	reloc  126 offset  be8 [2bbe8] DIR64
 	reloc  127 offset  c28 [2bc28] DIR64
 	reloc  128 offset  c60 [2bc60] DIR64
 	reloc  129 offset  c90 [2bc90] DIR64
 
-There is a debug directory in .rdata at 0x18001f738
+There is a debug directory in .rdata at 0x18001f748
 
 Type                Size     Rva      Offset
   2        CodeView 00000057 000206f0 0001f4f0
-(format RSDS signature 3c1af9298f184ee4ac610c6b43c28509 age 1 pdb C:\Users\qt\work\qt\qtnetworkauth_build\bin\Qt6NetworkAuth.pdb)
+(format RSDS signature 9f5df4a4bb4643748035cd42dc8c925c age 1 pdb C:\Users\qt\work\qt\qtnetworkauth_build\bin\Qt6NetworkAuth.pdb)
  12         Feature 00000014 00020748 0001f548
  13         CoffGrp 00000384 0002075c 0001f55c
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 2
 010   Entry: ID: 0x000010, Value: 0x80000020
 020    Name Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
@@ -7808,15 +7808,15 @@
 
 
 
 Disassembly of section .text:
 
 0000000180001000 <.text>:
    180001000:	sub    $0x48,%rsp
-   180001004:	lea    0x1c8d5(%rip),%rax        # 0x18001d8e0
+   180001004:	lea    0x1cfcd(%rip),%rax        # 0x18001dfd8
    18000100b:	movq   $0x0,0x20(%rsp)
    180001014:	lea    0x20(%rsp),%rdx
    180001019:	mov    %rax,0x28(%rsp)
    18000101e:	lea    0x2c093(%rip),%rcx        # 0x18002d0b8
    180001025:	movq   $0xc,0x30(%rsp)
    18000102e:	call   *0x1a39c(%rip)        # 0x18001b3d0
    180001034:	mov    0x20(%rsp),%rcx
@@ -7832,15 +7832,15 @@
    180001058:	call   *0x1a34a(%rip)        # 0x18001b3a8
    18000105e:	lea    0x195eb(%rip),%rcx        # 0x18001a650
    180001065:	add    $0x48,%rsp
    180001069:	jmp    0x180019a00
    18000106e:	int3
    18000106f:	int3
    180001070:	sub    $0x48,%rsp
-   180001074:	lea    0x1c885(%rip),%rax        # 0x18001d900
+   180001074:	lea    0x1cf7d(%rip),%rax        # 0x18001dff8
    18000107b:	movq   $0x0,0x20(%rsp)
    180001084:	lea    0x20(%rsp),%rdx
    180001089:	mov    %rax,0x28(%rsp)
    18000108e:	lea    0x2c06b(%rip),%rcx        # 0x18002d100
    180001095:	movq   $0x7,0x30(%rsp)
    18000109e:	call   *0x1a32c(%rip)        # 0x18001b3d0
    1800010a4:	mov    0x20(%rsp),%rcx
@@ -7856,15 +7856,15 @@
    1800010c8:	call   *0x1a2da(%rip)        # 0x18001b3a8
    1800010ce:	lea    0x1958b(%rip),%rcx        # 0x18001a660
    1800010d5:	add    $0x48,%rsp
    1800010d9:	jmp    0x180019a00
    1800010de:	int3
    1800010df:	int3
    1800010e0:	sub    $0x48,%rsp
-   1800010e4:	lea    0x1c825(%rip),%rax        # 0x18001d910
+   1800010e4:	lea    0x1cf1d(%rip),%rax        # 0x18001e008
    1800010eb:	movq   $0x0,0x20(%rsp)
    1800010f4:	lea    0x20(%rsp),%rdx
    1800010f9:	mov    %rax,0x28(%rsp)
    1800010fe:	lea    0x2c0bb(%rip),%rcx        # 0x18002d1c0
    180001105:	movq   $0x9,0x30(%rsp)
    18000110e:	call   *0x1a2bc(%rip)        # 0x18001b3d0
    180001114:	mov    0x20(%rsp),%rcx
@@ -7880,15 +7880,15 @@
    180001138:	call   *0x1a26a(%rip)        # 0x18001b3a8
    18000113e:	lea    0x1952b(%rip),%rcx        # 0x18001a670
    180001145:	add    $0x48,%rsp
    180001149:	jmp    0x180019a00
    18000114e:	int3
    18000114f:	int3
    180001150:	sub    $0x48,%rsp
-   180001154:	lea    0x1c7cd(%rip),%rax        # 0x18001d928
+   180001154:	lea    0x1cec5(%rip),%rax        # 0x18001e020
    18000115b:	movq   $0x0,0x20(%rsp)
    180001164:	lea    0x20(%rsp),%rdx
    180001169:	mov    %rax,0x28(%rsp)
    18000116e:	lea    0x2bf2b(%rip),%rcx        # 0x18002d0a0
    180001175:	movq   $0xd,0x30(%rsp)
    18000117e:	call   *0x1a24c(%rip)        # 0x18001b3d0
    180001184:	mov    0x20(%rsp),%rcx
@@ -7904,15 +7904,15 @@
    1800011a8:	call   *0x1a1fa(%rip)        # 0x18001b3a8
    1800011ae:	lea    0x194cb(%rip),%rcx        # 0x18001a680
    1800011b5:	add    $0x48,%rsp
    1800011b9:	jmp    0x180019a00
    1800011be:	int3
    1800011bf:	int3
    1800011c0:	sub    $0x48,%rsp
-   1800011c4:	lea    0x1c77d(%rip),%rax        # 0x18001d948
+   1800011c4:	lea    0x1ce75(%rip),%rax        # 0x18001e040
    1800011cb:	movq   $0x0,0x20(%rsp)
    1800011d4:	lea    0x20(%rsp),%rdx
    1800011d9:	mov    %rax,0x28(%rsp)
    1800011de:	lea    0x2be8b(%rip),%rcx        # 0x18002d070
    1800011e5:	movq   $0x4,0x30(%rsp)
    1800011ee:	call   *0x1a1dc(%rip)        # 0x18001b3d0
    1800011f4:	mov    0x20(%rsp),%rcx
@@ -7928,15 +7928,15 @@
    180001218:	call   *0x1a18a(%rip)        # 0x18001b3a8
    18000121e:	lea    0x1946b(%rip),%rcx        # 0x18001a690
    180001225:	add    $0x48,%rsp
    180001229:	jmp    0x180019a00
    18000122e:	int3
    18000122f:	int3
    180001230:	sub    $0x48,%rsp
-   180001234:	lea    0x1c71d(%rip),%rax        # 0x18001d958
+   180001234:	lea    0x1ce15(%rip),%rax        # 0x18001e050
    18000123b:	movq   $0x0,0x20(%rsp)
    180001244:	lea    0x20(%rsp),%rdx
    180001249:	mov    %rax,0x28(%rsp)
    18000124e:	lea    0x2bf53(%rip),%rcx        # 0x18002d1a8
    180001255:	movq   $0x5,0x30(%rsp)
    18000125e:	call   *0x1a16c(%rip)        # 0x18001b3d0
    180001264:	mov    0x20(%rsp),%rcx
@@ -7952,15 +7952,15 @@
    180001288:	call   *0x1a11a(%rip)        # 0x18001b3a8
    18000128e:	lea    0x1940b(%rip),%rcx        # 0x18001a6a0
    180001295:	add    $0x48,%rsp
    180001299:	jmp    0x180019a00
    18000129e:	int3
    18000129f:	int3
    1800012a0:	sub    $0x48,%rsp
-   1800012a4:	lea    0x1c6bd(%rip),%rax        # 0x18001d968
+   1800012a4:	lea    0x1cdb5(%rip),%rax        # 0x18001e060
    1800012ab:	movq   $0x0,0x20(%rsp)
    1800012b4:	lea    0x20(%rsp),%rdx
    1800012b9:	mov    %rax,0x28(%rsp)
    1800012be:	lea    0x2be23(%rip),%rcx        # 0x18002d0e8
    1800012c5:	movq   $0x11,0x30(%rsp)
    1800012ce:	call   *0x1a0fc(%rip)        # 0x18001b3d0
    1800012d4:	mov    0x20(%rsp),%rcx
@@ -7976,15 +7976,15 @@
    1800012f8:	call   *0x1a0aa(%rip)        # 0x18001b3a8
    1800012fe:	lea    0x193ab(%rip),%rcx        # 0x18001a6b0
    180001305:	add    $0x48,%rsp
    180001309:	jmp    0x180019a00
    18000130e:	int3
    18000130f:	int3
    180001310:	sub    $0x48,%rsp
-   180001314:	lea    0x1c675(%rip),%rax        # 0x18001d990
+   180001314:	lea    0x1cd6d(%rip),%rax        # 0x18001e088
    18000131b:	movq   $0x0,0x20(%rsp)
    180001324:	lea    0x20(%rsp),%rdx
    180001329:	mov    %rax,0x28(%rsp)
    18000132e:	lea    0x2bde3(%rip),%rcx        # 0x18002d118
    180001335:	movq   $0x9,0x30(%rsp)
    18000133e:	call   *0x1a08c(%rip)        # 0x18001b3d0
    180001344:	mov    0x20(%rsp),%rcx
@@ -8000,15 +8000,15 @@
    180001368:	call   *0x1a03a(%rip)        # 0x18001b3a8
    18000136e:	lea    0x1934b(%rip),%rcx        # 0x18001a6c0
    180001375:	add    $0x48,%rsp
    180001379:	jmp    0x180019a00
    18000137e:	int3
    18000137f:	int3
    180001380:	sub    $0x48,%rsp
-   180001384:	lea    0x1c61d(%rip),%rax        # 0x18001d9a8
+   180001384:	lea    0x1cd15(%rip),%rax        # 0x18001e0a0
    18000138b:	movq   $0x0,0x20(%rsp)
    180001394:	lea    0x20(%rsp),%rdx
    180001399:	mov    %rax,0x28(%rsp)
    18000139e:	lea    0x2bdeb(%rip),%rcx        # 0x18002d190
    1800013a5:	movq   $0xa,0x30(%rsp)
    1800013ae:	call   *0x1a01c(%rip)        # 0x18001b3d0
    1800013b4:	mov    0x20(%rsp),%rcx
@@ -8024,15 +8024,15 @@
    1800013d8:	call   *0x19fca(%rip)        # 0x18001b3a8
    1800013de:	lea    0x192eb(%rip),%rcx        # 0x18001a6d0
    1800013e5:	add    $0x48,%rsp
    1800013e9:	jmp    0x180019a00
    1800013ee:	int3
    1800013ef:	int3
    1800013f0:	sub    $0x48,%rsp
-   1800013f4:	lea    0x1c5c5(%rip),%rax        # 0x18001d9c0
+   1800013f4:	lea    0x1ccbd(%rip),%rax        # 0x18001e0b8
    1800013fb:	movq   $0x0,0x20(%rsp)
    180001404:	lea    0x20(%rsp),%rdx
    180001409:	mov    %rax,0x28(%rsp)
    18000140e:	lea    0x2bcbb(%rip),%rcx        # 0x18002d0d0
    180001415:	movq   $0xa,0x30(%rsp)
    18000141e:	call   *0x19fac(%rip)        # 0x18001b3d0
    180001424:	mov    0x20(%rsp),%rcx
@@ -8048,15 +8048,15 @@
    180001448:	call   *0x19f5a(%rip)        # 0x18001b3a8
    18000144e:	lea    0x1928b(%rip),%rcx        # 0x18001a6e0
    180001455:	add    $0x48,%rsp
    180001459:	jmp    0x180019a00
    18000145e:	int3
    18000145f:	int3
    180001460:	sub    $0x48,%rsp
-   180001464:	lea    0x1c56d(%rip),%rax        # 0x18001d9d8
+   180001464:	lea    0x1cc65(%rip),%rax        # 0x18001e0d0
    18000146b:	movq   $0x0,0x20(%rsp)
    180001474:	lea    0x20(%rsp),%rdx
    180001479:	mov    %rax,0x28(%rsp)
    18000147e:	lea    0x2bcf3(%rip),%rcx        # 0x18002d178
    180001485:	movq   $0xc,0x30(%rsp)
    18000148e:	call   *0x19f3c(%rip)        # 0x18001b3d0
    180001494:	mov    0x20(%rsp),%rcx
@@ -8072,15 +8072,15 @@
    1800014b8:	call   *0x19eea(%rip)        # 0x18001b3a8
    1800014be:	lea    0x1922b(%rip),%rcx        # 0x18001a6f0
    1800014c5:	add    $0x48,%rsp
    1800014c9:	jmp    0x180019a00
    1800014ce:	int3
    1800014cf:	int3
    1800014d0:	sub    $0x48,%rsp
-   1800014d4:	lea    0x1c51d(%rip),%rax        # 0x18001d9f8
+   1800014d4:	lea    0x1cc15(%rip),%rax        # 0x18001e0f0
    1800014db:	movq   $0x0,0x20(%rsp)
    1800014e4:	lea    0x20(%rsp),%rdx
    1800014e9:	mov    %rax,0x28(%rsp)
    1800014ee:	lea    0x2bb93(%rip),%rcx        # 0x18002d088
    1800014f5:	movq   $0xd,0x30(%rsp)
    1800014fe:	call   *0x19ecc(%rip)        # 0x18001b3d0
    180001504:	mov    0x20(%rsp),%rcx
@@ -8096,15 +8096,15 @@
    180001528:	call   *0x19e7a(%rip)        # 0x18001b3a8
    18000152e:	lea    0x191cb(%rip),%rcx        # 0x18001a700
    180001535:	add    $0x48,%rsp
    180001539:	jmp    0x180019a00
    18000153e:	int3
    18000153f:	int3
    180001540:	sub    $0x48,%rsp
-   180001544:	lea    0x1c4cd(%rip),%rax        # 0x18001da18
+   180001544:	lea    0x1cbc5(%rip),%rax        # 0x18001e110
    18000154b:	movq   $0x0,0x20(%rsp)
    180001554:	lea    0x20(%rsp),%rdx
    180001559:	mov    %rax,0x28(%rsp)
    18000155e:	lea    0x2bbe3(%rip),%rcx        # 0x18002d148
    180001565:	movq   $0xd,0x30(%rsp)
    18000156e:	call   *0x19e5c(%rip)        # 0x18001b3d0
    180001574:	mov    0x20(%rsp),%rcx
@@ -8120,15 +8120,15 @@
    180001598:	call   *0x19e0a(%rip)        # 0x18001b3a8
    18000159e:	lea    0x1916b(%rip),%rcx        # 0x18001a710
    1800015a5:	add    $0x48,%rsp
    1800015a9:	jmp    0x180019a00
    1800015ae:	int3
    1800015af:	int3
    1800015b0:	sub    $0x48,%rsp
-   1800015b4:	lea    0x1c47d(%rip),%rax        # 0x18001da38
+   1800015b4:	lea    0x1cb75(%rip),%rax        # 0x18001e130
    1800015bb:	movq   $0x0,0x20(%rsp)
    1800015c4:	lea    0x20(%rsp),%rdx
    1800015c9:	mov    %rax,0x28(%rsp)
    1800015ce:	lea    0x2bb8b(%rip),%rcx        # 0x18002d160
    1800015d5:	movq   $0x5,0x30(%rsp)
    1800015de:	call   *0x19dec(%rip)        # 0x18001b3d0
    1800015e4:	mov    0x20(%rsp),%rcx
@@ -8144,15 +8144,15 @@
    180001608:	call   *0x19d9a(%rip)        # 0x18001b3a8
    18000160e:	lea    0x1910b(%rip),%rcx        # 0x18001a720
    180001615:	add    $0x48,%rsp
    180001619:	jmp    0x180019a00
    18000161e:	int3
    18000161f:	int3
    180001620:	sub    $0x48,%rsp
-   180001624:	lea    0x1c41d(%rip),%rax        # 0x18001da48
+   180001624:	lea    0x1cb15(%rip),%rax        # 0x18001e140
    18000162b:	movq   $0x0,0x20(%rsp)
    180001634:	lea    0x20(%rsp),%rdx
    180001639:	mov    %rax,0x28(%rsp)
    18000163e:	lea    0x2baeb(%rip),%rcx        # 0x18002d130
    180001645:	movq   $0x5,0x30(%rsp)
    18000164e:	call   *0x19d7c(%rip)        # 0x18001b3d0
    180001654:	mov    0x20(%rsp),%rcx
@@ -8168,15 +8168,15 @@
    180001678:	call   *0x19d2a(%rip)        # 0x18001b3a8
    18000167e:	lea    0x190ab(%rip),%rcx        # 0x18001a730
    180001685:	add    $0x48,%rsp
    180001689:	jmp    0x180019a00
    18000168e:	int3
    18000168f:	int3
    180001690:	sub    $0x48,%rsp
-   180001694:	lea    0x1c3bd(%rip),%rax        # 0x18001da58
+   180001694:	lea    0x1cab5(%rip),%rax        # 0x18001e150
    18000169b:	movq   $0x0,0x20(%rsp)
    1800016a4:	lea    0x20(%rsp),%rdx
    1800016a9:	mov    %rax,0x28(%rsp)
    1800016ae:	lea    0x2b9a3(%rip),%rcx        # 0x18002d058
    1800016b5:	movq   $0xa,0x30(%rsp)
    1800016be:	call   *0x19d0c(%rip)        # 0x18001b3d0
    1800016c4:	mov    0x20(%rsp),%rcx
@@ -8192,15 +8192,15 @@
    1800016e8:	call   *0x19cba(%rip)        # 0x18001b3a8
    1800016ee:	lea    0x1904b(%rip),%rcx        # 0x18001a740
    1800016f5:	add    $0x48,%rsp
    1800016f9:	jmp    0x180019a00
    1800016fe:	int3
    1800016ff:	int3
    180001700:	sub    $0x48,%rsp
-   180001704:	lea    0x1cfb5(%rip),%rax        # 0x18001e6c0
+   180001704:	lea    0x1cfc5(%rip),%rax        # 0x18001e6d0
    18000170b:	movq   $0x0,0x20(%rsp)
    180001714:	lea    0x20(%rsp),%rdx
    180001719:	mov    %rax,0x28(%rsp)
    18000171e:	lea    0x2bb93(%rip),%rcx        # 0x18002d2b8
    180001725:	movq   $0xe,0x30(%rsp)
    18000172e:	call   *0x19c9c(%rip)        # 0x18001b3d0
    180001734:	mov    0x20(%rsp),%rcx
@@ -8216,15 +8216,15 @@
    180001758:	call   *0x19c4a(%rip)        # 0x18001b3a8
    18000175e:	lea    0x18ffb(%rip),%rcx        # 0x18001a760
    180001765:	add    $0x48,%rsp
    180001769:	jmp    0x180019a00
    18000176e:	int3
    18000176f:	int3
    180001770:	sub    $0x48,%rsp
-   180001774:	lea    0x1cf65(%rip),%rax        # 0x18001e6e0
+   180001774:	lea    0x1cf75(%rip),%rax        # 0x18001e6f0
    18000177b:	movq   $0x0,0x20(%rsp)
    180001784:	lea    0x20(%rsp),%rdx
    180001789:	mov    %rax,0x28(%rsp)
    18000178e:	lea    0x2ba7b(%rip),%rcx        # 0x18002d210
    180001795:	movq   $0x18,0x30(%rsp)
    18000179e:	call   *0x19c2c(%rip)        # 0x18001b3d0
    1800017a4:	mov    0x20(%rsp),%rcx
@@ -8240,15 +8240,15 @@
    1800017c8:	call   *0x19bda(%rip)        # 0x18001b3a8
    1800017ce:	lea    0x18f9b(%rip),%rcx        # 0x18001a770
    1800017d5:	add    $0x48,%rsp
    1800017d9:	jmp    0x180019a00
    1800017de:	int3
    1800017df:	int3
    1800017e0:	sub    $0x48,%rsp
-   1800017e4:	lea    0x1cf2d(%rip),%rax        # 0x18001e718
+   1800017e4:	lea    0x1cf3d(%rip),%rax        # 0x18001e728
    1800017eb:	movq   $0x0,0x20(%rsp)
    1800017f4:	lea    0x20(%rsp),%rdx
    1800017f9:	mov    %rax,0x28(%rsp)
    1800017fe:	lea    0x2ba83(%rip),%rcx        # 0x18002d288
    180001805:	movq   $0x12,0x30(%rsp)
    18000180e:	call   *0x19bbc(%rip)        # 0x18001b3d0
    180001814:	mov    0x20(%rsp),%rcx
@@ -8264,15 +8264,15 @@
    180001838:	call   *0x19b6a(%rip)        # 0x18001b3a8
    18000183e:	lea    0x18f3b(%rip),%rcx        # 0x18001a780
    180001845:	add    $0x48,%rsp
    180001849:	jmp    0x180019a00
    18000184e:	int3
    18000184f:	int3
    180001850:	sub    $0x48,%rsp
-   180001854:	lea    0x1cee5(%rip),%rax        # 0x18001e740
+   180001854:	lea    0x1cef5(%rip),%rax        # 0x18001e750
    18000185b:	movq   $0x0,0x20(%rsp)
    180001864:	lea    0x20(%rsp),%rdx
    180001869:	mov    %rax,0x28(%rsp)
    18000186e:	lea    0x2b9fb(%rip),%rcx        # 0x18002d270
    180001875:	movq   $0xb,0x30(%rsp)
    18000187e:	call   *0x19b4c(%rip)        # 0x18001b3d0
    180001884:	mov    0x20(%rsp),%rcx
@@ -8288,15 +8288,15 @@
    1800018a8:	call   *0x19afa(%rip)        # 0x18001b3a8
    1800018ae:	lea    0x18edb(%rip),%rcx        # 0x18001a790
    1800018b5:	add    $0x48,%rsp
    1800018b9:	jmp    0x180019a00
    1800018be:	int3
    1800018bf:	int3
    1800018c0:	sub    $0x48,%rsp
-   1800018c4:	lea    0x1ce8d(%rip),%rax        # 0x18001e758
+   1800018c4:	lea    0x1ce9d(%rip),%rax        # 0x18001e768
    1800018cb:	movq   $0x0,0x20(%rsp)
    1800018d4:	lea    0x20(%rsp),%rdx
    1800018d9:	mov    %rax,0x28(%rsp)
    1800018de:	lea    0x2b913(%rip),%rcx        # 0x18002d1f8
    1800018e5:	movq   $0xf,0x30(%rsp)
    1800018ee:	call   *0x19adc(%rip)        # 0x18001b3d0
    1800018f4:	mov    0x20(%rsp),%rcx
@@ -8312,15 +8312,15 @@
    180001918:	call   *0x19a8a(%rip)        # 0x18001b3a8
    18000191e:	lea    0x18e7b(%rip),%rcx        # 0x18001a7a0
    180001925:	add    $0x48,%rsp
    180001929:	jmp    0x180019a00
    18000192e:	int3
    18000192f:	int3
    180001930:	sub    $0x48,%rsp
-   180001934:	lea    0x1ce3d(%rip),%rax        # 0x18001e778
+   180001934:	lea    0x1ce4d(%rip),%rax        # 0x18001e788
    18000193b:	movq   $0x0,0x20(%rsp)
    180001944:	lea    0x20(%rsp),%rdx
    180001949:	mov    %rax,0x28(%rsp)
    18000194e:	lea    0x2b94b(%rip),%rcx        # 0x18002d2a0
    180001955:	movq   $0x16,0x30(%rsp)
    18000195e:	call   *0x19a6c(%rip)        # 0x18001b3d0
    180001964:	mov    0x20(%rsp),%rcx
@@ -8336,15 +8336,15 @@
    180001988:	call   *0x19a1a(%rip)        # 0x18001b3a8
    18000198e:	lea    0x18e1b(%rip),%rcx        # 0x18001a7b0
    180001995:	add    $0x48,%rsp
    180001999:	jmp    0x180019a00
    18000199e:	int3
    18000199f:	int3
    1800019a0:	sub    $0x48,%rsp
-   1800019a4:	lea    0x1cdfd(%rip),%rax        # 0x18001e7a8
+   1800019a4:	lea    0x1ce0d(%rip),%rax        # 0x18001e7b8
    1800019ab:	movq   $0x0,0x20(%rsp)
    1800019b4:	lea    0x20(%rsp),%rdx
    1800019b9:	mov    %rax,0x28(%rsp)
    1800019be:	lea    0x2b893(%rip),%rcx        # 0x18002d258
    1800019c5:	movq   $0xf,0x30(%rsp)
    1800019ce:	call   *0x199fc(%rip)        # 0x18001b3d0
    1800019d4:	mov    0x20(%rsp),%rcx
@@ -8360,15 +8360,15 @@
    1800019f8:	call   *0x199aa(%rip)        # 0x18001b3a8
    1800019fe:	lea    0x18dbb(%rip),%rcx        # 0x18001a7c0
    180001a05:	add    $0x48,%rsp
    180001a09:	jmp    0x180019a00
    180001a0e:	int3
    180001a0f:	int3
    180001a10:	sub    $0x48,%rsp
-   180001a14:	lea    0x1cdad(%rip),%rax        # 0x18001e7c8
+   180001a14:	lea    0x1cdbd(%rip),%rax        # 0x18001e7d8
    180001a1b:	movq   $0x0,0x20(%rsp)
    180001a24:	lea    0x20(%rsp),%rdx
    180001a29:	mov    %rax,0x28(%rsp)
    180001a2e:	lea    0x2b80b(%rip),%rcx        # 0x18002d240
    180001a35:	movq   $0xb,0x30(%rsp)
    180001a3e:	call   *0x1998c(%rip)        # 0x18001b3d0
    180001a44:	mov    0x20(%rsp),%rcx
@@ -8384,15 +8384,15 @@
    180001a68:	call   *0x1993a(%rip)        # 0x18001b3a8
    180001a6e:	lea    0x18d5b(%rip),%rcx        # 0x18001a7d0
    180001a75:	add    $0x48,%rsp
    180001a79:	jmp    0x180019a00
    180001a7e:	int3
    180001a7f:	int3
    180001a80:	sub    $0x48,%rsp
-   180001a84:	lea    0x1cd55(%rip),%rax        # 0x18001e7e0
+   180001a84:	lea    0x1cd65(%rip),%rax        # 0x18001e7f0
    180001a8b:	movq   $0x0,0x20(%rsp)
    180001a94:	lea    0x20(%rsp),%rdx
    180001a99:	mov    %rax,0x28(%rsp)
    180001a9e:	lea    0x2b82b(%rip),%rcx        # 0x18002d2d0
    180001aa5:	movq   $0x12,0x30(%rsp)
    180001aae:	call   *0x1991c(%rip)        # 0x18001b3d0
    180001ab4:	mov    0x20(%rsp),%rcx
@@ -8408,15 +8408,15 @@
    180001ad8:	call   *0x198ca(%rip)        # 0x18001b3a8
    180001ade:	lea    0x18cfb(%rip),%rcx        # 0x18001a7e0
    180001ae5:	add    $0x48,%rsp
    180001ae9:	jmp    0x180019a00
    180001aee:	int3
    180001aef:	int3
    180001af0:	sub    $0x48,%rsp
-   180001af4:	lea    0x1cd0d(%rip),%rax        # 0x18001e808
+   180001af4:	lea    0x1cd1d(%rip),%rax        # 0x18001e818
    180001afb:	movq   $0x0,0x20(%rsp)
    180001b04:	lea    0x20(%rsp),%rdx
    180001b09:	mov    %rax,0x28(%rsp)
    180001b0e:	lea    0x2b7d3(%rip),%rcx        # 0x18002d2e8
    180001b15:	movq   $0xe,0x30(%rsp)
    180001b1e:	call   *0x198ac(%rip)        # 0x18001b3d0
    180001b24:	mov    0x20(%rsp),%rcx
@@ -8432,15 +8432,15 @@
    180001b48:	call   *0x1985a(%rip)        # 0x18001b3a8
    180001b4e:	lea    0x18c9b(%rip),%rcx        # 0x18001a7f0
    180001b55:	add    $0x48,%rsp
    180001b59:	jmp    0x180019a00
    180001b5e:	int3
    180001b5f:	int3
    180001b60:	sub    $0x48,%rsp
-   180001b64:	lea    0x1ccbd(%rip),%rax        # 0x18001e828
+   180001b64:	lea    0x1cccd(%rip),%rax        # 0x18001e838
    180001b6b:	movq   $0x0,0x20(%rsp)
    180001b74:	lea    0x20(%rsp),%rdx
    180001b79:	mov    %rax,0x28(%rsp)
    180001b7e:	lea    0x2b6a3(%rip),%rcx        # 0x18002d228
    180001b85:	movq   $0xd,0x30(%rsp)
    180001b8e:	call   *0x1983c(%rip)        # 0x18001b3d0
    180001b94:	mov    0x20(%rsp),%rcx
@@ -11713,15 +11713,15 @@
    180004510:	mov    %rbx,0x8(%rsp)
    180004515:	mov    %rsi,0x10(%rsp)
    18000451a:	mov    %rdi,0x18(%rsp)
    18000451f:	push   %r14
    180004521:	sub    $0x20,%rsp
    180004525:	mov    %rdx,%rbx
    180004528:	mov    %r9,%rdi
-   18000452b:	mov    $0x60501,%edx
+   18000452b:	mov    $0x60502,%edx
    180004530:	mov    %r8,%rsi
    180004533:	mov    %rcx,%r14
    180004536:	call   *0x16eec(%rip)        # 0x18001b428
    18000453c:	lea    0x1926d(%rip),%rax        # 0x18001d7b0
    180004543:	xor    %r8d,%r8d
    180004546:	lea    0x78(%r14),%rcx
    18000454a:	mov    %rax,(%r14)
@@ -13365,15 +13365,15 @@
    180005ad0:	rex push %rbx
    180005ad2:	sub    $0x30,%rsp
    180005ad6:	mov    %r9d,0x20(%rsp)
    180005adb:	mov    %rcx,%rbx
    180005ade:	mov    %r8,%r9
    180005ae1:	mov    %rdx,%r8
    180005ae4:	mov    %rcx,%rdx
-   180005ae7:	lea    0x19932(%rip),%rcx        # 0x18001f420
+   180005ae7:	lea    0x19942(%rip),%rcx        # 0x18001f430
    180005aee:	call   *0x1572c(%rip)        # 0x18001b220
    180005af4:	mov    %rbx,%rax
    180005af7:	add    $0x30,%rsp
    180005afb:	pop    %rbx
    180005afc:	ret
    180005afd:	int3
    180005afe:	int3
@@ -13459,15 +13459,15 @@
    180005bc3:	rex.W jmp *0x1587e(%rip)        # 0x18001b448
    180005bca:	int3
    180005bcb:	int3
    180005bcc:	int3
    180005bcd:	int3
    180005bce:	int3
    180005bcf:	int3
-   180005bd0:	lea    0x17e99(%rip),%rax        # 0x18001da70
+   180005bd0:	lea    0x18599(%rip),%rax        # 0x18001e170
    180005bd7:	ret
    180005bd8:	int3
    180005bd9:	int3
    180005bda:	int3
    180005bdb:	int3
    180005bdc:	int3
    180005bdd:	int3
@@ -13551,69 +13551,69 @@
    180005c84:	lea    -0x5c8b(%rip),%rdx        # 0x180000000
    180005c8b:	movslq %r8d,%rax
    180005c8e:	mov    %r14,0x18(%r11)
    180005c92:	mov    0x6248(%rdx,%rax,4),%eax
    180005c99:	add    %rdx,%rax
    180005c9c:	jmp    *%rax
    180005c9e:	mov    0x8(%r9),%rax
-   180005ca2:	lea    0x17dc7(%rip),%rdx        # 0x18001da70
+   180005ca2:	lea    0x184c7(%rip),%rdx        # 0x18001e170
    180005ca9:	lea    -0x28(%rbp),%r9
    180005cad:	mov    %rax,-0x20(%rbp)
    180005cb1:	xor    %r8d,%r8d
    180005cb4:	movq   $0x0,-0x28(%rbp)
    180005cbc:	call   *0x15566(%rip)        # 0x18001b228
    180005cc2:	jmp    0x180005e38
    180005cc7:	mov    0x8(%r9),%rax
-   180005ccb:	lea    0x17d9e(%rip),%rdx        # 0x18001da70
+   180005ccb:	lea    0x1849e(%rip),%rdx        # 0x18001e170
    180005cd2:	lea    -0x28(%rbp),%r9
    180005cd6:	mov    %rax,-0x20(%rbp)
    180005cda:	mov    $0x1,%r8d
    180005ce0:	movq   $0x0,-0x28(%rbp)
    180005ce8:	call   *0x1553a(%rip)        # 0x18001b228
    180005cee:	jmp    0x180005e38
    180005cf3:	mov    0x8(%r9),%rax
-   180005cf7:	lea    0x17d72(%rip),%rdx        # 0x18001da70
+   180005cf7:	lea    0x18472(%rip),%rdx        # 0x18001e170
    180005cfe:	lea    -0x28(%rbp),%r9
    180005d02:	mov    %rax,-0x20(%rbp)
    180005d06:	mov    $0x2,%r8d
    180005d0c:	movq   $0x0,-0x28(%rbp)
    180005d14:	call   *0x1550e(%rip)        # 0x18001b228
    180005d1a:	jmp    0x180005e38
    180005d1f:	mov    0x8(%r9),%rax
-   180005d23:	lea    0x17d46(%rip),%rdx        # 0x18001da70
+   180005d23:	lea    0x18446(%rip),%rdx        # 0x18001e170
    180005d2a:	lea    -0x28(%rbp),%r9
    180005d2e:	mov    %rax,-0x20(%rbp)
    180005d32:	mov    $0x3,%r8d
    180005d38:	movq   $0x0,-0x28(%rbp)
    180005d40:	call   *0x154e2(%rip)        # 0x18001b228
    180005d46:	jmp    0x180005e38
    180005d4b:	mov    0x8(%r9),%rax
-   180005d4f:	lea    0x17d1a(%rip),%rdx        # 0x18001da70
+   180005d4f:	lea    0x1841a(%rip),%rdx        # 0x18001e170
    180005d56:	lea    -0x28(%rbp),%r9
    180005d5a:	mov    %rax,-0x20(%rbp)
    180005d5e:	mov    $0x4,%r8d
    180005d64:	movq   $0x0,-0x28(%rbp)
    180005d6c:	call   *0x154b6(%rip)        # 0x18001b228
    180005d72:	jmp    0x180005e38
    180005d77:	mov    0x8(%r9),%rdx
    180005d7b:	call   0x1800072c0
    180005d80:	jmp    0x180005e38
    180005d85:	mov    0x8(%r9),%rax
-   180005d89:	lea    0x17ce0(%rip),%rdx        # 0x18001da70
+   180005d89:	lea    0x183e0(%rip),%rdx        # 0x18001e170
    180005d90:	lea    -0x28(%rbp),%r9
    180005d94:	mov    %rax,-0x20(%rbp)
    180005d98:	mov    $0x6,%r8d
    180005d9e:	movq   $0x0,-0x28(%rbp)
    180005da6:	call   *0x1547c(%rip)        # 0x18001b228
    180005dac:	jmp    0x180005e38
    180005db1:	mov    0x8(%r9),%rdx
    180005db5:	call   0x180008280
    180005dba:	jmp    0x180005e38
    180005dbc:	mov    0x8(%r9),%rax
-   180005dc0:	lea    0x17ca9(%rip),%rdx        # 0x18001da70
+   180005dc0:	lea    0x183a9(%rip),%rdx        # 0x18001e170
    180005dc7:	mov    %rax,-0x20(%rbp)
    180005dcb:	mov    $0x8,%r8d
    180005dd1:	mov    0x10(%r9),%rax
    180005dd5:	mov    %rax,-0x18(%rbp)
    180005dd9:	mov    0x18(%r9),%rax
    180005ddd:	lea    -0x28(%rbp),%r9
    180005de1:	mov    %rax,-0x10(%rbp)
@@ -13959,15 +13959,15 @@
    1800062cd:	int3
    1800062ce:	int3
    1800062cf:	int3
    1800062d0:	rex push %rbx
    1800062d2:	sub    $0x20,%rsp
    1800062d6:	mov    %rcx,%rbx
    1800062d9:	call   0x1800044d0
-   1800062de:	lea    0x181bb(%rip),%rax        # 0x18001e4a0
+   1800062de:	lea    0x181c3(%rip),%rax        # 0x18001e4a8
    1800062e5:	mov    %rax,(%rbx)
    1800062e8:	mov    %rbx,%rax
    1800062eb:	add    $0x20,%rsp
    1800062ef:	pop    %rbx
    1800062f0:	ret
    1800062f1:	int3
    1800062f2:	int3
@@ -14012,18 +14012,18 @@
    18000635f:	call   *0x14eeb(%rip)        # 0x18001b250
    180006365:	mov    %rbx,%rdx
    180006368:	lea    -0x31(%rbp),%rcx
    18000636c:	call   *0x14ede(%rip)        # 0x18001b250
    180006372:	lea    -0x49(%rbp),%r9
    180006376:	mov    %rsi,0x20(%rsp)
    18000637b:	mov    %rdi,%r8
-   18000637e:	lea    0x181f3(%rip),%rdx        # 0x18001e578
+   18000637e:	lea    0x181fb(%rip),%rdx        # 0x18001e580
    180006385:	mov    %r14,%rcx
    180006388:	call   0x180004510
-   18000638d:	lea    0x181d4(%rip),%rax        # 0x18001e568
+   18000638d:	lea    0x181dc(%rip),%rax        # 0x18001e570
    180006394:	lea    0x148(%r14),%rcx
    18000639b:	mov    %rax,(%r14)
    18000639e:	lea    -0x31(%rbp),%rdx
    1800063a2:	call   *0x14e98(%rip)        # 0x18001b240
    1800063a8:	lea    0x160(%r14),%rcx
    1800063af:	call   *0x14e83(%rip)        # 0x18001b238
    1800063b5:	mov    $0x8,%dl
@@ -14046,15 +14046,15 @@
    1800063f3:	mov    %rax,0x38(%rsp)
    1800063f8:	lea    0x178(%r14),%rcx
    1800063ff:	movaps 0x30(%rsp),%xmm0
    180006404:	movdqa %xmm0,0x30(%rsp)
    18000640a:	call   *0x150f8(%rip)        # 0x18001b508
    180006410:	lea    -0x19(%rbp),%rcx
    180006414:	call   *0x14db6(%rip)        # 0x18001b1d0
-   18000641a:	lea    0x1816f(%rip),%rax        # 0x18001e590
+   18000641a:	lea    0x1817f(%rip),%rax        # 0x18001e5a0
    180006421:	movq   $0x0,-0x79(%rbp)
    180006429:	lea    0x190(%r14),%rcx
    180006430:	mov    %rax,-0x71(%rbp)
    180006434:	lea    -0x79(%rbp),%rdx
    180006438:	movq   $0x20,-0x69(%rbp)
    180006440:	call   *0x14f8a(%rip)        # 0x18001b3d0
    180006446:	mov    -0x79(%rbp),%rcx
@@ -14067,15 +14067,15 @@
    18000645d:	jne    0x180006470
    18000645f:	mov    -0x79(%rbp),%rcx
    180006463:	lea    0x3(%rbx),%edx
    180006466:	lea    0x9(%rbx),%r8d
    18000646a:	call   *0x14f38(%rip)        # 0x18001b3a8
    180006470:	lea    0x1a8(%r14),%rcx
    180006477:	call   *0x14dbb(%rip)        # 0x18001b238
-   18000647d:	lea    0x18154(%rip),%rax        # 0x18001e5d8
+   18000647d:	lea    0x18164(%rip),%rax        # 0x18001e5e8
    180006484:	movq   $0x0,-0x61(%rbp)
    18000648c:	lea    0x1c0(%r14),%rcx
    180006493:	mov    %rax,-0x59(%rbp)
    180006497:	lea    -0x61(%rbp),%rdx
    18000649b:	movq   $0x9,-0x51(%rbp)
    1800064a3:	call   *0x14f27(%rip)        # 0x18001b3d0
    1800064a9:	mov    -0x61(%rbp),%rax
@@ -14103,15 +14103,15 @@
    18000650a:	call   *0x14d38(%rip)        # 0x18001b248
    180006510:	lea    -0x1(%rbp),%rcx
    180006514:	call   *0x14d2e(%rip)        # 0x18001b248
    18000651a:	lea    0x17(%rbp),%rcx
    18000651e:	call   *0x14d24(%rip)        # 0x18001b248
    180006524:	lea    0x67(%rbp),%rcx
    180006528:	call   *0x14d6a(%rip)        # 0x18001b298
-   18000652e:	lea    0x17f6b(%rip),%rax        # 0x18001e4a0
+   18000652e:	lea    0x17f73(%rip),%rax        # 0x18001e4a8
    180006535:	lea    0xf0(%rsp),%r11
    18000653d:	mov    %rax,(%r15)
    180006540:	mov    0x38(%r11),%rbx
    180006544:	mov    %r15,%rax
    180006547:	mov    0x40(%r11),%rsi
    18000654b:	mov    %r11,%rsp
    18000654e:	pop    %r15
@@ -14131,15 +14131,15 @@
    18000655f:	int3
    180006560:	rex push %rbx
    180006562:	sub    $0x20,%rsp
    180006566:	mov    %rdx,%r8
    180006569:	mov    %rcx,%rbx
    18000656c:	xor    %edx,%edx
    18000656e:	call   0x180006300
-   180006573:	lea    0x17f26(%rip),%rax        # 0x18001e4a0
+   180006573:	lea    0x17f2e(%rip),%rax        # 0x18001e4a8
    18000657a:	mov    %rax,(%rbx)
    18000657d:	mov    %rbx,%rax
    180006580:	add    $0x20,%rsp
    180006584:	pop    %rbx
    180006585:	ret
    180006586:	int3
    180006587:	int3
@@ -14156,17 +14156,17 @@
    18000659a:	mov    %rsi,0x18(%rsp)
    18000659f:	push   %rdi
    1800065a0:	sub    $0x90,%rsp
    1800065a7:	mov    %r9,0x20(%rsp)
    1800065ac:	mov    %rdx,%rbx
    1800065af:	mov    %rdx,%r9
    1800065b2:	mov    %rcx,%rdi
-   1800065b5:	lea    0x17fbc(%rip),%rdx        # 0x18001e578
+   1800065b5:	lea    0x17fc4(%rip),%rdx        # 0x18001e580
    1800065bc:	call   0x180004510
-   1800065c1:	lea    0x17fa0(%rip),%rax        # 0x18001e568
+   1800065c1:	lea    0x17fa8(%rip),%rax        # 0x18001e570
    1800065c8:	lea    0x18(%rbx),%rdx
    1800065cc:	mov    %rax,(%rdi)
    1800065cf:	lea    0x148(%rdi),%rcx
    1800065d6:	call   *0x14c64(%rip)        # 0x18001b240
    1800065dc:	lea    0x160(%rdi),%rcx
    1800065e3:	call   *0x14c4f(%rip)        # 0x18001b238
    1800065e9:	mov    $0x8,%dl
@@ -14187,15 +14187,15 @@
    18000661e:	lea    0x30(%rsp),%rdx
    180006623:	mov    %rbp,0x30(%rsp)
    180006628:	lea    0x178(%rdi),%rcx
    18000662f:	mov    %rax,0x38(%rsp)
    180006634:	call   *0x14ece(%rip)        # 0x18001b508
    18000663a:	lea    0x70(%rsp),%rcx
    18000663f:	call   *0x14b8b(%rip)        # 0x18001b1d0
-   180006645:	lea    0x17f44(%rip),%rax        # 0x18001e590
+   180006645:	lea    0x17f54(%rip),%rax        # 0x18001e5a0
    18000664c:	movq   $0x0,0x40(%rsp)
    180006655:	lea    0x190(%rdi),%rcx
    18000665c:	mov    %rax,0x48(%rsp)
    180006661:	lea    0x40(%rsp),%rdx
    180006666:	movq   $0x20,0x50(%rsp)
    18000666f:	call   *0x14d5b(%rip)        # 0x18001b3d0
    180006675:	mov    0x40(%rsp),%rcx
@@ -14208,15 +14208,15 @@
    18000668d:	jne    0x1800066a1
    18000668f:	mov    0x40(%rsp),%rcx
    180006694:	lea    0x3(%rbx),%edx
    180006697:	lea    0x9(%rbx),%r8d
    18000669b:	call   *0x14d07(%rip)        # 0x18001b3a8
    1800066a1:	lea    0x1a8(%rdi),%rcx
    1800066a8:	call   *0x14b8a(%rip)        # 0x18001b238
-   1800066ae:	lea    0x17f23(%rip),%rax        # 0x18001e5d8
+   1800066ae:	lea    0x17f33(%rip),%rax        # 0x18001e5e8
    1800066b5:	movq   $0x0,0x58(%rsp)
    1800066be:	lea    0x1c0(%rdi),%rcx
    1800066c5:	mov    %rax,0x60(%rsp)
    1800066ca:	lea    0x58(%rsp),%rdx
    1800066cf:	movq   $0x9,0x68(%rsp)
    1800066d8:	call   *0x14cf2(%rip)        # 0x18001b3d0
    1800066de:	mov    0x58(%rsp),%rax
@@ -14238,21 +14238,21 @@
    18000672c:	mov    0x10(%r11),%rbx
    180006730:	mov    %rdi,%rax
    180006733:	mov    0x18(%r11),%rbp
    180006737:	mov    0x20(%r11),%rsi
    18000673b:	mov    %r11,%rsp
    18000673e:	pop    %rdi
    18000673f:	ret
-   180006740:	lea    0x17d59(%rip),%rax        # 0x18001e4a0
+   180006740:	lea    0x17d61(%rip),%rax        # 0x18001e4a8
    180006747:	mov    %rax,(%rcx)
    18000674a:	jmp    0x180004610
    18000674f:	int3
    180006750:	rex push %rbx
    180006752:	sub    $0x20,%rsp
-   180006756:	lea    0x17e0b(%rip),%rax        # 0x18001e568
+   180006756:	lea    0x17e13(%rip),%rax        # 0x18001e570
    18000675d:	mov    %rcx,%rbx
    180006760:	mov    %rax,(%rcx)
    180006763:	add    $0x1f8,%rcx
    18000676a:	cmpb   $0x0,0x8(%rcx)
    18000676e:	je     0x180006776
    180006770:	call   *0x1519a(%rip)        # 0x18001b910
    180006776:	lea    0x1e0(%rbx),%rcx
@@ -14284,44 +14284,44 @@
    1800067f4:	mov    0x2512d(%rip),%rax        # 0x18002b928
    1800067fb:	xor    %rsp,%rax
    1800067fe:	mov    %rax,0x68(%rsp)
    180006803:	mov    0x26843(%rip),%eax        # 0x18002d04c
    180006809:	nop
    18000680a:	test   %eax,%eax
    18000680c:	jne    0x1800068d0
-   180006812:	movdqa 0x17e06(%rip),%xmm0        # 0x18001e620
+   180006812:	movdqa 0x17e16(%rip),%xmm0        # 0x18001e630
    18000681a:	lea    0x12(%rax),%edx
-   18000681d:	lea    0x1705c(%rip),%rcx        # 0x18001d880
+   18000681d:	lea    0x17754(%rip),%rcx        # 0x18001df78
    180006824:	movw   $0x6e,0x60(%rsp)
    18000682b:	movdqu %xmm0,0x50(%rsp)
    180006831:	call   *0x14cb1(%rip)        # 0x18001b4e8
    180006837:	lea    0x50(%rsp),%rcx
    18000683c:	mov    $0xffffffffffffffff,%r8
    180006843:	inc    %r8
    180006846:	cmpb   $0x0,(%rcx,%r8,1)
    18000684b:	jne    0x180006843
    18000684d:	mov    %rbx,0x70(%rsp)
    180006852:	cmp    %rax,%r8
    180006855:	jne    0x18000689a
    180006857:	test   %r8,%r8
    18000685a:	je     0x180006871
-   18000685c:	lea    0x1701d(%rip),%rdx        # 0x18001d880
+   18000685c:	lea    0x17715(%rip),%rdx        # 0x18001df78
    180006863:	lea    0x50(%rsp),%rcx
    180006868:	call   0x18001a42c
    18000686d:	test   %eax,%eax
    18000686f:	jne    0x18000689a
    180006871:	mov    $0xffffffffffffffff,%r8
    180006878:	lea    0x50(%rsp),%rdx
    18000687d:	lea    0x20(%rsp),%rcx
    180006882:	call   *0x14c68(%rip)        # 0x18001b4f0
    180006888:	lea    0x20(%rsp),%rcx
    18000688d:	call   *0x1509d(%rip)        # 0x18001b930
    180006893:	lea    0x20(%rsp),%rcx
    180006898:	jmp    0x1800068bc
-   18000689a:	lea    0x16fdf(%rip),%rdx        # 0x18001d880
+   18000689a:	lea    0x176d7(%rip),%rdx        # 0x18001df78
    1800068a1:	lea    0x38(%rsp),%rcx
    1800068a6:	call   *0x14c64(%rip)        # 0x18001b510
    1800068ac:	lea    0x38(%rsp),%rcx
    1800068b1:	call   *0x15079(%rip)        # 0x18001b930
    1800068b7:	lea    0x38(%rsp),%rcx
    1800068bc:	mov    %eax,%ebx
    1800068be:	call   *0x1490c(%rip)        # 0x18001b1d0
@@ -14534,15 +14534,15 @@
    180006bae:	mov    -0x8(%rcx),%rdi
    180006bb2:	mov    %rdi,%rbx
    180006bb5:	mov    %r14,0x50(%rsp)
    180006bba:	shl    $0x4,%rbx
    180006bbe:	add    %rcx,%rbx
    180006bc1:	test   %rdi,%rdi
    180006bc4:	je     0x180006be5
-   180006bc6:	lea    0x178d3(%rip),%rbp        # 0x18001e4a0
+   180006bc6:	lea    0x178db(%rip),%rbp        # 0x18001e4a8
    180006bcd:	nopl   (%rax)
    180006bd0:	sub    $0x10,%rbx
    180006bd4:	mov    %rbx,%rcx
    180006bd7:	mov    %rbp,(%rbx)
    180006bda:	call   0x180004610
    180006bdf:	sub    $0x1,%rdi
    180006be3:	jne    0x180006bd0
@@ -14558,15 +14558,15 @@
    180006c0a:	mov    0x50(%rsp),%r14
    180006c0f:	lea    -0x8(%rsi),%rax
    180006c13:	add    $0x20,%rsp
    180006c17:	pop    %r15
    180006c19:	pop    %rsi
    180006c1a:	pop    %rbp
    180006c1b:	ret
-   180006c1c:	lea    0x1787d(%rip),%rbp        # 0x18001e4a0
+   180006c1c:	lea    0x17885(%rip),%rbp        # 0x18001e4a8
    180006c23:	mov    %rbp,(%rcx)
    180006c26:	call   0x180004610
    180006c2b:	test   $0x1,%r15b
    180006c2f:	je     0x180006c3e
    180006c31:	mov    $0x10,%edx
    180006c36:	mov    %rsi,%rcx
    180006c39:	call   0x180019368
@@ -14584,15 +14584,15 @@
    180006c4f:	int3
    180006c50:	rex push %rbx
    180006c52:	sub    $0x20,%rsp
    180006c56:	xor    %r8d,%r8d
    180006c59:	xor    %edx,%edx
    180006c5b:	mov    %rcx,%rbx
    180006c5e:	call   0x180006300
-   180006c63:	lea    0x17836(%rip),%rax        # 0x18001e4a0
+   180006c63:	lea    0x1783e(%rip),%rax        # 0x18001e4a8
    180006c6a:	mov    %rax,(%rbx)
    180006c6d:	add    $0x20,%rsp
    180006c71:	pop    %rbx
    180006c72:	ret
    180006c73:	int3
    180006c74:	int3
    180006c75:	int3
@@ -14605,15 +14605,15 @@
    180006c7c:	int3
    180006c7d:	int3
    180006c7e:	int3
    180006c7f:	int3
    180006c80:	mov    %rbx,0x8(%rsp)
    180006c85:	push   %rdi
    180006c86:	sub    $0x20,%rsp
-   180006c8a:	lea    0x178d7(%rip),%rax        # 0x18001e568
+   180006c8a:	lea    0x178df(%rip),%rax        # 0x18001e570
    180006c91:	mov    %rcx,%rbx
    180006c94:	mov    %rax,(%rcx)
    180006c97:	mov    %edx,%edi
    180006c99:	add    $0x1f8,%rcx
    180006ca0:	cmpb   $0x0,0x8(%rcx)
    180006ca4:	je     0x180006cac
    180006ca6:	call   *0x14c64(%rip)        # 0x18001b910
@@ -14647,15 +14647,15 @@
    180006d3c:	ret
    180006d3d:	int3
    180006d3e:	int3
    180006d3f:	int3
    180006d40:	sub    $0x38,%rsp
    180006d44:	mov    %rdx,0x28(%rsp)
    180006d49:	lea    0x20(%rsp),%r9
-   180006d4e:	lea    0x16d1b(%rip),%rdx        # 0x18001da70
+   180006d4e:	lea    0x1741b(%rip),%rdx        # 0x18001e170
    180006d55:	movq   $0x0,0x20(%rsp)
    180006d5e:	mov    $0x9,%r8d
    180006d64:	call   *0x144be(%rip)        # 0x18001b228
    180006d6a:	add    $0x38,%rsp
    180006d6e:	ret
    180006d6f:	int3
    180006d70:	rex push %rbx
@@ -14678,15 +14678,15 @@
    180006d9c:	int3
    180006d9d:	int3
    180006d9e:	int3
    180006d9f:	int3
    180006da0:	sub    $0x38,%rsp
    180006da4:	mov    %rdx,0x28(%rsp)
    180006da9:	lea    0x20(%rsp),%r9
-   180006dae:	lea    0x16cbb(%rip),%rdx        # 0x18001da70
+   180006dae:	lea    0x173bb(%rip),%rdx        # 0x18001e170
    180006db5:	movq   $0x0,0x20(%rsp)
    180006dbe:	mov    $0x3,%r8d
    180006dc4:	call   *0x1445e(%rip)        # 0x18001b228
    180006dca:	add    $0x38,%rsp
    180006dce:	ret
    180006dcf:	int3
    180006dd0:	mov    %rbx,0x10(%rsp)
@@ -14706,15 +14706,15 @@
    180006e08:	lea    0x40(%rsp),%rcx
    180006e0d:	xor    %r9d,%r9d
    180006e10:	mov    %rax,0x20(%rsp)
    180006e15:	xor    %r8d,%r8d
    180006e18:	xor    %edx,%edx
    180006e1a:	call   *0x146b8(%rip)        # 0x18001b4d8
    180006e20:	mov    %rax,%rcx
-   180006e23:	lea    0x177d6(%rip),%rdx        # 0x18001e600
+   180006e23:	lea    0x177e6(%rip),%rdx        # 0x18001e610
    180006e2a:	call   *0x146b0(%rip)        # 0x18001b4e0
    180006e30:	mov    %rsi,%rcx
    180006e33:	call   *0x14447(%rip)        # 0x18001b280
    180006e39:	jmp    0x180006f27
    180006e3e:	mov    %r8,%rdx
    180006e41:	lea    0x70(%rsp),%rcx
    180006e46:	call   *0x1443c(%rip)        # 0x18001b288
@@ -14848,15 +14848,15 @@
    18000706f:	xor    %r9d,%r9d
    180007072:	lea    0x58(%rsp),%rdx
    180007077:	call   *0x1447b(%rip)        # 0x18001b4f8
    18000707d:	lea    0x70(%rsp),%rdx
    180007082:	lea    0x58(%rsp),%rcx
    180007087:	call   *0x14473(%rip)        # 0x18001b500
    18000708d:	mov    $0xffffffffffffffff,%r8
-   180007094:	lea    0x17555(%rip),%rdx        # 0x18001e5f0
+   180007094:	lea    0x17565(%rip),%rdx        # 0x18001e600
    18000709b:	lea    0x40(%rsp),%rcx
    1800070a0:	mov    %rax,%rbx
    1800070a3:	call   *0x14447(%rip)        # 0x18001b4f0
    1800070a9:	mov    %rbx,%r8
    1800070ac:	lea    0x40(%rsp),%rdx
    1800070b1:	mov    %rsi,%rcx
    1800070b4:	call   *0x1483e(%rip)        # 0x18001b8f8
@@ -14950,15 +14950,15 @@
    18000722e:	int3
    18000722f:	int3
    180007230:	sub    $0x58,%rsp
    180007234:	mov    0x246ed(%rip),%rax        # 0x18002b928
    18000723b:	xor    %rsp,%rax
    18000723e:	mov    %rax,0x40(%rsp)
    180007243:	mov    %rdx,0x28(%rsp)
-   180007248:	lea    0x16821(%rip),%rdx        # 0x18001da70
+   180007248:	lea    0x16f21(%rip),%rdx        # 0x18001e170
    18000724f:	mov    %r8,0x30(%rsp)
    180007254:	mov    $0x8,%r8d
    18000725a:	mov    %r9,0x38(%rsp)
    18000725f:	lea    0x20(%rsp),%r9
    180007264:	movq   $0x0,0x20(%rsp)
    18000726d:	call   *0x13fb5(%rip)        # 0x18001b228
    180007273:	mov    0x40(%rsp),%rcx
@@ -14997,15 +14997,15 @@
    1800072bc:	int3
    1800072bd:	int3
    1800072be:	int3
    1800072bf:	int3
    1800072c0:	sub    $0x38,%rsp
    1800072c4:	mov    %rdx,0x28(%rsp)
    1800072c9:	lea    0x20(%rsp),%r9
-   1800072ce:	lea    0x1679b(%rip),%rdx        # 0x18001da70
+   1800072ce:	lea    0x16e9b(%rip),%rdx        # 0x18001e170
    1800072d5:	movq   $0x0,0x20(%rsp)
    1800072de:	mov    $0x5,%r8d
    1800072e4:	call   *0x13f3e(%rip)        # 0x18001b228
    1800072ea:	add    $0x38,%rsp
    1800072ee:	ret
    1800072ef:	int3
    1800072f0:	mov    %rbx,0x8(%rsp)
@@ -15227,15 +15227,15 @@
    18000761d:	int3
    18000761e:	int3
    18000761f:	int3
    180007620:	mov    0x8(%rcx),%rcx
    180007624:	cmpq   $0x0,0x38(%rcx)
    180007629:	je     0x180007632
    18000762b:	rex.W jmp *0x13cd6(%rip)        # 0x18001b308
-   180007632:	lea    0x16437(%rip),%rax        # 0x18001da70
+   180007632:	lea    0x16b37(%rip),%rax        # 0x18001e170
    180007639:	ret
    18000763a:	int3
    18000763b:	int3
    18000763c:	int3
    18000763d:	int3
    18000763e:	int3
    18000763f:	int3
@@ -15428,15 +15428,15 @@
    18000794e:	xor    %r9d,%r9d
    180007951:	lea    0x48(%rsp),%rdx
    180007956:	call   *0x13b9c(%rip)        # 0x18001b4f8
    18000795c:	lea    0x60(%rsp),%rdx
    180007961:	lea    0x48(%rsp),%rcx
    180007966:	call   *0x13b94(%rip)        # 0x18001b500
    18000796c:	mov    $0xffffffffffffffff,%r8
-   180007973:	lea    0x16c76(%rip),%rdx        # 0x18001e5f0
+   180007973:	lea    0x16c86(%rip),%rdx        # 0x18001e600
    18000797a:	lea    0x30(%rsp),%rcx
    18000797f:	mov    %rax,%rbx
    180007982:	call   *0x13b68(%rip)        # 0x18001b4f0
    180007988:	mov    %rbx,%r8
    18000798b:	lea    0x30(%rsp),%rdx
    180007990:	mov    %rdi,%rcx
    180007993:	call   *0x13f5f(%rip)        # 0x18001b8f8
@@ -15689,15 +15689,15 @@
    180007d1f:	int3
    180007d20:	mov    %rdx,%r9
    180007d23:	mov    %rcx,%r10
    180007d26:	test   %rdx,%rdx
    180007d29:	jne    0x180007d2e
    180007d2b:	xor    %eax,%eax
    180007d2d:	ret
-   180007d2e:	lea    0x15e93(%rip),%r8        # 0x18001dbc8
+   180007d2e:	lea    0x16593(%rip),%r8        # 0x18001e2c8
    180007d35:	mov    %r9,%rax
    180007d38:	sub    %r9,%r8
    180007d3b:	nopl   0x0(%rax,%rax,1)
    180007d40:	movzbl (%rax),%edx
    180007d43:	movzbl (%rax,%r8,1),%ecx
    180007d48:	sub    %ecx,%edx
    180007d4a:	jne    0x180007d53
@@ -15741,15 +15741,15 @@
    180007d9c:	int3
    180007d9d:	int3
    180007d9e:	int3
    180007d9f:	int3
    180007da0:	sub    $0x38,%rsp
    180007da4:	mov    %rdx,0x28(%rsp)
    180007da9:	lea    0x20(%rsp),%r9
-   180007dae:	lea    0x15cbb(%rip),%rdx        # 0x18001da70
+   180007dae:	lea    0x163bb(%rip),%rdx        # 0x18001e170
    180007db5:	movq   $0x0,0x20(%rsp)
    180007dbe:	mov    $0x6,%r8d
    180007dc4:	call   *0x1345e(%rip)        # 0x18001b228
    180007dca:	add    $0x38,%rsp
    180007dce:	ret
    180007dcf:	int3
    180007dd0:	rex push %rbx
@@ -15772,15 +15772,15 @@
    180007dfc:	int3
    180007dfd:	int3
    180007dfe:	int3
    180007dff:	int3
    180007e00:	sub    $0x38,%rsp
    180007e04:	mov    %rdx,0x28(%rsp)
    180007e09:	lea    0x20(%rsp),%r9
-   180007e0e:	lea    0x15c5b(%rip),%rdx        # 0x18001da70
+   180007e0e:	lea    0x1635b(%rip),%rdx        # 0x18001e170
    180007e15:	movq   $0x0,0x20(%rsp)
    180007e1e:	mov    $0x2,%r8d
    180007e24:	call   *0x133fe(%rip)        # 0x18001b228
    180007e2a:	add    $0x38,%rsp
    180007e2e:	ret
    180007e2f:	int3
    180007e30:	rex push %rbx
@@ -15803,15 +15803,15 @@
    180007e5c:	int3
    180007e5d:	int3
    180007e5e:	int3
    180007e5f:	int3
    180007e60:	sub    $0x38,%rsp
    180007e64:	mov    %rdx,0x28(%rsp)
    180007e69:	lea    0x20(%rsp),%r9
-   180007e6e:	lea    0x15bfb(%rip),%rdx        # 0x18001da70
+   180007e6e:	lea    0x162fb(%rip),%rdx        # 0x18001e170
    180007e75:	movq   $0x0,0x20(%rsp)
    180007e7e:	xor    %r8d,%r8d
    180007e81:	call   *0x133a1(%rip)        # 0x18001b228
    180007e87:	add    $0x38,%rsp
    180007e8b:	ret
    180007e8c:	int3
    180007e8d:	int3
@@ -15831,15 +15831,15 @@
    180007eb9:	mov    %rbx,%rdx
    180007ebc:	lea    0x148(%rsi),%rcx
    180007ec3:	call   *0x134f7(%rip)        # 0x18001b3c0
    180007ec9:	lea    0x20(%rsp),%r9
    180007ece:	movq   $0x0,0x20(%rsp)
    180007ed7:	mov    $0x3,%r8d
    180007edd:	mov    %rbx,0x28(%rsp)
-   180007ee2:	lea    0x15b87(%rip),%rdx        # 0x18001da70
+   180007ee2:	lea    0x16287(%rip),%rdx        # 0x18001e170
    180007ee9:	mov    %rdi,%rcx
    180007eec:	call   *0x13336(%rip)        # 0x18001b228
    180007ef2:	mov    0x40(%rsp),%rbx
    180007ef7:	mov    0x48(%rsp),%rsi
    180007efc:	add    $0x30,%rsp
    180007f00:	pop    %rdi
    180007f01:	ret
@@ -15871,15 +15871,15 @@
    180007f39:	mov    %rbx,%rdx
    180007f3c:	lea    0x1e0(%rsi),%rcx
    180007f43:	call   *0x13477(%rip)        # 0x18001b3c0
    180007f49:	lea    0x20(%rsp),%r9
    180007f4e:	movq   $0x0,0x20(%rsp)
    180007f57:	mov    $0x6,%r8d
    180007f5d:	mov    %rbx,0x28(%rsp)
-   180007f62:	lea    0x15b07(%rip),%rdx        # 0x18001da70
+   180007f62:	lea    0x16207(%rip),%rdx        # 0x18001e170
    180007f69:	mov    %rdi,%rcx
    180007f6c:	call   *0x132b6(%rip)        # 0x18001b228
    180007f72:	mov    0x40(%rsp),%rbx
    180007f77:	mov    0x48(%rsp),%rsi
    180007f7c:	add    $0x30,%rsp
    180007f80:	pop    %rdi
    180007f81:	ret
@@ -15911,15 +15911,15 @@
    180007fb9:	mov    %rbx,%rdx
    180007fbc:	lea    0x1a8(%rsi),%rcx
    180007fc3:	call   *0x133f7(%rip)        # 0x18001b3c0
    180007fc9:	lea    0x20(%rsp),%r9
    180007fce:	movq   $0x0,0x20(%rsp)
    180007fd7:	mov    $0x2,%r8d
    180007fdd:	mov    %rbx,0x28(%rsp)
-   180007fe2:	lea    0x15a87(%rip),%rdx        # 0x18001da70
+   180007fe2:	lea    0x16187(%rip),%rdx        # 0x18001e170
    180007fe9:	mov    %rdi,%rcx
    180007fec:	call   *0x13236(%rip)        # 0x18001b228
    180007ff2:	mov    0x40(%rsp),%rbx
    180007ff7:	mov    0x48(%rsp),%rsi
    180007ffc:	add    $0x30,%rsp
    180008000:	pop    %rdi
    180008001:	ret
@@ -15951,15 +15951,15 @@
    180008039:	mov    %rbx,%rdx
    18000803c:	lea    0x160(%rsi),%rcx
    180008043:	call   *0x13377(%rip)        # 0x18001b3c0
    180008049:	lea    0x20(%rsp),%r9
    18000804e:	movq   $0x0,0x20(%rsp)
    180008057:	xor    %r8d,%r8d
    18000805a:	mov    %rbx,0x28(%rsp)
-   18000805f:	lea    0x15a0a(%rip),%rdx        # 0x18001da70
+   18000805f:	lea    0x1610a(%rip),%rdx        # 0x18001e170
    180008066:	mov    %rdi,%rcx
    180008069:	call   *0x131b9(%rip)        # 0x18001b228
    18000806f:	mov    0x40(%rsp),%rbx
    180008074:	mov    0x48(%rsp),%rsi
    180008079:	add    $0x30,%rsp
    18000807d:	pop    %rdi
    18000807e:	ret
@@ -15987,15 +15987,15 @@
    1800080d0:	lea    0x1f8(%rbx),%rcx
    1800080d7:	call   *0x1382b(%rip)        # 0x18001b908
    1800080dd:	movb   $0x1,0x200(%rbx)
    1800080e4:	lea    0x20(%rsp),%r9
    1800080e9:	movq   $0x0,0x20(%rsp)
    1800080f2:	mov    $0x7,%r8d
    1800080f8:	mov    %rdi,0x28(%rsp)
-   1800080fd:	lea    0x1596c(%rip),%rdx        # 0x18001da70
+   1800080fd:	lea    0x1606c(%rip),%rdx        # 0x18001e170
    180008104:	mov    %rsi,%rcx
    180008107:	call   *0x1311b(%rip)        # 0x18001b228
    18000810d:	mov    0x40(%rsp),%rbx
    180008112:	mov    0x48(%rsp),%rsi
    180008117:	add    $0x30,%rsp
    18000811b:	pop    %rdi
    18000811c:	ret
@@ -16017,15 +16017,15 @@
    18000814c:	mov    %rbx,%rdx
    18000814f:	lea    0x178(%rsi),%rcx
    180008156:	call   *0x13264(%rip)        # 0x18001b3c0
    18000815c:	lea    0x20(%rsp),%r9
    180008161:	movq   $0x0,0x20(%rsp)
    18000816a:	mov    $0x4,%r8d
    180008170:	mov    %rbx,0x28(%rsp)
-   180008175:	lea    0x158f4(%rip),%rdx        # 0x18001da70
+   180008175:	lea    0x15ff4(%rip),%rdx        # 0x18001e170
    18000817c:	mov    %rdi,%rcx
    18000817f:	call   *0x130a3(%rip)        # 0x18001b228
    180008185:	mov    0x40(%rsp),%rbx
    18000818a:	mov    0x48(%rsp),%rsi
    18000818f:	add    $0x30,%rsp
    180008193:	pop    %rdi
    180008194:	ret
@@ -16054,15 +16054,15 @@
    1800081c9:	mov    %rbx,%rdx
    1800081cc:	lea    0x190(%rsi),%rcx
    1800081d3:	call   *0x131e7(%rip)        # 0x18001b3c0
    1800081d9:	lea    0x20(%rsp),%r9
    1800081de:	movq   $0x0,0x20(%rsp)
    1800081e7:	mov    $0x1,%r8d
    1800081ed:	mov    %rbx,0x28(%rsp)
-   1800081f2:	lea    0x15877(%rip),%rdx        # 0x18001da70
+   1800081f2:	lea    0x15f77(%rip),%rdx        # 0x18001e170
    1800081f9:	mov    %rdi,%rcx
    1800081fc:	call   *0x13026(%rip)        # 0x18001b228
    180008202:	mov    0x40(%rsp),%rbx
    180008207:	mov    0x48(%rsp),%rsi
    18000820c:	add    $0x30,%rsp
    180008210:	pop    %rdi
    180008211:	ret
@@ -16114,15 +16114,15 @@
    18000827c:	int3
    18000827d:	int3
    18000827e:	int3
    18000827f:	int3
    180008280:	sub    $0x38,%rsp
    180008284:	mov    %rdx,0x28(%rsp)
    180008289:	lea    0x20(%rsp),%r9
-   18000828e:	lea    0x157db(%rip),%rdx        # 0x18001da70
+   18000828e:	lea    0x15edb(%rip),%rdx        # 0x18001e170
    180008295:	movq   $0x0,0x20(%rsp)
    18000829e:	mov    $0x7,%r8d
    1800082a4:	call   *0x12f7e(%rip)        # 0x18001b228
    1800082aa:	add    $0x38,%rsp
    1800082ae:	ret
    1800082af:	int3
    1800082b0:	rex push %rbx
@@ -16145,29 +16145,29 @@
    1800082dc:	int3
    1800082dd:	int3
    1800082de:	int3
    1800082df:	int3
    1800082e0:	sub    $0x38,%rsp
    1800082e4:	mov    %rdx,0x28(%rsp)
    1800082e9:	lea    0x20(%rsp),%r9
-   1800082ee:	lea    0x1577b(%rip),%rdx        # 0x18001da70
+   1800082ee:	lea    0x15e7b(%rip),%rdx        # 0x18001e170
    1800082f5:	movq   $0x0,0x20(%rsp)
    1800082fe:	mov    $0x4,%r8d
    180008304:	call   *0x12f1e(%rip)        # 0x18001b228
    18000830a:	add    $0x38,%rsp
    18000830e:	ret
    18000830f:	int3
    180008310:	rex push %rbx
    180008312:	sub    $0x30,%rsp
    180008316:	mov    %r9d,0x20(%rsp)
    18000831b:	mov    %rcx,%rbx
    18000831e:	mov    %r8,%r9
    180008321:	mov    %rdx,%r8
    180008324:	mov    %rcx,%rdx
-   180008327:	lea    0x15742(%rip),%rcx        # 0x18001da70
+   180008327:	lea    0x15e42(%rip),%rcx        # 0x18001e170
    18000832e:	call   *0x12eec(%rip)        # 0x18001b220
    180008334:	mov    %rbx,%rax
    180008337:	add    $0x30,%rsp
    18000833b:	pop    %rbx
    18000833c:	ret
    18000833d:	int3
    18000833e:	int3
@@ -16192,26 +16192,26 @@
    18000836c:	int3
    18000836d:	int3
    18000836e:	int3
    18000836f:	int3
    180008370:	sub    $0x38,%rsp
    180008374:	mov    %rdx,0x28(%rsp)
    180008379:	lea    0x20(%rsp),%r9
-   18000837e:	lea    0x156eb(%rip),%rdx        # 0x18001da70
+   18000837e:	lea    0x15deb(%rip),%rdx        # 0x18001e170
    180008385:	movq   $0x0,0x20(%rsp)
    18000838e:	mov    $0x1,%r8d
    180008394:	call   *0x12e8e(%rip)        # 0x18001b228
    18000839a:	add    $0x38,%rsp
    18000839e:	ret
    18000839f:	int3
    1800083a0:	rex push %rbx
    1800083a2:	sub    $0x20,%rsp
    1800083a6:	mov    %rcx,%rbx
    1800083a9:	call   *0x13051(%rip)        # 0x18001b400
-   1800083af:	lea    0x16282(%rip),%rax        # 0x18001e638
+   1800083af:	lea    0x16292(%rip),%rax        # 0x18001e648
    1800083b6:	mov    %rax,(%rbx)
    1800083b9:	mov    %rbx,%rax
    1800083bc:	add    $0x20,%rsp
    1800083c0:	pop    %rbx
    1800083c1:	ret
    1800083c2:	int3
    1800083c3:	int3
@@ -16227,15 +16227,15 @@
    1800083cd:	int3
    1800083ce:	int3
    1800083cf:	int3
    1800083d0:	rex push %rbx
    1800083d2:	sub    $0x20,%rsp
    1800083d6:	mov    %rcx,%rbx
    1800083d9:	call   *0x131a9(%rip)        # 0x18001b588
-   1800083df:	lea    0x16252(%rip),%rax        # 0x18001e638
+   1800083df:	lea    0x16262(%rip),%rax        # 0x18001e648
    1800083e6:	mov    %rax,(%rbx)
    1800083e9:	mov    %rbx,%rax
    1800083ec:	add    $0x20,%rsp
    1800083f0:	pop    %rbx
    1800083f1:	ret
    1800083f2:	int3
    1800083f3:	int3
@@ -16247,15 +16247,15 @@
    1800083f9:	int3
    1800083fa:	int3
    1800083fb:	int3
    1800083fc:	int3
    1800083fd:	int3
    1800083fe:	int3
    1800083ff:	int3
-   180008400:	lea    0x16231(%rip),%rax        # 0x18001e638
+   180008400:	lea    0x16241(%rip),%rax        # 0x18001e648
    180008407:	mov    %rax,(%rcx)
    18000840a:	rex.W jmp *0x12fdf(%rip)        # 0x18001b3f0
    180008411:	int3
    180008412:	int3
    180008413:	int3
    180008414:	int3
    180008415:	int3
@@ -16282,15 +16282,15 @@
    18000843e:	mov    -0x8(%rcx),%rdi
    180008442:	mov    %rdi,%rbx
    180008445:	mov    %r14,0x50(%rsp)
    18000844a:	shl    $0x4,%rbx
    18000844e:	add    %rcx,%rbx
    180008451:	test   %rdi,%rdi
    180008454:	je     0x180008476
-   180008456:	lea    0x161db(%rip),%rbp        # 0x18001e638
+   180008456:	lea    0x161eb(%rip),%rbp        # 0x18001e648
    18000845d:	nopl   (%rax)
    180008460:	sub    $0x10,%rbx
    180008464:	mov    %rbx,%rcx
    180008467:	mov    %rbp,(%rbx)
    18000846a:	call   *0x12f80(%rip)        # 0x18001b3f0
    180008470:	sub    $0x1,%rdi
    180008474:	jne    0x180008460
@@ -16306,15 +16306,15 @@
    18000849b:	mov    0x50(%rsp),%r14
    1800084a0:	lea    -0x8(%rsi),%rax
    1800084a4:	add    $0x20,%rsp
    1800084a8:	pop    %r15
    1800084aa:	pop    %rsi
    1800084ab:	pop    %rbp
    1800084ac:	ret
-   1800084ad:	lea    0x16184(%rip),%rbp        # 0x18001e638
+   1800084ad:	lea    0x16194(%rip),%rbp        # 0x18001e648
    1800084b4:	mov    %rbp,(%rcx)
    1800084b7:	call   *0x12f33(%rip)        # 0x18001b3f0
    1800084bd:	test   $0x1,%r15b
    1800084c1:	je     0x1800084d0
    1800084c3:	mov    $0x10,%edx
    1800084c8:	mov    %rsi,%rcx
    1800084cb:	call   0x180019368
@@ -16344,15 +16344,15 @@
    180008516:	lea    0x24cd3(%rip),%rcx        # 0x18002d1f0
    18000851d:	call   0x180019588
    180008522:	cmpl   $0xffffffff,0x24cc7(%rip)        # 0x18002d1f0
    180008529:	jne    0x180008509
    18000852b:	lea    0x24ca6(%rip),%rbx        # 0x18002d1d8
    180008532:	xor    %r8d,%r8d
    180008535:	mov    %rbx,%rcx
-   180008538:	lea    0x16161(%rip),%rdx        # 0x18001e6a0
+   180008538:	lea    0x16171(%rip),%rdx        # 0x18001e6b0
    18000853f:	call   *0x12ef3(%rip)        # 0x18001b438
    180008545:	lea    0x12204(%rip),%rcx        # 0x18001a750
    18000854c:	call   0x180019a00
    180008551:	lea    0x24c98(%rip),%rcx        # 0x18002d1f0
    180008558:	call   0x180019528
    18000855d:	mov    %rbx,%rax
    180008560:	add    $0x20,%rsp
@@ -16666,15 +16666,15 @@
    18000896d:	mov    %edi,0x24991(%rip)        # 0x18002d304
    180008973:	call   0x180019528
    180008978:	jmp    0x1800088d1
    18000897d:	cmp    %rax,%r8
    180008980:	jne    0x180008a35
    180008986:	test   %r8,%r8
    180008989:	je     0x1800089a3
-   18000898b:	lea    0x15f56(%rip),%rdx        # 0x18001e8e8
+   18000898b:	lea    0x15f66(%rip),%rdx        # 0x18001e8f8
    180008992:	lea    -0x21(%rbp),%rcx
    180008996:	call   0x18001a42c
    18000899b:	test   %eax,%eax
    18000899d:	jne    0x180008a35
    1800089a3:	mov    $0xffffffffffffffff,%r8
    1800089aa:	lea    -0x21(%rbp),%rdx
    1800089ae:	lea    -0x51(%rbp),%rcx
@@ -16687,26 +16687,26 @@
    1800089d2:	call   0x180019588
    1800089d7:	cmpl   $0xffffffff,0x2492a(%rip)        # 0x18002d308
    1800089de:	jne    0x1800088d1
    1800089e4:	mov    0x2480a(%rip),%ebx        # 0x18002d1f4
    1800089ea:	nop
    1800089eb:	test   %ebx,%ebx
    1800089ed:	jne    0x180008960
-   1800089f3:	movdqa 0x16175(%rip),%xmm0        # 0x18001eb70
+   1800089f3:	movdqa 0x16185(%rip),%xmm0        # 0x18001eb80
    1800089fb:	lea    0x1c(%rbx),%edx
-   1800089fe:	lea    0x15ee3(%rip),%rcx        # 0x18001e8e8
+   1800089fe:	lea    0x15ef3(%rip),%rcx        # 0x18001e8f8
    180008a05:	movl   $0x6f777465,-0x11(%rbp)
    180008a0c:	movdqu %xmm0,-0x21(%rbp)
    180008a11:	movl   $0x72456b72,-0xd(%rbp)
    180008a18:	movl   $0x726f72,-0x9(%rbp)
    180008a1f:	call   *0x12ac3(%rip)        # 0x18001b4e8
    180008a25:	lea    -0x21(%rbp),%rcx
    180008a29:	mov    $0xffffffffffffffff,%r8
    180008a30:	jmp    0x180008955
-   180008a35:	lea    0x15eac(%rip),%rdx        # 0x18001e8e8
+   180008a35:	lea    0x15ebc(%rip),%rdx        # 0x18001e8f8
    180008a3c:	lea    -0x39(%rbp),%rcx
    180008a40:	call   *0x12aca(%rip)        # 0x18001b510
    180008a46:	lea    -0x39(%rbp),%rcx
    180008a4a:	call   *0x12e18(%rip)        # 0x18001b868
    180008a50:	lea    -0x39(%rbp),%rcx
    180008a54:	mov    %eax,%ebx
    180008a56:	call   *0x12774(%rip)        # 0x18001b1d0
@@ -17038,20 +17038,20 @@
    180008ed0:	lea    0x90(%rsp),%rcx
    180008ed8:	call   *0x12362(%rip)        # 0x18001b240
    180008ede:	lea    0xd0(%rsp),%rcx
    180008ee6:	call   *0x12394(%rip)        # 0x18001b280
    180008eec:	lea    0x78(%rsp),%r9
    180008ef1:	mov    %rsi,0x20(%rsp)
    180008ef6:	mov    %rax,%r8
-   180008ef9:	lea    0x15a20(%rip),%rdx        # 0x18001e920
+   180008ef9:	lea    0x15a30(%rip),%rdx        # 0x18001e930
    180008f00:	mov    %r14,%rcx
    180008f03:	call   0x180004510
    180008f08:	lea    0xd0(%rsp),%rcx
    180008f10:	call   *0x12382(%rip)        # 0x18001b298
-   180008f16:	lea    0x159f3(%rip),%rax        # 0x18001e910
+   180008f16:	lea    0x15a03(%rip),%rax        # 0x18001e920
    180008f1d:	lea    0x148(%r14),%rcx
    180008f24:	mov    %rax,(%r14)
    180008f27:	lea    0x90(%rsp),%rdx
    180008f2f:	call   *0x1230b(%rip)        # 0x18001b240
    180008f35:	lea    0x160(%r14),%rcx
    180008f3c:	call   *0x122f6(%rip)        # 0x18001b238
    180008f42:	lea    0x178(%r14),%rcx
@@ -17062,52 +17062,52 @@
    180008f63:	call   *0x12317(%rip)        # 0x18001b280
    180008f69:	xor    %eax,%eax
    180008f6b:	movq   $0x3,0x40(%rsp)
    180008f74:	mov    %eax,0x1a0(%r14)
    180008f7b:	lea    0x1a8(%r14),%rcx
    180008f82:	mov    %rax,0x30(%rsp)
    180008f87:	lea    0x30(%rsp),%rdx
-   180008f8c:	lea    0x159a5(%rip),%rax        # 0x18001e938
+   180008f8c:	lea    0x159b5(%rip),%rax        # 0x18001e948
    180008f93:	mov    %rax,0x38(%rsp)
    180008f98:	call   *0x12432(%rip)        # 0x18001b3d0
    180008f9e:	mov    0x30(%rsp),%rcx
    180008fa3:	test   %rcx,%rcx
    180008fa6:	je     0x180008fc8
    180008fa8:	mov    $0xffffffff,%eax
    180008fad:	lock xadd %eax,(%rcx)
    180008fb1:	cmp    $0x1,%eax
    180008fb4:	jne    0x180008fc8
    180008fb6:	mov    0x30(%rsp),%rcx
    180008fbb:	lea    0x1(%rax),%edx
    180008fbe:	lea    0x7(%rax),%r8d
    180008fc2:	call   *0x123e0(%rip)        # 0x18001b3a8
-   180008fc8:	lea    0x15919(%rip),%rdx        # 0x18001e8e8
+   180008fc8:	lea    0x15929(%rip),%rdx        # 0x18001e8f8
    180008fcf:	movb   $0x0,0x1c0(%r14)
    180008fd7:	lea    0x48(%rsp),%rcx
    180008fdc:	call   *0x1252e(%rip)        # 0x18001b510
    180008fe2:	lea    0x48(%rsp),%rcx
    180008fe7:	call   *0x1287b(%rip)        # 0x18001b868
    180008fed:	lea    0x48(%rsp),%rcx
    180008ff2:	call   *0x121d8(%rip)        # 0x18001b1d0
-   180008ff8:	lea    0x15941(%rip),%rdx        # 0x18001e940
+   180008ff8:	lea    0x15951(%rip),%rdx        # 0x18001e950
    180008fff:	lea    0x60(%rsp),%rcx
    180009004:	call   *0x12506(%rip)        # 0x18001b510
    18000900a:	lea    0x60(%rsp),%rcx
    18000900f:	call   0x180002e90
    180009014:	lea    0x60(%rsp),%rcx
    180009019:	call   *0x121b1(%rip)        # 0x18001b1d0
    18000901f:	mov    0xf0(%rsp),%r8
    180009027:	mov    %r14,%rdx
    18000902a:	mov    %r15,%rcx
    18000902d:	call   0x1800044d0
    180009032:	lea    0x90(%rsp),%rcx
    18000903a:	call   *0x12208(%rip)        # 0x18001b248
    180009040:	lea    0x78(%rsp),%rcx
    180009045:	call   *0x121fd(%rip)        # 0x18001b248
-   18000904b:	lea    0x157fe(%rip),%rax        # 0x18001e850
+   18000904b:	lea    0x1580e(%rip),%rax        # 0x18001e860
    180009052:	lea    0xb0(%rsp),%r11
    18000905a:	mov    %rax,(%r15)
    18000905d:	mov    0x28(%r11),%rbx
    180009061:	mov    %r15,%rax
    180009064:	mov    0x30(%r11),%rsi
    180009068:	mov    %r11,%rsp
    18000906b:	pop    %r15
@@ -17149,15 +17149,15 @@
    1800090c5:	mov    %r14,%rcx
    1800090c8:	call   0x180008e90
    1800090cd:	lea    0x30(%rsp),%rcx
    1800090d2:	call   *0x12170(%rip)        # 0x18001b248
    1800090d8:	lea    0x48(%rsp),%rcx
    1800090dd:	call   *0x12165(%rip)        # 0x18001b248
    1800090e3:	mov    0x70(%rsp),%rbx
-   1800090e8:	lea    0x15761(%rip),%rax        # 0x18001e850
+   1800090e8:	lea    0x15771(%rip),%rax        # 0x18001e860
    1800090ef:	mov    0x78(%rsp),%rsi
    1800090f4:	mov    0x80(%rsp),%rdi
    1800090fc:	mov    %rax,(%r14)
    1800090ff:	mov    %r14,%rax
    180009102:	add    $0x60,%rsp
    180009106:	pop    %r14
    180009108:	ret
@@ -17170,15 +17170,15 @@
    18000910f:	int3
    180009110:	rex push %rbx
    180009112:	sub    $0x20,%rsp
    180009116:	mov    %rdx,%r8
    180009119:	mov    %rcx,%rbx
    18000911c:	xor    %edx,%edx
    18000911e:	call   0x180009080
-   180009123:	lea    0x15726(%rip),%rax        # 0x18001e850
+   180009123:	lea    0x15736(%rip),%rax        # 0x18001e860
    18000912a:	mov    %rax,(%rbx)
    18000912d:	mov    %rbx,%rax
    180009130:	add    $0x20,%rsp
    180009134:	pop    %rbx
    180009135:	ret
    180009136:	int3
    180009137:	int3
@@ -18501,15 +18501,15 @@
    18000a40e:	lea    -0x58(%rbp),%r9
    18000a412:	mov    %rbx,%rcx
    18000a415:	lea    0x22e6c(%rip),%r8        # 0x18002d288
    18000a41c:	lea    0x28(%rsp),%rdx
    18000a421:	call   0x18000b770
    18000a426:	lea    -0x58(%rbp),%rcx
    18000a42a:	call   *0x10f40(%rip)        # 0x18001b370
-   18000a430:	lea    0x14501(%rip),%rax        # 0x18001e938
+   18000a430:	lea    0x14511(%rip),%rax        # 0x18001e948
    18000a437:	movq   $0x0,0x38(%rsp)
    18000a440:	lea    0x38(%rsp),%rdx
    18000a445:	mov    %rax,0x40(%rsp)
    18000a44a:	lea    0x78(%rsp),%rcx
    18000a44f:	movq   $0x3,0x48(%rsp)
    18000a458:	call   *0x10f72(%rip)        # 0x18001b3d0
    18000a45e:	mov    %rax,%rdx
@@ -18647,15 +18647,15 @@
    18000a65e:	lea    0x60(%rsp),%rcx
    18000a663:	xor    %r9d,%r9d
    18000a666:	mov    %rax,0x20(%rsp)
    18000a66b:	xor    %r8d,%r8d
    18000a66e:	xor    %edx,%edx
    18000a670:	call   *0x10e62(%rip)        # 0x18001b4d8
    18000a676:	mov    %rax,%rcx
-   18000a679:	lea    0x142e0(%rip),%rdx        # 0x18001e960
+   18000a679:	lea    0x142f0(%rip),%rdx        # 0x18001e970
    18000a680:	call   *0x10e5a(%rip)        # 0x18001b4e0
    18000a686:	xor    %eax,%eax
    18000a688:	jmp    0x18000a777
    18000a68d:	mov    %rbp,%rdx
    18000a690:	lea    0xa0(%rsp),%rcx
    18000a698:	call   *0x111f2(%rip)        # 0x18001b890
    18000a69e:	mov    $0x5,%r9d
@@ -18871,15 +18871,15 @@
    18000a9ca:	push   %r13
    18000a9cc:	lea    -0x40(%rsp),%rbp
    18000a9d1:	sub    $0x140,%rsp
    18000a9d8:	mov    %rdx,%rbx
    18000a9db:	movq   $0x0,0x38(%rsp)
    18000a9e4:	mov    %rcx,%r13
    18000a9e7:	movq   $0x6,0x48(%rsp)
-   18000a9f0:	lea    0x140e1(%rip),%rax        # 0x18001ead8
+   18000a9f0:	lea    0x140f1(%rip),%rax        # 0x18001eae8
    18000a9f7:	mov    $0x1,%r12b
    18000a9fa:	lea    0x38(%rsp),%rdx
    18000a9ff:	mov    %rax,0x40(%rsp)
    18000aa04:	lea    0x20(%rsp),%rcx
    18000aa09:	call   *0x109c1(%rip)        # 0x18001b3d0
    18000aa0f:	mov    0x38(%rsp),%r8
    18000aa14:	test   %r8,%r8
@@ -18907,18 +18907,18 @@
    18000aa73:	mov    %rbx,0x88(%rbp)
    18000aa7a:	call   0x18000a790
    18000aa7f:	mov    0x80(%rbp),%rdi
    18000aa86:	mov    0x8(%rdi),%rdi
    18000aa8a:	cmp    %rdi,%rbx
    18000aa8d:	je     0x18000ad22
    18000aa93:	mov    %rsi,0x138(%rsp)
-   18000aa9b:	lea    0x14046(%rip),%r13        # 0x18001eae8
+   18000aa9b:	lea    0x14056(%rip),%r13        # 0x18001eaf8
    18000aaa2:	mov    %r14,0x130(%rsp)
    18000aaaa:	mov    %r15,0x128(%rsp)
-   18000aab2:	lea    0x14033(%rip),%r15        # 0x18001eaec
+   18000aab2:	lea    0x14043(%rip),%r15        # 0x18001eafc
    18000aab9:	movaps %xmm6,0x110(%rsp)
    18000aac1:	test   %r12b,%r12b
    18000aac4:	je     0x18000aacb
    18000aac6:	xor    %r12b,%r12b
    18000aac9:	jmp    0x18000aae9
    18000aacb:	lea    0x70(%rsp),%rdx
    18000aad0:	movq   $0x1,0x70(%rsp)
@@ -19045,15 +19045,15 @@
    18000acc7:	lea    -0x20(%rbp),%rcx
    18000accb:	call   *0x104ff(%rip)        # 0x18001b1d0
    18000acd1:	lea    -0x8(%rbp),%rcx
    18000acd5:	call   *0x104f5(%rip)        # 0x18001b1d0
    18000acdb:	lea    0x88(%rbp),%rcx
    18000ace2:	call   0x180003540
    18000ace7:	mov    0x88(%rbp),%rbx
-   18000acee:	lea    0x13df7(%rip),%r15        # 0x18001eaec
+   18000acee:	lea    0x13e07(%rip),%r15        # 0x18001eafc
    18000acf5:	cmp    %rdi,%rbx
    18000acf8:	jne    0x18000aac1
    18000acfe:	mov    0x70(%rbp),%r13
    18000ad02:	movaps 0x110(%rsp),%xmm6
    18000ad0a:	mov    0x128(%rsp),%r15
    18000ad12:	mov    0x130(%rsp),%r14
    18000ad1a:	mov    0x138(%rsp),%rsi
@@ -19101,15 +19101,15 @@
    18000adae:	je     0x18000adde
    18000adb0:	xor    %r9d,%r9d
    18000adb3:	lea    0x30(%rsp),%rcx
    18000adb8:	xor    %r8d,%r8d
    18000adbb:	xor    %edx,%edx
    18000adbd:	call   *0x107cd(%rip)        # 0x18001b590
    18000adc3:	mov    %rax,%rcx
-   18000adc6:	lea    0x13c93(%rip),%rdx        # 0x18001ea60
+   18000adc6:	lea    0x13ca3(%rip),%rdx        # 0x18001ea70
    18000adcd:	call   *0x107c5(%rip)        # 0x18001b598
    18000add3:	mov    %rdi,%rcx
    18000add6:	call   *0x103e4(%rip)        # 0x18001b1c0
    18000addc:	jmp    0x18000ae16
    18000adde:	mov    %rdi,%rdx
    18000ade1:	lea    0x60(%rsp),%rcx
    18000ade6:	call   0x18000f470
@@ -19153,15 +19153,15 @@
    18000ae6e:	lea    0x60(%rsp),%rcx
    18000ae73:	xor    %r9d,%r9d
    18000ae76:	mov    %rax,0x20(%rsp)
    18000ae7b:	xor    %r8d,%r8d
    18000ae7e:	xor    %edx,%edx
    18000ae80:	call   *0x10652(%rip)        # 0x18001b4d8
    18000ae86:	mov    %rax,%rcx
-   18000ae89:	lea    0x13ad0(%rip),%rdx        # 0x18001e960
+   18000ae89:	lea    0x13ae0(%rip),%rdx        # 0x18001e970
    18000ae90:	call   *0x1064a(%rip)        # 0x18001b4e0
    18000ae96:	xor    %eax,%eax
    18000ae98:	jmp    0x18000af87
    18000ae9d:	mov    %rbp,%rdx
    18000aea0:	lea    0xa0(%rsp),%rcx
    18000aea8:	call   *0x109e2(%rip)        # 0x18001b890
    18000aeae:	mov    $0x2,%r9d
@@ -19238,15 +19238,15 @@
    18000afe8:	lea    0x17(%rbp),%rcx
    18000afec:	xor    %r9d,%r9d
    18000afef:	mov    %rax,0x20(%rsp)
    18000aff4:	xor    %r8d,%r8d
    18000aff7:	xor    %edx,%edx
    18000aff9:	call   *0x104d9(%rip)        # 0x18001b4d8
    18000afff:	mov    %rax,%rcx
-   18000b002:	lea    0x13b07(%rip),%rdx        # 0x18001eb10
+   18000b002:	lea    0x13b17(%rip),%rdx        # 0x18001eb20
    18000b009:	call   *0x104d1(%rip)        # 0x18001b4e0
    18000b00f:	add    $0x88,%rsp
    18000b016:	pop    %rbx
    18000b017:	pop    %rbp
    18000b018:	ret
    18000b019:	mov    0x67(%rbp),%rcx
    18000b01d:	add    $0x198,%rcx
@@ -19262,15 +19262,15 @@
    18000b04b:	lea    0x17(%rbp),%rcx
    18000b04f:	xor    %r9d,%r9d
    18000b052:	mov    %rax,0x20(%rsp)
    18000b057:	xor    %r8d,%r8d
    18000b05a:	xor    %edx,%edx
    18000b05c:	call   *0x10476(%rip)        # 0x18001b4d8
    18000b062:	mov    %rax,%rcx
-   18000b065:	lea    0x13ac4(%rip),%rdx        # 0x18001eb30
+   18000b065:	lea    0x13ad4(%rip),%rdx        # 0x18001eb40
    18000b06c:	call   *0x1046e(%rip)        # 0x18001b4e0
    18000b072:	add    $0x88,%rsp
    18000b079:	pop    %rbx
    18000b07a:	pop    %rbp
    18000b07b:	ret
    18000b07c:	mov    0x67(%rbp),%rax
    18000b080:	cmpq   $0x0,0xb8(%rax)
@@ -19288,15 +19288,15 @@
    18000b0b4:	lea    0x17(%rbp),%rcx
    18000b0b8:	xor    %r9d,%r9d
    18000b0bb:	mov    %rax,0x20(%rsp)
    18000b0c0:	xor    %r8d,%r8d
    18000b0c3:	xor    %edx,%edx
    18000b0c5:	call   *0x1040d(%rip)        # 0x18001b4d8
    18000b0cb:	mov    %rax,%rcx
-   18000b0ce:	lea    0x13a7b(%rip),%rdx        # 0x18001eb50
+   18000b0ce:	lea    0x13a8b(%rip),%rdx        # 0x18001eb60
    18000b0d5:	call   *0x10405(%rip)        # 0x18001b4e0
    18000b0db:	add    $0x88,%rsp
    18000b0e2:	pop    %rbx
    18000b0e3:	pop    %rbp
    18000b0e4:	ret
    18000b0e5:	mov    %rsi,0x80(%rsp)
    18000b0ed:	lea    0x6f(%rbp),%rcx
@@ -19330,15 +19330,15 @@
    18000b173:	lea    0x6f(%rbp),%rcx
    18000b177:	call   *0x10453(%rip)        # 0x18001b5d0
    18000b17d:	lea    0x77(%rbp),%rcx
    18000b181:	call   *0x10391(%rip)        # 0x18001b518
    18000b187:	mov    %rbx,%rcx
    18000b18a:	call   0x1800055a0
    18000b18f:	mov    %rax,%rdx
-   18000b192:	lea    0x14007(%rip),%rcx        # 0x18001f1a0
+   18000b192:	lea    0x14017(%rip),%rcx        # 0x18001f1b0
    18000b199:	call   *0x10421(%rip)        # 0x18001b5c0
    18000b19f:	mov    %rax,%rdi
    18000b1a2:	test   %rax,%rax
    18000b1a5:	je     0x18000b220
    18000b1a7:	lea    0x67(%rbp),%rax
    18000b1ab:	mov    %rbx,0x1f(%rbp)
    18000b1af:	mov    %rax,0x17(%rbp)
@@ -19435,15 +19435,15 @@
    18000b333:	lea    0x30(%rsp),%rcx
    18000b338:	xor    %r9d,%r9d
    18000b33b:	mov    %rax,0x20(%rsp)
    18000b340:	xor    %r8d,%r8d
    18000b343:	xor    %edx,%edx
    18000b345:	call   *0x1018d(%rip)        # 0x18001b4d8
    18000b34b:	mov    %rax,%rcx
-   18000b34e:	lea    0x1360b(%rip),%rdx        # 0x18001e960
+   18000b34e:	lea    0x1361b(%rip),%rdx        # 0x18001e970
    18000b355:	call   *0x10185(%rip)        # 0x18001b4e0
    18000b35b:	xor    %eax,%eax
    18000b35d:	jmp    0x18000b3aa
    18000b35f:	mov    %rbp,%rdx
    18000b362:	lea    0x60(%rsp),%rcx
    18000b367:	call   *0x10523(%rip)        # 0x18001b890
    18000b36d:	mov    $0x1,%r9d
@@ -19549,15 +19549,15 @@
    18000b50f:	call   *0xffc3(%rip)        # 0x18001b4d8
    18000b515:	lea    0x48(%rsp),%rdx
    18000b51a:	mov    %rax,%rbx
    18000b51d:	lea    0x21dc4(%rip),%rcx        # 0x18002d2e8
    18000b524:	call   *0x100fe(%rip)        # 0x18001b628
    18000b52a:	mov    %rax,%rcx
    18000b52d:	call   *0x1007d(%rip)        # 0x18001b5b0
-   18000b533:	lea    0x135b6(%rip),%rdx        # 0x18001eaf0
+   18000b533:	lea    0x135c6(%rip),%rdx        # 0x18001eb00
    18000b53a:	mov    %rbx,%rcx
    18000b53d:	mov    %rax,%r8
    18000b540:	call   *0xff9a(%rip)        # 0x18001b4e0
    18000b546:	lea    0x48(%rsp),%rcx
    18000b54b:	call   *0xfc7f(%rip)        # 0x18001b1d0
    18000b551:	lea    0x30(%rsp),%rcx
    18000b556:	call   *0xfcec(%rip)        # 0x18001b248
@@ -20030,15 +20030,15 @@
    18000bb1e:	lea    0x60(%rsp),%rcx
    18000bb23:	xor    %r9d,%r9d
    18000bb26:	mov    %rax,0x20(%rsp)
    18000bb2b:	xor    %r8d,%r8d
    18000bb2e:	xor    %edx,%edx
    18000bb30:	call   *0xf9a2(%rip)        # 0x18001b4d8
    18000bb36:	mov    %rax,%rcx
-   18000bb39:	lea    0x12e20(%rip),%rdx        # 0x18001e960
+   18000bb39:	lea    0x12e30(%rip),%rdx        # 0x18001e970
    18000bb40:	call   *0xf99a(%rip)        # 0x18001b4e0
    18000bb46:	xor    %eax,%eax
    18000bb48:	jmp    0x18000bc70
    18000bb4d:	mov    %rbp,%rdx
    18000bb50:	lea    0xc0(%rsp),%rcx
    18000bb58:	call   *0xfd32(%rip)        # 0x18001b890
    18000bb5e:	mov    $0x4,%r9d
@@ -20144,15 +20144,15 @@
    18000bcf4:	jmp    0x18000bcff
    18000bcf6:	mov    %r14,%rcx
    18000bcf9:	call   *0xf4e9(%rip)        # 0x18001b1e8
    18000bcff:	mov    %rsi,0x158(%rsp)
    18000bd07:	cmp    $0x4,%rbx
    18000bd0b:	jne    0x18000bd91
    18000bd11:	mov    %rbx,%r8
-   18000bd14:	lea    0x12d89(%rip),%rdx        # 0x18001eaa4
+   18000bd14:	lea    0x12d99(%rip),%rdx        # 0x18001eab4
    18000bd1b:	mov    %rax,%rcx
    18000bd1e:	call   0x18001a42c
    18000bd23:	test   %eax,%eax
    18000bd25:	jne    0x18000bd91
    18000bd27:	xor    %r8d,%r8d
    18000bd2a:	lea    0x20(%rbp),%rdx
    18000bd2e:	mov    %r12,%rcx
@@ -20172,15 +20172,15 @@
    18000bd64:	xor    %eax,%eax
    18000bd66:	jmp    0x18000bd71
    18000bd68:	mov    %rbx,%rcx
    18000bd6b:	call   *0xf477(%rip)        # 0x18001b1e8
    18000bd71:	cmp    $0x21,%rsi
    18000bd75:	jne    0x18000bd91
    18000bd77:	mov    %rsi,%r8
-   18000bd7a:	lea    0x12d2f(%rip),%rdx        # 0x18001eab0
+   18000bd7a:	lea    0x12d3f(%rip),%rdx        # 0x18001eac0
    18000bd81:	mov    %rax,%rcx
    18000bd84:	call   0x18001a42c
    18000bd89:	test   %eax,%eax
    18000bd8b:	jne    0x18000bd91
    18000bd8d:	mov    $0x1,%bl
    18000bd8f:	jmp    0x18000bd93
    18000bd91:	xor    %bl,%bl
@@ -20559,15 +20559,15 @@
    18000c34e:	lea    0x50(%rsp),%rcx
    18000c353:	xor    %r9d,%r9d
    18000c356:	mov    %rax,0x20(%rsp)
    18000c35b:	xor    %r8d,%r8d
    18000c35e:	xor    %edx,%edx
    18000c360:	call   *0xf172(%rip)        # 0x18001b4d8
    18000c366:	mov    %rax,%rcx
-   18000c369:	lea    0x125f0(%rip),%rdx        # 0x18001e960
+   18000c369:	lea    0x12600(%rip),%rdx        # 0x18001e970
    18000c370:	call   *0xf16a(%rip)        # 0x18001b4e0
    18000c376:	xor    %eax,%eax
    18000c378:	jmp    0x18000c497
    18000c37d:	mov    %rbp,%rdx
    18000c380:	lea    0xb0(%rsp),%rcx
    18000c388:	call   *0xf502(%rip)        # 0x18001b890
    18000c38e:	mov    $0x3,%r9d
@@ -20954,15 +20954,15 @@
    18000c988:	lea    0x130(%rbp),%rcx
    18000c98f:	xor    %r9d,%r9d
    18000c992:	mov    %rax,0x20(%rsp)
    18000c997:	xor    %r8d,%r8d
    18000c99a:	xor    %edx,%edx
    18000c99c:	call   *0xeb36(%rip)        # 0x18001b4d8
    18000c9a2:	mov    %rax,%rcx
-   18000c9a5:	lea    0x11fb4(%rip),%rdx        # 0x18001e960
+   18000c9a5:	lea    0x11fc4(%rip),%rdx        # 0x18001e970
    18000c9ac:	call   *0xeb2e(%rip)        # 0x18001b4e0
    18000c9b2:	xor    %eax,%eax
    18000c9b4:	jmp    0x18000d4e0
    18000c9b9:	mov    %r12,%rcx
    18000c9bc:	call   *0xec7e(%rip)        # 0x18001b640
    18000c9c2:	test   %al,%al
    18000c9c4:	je     0x18000ca10
@@ -20974,15 +20974,15 @@
    18000c9df:	lea    0x130(%rbp),%rcx
    18000c9e6:	xor    %r9d,%r9d
    18000c9e9:	mov    %rax,0x20(%rsp)
    18000c9ee:	xor    %r8d,%r8d
    18000c9f1:	xor    %edx,%edx
    18000c9f3:	call   *0xeadf(%rip)        # 0x18001b4d8
    18000c9f9:	mov    %rax,%rcx
-   18000c9fc:	lea    0x11f85(%rip),%rdx        # 0x18001e988
+   18000c9fc:	lea    0x11f95(%rip),%rdx        # 0x18001e998
    18000ca03:	call   *0xead7(%rip)        # 0x18001b4e0
    18000ca09:	xor    %eax,%eax
    18000ca0b:	jmp    0x18000d4e0
    18000ca10:	lea    -0x2(%r13),%eax
    18000ca14:	test   $0xfffffffd,%eax
    18000ca19:	je     0x18000ca61
    18000ca1b:	lea    0x78(%r14),%rcx
@@ -20993,15 +20993,15 @@
    18000ca30:	lea    0x130(%rbp),%rcx
    18000ca37:	xor    %r9d,%r9d
    18000ca3a:	mov    %rax,0x20(%rsp)
    18000ca3f:	xor    %r8d,%r8d
    18000ca42:	xor    %edx,%edx
    18000ca44:	call   *0xea8e(%rip)        # 0x18001b4d8
    18000ca4a:	mov    %rax,%rcx
-   18000ca4d:	lea    0x11f4c(%rip),%rdx        # 0x18001e9a0
+   18000ca4d:	lea    0x11f5c(%rip),%rdx        # 0x18001e9b0
    18000ca54:	call   *0xea86(%rip)        # 0x18001b4e0
    18000ca5a:	xor    %eax,%eax
    18000ca5c:	jmp    0x18000d4e0
    18000ca61:	mov    %rbx,0x460(%rsp)
    18000ca69:	lea    0x60(%rsp),%rcx
    18000ca6e:	mov    %rsi,0x458(%rsp)
    18000ca76:	mov    %r12,%rdx
@@ -21168,15 +21168,15 @@
    18000cd99:	mov    0x8(%rdi),%rbx
    18000cd9d:	mov    0x8(%rdi),%rdi
    18000cda1:	mov    (%rbx),%rbx
    18000cda4:	mov    %rbx,-0x70(%rbp)
    18000cda8:	mov    $0xffffffffffffffff,%rsi
    18000cdaf:	cmp    %rdi,%rbx
    18000cdb2:	je     0x18000ceb0
-   18000cdb8:	lea    0x11bf9(%rip),%r15        # 0x18001e9b8
+   18000cdb8:	lea    0x11c09(%rip),%r15        # 0x18001e9c8
    18000cdbf:	nop
    18000cdc0:	lea    0x20(%rbx),%rdx
    18000cdc4:	lea    0x48(%rbp),%rcx
    18000cdc8:	call   *0xe472(%rip)        # 0x18001b240
    18000cdce:	lea    0x38(%rbx),%rdx
    18000cdd2:	lea    0x230(%rbp),%rcx
    18000cdd9:	call   *0xe599(%rip)        # 0x18001b378
@@ -21346,15 +21346,15 @@
    18000d0dd:	mov    %eax,%edx
    18000d0df:	mov    %rbx,%rcx
    18000d0e2:	call   0x1800095e0
    18000d0e7:	lea    0x50(%rsp),%rdx
    18000d0ec:	lea    0x1b0(%rbp),%rcx
    18000d0f3:	call   0x18000a9c0
    18000d0f8:	mov    %rsi,%r8
-   18000d0fb:	lea    0x114ee(%rip),%rdx        # 0x18001e5f0
+   18000d0fb:	lea    0x114fe(%rip),%rdx        # 0x18001e600
    18000d102:	lea    0x100(%rbp),%rcx
    18000d109:	mov    %rax,%rbx
    18000d10c:	call   *0xe3de(%rip)        # 0x18001b4f0
    18000d112:	mov    %rbx,%r8
    18000d115:	lea    0x100(%rbp),%rdx
    18000d11c:	lea    0x60(%rsp),%rcx
    18000d121:	call   *0xe7d1(%rip)        # 0x18001b8f8
@@ -21891,15 +21891,15 @@
    18000d8f9:	je     0x18000d929
    18000d8fb:	xor    %r9d,%r9d
    18000d8fe:	lea    0xf(%rbp),%rcx
    18000d902:	xor    %r8d,%r8d
    18000d905:	xor    %edx,%edx
    18000d907:	call   *0xdc83(%rip)        # 0x18001b590
    18000d90d:	mov    %rax,%rcx
-   18000d910:	lea    0x11149(%rip),%rdx        # 0x18001ea60
+   18000d910:	lea    0x11159(%rip),%rdx        # 0x18001ea70
    18000d917:	call   *0xdc7b(%rip)        # 0x18001b598
    18000d91d:	lea    -0x9(%rbp),%rcx
    18000d921:	call   *0xd899(%rip)        # 0x18001b1c0
    18000d927:	jmp    0x18000d95f
    18000d929:	lea    -0x9(%rbp),%rdx
    18000d92d:	lea    -0x29(%rbp),%rcx
    18000d931:	call   0x18000f470
@@ -21931,15 +21931,15 @@
    18000d9a6:	call   *0xd824(%rip)        # 0x18001b1d0
    18000d9ac:	lea    -0x19(%rbp),%rcx
    18000d9b0:	call   0x180003330
    18000d9b5:	lea    -0x21(%rbp),%rdx
    18000d9b9:	lea    0xf(%rbp),%rcx
    18000d9bd:	call   0x18000a9c0
    18000d9c2:	mov    $0xffffffffffffffff,%r8
-   18000d9c9:	lea    0x10c20(%rip),%rdx        # 0x18001e5f0
+   18000d9c9:	lea    0x10c30(%rip),%rdx        # 0x18001e600
    18000d9d0:	lea    -0x9(%rbp),%rcx
    18000d9d4:	mov    %rax,%rbx
    18000d9d7:	call   *0xdb13(%rip)        # 0x18001b4f0
    18000d9dd:	mov    %rbx,%r8
    18000d9e0:	lea    -0x9(%rbp),%rdx
    18000d9e4:	mov    %r14,%rcx
    18000d9e7:	call   *0xdf0b(%rip)        # 0x18001b8f8
@@ -22017,15 +22017,15 @@
    18000dae9:	je     0x18000db19
    18000daeb:	xor    %r9d,%r9d
    18000daee:	lea    -0x40(%rbp),%rcx
    18000daf2:	xor    %r8d,%r8d
    18000daf5:	xor    %edx,%edx
    18000daf7:	call   *0xda93(%rip)        # 0x18001b590
    18000dafd:	mov    %rax,%rcx
-   18000db00:	lea    0x10f59(%rip),%rdx        # 0x18001ea60
+   18000db00:	lea    0x10f69(%rip),%rdx        # 0x18001ea70
    18000db07:	call   *0xda8b(%rip)        # 0x18001b598
    18000db0d:	lea    -0x78(%rbp),%rcx
    18000db11:	call   *0xd6a9(%rip)        # 0x18001b1c0
    18000db17:	jmp    0x18000db51
    18000db19:	lea    -0x78(%rbp),%rdx
    18000db1d:	lea    0x40(%rsp),%rcx
    18000db22:	call   0x18000f470
@@ -22109,15 +22109,15 @@
    18000dc81:	call   *0xd7e1(%rip)        # 0x18001b468
    18000dc87:	lea    0x30(%rsp),%rcx
    18000dc8c:	call   *0xd606(%rip)        # 0x18001b298
    18000dc92:	lea    0x38(%rsp),%rdx
    18000dc97:	lea    0x10(%rbp),%rcx
    18000dc9b:	call   0x18000a9c0
    18000dca0:	mov    $0xffffffffffffffff,%rdi
-   18000dca7:	lea    0x10942(%rip),%rdx        # 0x18001e5f0
+   18000dca7:	lea    0x10952(%rip),%rdx        # 0x18001e600
    18000dcae:	mov    %rdi,%r8
    18000dcb1:	lea    -0x58(%rbp),%rcx
    18000dcb5:	mov    %rax,%rbx
    18000dcb8:	call   *0xd832(%rip)        # 0x18001b4f0
    18000dcbe:	mov    %rbx,%r8
    18000dcc1:	lea    -0x58(%rbp),%rdx
    18000dcc5:	mov    %rsi,%rcx
@@ -22198,36 +22198,36 @@
    18000ddcf:	je     0x18000de06
    18000ddd1:	xor    %r9d,%r9d
    18000ddd4:	lea    0x20(%rsp),%rcx
    18000ddd9:	xor    %r8d,%r8d
    18000dddc:	xor    %edx,%edx
    18000ddde:	call   *0xd7ac(%rip)        # 0x18001b590
    18000dde4:	mov    %rax,%rcx
-   18000dde7:	lea    0x10c4a(%rip),%rdx        # 0x18001ea38
+   18000dde7:	lea    0x10c5a(%rip),%rdx        # 0x18001ea48
    18000ddee:	call   *0xd7a4(%rip)        # 0x18001b598
    18000ddf4:	mov    %rbx,%rcx
    18000ddf7:	call   *0xd43b(%rip)        # 0x18001b238
    18000ddfd:	mov    %rbx,%rax
    18000de00:	add    $0x60,%rsp
    18000de04:	pop    %rbx
    18000de05:	ret
-   18000de06:	lea    0x10bbb(%rip),%rax        # 0x18001e9c8
+   18000de06:	lea    0x10bcb(%rip),%rax        # 0x18001e9d8
    18000de0d:	jmp    0x18000de4b
    18000de0f:	xor    %r9d,%r9d
    18000de12:	lea    0x40(%rsp),%rcx
    18000de17:	xor    %r8d,%r8d
    18000de1a:	xor    %edx,%edx
    18000de1c:	call   *0xd76e(%rip)        # 0x18001b590
    18000de22:	mov    %rax,%rcx
-   18000de25:	lea    0x10bcc(%rip),%rdx        # 0x18001e9f8
+   18000de25:	lea    0x10bdc(%rip),%rdx        # 0x18001ea08
    18000de2c:	call   *0xd766(%rip)        # 0x18001b598
-   18000de32:	lea    0x10be7(%rip),%rax        # 0x18001ea20
+   18000de32:	lea    0x10bf7(%rip),%rax        # 0x18001ea30
    18000de39:	movq   $0x8,0x30(%rsp)
    18000de42:	jmp    0x18000de54
-   18000de44:	lea    0x10b95(%rip),%rax        # 0x18001e9e0
+   18000de44:	lea    0x10ba5(%rip),%rax        # 0x18001e9f0
    18000de4b:	movq   $0x9,0x30(%rsp)
    18000de54:	lea    0x20(%rsp),%rdx
    18000de59:	movq   $0x0,0x20(%rsp)
    18000de62:	mov    %rbx,%rcx
    18000de65:	mov    %rax,0x28(%rsp)
    18000de6a:	call   *0xd560(%rip)        # 0x18001b3d0
    18000de70:	mov    0x20(%rsp),%rcx
@@ -22319,15 +22319,15 @@
    18000df50:	rex push %rbx
    18000df52:	sub    $0x30,%rsp
    18000df56:	mov    %r9d,0x20(%rsp)
    18000df5b:	mov    %rcx,%rbx
    18000df5e:	mov    %r8,%r9
    18000df61:	mov    %rdx,%r8
    18000df64:	mov    %rcx,%rdx
-   18000df67:	lea    0x11232(%rip),%rcx        # 0x18001f1a0
+   18000df67:	lea    0x11242(%rip),%rcx        # 0x18001f1b0
    18000df6e:	call   *0xd2ac(%rip)        # 0x18001b220
    18000df74:	mov    %rbx,%rax
    18000df77:	add    $0x30,%rsp
    18000df7b:	pop    %rbx
    18000df7c:	ret
    18000df7d:	int3
    18000df7e:	int3
@@ -23650,15 +23650,15 @@
    18000f0d6:	lea    0x1e24b(%rip),%rcx        # 0x18002d328
    18000f0dd:	call   0x180019588
    18000f0e2:	cmpl   $0xffffffff,0x1e23f(%rip)        # 0x18002d328
    18000f0e9:	jne    0x18000f0c9
    18000f0eb:	lea    0x1e21e(%rip),%rbx        # 0x18002d310
    18000f0f2:	xor    %r8d,%r8d
    18000f0f5:	mov    %rbx,%rcx
-   18000f0f8:	lea    0xfa81(%rip),%rdx        # 0x18001eb80
+   18000f0f8:	lea    0xfa91(%rip),%rdx        # 0x18001eb90
    18000f0ff:	call   *0xc333(%rip)        # 0x18001b438
    18000f105:	lea    0xb754(%rip),%rcx        # 0x18001a860
    18000f10c:	call   0x180019a00
    18000f111:	lea    0x1e210(%rip),%rcx        # 0x18002d328
    18000f118:	call   0x180019528
    18000f11d:	mov    %rbx,%rax
    18000f120:	add    $0x20,%rsp
@@ -23788,21 +23788,21 @@
    18000f2c7:	call   *0xc20b(%rip)        # 0x18001b4d8
    18000f2cd:	lea    -0x69(%rbp),%rdx
    18000f2d1:	mov    %rax,%rbx
    18000f2d4:	lea    0x20(%rdi),%rcx
    18000f2d8:	call   *0xc34a(%rip)        # 0x18001b628
    18000f2de:	mov    %rax,%rcx
    18000f2e1:	call   *0xc2c9(%rip)        # 0x18001b5b0
-   18000f2e7:	lea    0xf972(%rip),%rdx        # 0x18001ec60
+   18000f2e7:	lea    0xf982(%rip),%rdx        # 0x18001ec70
    18000f2ee:	mov    %rbx,%rcx
    18000f2f1:	mov    %rax,%r8
    18000f2f4:	call   *0xc1e6(%rip)        # 0x18001b4e0
    18000f2fa:	lea    -0x69(%rbp),%rcx
    18000f2fe:	call   *0xbecc(%rip)        # 0x18001b1d0
-   18000f304:	lea    0xf951(%rip),%rdx        # 0x18001ec5c
+   18000f304:	lea    0xf961(%rip),%rdx        # 0x18001ec6c
    18000f30b:	mov    %r15,%rcx
    18000f30e:	call   *0xbedc(%rip)        # 0x18001b1f0
    18000f314:	lea    -0x9(%rbp),%rcx
    18000f318:	call   *0xbea2(%rip)        # 0x18001b1c0
    18000f31e:	lea    -0x49(%rbp),%rcx
    18000f322:	mov    %rax,%rbx
    18000f325:	call   *0xbe95(%rip)        # 0x18001b1c0
@@ -23816,15 +23816,15 @@
    18000f345:	call   *0xc39d(%rip)        # 0x18001b6e8
    18000f34b:	lea    -0x69(%rbp),%rcx
    18000f34f:	call   *0xbe7b(%rip)        # 0x18001b1d0
    18000f355:	lea    -0x49(%rbp),%rcx
    18000f359:	call   *0xbe71(%rip)        # 0x18001b1d0
    18000f35f:	lea    -0x9(%rbp),%rcx
    18000f363:	call   *0xbe67(%rip)        # 0x18001b1d0
-   18000f369:	lea    0xf904(%rip),%rdx        # 0x18001ec74
+   18000f369:	lea    0xf914(%rip),%rdx        # 0x18001ec84
    18000f370:	mov    %r15,%rcx
    18000f373:	call   *0xbe77(%rip)        # 0x18001b1f0
    18000f379:	lea    0xf(%rbp),%rcx
    18000f37d:	call   *0xbe3d(%rip)        # 0x18001b1c0
    18000f383:	lea    -0x49(%rbp),%rcx
    18000f387:	mov    %rax,%rsi
    18000f38a:	call   *0xbe30(%rip)        # 0x18001b1c0
@@ -24483,15 +24483,15 @@
    18000fcb6:	lea    0x30(%rsp),%rcx
    18000fcbb:	xor    %r9d,%r9d
    18000fcbe:	mov    %rax,0x20(%rsp)
    18000fcc3:	xor    %r8d,%r8d
    18000fcc6:	xor    %edx,%edx
    18000fcc8:	call   *0xb80a(%rip)        # 0x18001b4d8
    18000fcce:	mov    %rax,%rcx
-   18000fcd1:	lea    0xefa0(%rip),%rdx        # 0x18001ec78
+   18000fcd1:	lea    0xefb0(%rip),%rdx        # 0x18001ec88
    18000fcd8:	call   *0xb9ca(%rip)        # 0x18001b6a8
    18000fcde:	mov    %rbx,%rcx
    18000fce1:	call   *0xb4d9(%rip)        # 0x18001b1c0
    18000fce7:	mov    %rbx,%rax
    18000fcea:	mov    0x60(%rsp),%rbx
    18000fcef:	add    $0x50,%rsp
    18000fcf3:	pop    %rdi
@@ -24912,31 +24912,31 @@
    180010245:	cmp    $0x5,%eax
    180010248:	ja     0x180010322
    18001024e:	lea    -0x10255(%rip),%rdx        # 0x180000000
    180010255:	cltq
    180010257:	mov    0x108b8(%rdx,%rax,4),%ecx
    18001025e:	add    %rdx,%rcx
    180010261:	jmp    *%rcx
-   180010263:	lea    0xe936(%rip),%rdx        # 0x18001eba0
+   180010263:	lea    0xe946(%rip),%rdx        # 0x18001ebb0
    18001026a:	mov    %r13,%rcx
    18001026d:	call   *0xaf7d(%rip)        # 0x18001b1f0
    180010273:	jmp    0x180010362
-   180010278:	lea    0xe929(%rip),%rdx        # 0x18001eba8
+   180010278:	lea    0xe939(%rip),%rdx        # 0x18001ebb8
    18001027f:	mov    %r13,%rcx
    180010282:	call   *0xaf68(%rip)        # 0x18001b1f0
    180010288:	jmp    0x180010362
-   18001028d:	lea    0xe918(%rip),%rdx        # 0x18001ebac
+   18001028d:	lea    0xe928(%rip),%rdx        # 0x18001ebbc
    180010294:	mov    %r13,%rcx
    180010297:	call   *0xaf53(%rip)        # 0x18001b1f0
    18001029d:	jmp    0x180010362
-   1800102a2:	lea    0xe7fb(%rip),%rdx        # 0x18001eaa4
+   1800102a2:	lea    0xe80b(%rip),%rdx        # 0x18001eab4
    1800102a9:	mov    %r13,%rcx
    1800102ac:	call   *0xaf3e(%rip)        # 0x18001b1f0
    1800102b2:	jmp    0x180010362
-   1800102b7:	lea    0xe8f2(%rip),%rdx        # 0x18001ebb0
+   1800102b7:	lea    0xe902(%rip),%rdx        # 0x18001ebc0
    1800102be:	mov    %r13,%rcx
    1800102c1:	call   *0xaf29(%rip)        # 0x18001b1f0
    1800102c7:	jmp    0x180010362
    1800102cc:	lea    0x8(%r14),%rcx
    1800102d0:	call   *0xb3ea(%rip)        # 0x18001b6c0
    1800102d6:	test   %al,%al
    1800102d8:	jne    0x1800102e9
@@ -24953,30 +24953,30 @@
    1800102fe:	mov    0x8(%rbx),%rax
    180010302:	lea    0x60(%rbp),%rcx
    180010306:	xor    %r9d,%r9d
    180010309:	mov    %rax,0x20(%rsp)
    18001030e:	xor    %r8d,%r8d
    180010311:	xor    %edx,%edx
    180010313:	call   *0xb1bf(%rip)        # 0x18001b4d8
-   180010319:	lea    0xe8a0(%rip),%rdx        # 0x18001ebc0
+   180010319:	lea    0xe8b0(%rip),%rdx        # 0x18001ebd0
    180010320:	jmp    0x180010359
    180010322:	call   0x18000f0a0
    180010327:	mov    %rax,%rcx
    18001032a:	mov    %rax,%rbx
    18001032d:	call   *0xb3dd(%rip)        # 0x18001b710
    180010333:	test   %al,%al
    180010335:	je     0x180010362
    180010337:	mov    0x8(%rbx),%rax
    18001033b:	lea    0x60(%rbp),%rcx
    18001033f:	xor    %r9d,%r9d
    180010342:	mov    %rax,0x20(%rsp)
    180010347:	xor    %r8d,%r8d
    18001034a:	xor    %edx,%edx
    18001034c:	call   *0xb186(%rip)        # 0x18001b4d8
-   180010352:	lea    0xe8cf(%rip),%rdx        # 0x18001ec28
+   180010352:	lea    0xe8df(%rip),%rdx        # 0x18001ec38
    180010359:	mov    %rax,%rcx
    18001035c:	call   *0xb346(%rip)        # 0x18001b6a8
    180010362:	mov    $0x26,%dl
    180010364:	mov    %r13,%rcx
    180010367:	call   *0xb04b(%rip)        # 0x18001b3b8
    18001036d:	lea    -0x8(%rbp),%rcx
    180010371:	call   *0xae49(%rip)        # 0x18001b1c0
@@ -25015,15 +25015,15 @@
    1800103fe:	je     0x180010410
    180010400:	movzbl (%rsi),%ecx
    180010403:	inc    %rsi
    180010406:	mov    %cl,(%rdi)
    180010408:	inc    %rdi
    18001040b:	cmp    %rax,%rsi
    18001040e:	jne    0x180010400
-   180010410:	lea    0xe845(%rip),%rcx        # 0x18001ec5c
+   180010410:	lea    0xe855(%rip),%rcx        # 0x18001ec6c
    180010417:	mov    $0x26,%al
    180010419:	sub    %rdi,%rcx
    18001041c:	nopl   0x0(%rax)
    180010420:	mov    %al,(%rdi)
    180010422:	inc    %rdi
    180010425:	movzbl (%rcx,%rdi,1),%eax
    180010429:	test   %al,%al
@@ -25799,105 +25799,105 @@
    180010f09:	int3
    180010f0a:	int3
    180010f0b:	int3
    180010f0c:	int3
    180010f0d:	int3
    180010f0e:	int3
    180010f0f:	int3
-   180010f10:	lea    0xdf19(%rip),%rax        # 0x18001ee30
-   180010f17:	ret
-   180010f18:	int3
-   180010f19:	int3
-   180010f1a:	int3
-   180010f1b:	int3
-   180010f1c:	int3
-   180010f1d:	int3
-   180010f1e:	int3
-   180010f1f:	int3
-   180010f20:	sub    $0x38,%rsp
-   180010f24:	test   %edx,%edx
-   180010f26:	jne    0x180010f87
-   180010f28:	test   %r8d,%r8d
-   180010f2b:	je     0x180010f5b
-   180010f2d:	sub    $0x1,%r8d
-   180010f31:	je     0x180010f46
-   180010f33:	cmp    $0x1,%r8d
-   180010f37:	jne    0x180010ff0
-   180010f3d:	add    $0x38,%rsp
-   180010f41:	jmp    0x180013610
-   180010f46:	mov    (%rcx),%rax
-   180010f49:	mov    0x88(%rax),%rax
-   180010f50:	add    $0x38,%rsp
-   180010f54:	rex.W jmp *0xab2d(%rip)        # 0x18001ba88
-   180010f5b:	mov    0x8(%r9),%rax
-   180010f5f:	lea    0xdeca(%rip),%rdx        # 0x18001ee30
-   180010f66:	lea    0x20(%rsp),%r9
-   180010f6b:	mov    %rax,0x28(%rsp)
-   180010f70:	xor    %r8d,%r8d
-   180010f73:	movq   $0x0,0x20(%rsp)
-   180010f7c:	call   *0xa2a6(%rip)        # 0x18001b228
-   180010f82:	add    $0x38,%rsp
-   180010f86:	ret
-   180010f87:	cmp    $0x5,%edx
-   180010f8a:	jne    0x180010faa
-   180010f8c:	mov    0x8(%r9),%rax
-   180010f90:	lea    0x1949(%rip),%rcx        # 0x1800128e0
-   180010f97:	cmp    %rcx,(%rax)
-   180010f9a:	jne    0x180010ff0
-   180010f9c:	mov    (%r9),%rax
-   180010f9f:	movl   $0x0,(%rax)
-   180010fa5:	add    $0x38,%rsp
-   180010fa9:	ret
-   180010faa:	cmp    $0x1,%edx
-   180010fad:	jne    0x180010ff5
-   180010faf:	mov    %rbx,0x30(%rsp)
-   180010fb4:	mov    (%r9),%rbx
-   180010fb7:	test   %r8d,%r8d
-   180010fba:	jne    0x180010feb
-   180010fbc:	mov    0x8(%rcx),%rdx
-   180010fc0:	lea    0x20(%rsp),%rcx
-   180010fc5:	add    $0x208,%rdx
-   180010fcc:	call   *0xa2b6(%rip)        # 0x18001b288
-   180010fd2:	lea    0x20(%rsp),%rdx
-   180010fd7:	mov    %rbx,%rcx
-   180010fda:	call   *0xa2b0(%rip)        # 0x18001b290
-   180010fe0:	lea    0x20(%rsp),%rcx
-   180010fe5:	call   *0xa2ad(%rip)        # 0x18001b298
-   180010feb:	mov    0x30(%rsp),%rbx
-   180010ff0:	add    $0x38,%rsp
-   180010ff4:	ret
-   180010ff5:	cmp    $0x2,%edx
-   180010ff8:	jne    0x180010ff0
-   180010ffa:	test   %r8d,%r8d
-   180010ffd:	jne    0x180010ff0
-   180010fff:	mov    (%r9),%rdx
-   180011002:	add    $0x38,%rsp
-   180011006:	jmp    0x1800149b0
-   18001100b:	int3
-   18001100c:	int3
-   18001100d:	int3
-   18001100e:	int3
-   18001100f:	int3
-   180011010:	rex push %rbx
-   180011012:	sub    $0x40,%rsp
-   180011016:	lea    0x20(%rsp),%rcx
-   18001101b:	mov    %rdx,%rbx
-   18001101e:	call   *0xa214(%rip)        # 0x18001b238
-   180011024:	xor    %r9d,%r9d
-   180011027:	xor    %r8d,%r8d
-   18001102a:	mov    %rax,%rdx
-   18001102d:	mov    %rbx,%rcx
-   180011030:	call   0x180011310
-   180011035:	lea    0x20(%rsp),%rcx
-   18001103a:	call   *0xa208(%rip)        # 0x18001b248
-   180011040:	lea    0xde31(%rip),%rax        # 0x18001ee78
-   180011047:	mov    %rax,(%rbx)
-   18001104a:	add    $0x40,%rsp
-   18001104e:	pop    %rbx
-   18001104f:	ret
+   180010f10:	rex push %rbx
+   180010f12:	sub    $0x40,%rsp
+   180010f16:	lea    0x20(%rsp),%rcx
+   180010f1b:	mov    %rdx,%rbx
+   180010f1e:	call   *0xa314(%rip)        # 0x18001b238
+   180010f24:	xor    %r9d,%r9d
+   180010f27:	xor    %r8d,%r8d
+   180010f2a:	mov    %rax,%rdx
+   180010f2d:	mov    %rbx,%rcx
+   180010f30:	call   0x180011310
+   180010f35:	lea    0x20(%rsp),%rcx
+   180010f3a:	call   *0xa308(%rip)        # 0x18001b248
+   180010f40:	lea    0xdf41(%rip),%rax        # 0x18001ee88
+   180010f47:	mov    %rax,(%rbx)
+   180010f4a:	add    $0x40,%rsp
+   180010f4e:	pop    %rbx
+   180010f4f:	ret
+   180010f50:	lea    0xdee9(%rip),%rax        # 0x18001ee40
+   180010f57:	ret
+   180010f58:	int3
+   180010f59:	int3
+   180010f5a:	int3
+   180010f5b:	int3
+   180010f5c:	int3
+   180010f5d:	int3
+   180010f5e:	int3
+   180010f5f:	int3
+   180010f60:	sub    $0x38,%rsp
+   180010f64:	test   %edx,%edx
+   180010f66:	jne    0x180010fc7
+   180010f68:	test   %r8d,%r8d
+   180010f6b:	je     0x180010f9b
+   180010f6d:	sub    $0x1,%r8d
+   180010f71:	je     0x180010f86
+   180010f73:	cmp    $0x1,%r8d
+   180010f77:	jne    0x180011030
+   180010f7d:	add    $0x38,%rsp
+   180010f81:	jmp    0x180013610
+   180010f86:	mov    (%rcx),%rax
+   180010f89:	mov    0x88(%rax),%rax
+   180010f90:	add    $0x38,%rsp
+   180010f94:	rex.W jmp *0xaaed(%rip)        # 0x18001ba88
+   180010f9b:	mov    0x8(%r9),%rax
+   180010f9f:	lea    0xde9a(%rip),%rdx        # 0x18001ee40
+   180010fa6:	lea    0x20(%rsp),%r9
+   180010fab:	mov    %rax,0x28(%rsp)
+   180010fb0:	xor    %r8d,%r8d
+   180010fb3:	movq   $0x0,0x20(%rsp)
+   180010fbc:	call   *0xa266(%rip)        # 0x18001b228
+   180010fc2:	add    $0x38,%rsp
+   180010fc6:	ret
+   180010fc7:	cmp    $0x5,%edx
+   180010fca:	jne    0x180010fea
+   180010fcc:	mov    0x8(%r9),%rax
+   180010fd0:	lea    0x1909(%rip),%rcx        # 0x1800128e0
+   180010fd7:	cmp    %rcx,(%rax)
+   180010fda:	jne    0x180011030
+   180010fdc:	mov    (%r9),%rax
+   180010fdf:	movl   $0x0,(%rax)
+   180010fe5:	add    $0x38,%rsp
+   180010fe9:	ret
+   180010fea:	cmp    $0x1,%edx
+   180010fed:	jne    0x180011035
+   180010fef:	mov    %rbx,0x30(%rsp)
+   180010ff4:	mov    (%r9),%rbx
+   180010ff7:	test   %r8d,%r8d
+   180010ffa:	jne    0x18001102b
+   180010ffc:	mov    0x8(%rcx),%rdx
+   180011000:	lea    0x20(%rsp),%rcx
+   180011005:	add    $0x208,%rdx
+   18001100c:	call   *0xa276(%rip)        # 0x18001b288
+   180011012:	lea    0x20(%rsp),%rdx
+   180011017:	mov    %rbx,%rcx
+   18001101a:	call   *0xa270(%rip)        # 0x18001b290
+   180011020:	lea    0x20(%rsp),%rcx
+   180011025:	call   *0xa26d(%rip)        # 0x18001b298
+   18001102b:	mov    0x30(%rsp),%rbx
+   180011030:	add    $0x38,%rsp
+   180011034:	ret
+   180011035:	cmp    $0x2,%edx
+   180011038:	jne    0x180011030
+   18001103a:	test   %r8d,%r8d
+   18001103d:	jne    0x180011030
+   18001103f:	mov    (%r9),%rdx
+   180011042:	add    $0x38,%rsp
+   180011046:	jmp    0x1800149b0
+   18001104b:	int3
+   18001104c:	int3
+   18001104d:	int3
+   18001104e:	int3
+   18001104f:	int3
    180011050:	mov    %rbx,0x10(%rsp)
    180011055:	mov    %rbp,0x18(%rsp)
    18001105a:	mov    %rsi,0x20(%rsp)
    18001105f:	push   %rdi
    180011060:	push   %r14
    180011062:	push   %r15
    180011064:	sub    $0x40,%rsp
@@ -26086,15 +26086,15 @@
    1800112ce:	mov    %rax,%rcx
    1800112d1:	call   0x180011500
    1800112d6:	mov    0x68(%rsp),%r8
    1800112db:	mov    %rax,%rdx
    1800112de:	mov    %r14,%rcx
    1800112e1:	call   0x1800062d0
    1800112e6:	mov    0x40(%rsp),%rbx
-   1800112eb:	lea    0xdb86(%rip),%rax        # 0x18001ee78
+   1800112eb:	lea    0xdb96(%rip),%rax        # 0x18001ee88
    1800112f2:	mov    0x48(%rsp),%rsi
    1800112f7:	mov    0x50(%rsp),%rdi
    1800112fc:	mov    %rax,(%r14)
    1800112ff:	mov    %r14,%rax
    180011302:	add    $0x30,%rsp
    180011306:	pop    %r14
    180011308:	ret
@@ -26135,15 +26135,15 @@
    18001136e:	mov    %r15,%rcx
    180011371:	call   0x1800062d0
    180011376:	lea    0x60(%rsp),%rcx
    18001137b:	call   *0x9f17(%rip)        # 0x18001b298
    180011381:	lea    0x78(%rsp),%rcx
    180011386:	call   *0x9f0c(%rip)        # 0x18001b298
    18001138c:	mov    0x68(%rsp),%rbx
-   180011391:	lea    0xdae0(%rip),%rax        # 0x18001ee78
+   180011391:	lea    0xdaf0(%rip),%rax        # 0x18001ee88
    180011398:	mov    %rax,(%r15)
    18001139b:	mov    %r15,%rax
    18001139e:	add    $0x30,%rsp
    1800113a2:	pop    %r15
    1800113a4:	pop    %r14
    1800113a6:	pop    %rdi
    1800113a7:	pop    %rsi
@@ -26179,15 +26179,15 @@
    180011404:	mov    0x80(%rsp),%r8
    18001140c:	mov    %rax,%rdx
    18001140f:	mov    %r14,%rcx
    180011412:	call   0x1800062d0
    180011417:	lea    0x30(%rsp),%rcx
    18001141c:	call   *0x9e26(%rip)        # 0x18001b248
    180011422:	mov    0x60(%rsp),%rbx
-   180011427:	lea    0xda4a(%rip),%rax        # 0x18001ee78
+   180011427:	lea    0xda5a(%rip),%rax        # 0x18001ee88
    18001142e:	mov    0x68(%rsp),%rbp
    180011433:	mov    0x70(%rsp),%rsi
    180011438:	mov    0x78(%rsp),%rdi
    18001143d:	mov    %rax,(%r14)
    180011440:	mov    %r14,%rax
    180011443:	add    $0x50,%rsp
    180011447:	pop    %r14
@@ -26211,15 +26211,15 @@
    180011476:	mov    %rdi,%r8
    180011479:	mov    %rax,%rdx
    18001147c:	mov    %rsi,%rcx
    18001147f:	call   0x180011310
    180011484:	lea    0x20(%rsp),%rcx
    180011489:	call   *0x9db9(%rip)        # 0x18001b248
    18001148f:	mov    0x50(%rsp),%rbx
-   180011494:	lea    0xd9dd(%rip),%rax        # 0x18001ee78
+   180011494:	lea    0xd9ed(%rip),%rax        # 0x18001ee88
    18001149b:	mov    %rax,(%rsi)
    18001149e:	mov    %rsi,%rax
    1800114a1:	mov    0x58(%rsp),%rsi
    1800114a6:	add    $0x40,%rsp
    1800114aa:	pop    %rdi
    1800114ab:	ret
    1800114ac:	int3
@@ -26237,15 +26237,15 @@
    1800114ce:	xor    %r8d,%r8d
    1800114d1:	mov    %rax,%rdx
    1800114d4:	mov    %rdi,%rcx
    1800114d7:	call   0x180011310
    1800114dc:	lea    0x20(%rsp),%rcx
    1800114e1:	call   *0x9d61(%rip)        # 0x18001b248
    1800114e7:	mov    0x50(%rsp),%rbx
-   1800114ec:	lea    0xd985(%rip),%rax        # 0x18001ee78
+   1800114ec:	lea    0xd995(%rip),%rax        # 0x18001ee88
    1800114f3:	mov    %rax,(%rdi)
    1800114f6:	mov    %rdi,%rax
    1800114f9:	add    $0x40,%rsp
    1800114fd:	pop    %rdi
    1800114fe:	ret
    1800114ff:	int3
    180011500:	mov    %rbx,0x8(%rsp)
@@ -26274,29 +26274,29 @@
    180011566:	call   0x180006590
    18001156b:	lea    0x50(%rsp),%rcx
    180011570:	call   *0x9cd2(%rip)        # 0x18001b248
    180011576:	lea    0x38(%rsp),%rcx
    18001157b:	call   *0x9cc7(%rip)        # 0x18001b248
    180011581:	lea    0x68(%rsp),%rcx
    180011586:	call   *0x9cbc(%rip)        # 0x18001b248
-   18001158c:	lea    0xd9ad(%rip),%rax        # 0x18001ef40
+   18001158c:	lea    0xd9bd(%rip),%rax        # 0x18001ef50
    180011593:	mov    %rbp,%rdx
    180011596:	lea    0x208(%r14),%rcx
    18001159d:	mov    %rax,(%r14)
    1800115a0:	call   *0x9ce2(%rip)        # 0x18001b288
    1800115a6:	lea    0x210(%r14),%rcx
    1800115ad:	call   *0x9c85(%rip)        # 0x18001b238
    1800115b3:	xor    %eax,%eax
    1800115b5:	movq   $0x4,0x30(%rsp)
    1800115be:	mov    %rax,0x228(%r14)
    1800115c5:	lea    0x20(%rsp),%rdx
    1800115ca:	mov    %rax,0x230(%r14)
    1800115d1:	lea    0x80(%rsp),%rcx
    1800115d9:	mov    %rax,0x20(%rsp)
-   1800115de:	lea    0xc363(%rip),%rax        # 0x18001d948
+   1800115de:	lea    0xca5b(%rip),%rax        # 0x18001e040
    1800115e5:	mov    %rax,0x28(%rsp)
    1800115ea:	call   *0x9de0(%rip)        # 0x18001b3d0
    1800115f0:	mov    %rax,%rdx
    1800115f3:	lea    0x1a8(%r14),%rcx
    1800115fa:	call   *0x9c58(%rip)        # 0x18001b258
    180011600:	lea    0x80(%rsp),%rcx
    180011608:	call   *0x9c3a(%rip)        # 0x18001b248
@@ -26323,15 +26323,15 @@
    180011659:	int3
    18001165a:	int3
    18001165b:	int3
    18001165c:	int3
    18001165d:	int3
    18001165e:	int3
    18001165f:	int3
-   180011660:	lea    0xd811(%rip),%rax        # 0x18001ee78
+   180011660:	lea    0xd821(%rip),%rax        # 0x18001ee88
    180011667:	mov    %rax,(%rcx)
    18001166a:	jmp    0x180006740
    18001166f:	int3
    180011670:	mov    (%rcx),%rdx
    180011673:	mov    %rcx,%r8
    180011676:	cmpb   $0x0,0x19(%rdx)
    18001167a:	je     0x180011687
@@ -26400,15 +26400,15 @@
    18001171e:	mov    -0x8(%rcx),%rdi
    180011722:	mov    %rdi,%rbx
    180011725:	mov    %r14,0x50(%rsp)
    18001172a:	shl    $0x4,%rbx
    18001172e:	add    %rcx,%rbx
    180011731:	test   %rdi,%rdi
    180011734:	je     0x180011755
-   180011736:	lea    0xd73b(%rip),%rbp        # 0x18001ee78
+   180011736:	lea    0xd74b(%rip),%rbp        # 0x18001ee88
    18001173d:	nopl   (%rax)
    180011740:	sub    $0x10,%rbx
    180011744:	mov    %rbx,%rcx
    180011747:	mov    %rbp,(%rbx)
    18001174a:	call   0x180006740
    18001174f:	sub    $0x1,%rdi
    180011753:	jne    0x180011740
@@ -26424,15 +26424,15 @@
    18001177a:	mov    0x50(%rsp),%r14
    18001177f:	lea    -0x8(%rsi),%rax
    180011783:	add    $0x20,%rsp
    180011787:	pop    %r15
    180011789:	pop    %rsi
    18001178a:	pop    %rbp
    18001178b:	ret
-   18001178c:	lea    0xd6e5(%rip),%rbp        # 0x18001ee78
+   18001178c:	lea    0xd6f5(%rip),%rbp        # 0x18001ee88
    180011793:	mov    %rbp,(%rcx)
    180011796:	call   0x180006740
    18001179b:	test   $0x1,%r15b
    18001179f:	je     0x1800117ae
    1800117a1:	mov    $0x10,%edx
    1800117a6:	mov    %rsi,%rcx
    1800117a9:	call   0x180019368
@@ -26456,15 +26456,15 @@
    1800117d4:	xor    %r9d,%r9d
    1800117d7:	xor    %r8d,%r8d
    1800117da:	mov    %rax,%rdx
    1800117dd:	mov    %rbx,%rcx
    1800117e0:	call   0x180011310
    1800117e5:	lea    0x20(%rsp),%rcx
    1800117ea:	call   *0x9a58(%rip)        # 0x18001b248
-   1800117f0:	lea    0xd681(%rip),%rax        # 0x18001ee78
+   1800117f0:	lea    0xd691(%rip),%rax        # 0x18001ee88
    1800117f7:	mov    %rax,(%rbx)
    1800117fa:	add    $0x40,%rsp
    1800117fe:	pop    %rbx
    1800117ff:	ret
    180011800:	mov    %rbx,0x8(%rsp)
    180011805:	push   %rdi
    180011806:	sub    $0x20,%rsp
@@ -26604,15 +26604,15 @@
    180011a07:	call   *0x9acb(%rip)        # 0x18001b4d8
    180011a0d:	lea    -0x80(%rbp),%rdx
    180011a11:	mov    %rax,%rbx
    180011a14:	lea    0x50(%rsp),%rcx
    180011a19:	call   *0x9c09(%rip)        # 0x18001b628
    180011a1f:	mov    %rax,%rcx
    180011a22:	call   *0x9b88(%rip)        # 0x18001b5b0
-   180011a28:	lea    0xd5a1(%rip),%rdx        # 0x18001efd0
+   180011a28:	lea    0xd5b1(%rip),%rdx        # 0x18001efe0
    180011a2f:	mov    %rbx,%rcx
    180011a32:	mov    %rax,%r8
    180011a35:	call   *0x9aa5(%rip)        # 0x18001b4e0
    180011a3b:	lea    -0x80(%rbp),%rcx
    180011a3f:	call   *0x978b(%rip)        # 0x18001b1d0
    180011a45:	lea    0x50(%rsp),%rcx
    180011a4a:	call   *0x97f8(%rip)        # 0x18001b248
@@ -26914,15 +26914,15 @@
    180011efb:	lea    0x78(%rbp),%rcx
    180011eff:	xor    %r9d,%r9d
    180011f02:	mov    %rax,0x20(%rsp)
    180011f07:	xor    %r8d,%r8d
    180011f0a:	xor    %edx,%edx
    180011f0c:	call   *0x95c6(%rip)        # 0x18001b4d8
    180011f12:	mov    %rax,%rcx
-   180011f15:	lea    0xd0c4(%rip),%rdx        # 0x18001efe0
+   180011f15:	lea    0xd0d4(%rip),%rdx        # 0x18001eff0
    180011f1c:	call   *0x95be(%rip)        # 0x18001b4e0
    180011f22:	jmp    0x18001203e
    180011f27:	mov    0x38(%rsp),%rsi
    180011f2c:	lea    0x68(%rsp),%rdx
    180011f31:	mov    %rsi,%rcx
    180011f34:	call   0x180005a30
    180011f39:	lea    0x40(%rsp),%rcx
@@ -27075,15 +27075,15 @@
    180012183:	lea    0x28(%rbp),%rcx
    180012187:	xor    %r9d,%r9d
    18001218a:	mov    %rax,0x20(%rsp)
    18001218f:	xor    %r8d,%r8d
    180012192:	xor    %edx,%edx
    180012194:	call   *0x933e(%rip)        # 0x18001b4d8
    18001219a:	mov    %rax,%rcx
-   18001219d:	lea    0xcdac(%rip),%rdx        # 0x18001ef50
+   18001219d:	lea    0xcdbc(%rip),%rdx        # 0x18001ef60
    1800121a4:	call   *0x9336(%rip)        # 0x18001b4e0
    1800121aa:	jmp    0x18001288d
    1800121af:	mov    %rbx,0x208(%rsp)
    1800121b7:	lea    0x88(%rbp),%rcx
    1800121be:	mov    %rdi,0x210(%rsp)
    1800121c6:	mov    %r12,0x218(%rsp)
    1800121ce:	mov    %r15,0x1d0(%rsp)
@@ -27337,15 +27337,15 @@
    1800125ad:	lea    -0x28(%rbp),%rcx
    1800125b1:	call   *0x9071(%rip)        # 0x18001b628
    1800125b7:	mov    %rax,%rcx
    1800125ba:	call   *0x8ff0(%rip)        # 0x18001b5b0
    1800125c0:	mov    %rbx,%r9
    1800125c3:	mov    %rdi,0x20(%rsp)
    1800125c8:	mov    %rax,%r8
-   1800125cb:	lea    0xc98e(%rip),%rdx        # 0x18001ef60
+   1800125cb:	lea    0xc99e(%rip),%rdx        # 0x18001ef70
    1800125d2:	mov    %rsi,%rcx
    1800125d5:	call   *0x8f05(%rip)        # 0x18001b4e0
    1800125db:	lea    -0x60(%rbp),%rcx
    1800125df:	call   *0x8beb(%rip)        # 0x18001b1d0
    1800125e5:	lea    0x40(%rsp),%rcx
    1800125ea:	call   *0x8be0(%rip)        # 0x18001b1d0
    1800125f0:	lea    0x48(%rbp),%rcx
@@ -27375,15 +27375,15 @@
    180012660:	mov    0x80(%rsi),%rax
    180012667:	lea    0x28(%rbp),%rcx
    18001266b:	xor    %r9d,%r9d
    18001266e:	mov    %rax,0x20(%rsp)
    180012673:	xor    %r8d,%r8d
    180012676:	xor    %edx,%edx
    180012678:	call   *0x8e5a(%rip)        # 0x18001b4d8
-   18001267e:	lea    0xc8fb(%rip),%rdx        # 0x18001ef80
+   18001267e:	lea    0xc90b(%rip),%rdx        # 0x18001ef90
    180012685:	jmp    0x180012846
    18001268a:	mov    -0x30(%rbp),%rdi
    18001268e:	test   %rdi,%rdi
    180012691:	jne    0x1800126cf
    180012693:	lea    0x78(%rsi),%rcx
    180012697:	call   *0x8edb(%rip)        # 0x18001b578
    18001269d:	test   %al,%al
@@ -27391,15 +27391,15 @@
    1800126a5:	mov    0x80(%rsi),%rax
    1800126ac:	lea    0x28(%rbp),%rcx
    1800126b0:	xor    %r9d,%r9d
    1800126b3:	mov    %rax,0x20(%rsp)
    1800126b8:	xor    %r8d,%r8d
    1800126bb:	xor    %edx,%edx
    1800126bd:	call   *0x8e15(%rip)        # 0x18001b4d8
-   1800126c3:	lea    0xc8de(%rip),%rdx        # 0x18001efa8
+   1800126c3:	lea    0xc8ee(%rip),%rdx        # 0x18001efb8
    1800126ca:	jmp    0x180012846
    1800126cf:	cmp    %rdi,0x188(%rsi)
    1800126d6:	jne    0x180012813
    1800126dc:	lea    -0x40(%rbp),%rcx
    1800126e0:	call   *0x8b82(%rip)        # 0x18001b268
    1800126e6:	xor    %r15d,%r15d
    1800126e9:	test   %al,%al
@@ -27480,15 +27480,15 @@
    180012821:	mov    0x80(%rsi),%rax
    180012828:	lea    0x28(%rbp),%rcx
    18001282c:	xor    %r9d,%r9d
    18001282f:	mov    %rax,0x20(%rsp)
    180012834:	xor    %r8d,%r8d
    180012837:	xor    %edx,%edx
    180012839:	call   *0x8c99(%rip)        # 0x18001b4d8
-   18001283f:	lea    0xc77a(%rip),%rdx        # 0x18001efc0
+   18001283f:	lea    0xc78a(%rip),%rdx        # 0x18001efd0
    180012846:	mov    %rax,%rcx
    180012849:	call   *0x8c91(%rip)        # 0x18001b4e0
    18001284f:	lea    -0x40(%rbp),%rcx
    180012853:	call   *0x89ef(%rip)        # 0x18001b248
    180012859:	lea    -0x10(%rbp),%rcx
    18001285d:	call   *0x89e5(%rip)        # 0x18001b248
    180012863:	lea    -0x28(%rbp),%rcx
@@ -27532,15 +27532,15 @@
    1800128dc:	int3
    1800128dd:	int3
    1800128de:	int3
    1800128df:	int3
    1800128e0:	sub    $0x38,%rsp
    1800128e4:	mov    %rdx,0x28(%rsp)
    1800128e9:	lea    0x20(%rsp),%r9
-   1800128ee:	lea    0xc53b(%rip),%rdx        # 0x18001ee30
+   1800128ee:	lea    0xc54b(%rip),%rdx        # 0x18001ee40
    1800128f5:	movq   $0x0,0x20(%rsp)
    1800128fe:	xor    %r8d,%r8d
    180012901:	call   *0x8921(%rip)        # 0x18001b228
    180012907:	add    $0x38,%rsp
    18001290b:	ret
    18001290c:	int3
    18001290d:	int3
@@ -27717,15 +27717,15 @@
    180012c3c:	mov    %rax,%rbx
    180012c3f:	call   *0x8ac3(%rip)        # 0x18001b708
    180012c45:	mov    %rax,%rcx
    180012c48:	lea    -0x28(%rbp),%rdx
    180012c4c:	call   *0x8ad6(%rip)        # 0x18001b728
    180012c52:	mov    %rax,%rcx
    180012c55:	call   *0x8955(%rip)        # 0x18001b5b0
-   180012c5b:	lea    0xc45e(%rip),%rdx        # 0x18001f0c0
+   180012c5b:	lea    0xc46e(%rip),%rdx        # 0x18001f0d0
    180012c62:	mov    %rbx,%rcx
    180012c65:	mov    %rax,%r8
    180012c68:	call   *0x8ab2(%rip)        # 0x18001b720
    180012c6e:	lea    -0x28(%rbp),%rcx
    180012c72:	call   *0x8558(%rip)        # 0x18001b1d0
    180012c78:	lea    -0x10(%rbp),%rcx
    180012c7c:	call   *0x85c6(%rip)        # 0x18001b248
@@ -27944,15 +27944,15 @@
    180012f50:	lea    0x30(%rsp),%rcx
    180012f55:	xor    %r9d,%r9d
    180012f58:	mov    %rax,0x20(%rsp)
    180012f5d:	xor    %r8d,%r8d
    180012f60:	xor    %edx,%edx
    180012f62:	call   *0x8570(%rip)        # 0x18001b4d8
    180012f68:	mov    %rax,%rcx
-   180012f6b:	lea    0xc08e(%rip),%rdx        # 0x18001f000
+   180012f6b:	lea    0xc09e(%rip),%rdx        # 0x18001f010
    180012f72:	call   *0x8568(%rip)        # 0x18001b4e0
    180012f78:	mov    0x68(%rsp),%rbx
    180012f7d:	mov    0x70(%rsp),%rsi
    180012f82:	add    $0x50,%rsp
    180012f86:	pop    %rdi
    180012f87:	ret
    180012f88:	lea    0x208(%rbx),%rcx
@@ -27967,15 +27967,15 @@
    180012fb2:	lea    0x30(%rsp),%rcx
    180012fb7:	xor    %r9d,%r9d
    180012fba:	mov    %rax,0x20(%rsp)
    180012fbf:	xor    %r8d,%r8d
    180012fc2:	xor    %edx,%edx
    180012fc4:	call   *0x850e(%rip)        # 0x18001b4d8
    180012fca:	mov    %rax,%rcx
-   180012fcd:	lea    0xc044(%rip),%rdx        # 0x18001f018
+   180012fcd:	lea    0xc054(%rip),%rdx        # 0x18001f028
    180012fd4:	call   *0x8506(%rip)        # 0x18001b4e0
    180012fda:	mov    0x68(%rsp),%rbx
    180012fdf:	mov    0x70(%rsp),%rsi
    180012fe4:	add    $0x50,%rsp
    180012fe8:	pop    %rdi
    180012fe9:	ret
    180012fea:	mov    (%rdi),%rax
@@ -28355,15 +28355,15 @@
    1800134fd:	int3
    1800134fe:	int3
    1800134ff:	int3
    180013500:	mov    0x8(%rcx),%rcx
    180013504:	cmpq   $0x0,0x38(%rcx)
    180013509:	je     0x180013512
    18001350b:	rex.W jmp *0x7df6(%rip)        # 0x18001b308
-   180013512:	lea    0xb917(%rip),%rax        # 0x18001ee30
+   180013512:	lea    0xb927(%rip),%rax        # 0x18001ee40
    180013519:	ret
    18001351a:	int3
    18001351b:	int3
    18001351c:	int3
    18001351d:	int3
    18001351e:	int3
    18001351f:	int3
@@ -28383,15 +28383,15 @@
    180013549:	jne    0x180013565
    18001354b:	cmp    $0x3,%eax
    18001354e:	jge    0x180013579
    180013550:	mov    %rsi,%r9
    180013553:	mov    %eax,%r8d
    180013556:	xor    %edx,%edx
    180013558:	mov    %rbp,%rcx
-   18001355b:	call   0x180010f20
+   18001355b:	call   0x180010f60
    180013560:	sub    $0x3,%ebx
    180013563:	jmp    0x18001359f
    180013565:	cmp    $0x7,%edi
    180013568:	jne    0x18001357e
    18001356a:	cmp    $0x3,%ebx
    18001356d:	jge    0x180013579
    18001356f:	mov    (%rsi),%rax
@@ -28403,15 +28403,15 @@
    180013583:	mov    $0x14e,%eax
    180013588:	bt     %edi,%eax
    18001358b:	jae    0x18001359f
    18001358d:	mov    %rsi,%r9
    180013590:	mov    %ebx,%r8d
    180013593:	mov    %edi,%edx
    180013595:	mov    %rbp,%rcx
-   180013598:	call   0x180010f20
+   180013598:	call   0x180010f60
    18001359d:	dec    %ebx
    18001359f:	mov    %ebx,%eax
    1800135a1:	mov    0x30(%rsp),%rbx
    1800135a6:	mov    0x38(%rsp),%rbp
    1800135ab:	mov    0x40(%rsp),%rsi
    1800135b0:	add    $0x20,%rsp
    1800135b4:	pop    %rdi
@@ -28428,15 +28428,15 @@
    1800135bf:	int3
    1800135c0:	mov    %rdx,%r9
    1800135c3:	mov    %rcx,%r10
    1800135c6:	test   %rdx,%rdx
    1800135c9:	jne    0x1800135ce
    1800135cb:	xor    %eax,%eax
    1800135cd:	ret
-   1800135ce:	lea    0xb6fb(%rip),%r8        # 0x18001ecd0
+   1800135ce:	lea    0xb70b(%rip),%r8        # 0x18001ece0
    1800135d5:	mov    %r9,%rax
    1800135d8:	sub    %r9,%r8
    1800135db:	nopl   0x0(%rax,%rax,1)
    1800135e0:	movzbl (%rax),%edx
    1800135e3:	movzbl (%rax,%r8,1),%ecx
    1800135e8:	sub    %ecx,%edx
    1800135ea:	jne    0x1800135f3
@@ -28480,15 +28480,15 @@
    18001365f:	lea    0x110(%rbp),%rcx
    180013666:	xor    %r9d,%r9d
    180013669:	mov    %rax,0x20(%rsp)
    18001366e:	xor    %r8d,%r8d
    180013671:	xor    %edx,%edx
    180013673:	call   *0x7e5f(%rip)        # 0x18001b4d8
    180013679:	mov    %rax,%rcx
-   18001367c:	lea    0xb9b5(%rip),%rdx        # 0x18001f038
+   18001367c:	lea    0xb9c5(%rip),%rdx        # 0x18001f048
    180013683:	call   *0x7e57(%rip)        # 0x18001b4e0
    180013689:	jmp    0x180013dc9
    18001368e:	cmpl   $0x3,0xd0(%rsi)
    180013695:	jne    0x1800136df
    180013697:	lea    0x78(%rsi),%rcx
    18001369b:	call   *0x7ed7(%rip)        # 0x18001b578
    1800136a1:	test   %al,%al
@@ -28497,15 +28497,15 @@
    1800136b0:	lea    0x110(%rbp),%rcx
    1800136b7:	xor    %r9d,%r9d
    1800136ba:	mov    %rax,0x20(%rsp)
    1800136bf:	xor    %r8d,%r8d
    1800136c2:	xor    %edx,%edx
    1800136c4:	call   *0x7e0e(%rip)        # 0x18001b4d8
    1800136ca:	mov    %rax,%rcx
-   1800136cd:	lea    0xb99c(%rip),%rdx        # 0x18001f070
+   1800136cd:	lea    0xb9ac(%rip),%rdx        # 0x18001f080
    1800136d4:	call   *0x7e06(%rip)        # 0x18001b4e0
    1800136da:	jmp    0x180013dc9
    1800136df:	mov    %rbx,0x338(%rsp)
    1800136e7:	lea    0x208(%rsi),%rdx
    1800136ee:	mov    %rdi,0x340(%rsp)
    1800136f6:	lea    0x58(%rsp),%rcx
    1800136fb:	mov    %r12,0x308(%rsp)
@@ -28520,15 +28520,15 @@
    18001372f:	test   %al,%al
    180013731:	jne    0x180013745
    180013733:	lea    0x1f8(%rsi),%rdx
    18001373a:	lea    0x58(%rsp),%rcx
    18001373f:	call   *0x811b(%rip)        # 0x18001b860
    180013745:	lea    0x68(%rsp),%rcx
    18001374a:	call   *0x7d10(%rip)        # 0x18001b460
-   180013750:	lea    0xa2a1(%rip),%rax        # 0x18001d9f8
+   180013750:	lea    0xa999(%rip),%rax        # 0x18001e0f0
    180013757:	mov    %r12,-0x28(%rbp)
    18001375b:	lea    -0x28(%rbp),%rdx
    18001375f:	mov    %rax,-0x20(%rbp)
    180013763:	lea    0x68(%rbp),%rcx
    180013767:	movq   $0xd,-0x18(%rbp)
    18001376f:	call   *0x7c5b(%rip)        # 0x18001b3d0
    180013775:	mov    %rax,%rdx
@@ -29047,15 +29047,15 @@
    1800140cc:	test   %al,%al
    1800140ce:	jne    0x1800140e2
    1800140d0:	lea    0x1f8(%rsi),%rdx
    1800140d7:	lea    0x58(%rsp),%rcx
    1800140dc:	call   *0x777e(%rip)        # 0x18001b860
    1800140e2:	lea    0x68(%rsp),%rcx
    1800140e7:	call   *0x7373(%rip)        # 0x18001b460
-   1800140ed:	lea    0xafe4(%rip),%rax        # 0x18001f0d8
+   1800140ed:	lea    0xaff4(%rip),%rax        # 0x18001f0e8
    1800140f4:	mov    %r12,-0x38(%rbp)
    1800140f8:	lea    -0x38(%rbp),%rdx
    1800140fc:	mov    %rax,-0x30(%rbp)
    180014100:	lea    0x48(%rbp),%rcx
    180014104:	movq   $0x12,-0x28(%rbp)
    18001410c:	call   *0x72be(%rip)        # 0x18001b3d0
    180014112:	mov    %rax,%rdx
@@ -29479,15 +29479,15 @@
    180014883:	mov    %rax,%rbx
    180014886:	call   *0x6e7c(%rip)        # 0x18001b708
    18001488c:	mov    %rax,%rcx
    18001488f:	lea    0x60(%rsp),%rdx
    180014894:	call   *0x6e8e(%rip)        # 0x18001b728
    18001489a:	mov    %rax,%rcx
    18001489d:	call   *0x6d0d(%rip)        # 0x18001b5b0
-   1800148a3:	lea    0xa856(%rip),%rdx        # 0x18001f100
+   1800148a3:	lea    0xa866(%rip),%rdx        # 0x18001f110
    1800148aa:	mov    %rbx,%rcx
    1800148ad:	mov    %rax,%r8
    1800148b0:	call   *0x6c2a(%rip)        # 0x18001b4e0
    1800148b6:	lea    0x60(%rsp),%rcx
    1800148bb:	call   *0x690f(%rip)        # 0x18001b1d0
    1800148c1:	lea    0x78(%rsp),%rcx
    1800148c6:	call   *0x697c(%rip)        # 0x18001b248
@@ -29502,15 +29502,15 @@
    1800148f8:	lea    -0xdbbf(%rip),%rax        # 0x180006d40
    1800148ff:	mov    %rax,0x50(%rsp)
    180014904:	call   0x18001932c
    180014909:	mov    0xd0(%rsp),%rcx
    180014911:	lea    -0x92f8(%rip),%rdx        # 0x18000b620
    180014918:	lea    0x50(%rsp),%r8
    18001491d:	mov    %rcx,0x10(%rax)
-   180014921:	lea    0x9148(%rip),%rcx        # 0x18001da70
+   180014921:	lea    0x9848(%rip),%rcx        # 0x18001e170
    180014928:	mov    %rcx,0x40(%rsp)
    18001492d:	lea    0x58(%rsp),%rcx
    180014932:	mov    %rdx,0x8(%rax)
    180014936:	mov    %rdi,%rdx
    180014939:	movq   $0x0,0x38(%rsp)
    180014942:	movl   $0x1,(%rax)
    180014948:	mov    0x8(%rbx),%r9
@@ -29554,39 +29554,39 @@
    1800149da:	mov    %rbx,%rdx
    1800149dd:	lea    0x208(%rsi),%rcx
    1800149e4:	call   *0x69ee(%rip)        # 0x18001b3d8
    1800149ea:	lea    0x20(%rsp),%r9
    1800149ef:	movq   $0x0,0x20(%rsp)
    1800149f8:	xor    %r8d,%r8d
    1800149fb:	mov    %rbx,0x28(%rsp)
-   180014a00:	lea    0xa429(%rip),%rdx        # 0x18001ee30
+   180014a00:	lea    0xa439(%rip),%rdx        # 0x18001ee40
    180014a07:	mov    %rdi,%rcx
    180014a0a:	call   *0x6818(%rip)        # 0x18001b228
    180014a10:	mov    0x40(%rsp),%rbx
    180014a15:	mov    0x48(%rsp),%rsi
    180014a1a:	add    $0x30,%rsp
    180014a1e:	pop    %rdi
    180014a1f:	ret
    180014a20:	rex push %rbx
    180014a22:	sub    $0x30,%rsp
    180014a26:	mov    %r9d,0x20(%rsp)
    180014a2b:	mov    %rcx,%rbx
    180014a2e:	mov    %r8,%r9
    180014a31:	mov    %rdx,%r8
    180014a34:	mov    %rcx,%rdx
-   180014a37:	lea    0xa3f2(%rip),%rcx        # 0x18001ee30
+   180014a37:	lea    0xa402(%rip),%rcx        # 0x18001ee40
    180014a3e:	call   *0x67dc(%rip)        # 0x18001b220
    180014a44:	mov    %rbx,%rax
    180014a47:	add    $0x30,%rsp
    180014a4b:	pop    %rbx
    180014a4c:	ret
    180014a4d:	int3
    180014a4e:	int3
    180014a4f:	int3
-   180014a50:	lea    0xa749(%rip),%rax        # 0x18001f1a0
+   180014a50:	lea    0xa759(%rip),%rax        # 0x18001f1b0
    180014a57:	ret
    180014a58:	int3
    180014a59:	int3
    180014a5a:	int3
    180014a5b:	int3
    180014a5c:	int3
    180014a5d:	int3
@@ -29601,29 +29601,29 @@
    180014a79:	xor    %r8d,%r8d
    180014a7c:	lea    0x38(%rsp),%rdx
    180014a81:	xor    %r9d,%r9d
    180014a84:	mov    %rbx,%rcx
    180014a87:	call   0x180015140
    180014a8c:	lea    0x38(%rsp),%rcx
    180014a91:	call   *0x6d81(%rip)        # 0x18001b818
-   180014a97:	lea    0xa74a(%rip),%rax        # 0x18001f1e8
+   180014a97:	lea    0xa75a(%rip),%rax        # 0x18001f1f8
    180014a9e:	mov    %rax,(%rbx)
    180014aa1:	add    $0x20,%rsp
    180014aa5:	pop    %rbx
    180014aa6:	ret
    180014aa7:	int3
    180014aa8:	int3
    180014aa9:	int3
    180014aaa:	int3
    180014aab:	int3
    180014aac:	int3
    180014aad:	int3
    180014aae:	int3
    180014aaf:	int3
-   180014ab0:	lea    0xa969(%rip),%rax        # 0x18001f420
+   180014ab0:	lea    0xa979(%rip),%rax        # 0x18001f430
    180014ab7:	ret
    180014ab8:	int3
    180014ab9:	int3
    180014aba:	int3
    180014abb:	int3
    180014abc:	int3
    180014abd:	int3
@@ -30149,26 +30149,26 @@
    18001514c:	push   %r14
    18001514e:	sub    $0x60,%rsp
    180015152:	mov    %rdx,%rbp
    180015155:	movzwl %r8w,%esi
    180015159:	mov    %r9,%rdx
    18001515c:	mov    %rcx,%r14
    18001515f:	call   0x180018200
-   180015164:	lea    0xa07d(%rip),%rax        # 0x18001f1e8
+   180015164:	lea    0xa08d(%rip),%rax        # 0x18001f1f8
    18001516b:	mov    $0x58,%ecx
    180015170:	mov    %rax,(%r14)
    180015173:	call   0x18001932c
    180015178:	xor    %edx,%edx
    18001517a:	mov    %rax,%rcx
    18001517d:	mov    %rax,%rdi
    180015180:	call   *0x668a(%rip)        # 0x18001b810
    180015186:	lea    0x10(%rdi),%rcx
    18001518a:	mov    $0xffffffff,%r9d
    180015190:	xor    %r8d,%r8d
-   180015193:	lea    0xa0b6(%rip),%rdx        # 0x18001f250
+   180015193:	lea    0xa0c6(%rip),%rdx        # 0x18001f260
    18001519a:	call   *0x5fc8(%rip)        # 0x18001b168
    1800151a0:	lea    0x28(%rdi),%rcx
    1800151a4:	mov    $0x2,%edx
    1800151a9:	call   *0x6671(%rip)        # 0x18001b820
    1800151af:	lea    0x30(%rdi),%rcx
    1800151b3:	call   *0x607f(%rip)        # 0x18001b238
    1800151b9:	mov    0x6620(%rip),%rax        # 0x18001b7e0
@@ -30224,15 +30224,15 @@
    18001529b:	lea    0x30(%rsp),%rdx
    1800152a0:	movzwl %di,%r8d
    1800152a4:	mov    %rsi,%rcx
    1800152a7:	call   0x180015140
    1800152ac:	lea    0x30(%rsp),%rcx
    1800152b1:	call   *0x6561(%rip)        # 0x18001b818
    1800152b7:	mov    0x38(%rsp),%rbx
-   1800152bc:	lea    0x9f25(%rip),%rax        # 0x18001f1e8
+   1800152bc:	lea    0x9f35(%rip),%rax        # 0x18001f1f8
    1800152c3:	mov    %rax,(%rsi)
    1800152c6:	mov    %rsi,%rax
    1800152c9:	mov    0x40(%rsp),%rsi
    1800152ce:	add    $0x20,%rsp
    1800152d2:	pop    %rdi
    1800152d3:	ret
    1800152d4:	int3
@@ -30259,15 +30259,15 @@
    180015303:	lea    0x30(%rsp),%rdx
    180015308:	mov    %rbx,%r9
    18001530b:	mov    %rdi,%rcx
    18001530e:	call   0x180015140
    180015313:	lea    0x30(%rsp),%rcx
    180015318:	call   *0x64fa(%rip)        # 0x18001b818
    18001531e:	mov    0x38(%rsp),%rbx
-   180015323:	lea    0x9ebe(%rip),%rax        # 0x18001f1e8
+   180015323:	lea    0x9ece(%rip),%rax        # 0x18001f1f8
    18001532a:	mov    %rax,(%rdi)
    18001532d:	mov    %rdi,%rax
    180015330:	add    $0x20,%rsp
    180015334:	pop    %rdi
    180015335:	ret
    180015336:	int3
    180015337:	int3
@@ -30376,15 +30376,15 @@
    18001548b:	ret
    18001548c:	int3
    18001548d:	int3
    18001548e:	int3
    18001548f:	int3
    180015490:	rex push %rbx
    180015492:	sub    $0x20,%rsp
-   180015496:	lea    0x9d4b(%rip),%rax        # 0x18001f1e8
+   180015496:	lea    0x9d5b(%rip),%rax        # 0x18001f1f8
    18001549d:	mov    %rcx,%rbx
    1800154a0:	mov    %rax,(%rcx)
    1800154a3:	add    $0x10,%rcx
    1800154a7:	call   0x180015420
    1800154ac:	mov    %rbx,%rcx
    1800154af:	add    $0x20,%rsp
    1800154b3:	pop    %rbx
@@ -30673,15 +30673,15 @@
    1800158ae:	mov    -0x8(%rcx),%rdi
    1800158b2:	mov    %r14,0x38(%rsp)
    1800158b7:	lea    -0x8(%rcx),%r14
    1800158bb:	lea    (%rdi,%rdi,2),%rax
    1800158bf:	lea    (%rcx,%rax,8),%rbx
    1800158c3:	test   %rdi,%rdi
    1800158c6:	je     0x1800158ee
-   1800158c8:	lea    0x9919(%rip),%rsi        # 0x18001f1e8
+   1800158c8:	lea    0x9929(%rip),%rsi        # 0x18001f1f8
    1800158cf:	nop
    1800158d0:	sub    $0x18,%rbx
    1800158d4:	lea    0x10(%rbx),%rcx
    1800158d8:	mov    %rsi,(%rbx)
    1800158db:	call   0x180015420
    1800158e0:	mov    %rbx,%rcx
    1800158e3:	call   0x180008400
@@ -30698,15 +30698,15 @@
    180015910:	mov    %r14,%rax
    180015913:	mov    0x38(%rsp),%r14
    180015918:	mov    0x40(%rsp),%rbx
    18001591d:	mov    0x48(%rsp),%rbp
    180015922:	add    $0x20,%rsp
    180015926:	pop    %rsi
    180015927:	ret
-   180015928:	lea    0x98b9(%rip),%rsi        # 0x18001f1e8
+   180015928:	lea    0x98c9(%rip),%rsi        # 0x18001f1f8
    18001592f:	mov    %rsi,(%rcx)
    180015932:	add    $0x10,%rcx
    180015936:	call   0x180015420
    18001593b:	mov    %rbx,%rcx
    18001593e:	call   0x180008400
    180015943:	test   $0x1,%bpl
    180015947:	je     0x180015956
@@ -30751,15 +30751,15 @@
    1800159cc:	mov    %r14,%rcx
    1800159cf:	mov    %rax,0x50(%rsp)
    1800159d4:	call   *0x5796(%rip)        # 0x18001b170
    1800159da:	mov    0x40(%rbx),%rdx
    1800159de:	lea    0x30(%rbx),%rsi
    1800159e2:	mov    %rax,%r15
    1800159e5:	movq   $0x1,0x90(%rbp)
-   1800159f0:	lea    0x98d1(%rip),%rax        # 0x18001f2c8
+   1800159f0:	lea    0x98e1(%rip),%rax        # 0x18001f2d8
    1800159f7:	inc    %rdx
    1800159fa:	xor    %r8d,%r8d
    1800159fd:	mov    %rax,0x98(%rbp)
    180015a04:	lea    0x48(%rbp),%rcx
    180015a08:	call   *0x577a(%rip)        # 0x18001b188
    180015a0e:	lea    0x48(%rbp),%rcx
    180015a12:	call   *0x5be8(%rip)        # 0x18001b600
@@ -30813,15 +30813,15 @@
    180015ae8:	mov    %rax,%rbx
    180015aeb:	call   *0x5c17(%rip)        # 0x18001b708
    180015af1:	mov    %rax,%rcx
    180015af4:	lea    0xe0(%rbp),%rdx
    180015afb:	call   *0x5c27(%rip)        # 0x18001b728
    180015b01:	mov    %rax,%rcx
    180015b04:	call   *0x5aa6(%rip)        # 0x18001b5b0
-   180015b0a:	lea    0x97bf(%rip),%rdx        # 0x18001f2d0
+   180015b0a:	lea    0x97cf(%rip),%rdx        # 0x18001f2e0
    180015b11:	mov    %rbx,%rcx
    180015b14:	mov    %rax,%r8
    180015b17:	call   *0x59c3(%rip)        # 0x18001b4e0
    180015b1d:	lea    0xe0(%rbp),%rcx
    180015b24:	call   *0x56a6(%rip)        # 0x18001b1d0
    180015b2a:	lea    0x48(%rbp),%rcx
    180015b2e:	call   *0x5714(%rip)        # 0x18001b248
@@ -31119,15 +31119,15 @@
    180015ff3:	add    $0x30,%rdi
    180015ff7:	lea    0x1(%r12),%r15d
    180015ffc:	cmp    %rsi,%rdi
    180015fff:	jne    0x180015be5
    180016005:	mov    0x50(%rsp),%rcx
    18001600a:	lea    0x30(%rsp),%rdx
    18001600f:	call   0x180003b40
-   180016014:	lea    0x92cd(%rip),%rax        # 0x18001f2e8
+   180016014:	lea    0x92dd(%rip),%rax        # 0x18001f2f8
    18001601b:	mov    %r15,-0x18(%rbp)
    18001601f:	lea    -0x18(%rbp),%rdx
    180016023:	mov    %rax,-0x10(%rbp)
    180016027:	lea    0x1d0(%rbp),%rcx
    18001602e:	movq   $0xe,-0x8(%rbp)
    180016036:	call   *0x5774(%rip)        # 0x18001b7b0
    18001603c:	mov    0x40(%rsp),%rcx
@@ -31135,30 +31135,30 @@
    180016048:	add    $0x10,%rcx
    18001604c:	mov    %rax,%r14
    18001604f:	call   *0x54ab(%rip)        # 0x18001b500
    180016055:	lea    -0x30(%rbp),%rdx
    180016059:	mov    %r15,-0x30(%rbp)
    18001605d:	mov    %rax,%rsi
    180016060:	movq   $0x15,-0x20(%rbp)
-   180016068:	lea    0x9289(%rip),%rax        # 0x18001f2f8
+   180016068:	lea    0x9299(%rip),%rax        # 0x18001f308
    18001606f:	lea    0x1a0(%rbp),%rcx
    180016076:	mov    %rax,-0x28(%rbp)
    18001607a:	call   *0x5730(%rip)        # 0x18001b7b0
    180016080:	mov    %rax,%rdi
    180016083:	call   *0x50b7(%rip)        # 0x18001b140
    180016089:	lea    0x188(%rbp),%rcx
    180016090:	call   *0x50b2(%rip)        # 0x18001b148
    180016096:	mov    %rax,%rcx
    180016099:	lea    0x170(%rbp),%rdx
    1800160a0:	call   *0x5322(%rip)        # 0x18001b3c8
    1800160a6:	lea    -0x48(%rbp),%rdx
    1800160aa:	mov    %r15,-0x48(%rbp)
    1800160ae:	mov    %rax,%rbx
    1800160b1:	movq   $0x13,-0x38(%rbp)
-   1800160b9:	lea    0x9250(%rip),%rax        # 0x18001f310
+   1800160b9:	lea    0x9260(%rip),%rax        # 0x18001f320
    1800160c0:	lea    0x158(%rbp),%rcx
    1800160c7:	mov    %rax,-0x40(%rbp)
    1800160cb:	call   *0x56df(%rip)        # 0x18001b7b0
    1800160d1:	mov    %r14,%rcx
    1800160d4:	mov    %rbx,0xa8(%rbp)
    1800160db:	mov    %rax,0xa0(%rbp)
    1800160e2:	lea    0xa0(%rbp),%rax
@@ -31251,26 +31251,26 @@
    18001624e:	call   *0x5154(%rip)        # 0x18001b3a8
    180016254:	lea    0x30(%rbp),%rcx
    180016258:	call   *0x4f9a(%rip)        # 0x18001b1f8
    18001625e:	mov    $0xa,%r8d
    180016264:	lea    0x120(%rbp),%rcx
    18001626b:	mov    %rax,%rdx
    18001626e:	call   *0x5534(%rip)        # 0x18001b7a8
-   180016274:	lea    0x90a9(%rip),%rax        # 0x18001f324
+   180016274:	lea    0x90b9(%rip),%rax        # 0x18001f334
    18001627b:	mov    %r15,0x18(%rbp)
    18001627f:	lea    0x18(%rbp),%rdx
    180016283:	mov    %rax,0x20(%rbp)
    180016287:	lea    0x200(%rbp),%rcx
    18001628e:	movq   $0x4,0x28(%rbp)
    180016296:	call   *0x5514(%rip)        # 0x18001b7b0
    18001629c:	lea    0x0(%rbp),%rdx
    1800162a0:	mov    %r15,0x0(%rbp)
    1800162a4:	mov    %rax,%rbx
    1800162a7:	movq   $0x4c,0x10(%rbp)
-   1800162af:	lea    0x907a(%rip),%rax        # 0x18001f330
+   1800162af:	lea    0x908a(%rip),%rax        # 0x18001f340
    1800162b6:	lea    0x1e8(%rbp),%rcx
    1800162bd:	mov    %rax,0x8(%rbp)
    1800162c1:	call   *0x54e9(%rip)        # 0x18001b7b0
    1800162c7:	lea    -0x58(%rbp),%rcx
    1800162cb:	mov    %rbx,0xd8(%rbp)
    1800162d2:	mov    %rax,0xc0(%rbp)
    1800162d9:	lea    0x120(%rbp),%rax
@@ -31465,15 +31465,15 @@
    1800165a1:	lea    0x30(%rsp),%rcx
    1800165a6:	xor    %r9d,%r9d
    1800165a9:	mov    %rax,0x20(%rsp)
    1800165ae:	xor    %r8d,%r8d
    1800165b1:	xor    %edx,%edx
    1800165b3:	call   *0x4f1f(%rip)        # 0x18001b4d8
    1800165b9:	mov    %rax,%rcx
-   1800165bc:	lea    0x8cc5(%rip),%rdx        # 0x18001f288
+   1800165bc:	lea    0x8cd5(%rip),%rdx        # 0x18001f298
    1800165c3:	call   *0x4f17(%rip)        # 0x18001b4e0
    1800165c9:	test   %bpl,%bpl
    1800165cc:	jne    0x1800166ff
    1800165d2:	cmpl   $0x1,0x4(%rbx)
    1800165d6:	jne    0x180016639
    1800165d8:	mov    0x78(%rsp),%rdx
    1800165dd:	mov    %rbx,%rcx
@@ -31492,15 +31492,15 @@
    180016608:	lea    0x30(%rsp),%rcx
    18001660d:	xor    %r9d,%r9d
    180016610:	mov    %rax,0x20(%rsp)
    180016615:	xor    %r8d,%r8d
    180016618:	xor    %edx,%edx
    18001661a:	call   *0x4eb8(%rip)        # 0x18001b4d8
    180016620:	mov    %rax,%rcx
-   180016623:	lea    0x8c6e(%rip),%rdx        # 0x18001f298
+   180016623:	lea    0x8c7e(%rip),%rdx        # 0x18001f2a8
    18001662a:	call   *0x4eb0(%rip)        # 0x18001b4e0
    180016630:	test   %bpl,%bpl
    180016633:	jne    0x1800166ff
    180016639:	cmpl   $0x2,0x4(%rbx)
    18001663d:	jne    0x18001669c
    18001663f:	mov    0x78(%rsp),%rdx
    180016644:	mov    %rbx,%rcx
@@ -31519,15 +31519,15 @@
    18001666f:	lea    0x30(%rsp),%rcx
    180016674:	xor    %r9d,%r9d
    180016677:	mov    %rax,0x20(%rsp)
    18001667c:	xor    %r8d,%r8d
    18001667f:	xor    %edx,%edx
    180016681:	call   *0x4e51(%rip)        # 0x18001b4d8
    180016687:	mov    %rax,%rcx
-   18001668a:	lea    0x8c17(%rip),%rdx        # 0x18001f2a8
+   18001668a:	lea    0x8c27(%rip),%rdx        # 0x18001f2b8
    180016691:	call   *0x4e49(%rip)        # 0x18001b4e0
    180016697:	test   %bpl,%bpl
    18001669a:	jne    0x1800166ff
    18001669c:	cmpl   $0x3,0x4(%rbx)
    1800166a0:	jne    0x180016716
    1800166a2:	mov    0x78(%rsp),%rdx
    1800166a7:	mov    %rbx,%rcx
@@ -31546,15 +31546,15 @@
    1800166d2:	lea    0x30(%rsp),%rcx
    1800166d7:	xor    %r9d,%r9d
    1800166da:	mov    %rax,0x20(%rsp)
    1800166df:	xor    %r8d,%r8d
    1800166e2:	xor    %edx,%edx
    1800166e4:	call   *0x4dee(%rip)        # 0x18001b4d8
    1800166ea:	mov    %rax,%rcx
-   1800166ed:	lea    0x8bc4(%rip),%rdx        # 0x18001f2b8
+   1800166ed:	lea    0x8bd4(%rip),%rdx        # 0x18001f2c8
    1800166f4:	call   *0x4de6(%rip)        # 0x18001b4e0
    1800166fa:	test   %bpl,%bpl
    1800166fd:	je     0x180016716
    1800166ff:	mov    0x78(%rsp),%rcx
    180016704:	mov    (%rcx),%rax
    180016707:	mov    0xf8(%rax),%rax
    18001670e:	call   *0x5374(%rip)        # 0x18001ba88
@@ -31586,15 +31586,15 @@
    18001675f:	int3
    180016760:	mov    %rbx,0x10(%rsp)
    180016765:	mov    %rbp,0x18(%rsp)
    18001676a:	mov    %rsi,0x20(%rsp)
    18001676f:	push   %rdi
    180016770:	sub    $0x90,%rsp
    180016777:	mov    0x10(%rcx),%rdi
-   18001677b:	lea    0x8c7e(%rip),%rbx        # 0x18001f400
+   18001677b:	lea    0x8c8e(%rip),%rbx        # 0x18001f410
    180016782:	mov    %rdx,%rsi
    180016785:	mov    %rbx,%rcx
    180016788:	mov    $0x17,%edx
    18001678d:	call   *0x4d55(%rip)        # 0x18001b4e8
    180016793:	mov    %rbx,0x38(%rsp)
    180016798:	lea    0x30(%rsp),%rdx
    18001679d:	mov    %rax,0x30(%rsp)
@@ -32423,15 +32423,15 @@
    18001732d:	int3
    18001732e:	int3
    18001732f:	int3
    180017330:	mov    0x8(%rcx),%rcx
    180017334:	cmpq   $0x0,0x38(%rcx)
    180017339:	je     0x180017342
    18001733b:	rex.W jmp *0x3fc6(%rip)        # 0x18001b308
-   180017342:	lea    0x7e57(%rip),%rax        # 0x18001f1a0
+   180017342:	lea    0x7e67(%rip),%rax        # 0x18001f1b0
    180017349:	ret
    18001734a:	int3
    18001734b:	int3
    18001734c:	int3
    18001734d:	int3
    18001734e:	int3
    18001734f:	int3
@@ -32456,15 +32456,15 @@
    18001736f:	int3
    180017370:	mov    %rdx,%r9
    180017373:	mov    %rcx,%r10
    180017376:	test   %rdx,%rdx
    180017379:	jne    0x18001737e
    18001737b:	xor    %eax,%eax
    18001737d:	ret
-   18001737e:	lea    0x7d93(%rip),%r8        # 0x18001f118
+   18001737e:	lea    0x7da3(%rip),%r8        # 0x18001f128
    180017385:	mov    %r9,%rax
    180017388:	sub    %r9,%r8
    18001738b:	nopl   0x0(%rax,%rax,1)
    180017390:	movzbl (%rax),%edx
    180017393:	movzbl (%rax,%r8,1),%ecx
    180017398:	sub    %ecx,%edx
    18001739a:	jne    0x1800173a3
@@ -32498,15 +32498,15 @@
    1800173d8:	mov    %rcx,%rbp
    1800173db:	mov    %rdx,%rcx
    1800173de:	mov    %rdx,%rdi
    1800173e1:	mov    0x98(%rax),%rax
    1800173e8:	call   *0x469a(%rip)        # 0x18001ba88
    1800173ee:	test   %rax,%rax
    1800173f1:	je     0x180017579
-   1800173f7:	lea    0x7fea(%rip),%r14        # 0x18001f3e8
+   1800173f7:	lea    0x7ffa(%rip),%r14        # 0x18001f3f8
    1800173fe:	mov    %r14,0x28(%rsp)
    180017403:	lea    0xa8(%rsp),%rdx
    18001740b:	mov    %rdi,%rcx
    18001740e:	call   *0x3d44(%rip)        # 0x18001b158
    180017414:	movzbl 0xa8(%rsp),%edx
    18001741c:	lea    0x8(%rbp),%rcx
    180017420:	call   *0x3f92(%rip)        # 0x18001b3b8
@@ -32658,15 +32658,15 @@
    180017674:	mov    %ebx,%eax
    180017676:	jmp    0x180017682
    180017678:	lea    0x8(%rbp),%rcx
    18001767c:	call   *0x3b66(%rip)        # 0x18001b1e8
    180017682:	cmp    $0x4,%rsi
    180017686:	jne    0x1800176aa
    180017688:	mov    %rsi,%r8
-   18001768b:	lea    0x750e(%rip),%rdx        # 0x18001eba0
+   18001768b:	lea    0x751e(%rip),%rdx        # 0x18001ebb0
    180017692:	mov    %rax,%rcx
    180017695:	call   0x18001a42c
    18001769a:	test   %eax,%eax
    18001769c:	jne    0x1800176aa
    18001769e:	movl   $0x1,0x20(%rbp)
    1800176a5:	jmp    0x180017836
    1800176aa:	lea    0x8(%rbp),%rcx
@@ -32679,15 +32679,15 @@
    1800176c5:	mov    %rbx,%rax
    1800176c8:	jmp    0x1800176d4
    1800176ca:	lea    0x8(%rbp),%rcx
    1800176ce:	call   *0x3b14(%rip)        # 0x18001b1e8
    1800176d4:	cmp    $0x3,%rsi
    1800176d8:	jne    0x1800176fc
    1800176da:	mov    %rsi,%r8
-   1800176dd:	lea    0x74c4(%rip),%rdx        # 0x18001eba8
+   1800176dd:	lea    0x74d4(%rip),%rdx        # 0x18001ebb8
    1800176e4:	mov    %rax,%rcx
    1800176e7:	call   0x18001a42c
    1800176ec:	test   %eax,%eax
    1800176ee:	jne    0x1800176fc
    1800176f0:	movl   $0x2,0x20(%rbp)
    1800176f7:	jmp    0x180017836
    1800176fc:	lea    0x8(%rbp),%rcx
@@ -32700,15 +32700,15 @@
    180017717:	mov    %rbx,%rax
    18001771a:	jmp    0x180017726
    18001771c:	lea    0x8(%rbp),%rcx
    180017720:	call   *0x3ac2(%rip)        # 0x18001b1e8
    180017726:	cmp    $0x3,%rsi
    18001772a:	jne    0x18001774a
    18001772c:	mov    %rsi,%r8
-   18001772f:	lea    0x7476(%rip),%rdx        # 0x18001ebac
+   18001772f:	lea    0x7486(%rip),%rdx        # 0x18001ebbc
    180017736:	mov    %rax,%rcx
    180017739:	call   0x18001a42c
    18001773e:	test   %eax,%eax
    180017740:	jne    0x18001774a
    180017742:	mov    %esi,0x20(%rbp)
    180017745:	jmp    0x180017836
    18001774a:	lea    0x8(%rbp),%rcx
@@ -32721,15 +32721,15 @@
    180017765:	mov    %rbx,%rax
    180017768:	jmp    0x180017774
    18001776a:	lea    0x8(%rbp),%rcx
    18001776e:	call   *0x3a74(%rip)        # 0x18001b1e8
    180017774:	cmp    $0x4,%rsi
    180017778:	jne    0x180017798
    18001777a:	mov    %rsi,%r8
-   18001777d:	lea    0x7320(%rip),%rdx        # 0x18001eaa4
+   18001777d:	lea    0x7330(%rip),%rdx        # 0x18001eab4
    180017784:	mov    %rax,%rcx
    180017787:	call   0x18001a42c
    18001778c:	test   %eax,%eax
    18001778e:	jne    0x180017798
    180017790:	mov    %esi,0x20(%rbp)
    180017793:	jmp    0x180017836
    180017798:	lea    0x8(%rbp),%rcx
@@ -32741,15 +32741,15 @@
    1800177b1:	jne    0x1800177c0
    1800177b3:	lea    0x8(%rbp),%rcx
    1800177b7:	call   *0x3a2b(%rip)        # 0x18001b1e8
    1800177bd:	mov    %rax,%rbx
    1800177c0:	cmp    $0x6,%rsi
    1800177c4:	jne    0x1800177e5
    1800177c6:	mov    %rsi,%r8
-   1800177c9:	lea    0x73e0(%rip),%rdx        # 0x18001ebb0
+   1800177c9:	lea    0x73f0(%rip),%rdx        # 0x18001ebc0
    1800177d0:	mov    %rbx,%rcx
    1800177d3:	call   0x18001a42c
    1800177d8:	test   %eax,%eax
    1800177da:	jne    0x1800177e5
    1800177dc:	movl   $0x5,0x20(%rbp)
    1800177e3:	jmp    0x180017836
    1800177e5:	call   0x1800084e0
@@ -32764,15 +32764,15 @@
    180017806:	mov    %rax,0x20(%rsp)
    18001780b:	xor    %r8d,%r8d
    18001780e:	xor    %edx,%edx
    180017810:	call   *0x3cc2(%rip)        # 0x18001b4d8
    180017816:	lea    0x8(%rbp),%rcx
    18001781a:	mov    %rax,%rbx
    18001781d:	call   *0x3eb5(%rip)        # 0x18001b6d8
-   180017823:	lea    0x7b56(%rip),%rdx        # 0x18001f380
+   180017823:	lea    0x7b66(%rip),%rdx        # 0x18001f390
    18001782a:	mov    %rbx,%rcx
    18001782d:	mov    %rax,%r8
    180017830:	call   *0x3caa(%rip)        # 0x18001b4e0
    180017836:	lea    0x8(%rbp),%rcx
    18001783a:	movl   $0x1,0x4(%rbp)
    180017841:	call   *0x3f21(%rip)        # 0x18001b768
    180017847:	cmpl   $0x0,0x20(%rbp)
@@ -32806,15 +32806,15 @@
    18001788b:	mov    %rdx,%rsi
    18001788e:	xor    %bl,%bl
    180017890:	mov    0x98(%rax),%rax
    180017897:	call   *0x41eb(%rip)        # 0x18001ba88
    18001789d:	test   %rax,%rax
    1800178a0:	je     0x1800179e4
    1800178a6:	lea    0x8(%rbp),%rdi
-   1800178aa:	lea    0x7b37(%rip),%r14        # 0x18001f3e8
+   1800178aa:	lea    0x7b47(%rip),%r14        # 0x18001f3f8
    1800178b1:	test   %bl,%bl
    1800178b3:	jne    0x180017950
    1800178b9:	lea    0x88(%rsp),%rdx
    1800178c1:	mov    %rsi,%rcx
    1800178c4:	call   *0x388e(%rip)        # 0x18001b158
    1800178ca:	movzbl 0x88(%rsp),%edx
    1800178d2:	lea    0x8(%rbp),%rdi
@@ -32901,15 +32901,15 @@
    180017a14:	lea    0x40(%rsp),%rcx
    180017a19:	xor    %r9d,%r9d
    180017a1c:	mov    %rax,0x20(%rsp)
    180017a21:	xor    %r8d,%r8d
    180017a24:	xor    %edx,%edx
    180017a26:	call   *0x3aac(%rip)        # 0x18001b4d8
    180017a2c:	mov    %rax,%rcx
-   180017a2f:	lea    0x79ba(%rip),%rdx        # 0x18001f3f0
+   180017a2f:	lea    0x79ca(%rip),%rdx        # 0x18001f400
    180017a36:	call   *0x3aa4(%rip)        # 0x18001b4e0
    180017a3c:	xor    %al,%al
    180017a3e:	jmp    0x1800179e6
    180017a40:	rex push %rbp
    180017a42:	push   %rbx
    180017a43:	push   %rsi
    180017a44:	push   %rdi
@@ -32942,15 +32942,15 @@
    180017aac:	mov    %rbx,%rcx
    180017aaf:	mov    0x98(%rax),%rax
    180017ab6:	call   *0x3fcc(%rip)        # 0x18001ba88
    180017abc:	test   %rax,%rax
    180017abf:	jne    0x180017a76
    180017ac1:	test   %dil,%dil
    180017ac4:	je     0x180017db0
-   180017aca:	lea    0x77f7(%rip),%rbx        # 0x18001f2c8
+   180017aca:	lea    0x7807(%rip),%rbx        # 0x18001f2d8
    180017ad1:	mov    $0x2,%edx
    180017ad6:	mov    %rbx,%rcx
    180017ad9:	call   *0x3a09(%rip)        # 0x18001b4e8
    180017adf:	mov    %rbx,0x68(%rsp)
    180017ae4:	lea    -0x60(%rbp),%rdx
    180017ae8:	mov    %rax,0x60(%rsp)
    180017aed:	lea    0x8(%rsi),%rcx
@@ -32971,15 +32971,15 @@
    180017b29:	mov    %rax,0x20(%rsp)
    180017b2e:	xor    %r8d,%r8d
    180017b31:	xor    %edx,%edx
    180017b33:	call   *0x399f(%rip)        # 0x18001b4d8
    180017b39:	lea    0x8(%rsi),%rcx
    180017b3d:	mov    %rax,%rbx
    180017b40:	call   *0x3a6a(%rip)        # 0x18001b5b0
-   180017b46:	lea    0x784b(%rip),%rdx        # 0x18001f398
+   180017b46:	lea    0x785b(%rip),%rdx        # 0x18001f3a8
    180017b4d:	mov    %rbx,%rcx
    180017b50:	mov    %rax,%r8
    180017b53:	call   *0x3987(%rip)        # 0x18001b4e0
    180017b59:	xor    %al,%al
    180017b5b:	add    $0x118,%rsp
    180017b62:	pop    %rdi
    180017b63:	pop    %rsi
@@ -33010,15 +33010,15 @@
    180017bcd:	lea    -0x40(%rbp),%rcx
    180017bd1:	mov    $0xa,%r8d
    180017bd7:	call   *0x35b3(%rip)        # 0x18001b190
    180017bdd:	lea    0x30(%rsp),%rdx
    180017be2:	movq   $0x0,0x30(%rsp)
    180017beb:	mov    %rax,%r13
    180017bee:	movq   $0x11,0x40(%rsp)
-   180017bf7:	lea    0x77b2(%rip),%rax        # 0x18001f3b0
+   180017bf7:	lea    0x77c2(%rip),%rax        # 0x18001f3c0
    180017bfe:	lea    -0x20(%rbp),%rcx
    180017c02:	mov    %rax,0x38(%rsp)
    180017c07:	call   *0x37c3(%rip)        # 0x18001b3d0
    180017c0d:	mov    0x10(%r13),%rdx
    180017c11:	lea    -0x80(%rbp),%rcx
    180017c15:	xor    %r8d,%r8d
    180017c18:	mov    %rax,0x50(%rbp)
@@ -33104,15 +33104,15 @@
    180017d68:	mov    %rax,0x20(%rsp)
    180017d6d:	xor    %r8d,%r8d
    180017d70:	xor    %edx,%edx
    180017d72:	call   *0x3760(%rip)        # 0x18001b4d8
    180017d78:	lea    0x8(%rsi),%rcx
    180017d7c:	mov    %rax,%rbx
    180017d7f:	call   *0x382b(%rip)        # 0x18001b5b0
-   180017d85:	lea    0x764c(%rip),%rdx        # 0x18001f3d8
+   180017d85:	lea    0x765c(%rip),%rdx        # 0x18001f3e8
    180017d8c:	mov    %rbx,%rcx
    180017d8f:	mov    %rax,%r8
    180017d92:	call   *0x3748(%rip)        # 0x18001b4e0
    180017d98:	xor    %al,%al
    180017d9a:	add    $0x118,%rsp
    180017da1:	pop    %rdi
    180017da2:	pop    %rsi
@@ -33392,15 +33392,15 @@
    1800181cf:	int3
    1800181d0:	rex push %rbx
    1800181d2:	sub    $0x20,%rsp
    1800181d6:	mov    %rdx,%rbx
    1800181d9:	xor    %edx,%edx
    1800181db:	mov    %rbx,%rcx
    1800181de:	call   0x1800083d0
-   1800181e3:	lea    0x72fe(%rip),%rax        # 0x18001f4e8
+   1800181e3:	lea    0x730e(%rip),%rax        # 0x18001f4f8
    1800181ea:	mov    %rax,(%rbx)
    1800181ed:	add    $0x20,%rsp
    1800181f1:	pop    %rbx
    1800181f2:	ret
    1800181f3:	int3
    1800181f4:	int3
    1800181f5:	int3
@@ -33414,15 +33414,15 @@
    1800181fd:	int3
    1800181fe:	int3
    1800181ff:	int3
    180018200:	rex push %rbx
    180018202:	sub    $0x20,%rsp
    180018206:	mov    %rcx,%rbx
    180018209:	call   0x1800083d0
-   18001820e:	lea    0x72d3(%rip),%rax        # 0x18001f4e8
+   18001820e:	lea    0x72e3(%rip),%rax        # 0x18001f4f8
    180018215:	mov    %rax,(%rbx)
    180018218:	mov    %rbx,%rax
    18001821b:	add    $0x20,%rsp
    18001821f:	pop    %rbx
    180018220:	ret
    180018221:	int3
    180018222:	int3
@@ -33502,15 +33502,15 @@
    1800182ed:	int3
    1800182ee:	int3
    1800182ef:	int3
    1800182f0:	rex push %rbx
    1800182f2:	sub    $0x40,%rsp
    1800182f6:	mov    %rdx,%rbx
    1800182f9:	movq   $0x0,0x20(%rsp)
-   180018302:	lea    0x7247(%rip),%rax        # 0x18001f550
+   180018302:	lea    0x7257(%rip),%rax        # 0x18001f560
    180018309:	movq   $0x3,0x30(%rsp)
    180018312:	mov    %rbx,%rcx
    180018315:	mov    %rax,0x28(%rsp)
    18001831a:	lea    0x20(%rsp),%rdx
    18001831f:	call   *0x30ab(%rip)        # 0x18001b3d0
    180018325:	mov    0x20(%rsp),%rcx
    18001832a:	test   %rcx,%rcx
@@ -33535,15 +33535,15 @@
    18001835d:	int3
    18001835e:	int3
    18001835f:	int3
    180018360:	mov    0x8(%rcx),%rcx
    180018364:	cmpq   $0x0,0x38(%rcx)
    180018369:	je     0x180018372
    18001836b:	rex.W jmp *0x2f96(%rip)        # 0x18001b308
-   180018372:	lea    0x70a7(%rip),%rax        # 0x18001f420
+   180018372:	lea    0x70b7(%rip),%rax        # 0x18001f430
    180018379:	ret
    18001837a:	int3
    18001837b:	int3
    18001837c:	int3
    18001837d:	int3
    18001837e:	int3
    18001837f:	int3
@@ -33583,15 +33583,15 @@
    180018403:	mov    %rax,%rbx
    180018406:	call   *0x2ce4(%rip)        # 0x18001b0f0
    18001840c:	mov    %rax,%rcx
    18001840f:	lea    0x148(%rbp),%rdx
    180018416:	call   *0x330c(%rip)        # 0x18001b728
    18001841c:	mov    %rax,%rcx
    18001841f:	call   *0x318b(%rip)        # 0x18001b5b0
-   180018425:	lea    0x712c(%rip),%rdx        # 0x18001f558
+   180018425:	lea    0x713c(%rip),%rdx        # 0x18001f568
    18001842c:	mov    %rbx,%rcx
    18001842f:	mov    %rax,%r8
    180018432:	call   *0x30a8(%rip)        # 0x18001b4e0
    180018438:	lea    0x148(%rbp),%rcx
    18001843f:	call   *0x2d8b(%rip)        # 0x18001b1d0
    180018445:	lea    0x1c0(%rbp),%rcx
    18001844c:	call   *0x2df6(%rip)        # 0x18001b248
@@ -33617,27 +33617,27 @@
    1800184a4:	lea    0x50(%rbp),%rcx
    1800184a8:	xor    %r9d,%r9d
    1800184ab:	mov    %rax,0x20(%rsp)
    1800184b0:	xor    %r8d,%r8d
    1800184b3:	xor    %edx,%edx
    1800184b5:	call   *0x301d(%rip)        # 0x18001b4d8
    1800184bb:	mov    %rax,%rcx
-   1800184be:	lea    0x709b(%rip),%rdx        # 0x18001f560
+   1800184be:	lea    0x70ab(%rip),%rdx        # 0x18001f570
    1800184c5:	call   *0x3015(%rip)        # 0x18001b4e0
    1800184cb:	jmp    0x180018c14
    1800184d0:	mov    %rsi,0x370(%rsp)
    1800184d8:	lea    0x200(%rbp),%rdx
    1800184df:	xor    %r8d,%r8d
    1800184e2:	mov    %r12,0x378(%rsp)
    1800184ea:	mov    %r14,%rcx
    1800184ed:	call   *0x32cd(%rip)        # 0x18001b7c0
    1800184f3:	mov    %rax,%rcx
    1800184f6:	call   *0x2c34(%rip)        # 0x18001b130
    1800184fc:	mov    $0xffffffff,%esi
-   180018501:	lea    0x7078(%rip),%r12        # 0x18001f580
+   180018501:	lea    0x7088(%rip),%r12        # 0x18001f590
    180018508:	test   %al,%al
    18001850a:	je     0x18001856b
    18001850c:	lea    -0x78(%rbp),%rdx
    180018510:	mov    %rdi,-0x78(%rbp)
    180018514:	lea    0x70(%rbp),%rcx
    180018518:	mov    %r12,-0x70(%rbp)
    18001851c:	movq   $0x9,-0x68(%rbp)
@@ -33694,15 +33694,15 @@
    1800185ff:	lea    0x50(%rbp),%rcx
    180018603:	xor    %r9d,%r9d
    180018606:	mov    %rax,0x20(%rsp)
    18001860b:	xor    %r8d,%r8d
    18001860e:	xor    %edx,%edx
    180018610:	call   *0x2ec2(%rip)        # 0x18001b4d8
    180018616:	mov    %rax,%rcx
-   180018619:	lea    0x6f78(%rip),%rdx        # 0x18001f598
+   180018619:	lea    0x6f88(%rip),%rdx        # 0x18001f5a8
    180018620:	call   *0x2eba(%rip)        # 0x18001b4e0
    180018626:	jmp    0x180018bee
    18001862b:	lea    0x48(%rsp),%rdx
    180018630:	mov    %r15,%rcx
    180018633:	call   0x180004260
    180018638:	lea    -0x48(%rbp),%rdx
    18001863c:	mov    %rdi,0x30(%rsp)
@@ -33811,15 +33811,15 @@
    1800187e9:	call   *0x2be1(%rip)        # 0x18001b3d0
    1800187ef:	mov    $0x1,%r8d
    1800187f5:	lea    0x60(%rsp),%rcx
    1800187fa:	mov    %rax,%rdx
    1800187fd:	call   *0x2e15(%rip)        # 0x18001b618
    180018803:	test   %al,%al
    180018805:	jne    0x180018852
-   180018807:	lea    0x6da2(%rip),%rax        # 0x18001f5b0
+   180018807:	lea    0x6db2(%rip),%rax        # 0x18001f5c0
    18001880e:	mov    %rdi,-0x30(%rbp)
    180018812:	lea    -0x30(%rbp),%rdx
    180018816:	mov    %rax,-0x28(%rbp)
    18001881a:	lea    0xd0(%rbp),%rcx
    180018821:	movq   $0xf,-0x20(%rbp)
    180018829:	or     $0xc00,%ebx
    18001882f:	call   *0x2b9b(%rip)        # 0x18001b3d0
@@ -33902,15 +33902,15 @@
    180018965:	mov    %rdi,0x8(%rbp)
    180018969:	call   *0x2b99(%rip)        # 0x18001b508
    18001896f:	lea    0x100(%rbp),%rdx
    180018976:	lea    0x20(%rbp),%rcx
    18001897a:	call   *0x2da8(%rip)        # 0x18001b728
    180018980:	mov    %rax,%rcx
    180018983:	call   *0x2c27(%rip)        # 0x18001b5b0
-   180018989:	lea    0x6c40(%rip),%rdx        # 0x18001f5d0
+   180018989:	lea    0x6c50(%rip),%rdx        # 0x18001f5e0
    180018990:	mov    %rbx,%rcx
    180018993:	mov    %rax,%r8
    180018996:	call   *0x2b44(%rip)        # 0x18001b4e0
    18001899c:	lea    0x100(%rbp),%rcx
    1800189a3:	call   *0x2827(%rip)        # 0x18001b1d0
    1800189a9:	lea    0x20(%rbp),%rcx
    1800189ad:	call   *0x2895(%rip)        # 0x18001b248
@@ -33955,15 +33955,15 @@
    180018a59:	mov    %rax,0x18(%rbp)
    180018a5d:	call   *0x2aa5(%rip)        # 0x18001b508
    180018a63:	lea    0x118(%rbp),%rdx
    180018a6a:	lea    0x38(%rbp),%rcx
    180018a6e:	call   *0x2cb4(%rip)        # 0x18001b728
    180018a74:	mov    %rax,%rcx
    180018a77:	call   *0x2b33(%rip)        # 0x18001b5b0
-   180018a7d:	lea    0x6b74(%rip),%rdx        # 0x18001f5f8
+   180018a7d:	lea    0x6b84(%rip),%rdx        # 0x18001f608
    180018a84:	mov    %rbx,%rcx
    180018a87:	mov    %rax,%r8
    180018a8a:	call   *0x2a50(%rip)        # 0x18001b4e0
    180018a90:	lea    0x118(%rbp),%rcx
    180018a97:	call   *0x2733(%rip)        # 0x18001b1d0
    180018a9d:	lea    0x38(%rbp),%rcx
    180018aa1:	call   *0x27a1(%rip)        # 0x18001b248
@@ -34016,15 +34016,15 @@
    180018b61:	call   *0x2971(%rip)        # 0x18001b4d8
    180018b67:	lea    0x130(%rbp),%rdx
    180018b6e:	mov    %rax,%rbx
    180018b71:	lea    0x60(%rsp),%rcx
    180018b76:	call   *0x2aac(%rip)        # 0x18001b628
    180018b7c:	mov    %rax,%rcx
    180018b7f:	call   *0x2a2b(%rip)        # 0x18001b5b0
-   180018b85:	lea    0x6a8c(%rip),%rdx        # 0x18001f618
+   180018b85:	lea    0x6a9c(%rip),%rdx        # 0x18001f628
    180018b8c:	mov    %rbx,%rcx
    180018b8f:	mov    %rax,%r8
    180018b92:	call   *0x2948(%rip)        # 0x18001b4e0
    180018b98:	lea    0x130(%rbp),%rcx
    180018b9f:	call   *0x262b(%rip)        # 0x18001b1d0
    180018ba5:	mov    0x30(%rsp),%rax
    180018baa:	test   %rax,%rax
@@ -34446,15 +34446,15 @@
    1800191cf:	int3
    1800191d0:	mov    %rdx,%r9
    1800191d3:	mov    %rcx,%r10
    1800191d6:	test   %rdx,%rdx
    1800191d9:	jne    0x1800191de
    1800191db:	xor    %eax,%eax
    1800191dd:	ret
-   1800191de:	lea    0x6283(%rip),%r8        # 0x18001f468
+   1800191de:	lea    0x6293(%rip),%r8        # 0x18001f478
    1800191e5:	mov    %r9,%rax
    1800191e8:	sub    %r9,%r8
    1800191eb:	nopl   0x0(%rax,%rax,1)
    1800191f0:	movzbl (%rax),%edx
    1800191f3:	movzbl (%rax,%r8,1),%ecx
    1800191f8:	sub    %ecx,%edx
    1800191fa:	jne    0x180019203
@@ -34625,15 +34625,15 @@
    1800192fb:	int3
    1800192fc:	int3
    1800192fd:	int3
    1800192fe:	int3
    1800192ff:	int3
    180019300:	rex push %rbx
    180019302:	sub    $0x20,%rsp
-   180019306:	lea    0x6333(%rip),%rax        # 0x18001f640
+   180019306:	lea    0x6343(%rip),%rax        # 0x18001f650
    18001930d:	mov    %rcx,%rbx
    180019310:	mov    %rax,(%rcx)
    180019313:	test   $0x1,%dl
    180019316:	je     0x180019322
    180019318:	mov    $0x18,%edx
    18001931d:	call   0x180019368
    180019322:	mov    %rbx,%rax
@@ -34737,28 +34737,28 @@
    18001942f:	int3
    180019430:	mov    %rbx,0x8(%rsp)
    180019435:	push   %rdi
    180019436:	sub    $0x20,%rsp
    18001943a:	mov    $0xfa0,%edx
    18001943f:	lea    0x13f02(%rip),%rcx        # 0x18002d348
    180019446:	call   *0x1c6c(%rip)        # 0x18001b0b8
-   18001944c:	lea    0x61fd(%rip),%rcx        # 0x18001f650
+   18001944c:	lea    0x620d(%rip),%rcx        # 0x18001f660
    180019453:	call   *0x1c2f(%rip)        # 0x18001b088
    180019459:	mov    %rax,%rbx
    18001945c:	test   %rax,%rax
    18001945f:	jne    0x180019476
-   180019461:	lea    0x6230(%rip),%rcx        # 0x18001f698
+   180019461:	lea    0x6240(%rip),%rcx        # 0x18001f6a8
    180019468:	call   *0x1c1a(%rip)        # 0x18001b088
    18001946e:	mov    %rax,%rbx
    180019471:	test   %rax,%rax
    180019474:	je     0x1800194f5
-   180019476:	lea    0x623b(%rip),%rdx        # 0x18001f6b8
+   180019476:	lea    0x624b(%rip),%rdx        # 0x18001f6c8
    18001947d:	mov    %rbx,%rcx
    180019480:	call   *0x1bfa(%rip)        # 0x18001b080
-   180019486:	lea    0x624b(%rip),%rdx        # 0x18001f6d8
+   180019486:	lea    0x625b(%rip),%rdx        # 0x18001f6e8
    18001948d:	mov    %rbx,%rcx
    180019490:	mov    %rax,%rdi
    180019493:	call   *0x1be7(%rip)        # 0x18001b080
    180019499:	test   %rdi,%rdi
    18001949c:	je     0x1800194b3
    18001949e:	test   %rax,%rax
    1800194a1:	je     0x1800194b3
@@ -35038,15 +35038,15 @@
    180019881:	jne    0x180019893
    180019883:	lea    0x13b2e(%rip),%rcx        # 0x18002d3b8
    18001988a:	call   0x18001a488
    18001988f:	test   %eax,%eax
    180019891:	je     0x1800198c1
    180019893:	xor    %al,%al
    180019895:	jmp    0x1800198ca
-   180019897:	movdqa 0x5e61(%rip),%xmm0        # 0x18001f700
+   180019897:	movdqa 0x5e71(%rip),%xmm0        # 0x18001f710
    18001989f:	or     $0xffffffffffffffff,%rax
    1800198a3:	movdqu %xmm0,0x13af5(%rip)        # 0x18002d3a0
    1800198ab:	mov    %rax,0x13afe(%rip)        # 0x18002d3b0
    1800198b2:	movdqu %xmm0,0x13afe(%rip)        # 0x18002d3b8
    1800198ba:	mov    %rax,0x13b07(%rip)        # 0x18002d3c8
    1800198c1:	movb   $0x1,0x13ad1(%rip)        # 0x18002d399
    1800198c8:	mov    $0x1,%al
@@ -35323,15 +35323,15 @@
    180019c32:	cmp    %edx,0x13798(%rip)        # 0x18002d3d0
    180019c38:	jg     0x180019c41
    180019c3a:	xor    %eax,%eax
    180019c3c:	jmp    0x180019d2f
    180019c41:	lea    -0x1(%rdx),%eax
    180019c44:	cmp    $0x1,%eax
    180019c47:	ja     0x180019c8e
-   180019c49:	mov    0x5ac0(%rip),%rax        # 0x18001f710
+   180019c49:	mov    0x5ad0(%rip),%rax        # 0x18001f720
    180019c50:	test   %rax,%rax
    180019c53:	jne    0x180019c5f
    180019c55:	movl   $0x1,0x30(%rsp)
    180019c5d:	jmp    0x180019c73
    180019c5f:	call   *0x1e23(%rip)        # 0x18001ba88
    180019c65:	mov    %eax,%ebx
    180019c67:	mov    %eax,0x30(%rsp)
@@ -35358,15 +35358,15 @@
    180019caa:	mov    %rsi,%r8
    180019cad:	xor    %edx,%edx
    180019caf:	mov    %r14,%rcx
    180019cb2:	call   0x18001a328
    180019cb7:	test   %rsi,%rsi
    180019cba:	setne  %cl
    180019cbd:	call   0x180019b88
-   180019cc2:	mov    0x5a47(%rip),%rax        # 0x18001f710
+   180019cc2:	mov    0x5a57(%rip),%rax        # 0x18001f720
    180019cc9:	test   %rax,%rax
    180019ccc:	je     0x180019cdc
    180019cce:	mov    %rsi,%r8
    180019cd1:	xor    %edx,%edx
    180019cd3:	mov    %r14,%rcx
    180019cd6:	call   *0x1dac(%rip)        # 0x18001ba88
    180019cdc:	test   %edi,%edi
@@ -35377,15 +35377,15 @@
    180019ce8:	mov    %edi,%edx
    180019cea:	mov    %r14,%rcx
    180019ced:	call   0x180019a20
    180019cf2:	mov    %eax,%ebx
    180019cf4:	mov    %eax,0x30(%rsp)
    180019cf8:	test   %eax,%eax
    180019cfa:	je     0x180019d25
-   180019cfc:	mov    0x5a0d(%rip),%rax        # 0x18001f710
+   180019cfc:	mov    0x5a1d(%rip),%rax        # 0x18001f720
    180019d03:	test   %rax,%rax
    180019d06:	jne    0x180019d11
    180019d08:	lea    0x1(%rax),%ebx
    180019d0b:	mov    %ebx,0x30(%rsp)
    180019d0f:	jmp    0x180019d25
    180019d11:	mov    %rsi,%r8
    180019d14:	mov    %edi,%edx
@@ -35424,15 +35424,15 @@
    180019d73:	add    $0x20,%rsp
    180019d77:	pop    %rdi
    180019d78:	jmp    0x180019c0c
    180019d7d:	int3
    180019d7e:	int3
    180019d7f:	int3
    180019d80:	andq   $0x0,0x10(%rcx)
-   180019d85:	lea    0x598c(%rip),%rax        # 0x18001f718
+   180019d85:	lea    0x599c(%rip),%rax        # 0x18001f728
    180019d8c:	mov    %rax,0x8(%rcx)
    180019d90:	lea    0x38b9(%rip),%rax        # 0x18001d650
    180019d97:	mov    %rax,(%rcx)
    180019d9a:	mov    %rcx,%rax
    180019d9d:	ret
    180019d9e:	int3
    180019d9f:	int3
@@ -35505,15 +35505,15 @@
    180019ebc:	imul   $0x0,%rax,%rax
    180019ec0:	mov    0x11a61(%rip),%rcx        # 0x18002b928
    180019ec7:	mov    %rcx,0x20(%rsp,%rax,1)
    180019ecc:	mov    $0x8,%eax
    180019ed1:	imul   $0x1,%rax,%rax
    180019ed5:	mov    0x11a44(%rip),%rcx        # 0x18002b920
    180019edc:	mov    %rcx,0x20(%rsp,%rax,1)
-   180019ee1:	lea    0x5840(%rip),%rcx        # 0x18001f728
+   180019ee1:	lea    0x5850(%rip),%rcx        # 0x18001f738
    180019ee8:	call   0x180019de0
    180019eed:	add    $0x38,%rsp
    180019ef1:	ret
    180019ef2:	int3
    180019ef3:	int3
    180019ef4:	rex push %rbx
    180019ef6:	push   %rsi
@@ -35788,15 +35788,15 @@
    18001a31b:	mov    %rax,0x115fe(%rip)        # 0x18002b920
    18001a322:	add    $0x20,%rsp
    18001a326:	pop    %rbp
    18001a327:	ret
    18001a328:	sub    $0x28,%rsp
    18001a32c:	cmp    $0x1,%edx
    18001a32f:	jne    0x18001a341
-   18001a331:	cmpq   $0x0,0x53d7(%rip)        # 0x18001f710
+   18001a331:	cmpq   $0x0,0x53e7(%rip)        # 0x18001f720
    18001a339:	jne    0x18001a341
    18001a33b:	call   *0xccf(%rip)        # 0x18001b010
    18001a341:	mov    $0x1,%eax
    18001a346:	add    $0x28,%rsp
    18001a34a:	ret
    18001a34b:	int3
    18001a34c:	lea    0x1360d(%rip),%rcx        # 0x18002d960
@@ -37989,22 +37989,19 @@
    18001c17c:	add    (%rax),%ah
    18001c17e:	(bad)
    18001c17f:	add    %eax,(%rax)
    18001c181:	add    0xe(%rax),%dl
    18001c184:	add    %eax,(%rax)
    18001c186:	add    (%rax),%dl
    18001c188:	sgdt   (%rax)
-   18001c18b:	add    %ah,(%rax)
-   18001c18d:	sgdt   (%rax)
-   18001c190:	add    %dl,(%rax)
-   18001c192:	adc    %al,(%rcx)
-   18001c194:	add    %al,(%rax)
-   18001c196:	nop
-   18001c197:	adc    (%rcx),%al
-   18001c199:	add    %al,(%rdx)
+   18001c18b:	add    %dl,0xf(%rax)
+   18001c18e:	add    %eax,(%rax)
+   18001c190:	add    %ah,0xf(%rax)
+   18001c193:	add    %eax,(%rax)
+   18001c195:	add    %dl,0x2000112(%rax)
    18001c19b:	adc    %dl,(%rbx)
    18001c19d:	add    %eax,(%rax)
    18001c19f:	add    0x2000113(%rax),%dh
    18001c1a5:	push   %rax
    18001c1a6:	adc    $0x1,%al
    18001c1a8:	add    %al,(%rdx)
    18001c1aa:	mov    $0x14,%al
@@ -40230,2953 +40227,2944 @@
    18001d85c:	outsb  %ds:(%rsi),(%dx)
    18001d85d:	add    %ch,(%rdi)
    18001d85f:	add    %ch,0x0(%rdx)
    18001d862:	jae    0x18001d864
    18001d864:	outsl  %ds:(%rsi),(%dx)
    18001d865:	add    %ch,0x0(%rsi)
 	...
-   18001d870:	push   %rcx
-   18001d871:	rex.WRX
-   18001d872:	gs je  0x18001d8ec
-   18001d875:	outsl  %ds:(%rsi),(%dx)
-   18001d876:	jb     0x18001d8e3
-   18001d878:	push   %rdx
-   18001d879:	gs jo  0x18001d8e8
-   18001d87c:	jns    0x18001d8a8
+   18001d870:	or     (%rax),%eax
+	...
    18001d87e:	add    %al,(%rax)
-   18001d880:	push   %rcx
-   18001d881:	push   %rbx
-   18001d882:	jae    0x18001d8f0
-   18001d884:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001d886:	outsb  %ds:(%rsi),(%dx)
-   18001d887:	imul   $0x6172,0x75(%rdi),%sp
-   18001d88d:	je     0x18001d8f8
-   18001d88f:	outsl  %ds:(%rsi),(%dx)
-   18001d890:	outsb  %ds:(%rsi),(%dx)
-   18001d891:	add    %al,(%rax)
-   18001d893:	add    %al,(%rax)
-   18001d895:	add    %al,(%rax)
-   18001d897:	add    %dl,0x44(%rcx)
-   18001d89a:	(bad)
-   18001d89b:	je     0x18001d902
-   18001d89d:	push   %rsp
-   18001d89e:	imul   $0x0,0x65(%rbp),%ebp
+   18001d880:	sbb    (%rax),%al
+   18001d882:	add    %al,(%rax)
+   18001d884:	(bad)
+   18001d885:	add    %al,(%rax)
+   18001d887:	add    %al,(%rsi)
+   18001d889:	add    %al,(%rax)
+   18001d88b:	add    %dl,(%rax)
+   18001d88d:	add    %eax,(%rax)
+	...
+   18001d8a3:	add    %cl,(%rdx)
    18001d8a5:	add    %al,(%rax)
-   18001d8a7:	add    %dl,0x41(%rcx)
-   18001d8aa:	(bad)
-   18001d8af:	movsxd 0x41(%rdi,%rcx,2),%esi
-   18001d8b3:	jne    0x18001d929
-   18001d8b5:	push   $0x48510032
-   18001d8ba:	je     0x18001d930
-   18001d8bc:	jo     0x18001d90b
-   18001d8be:	jne    0x18001d92c
-   18001d8c0:	je     0x18001d92b
-   18001d8c2:	push   %rax
-   18001d8c3:	(bad)
-   18001d8c4:	jb     0x18001d93a
-   18001d8c6:	sub    (%rax),%al
-   18001d8c8:	push   %rcx
-   18001d8c9:	push   %rbx
-   18001d8ca:	jae    0x18001d938
-   18001d8cc:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001d8ce:	outsb  %ds:(%rsi),(%dx)
-   18001d8cf:	imul   $0x6172,0x75(%rdi),%sp
-   18001d8d5:	je     0x18001d940
-   18001d8d7:	outsl  %ds:(%rsi),(%dx)
-   18001d8d8:	outsb  %ds:(%rsi),(%dx)
+   18001d8a7:	add    %al,(%rcx)
+   18001d8a9:	add    %al,(%rax)
+   18001d8ab:	add    %al,(%rcx)
+   18001d8ad:	add    %al,(%rax)
+   18001d8af:	add    %ch,0x2000000(%rdx)
+   18001d8b5:	add    %al,(%rax)
+   18001d8b7:	add    %al,(%rsi)
+   18001d8b9:	add    %al,(%rax)
+   18001d8bb:	add    %al,(%rdi)
+   18001d8bd:	add    %al,(%rax)
+   18001d8bf:	add    %al,(%rax,%rax,1)
+   18001d8c2:	add    %al,(%rax)
+   18001d8c4:	add    %eax,(%rax)
+   18001d8c6:	add    %al,(%rax)
+   18001d8c8:	lods   %ds:(%rsi),%eax
+   18001d8c9:	add    %al,(%rax)
+   18001d8cb:	add    %al,(%rdx)
+   18001d8cd:	add    %al,(%rax)
+   18001d8cf:	add    %al,(%rsi)
+   18001d8d1:	add    %al,(%rax)
+   18001d8d3:	add    %cl,(%rcx)
+   18001d8d5:	add    %al,(%rax)
+   18001d8d7:	add    %al,(%rsi)
    18001d8d9:	add    %al,(%rax)
-   18001d8db:	add    %al,(%rax)
+   18001d8db:	add    %al,(%rcx)
    18001d8dd:	add    %al,(%rax)
-   18001d8df:	add    %ah,0x0(%rcx)
-   18001d8e2:	movsxd (%rax),%eax
-   18001d8e4:	movsxd (%rax),%eax
-   18001d8e6:	add    %dh,%gs:0x0(%rbx)
-   18001d8ea:	jae    0x18001d8ec
-   18001d8ec:	pop    %rdi
-   18001d8ed:	add    %dh,0x6f(%rax,%rax,1)
-   18001d8f1:	add    %ch,0x0(%rbx)
-   18001d8f4:	add    %ch,%gs:0x0(%rsi)
-	...
-   18001d900:	(bad)
-   18001d901:	add    %dh,0x0(%rax)
-   18001d904:	imul   $0x6b005f,(%rax),%eax
-   18001d90a:	add    %bh,%gs:0x0(%rcx)
-   18001d90e:	add    %al,(%rax)
-   18001d910:	movsxd (%rax),%eax
-   18001d912:	insb   (%dx),%es:(%rdi)
-   18001d913:	add    %ch,0x0(%rcx)
-   18001d916:	add    %ch,%gs:0x0(%rsi)
-   18001d91a:	je     0x18001d91c
-   18001d91c:	pop    %rdi
-   18001d91d:	add    %ch,0x0(%rcx)
-   18001d920:	add    %al,%fs:(%rax)
-   18001d923:	add    %al,(%rax)
-   18001d925:	add    %al,(%rax)
-   18001d927:	add    %ah,0x0(%rbx)
-   18001d92a:	insb   (%dx),%es:(%rdi)
-   18001d92b:	add    %ch,0x0(%rcx)
-   18001d92e:	add    %ch,%gs:0x0(%rsi)
-   18001d932:	je     0x18001d934
-   18001d934:	pop    %rdi
-   18001d935:	add    %dh,0x0(%rbx)
-   18001d938:	add    %ah,%gs:0x0(%rbx)
-   18001d93c:	jb     0x18001d93e
-   18001d93e:	add    %dh,%gs:0x0(%rax,%rax,1)
-   18001d943:	add    %al,(%rax)
-   18001d945:	add    %al,(%rax)
-   18001d947:	add    %ah,0x0(%rbx)
-   18001d94a:	outsl  %ds:(%rsi),(%dx)
-   18001d94b:	add    %ah,0x65(%rax,%rax,1)
-	...
-   18001d957:	add    %ah,0x0(%rbp)
-   18001d95a:	jb     0x18001d95c
-   18001d95c:	jb     0x18001d95e
-   18001d95e:	outsl  %ds:(%rsi),(%dx)
-   18001d95f:	add    %dh,0x0(%rdx)
-   18001d962:	add    %al,(%rax)
-   18001d964:	add    %al,(%rax)
-   18001d966:	add    %al,(%rax)
-   18001d968:	add    %dh,%gs:0x0(%rdx)
-   18001d96c:	jb     0x18001d96e
-   18001d96e:	outsl  %ds:(%rsi),(%dx)
-   18001d96f:	add    %dh,0x0(%rdx)
-   18001d972:	pop    %rdi
-   18001d973:	add    %ah,0x65(%rax,%rax,1)
-   18001d977:	add    %dh,0x0(%rbx)
-   18001d97a:	movsxd (%rax),%eax
-   18001d97c:	jb     0x18001d97e
-   18001d97e:	imul   $0x740070,(%rax),%eax
-   18001d984:	imul   $0x6e006f,(%rax),%eax
-   18001d98a:	add    %al,(%rax)
-   18001d98c:	add    %al,(%rax)
-   18001d98e:	add    %al,(%rax)
-   18001d990:	add    %dh,%gs:0x0(%rdx)
-   18001d994:	jb     0x18001d996
-   18001d996:	outsl  %ds:(%rsi),(%dx)
-   18001d997:	add    %dh,0x0(%rdx)
-   18001d99a:	pop    %rdi
-   18001d99b:	add    %dh,0x0(%rbp)
-   18001d99e:	jb     0x18001d9a0
-   18001d9a0:	imul   $0x0,(%rax),%eax
-   18001d9a6:	add    %al,(%rax)
-   18001d9a8:	add    %bh,%gs:0x0(%rax)
-   18001d9ac:	jo     0x18001d9ae
-   18001d9ae:	imul   $0x650072,(%rax),%eax
-   18001d9b4:	jae    0x18001d9b6
-   18001d9b6:	pop    %rdi
-   18001d9b7:	add    %ch,0x0(%rcx)
-   18001d9ba:	outsb  %ds:(%rsi),(%dx)
-   18001d9bb:	add    %al,(%rax)
+   18001d8df:	add    %dh,0x2000000(%rax)
+   18001d8e5:	add    %al,(%rax)
+   18001d8e7:	add    %al,(%rsi)
+   18001d8e9:	add    %al,(%rax)
+   18001d8eb:	add    %cl,(%rbx)
+   18001d8ed:	add    %al,(%rax)
+   18001d8ef:	add    %cl,(%rax)
+   18001d8f1:	add    %al,(%rax)
+   18001d8f3:	add    %al,(%rcx)
+   18001d8f5:	add    %al,(%rax)
+   18001d8f7:	add    %dh,0x2000000(%rbx)
+   18001d8fd:	add    %al,(%rax)
+   18001d8ff:	add    %al,(%rsi)
+   18001d901:	add    %al,(%rax)
+   18001d903:	add    %cl,0xa000000(%rip)        # 0x18a01d909
+   18001d909:	add    %al,(%rax)
+   18001d90b:	add    %al,(%rcx)
+   18001d90d:	add    %al,(%rax)
+   18001d90f:	add    %dh,0x2000000(%rsi)
+   18001d915:	add    %al,(%rax)
+   18001d917:	add    %al,(%rsi)
+   18001d919:	add    %al,(%rax)
+   18001d91b:	add    %cl,(%rdi)
+   18001d91d:	add    %al,(%rax)
+   18001d91f:	add    %cl,(%rax,%rax,1)
+   18001d922:	add    %al,(%rax)
+   18001d924:	add    %eax,(%rax)
+   18001d926:	add    %al,(%rax)
+   18001d928:	mov    $0x2000000,%ecx
+   18001d92d:	add    %al,(%rax)
+   18001d92f:	add    %al,(%rsi)
+   18001d931:	add    %al,(%rax)
+   18001d933:	add    %dl,(%rcx)
+   18001d935:	add    %al,(%rax)
+   18001d937:	add    %cl,(%rsi)
+   18001d939:	add    %al,(%rax)
+   18001d93b:	add    %al,(%rcx)
+   18001d93d:	add    %al,(%rax)
+   18001d93f:	add    %bh,0x20000(%rax,%rax,1)
+   18001d946:	add    %al,(%rax)
+   18001d948:	(bad)
+   18001d949:	add    %al,(%rax)
+   18001d94b:	add    %dl,(%rbx)
+   18001d94d:	add    %al,(%rax)
+   18001d94f:	add    %dl,(%rax)
+   18001d951:	add    %al,(%rax)
+   18001d953:	add    %al,(%rcx)
+   18001d955:	add    %al,(%rax)
+   18001d957:	add    %bh,0x2000000(%rdi)
+   18001d95d:	add    %al,(%rax)
+   18001d95f:	add    %al,(%rsi)
+   18001d961:	add    %al,(%rax)
+   18001d963:	add    %dl,0x13000000(%rip)        # 0x19301d969
+   18001d969:	add    %al,(%rax)
+   18001d96b:	add    %al,(%rbx)
+   18001d96d:	add    %al,(%rax)
+   18001d96f:	add    %al,%dl
+   18001d971:	add    %al,(%rax)
+   18001d973:	add    %al,(%rdx)
+   18001d975:	add    %al,(%rax)
+   18001d977:	add    %al,(%rsi)
+   18001d979:	add    %al,(%rax)
+   18001d97b:	add    %dl,(%rdi)
+   18001d97d:	add    %al,(%rax)
+   18001d97f:	add    %dl,(%rsi)
+   18001d981:	add    %al,(%rax)
+   18001d983:	add    %al,(%rcx)
+   18001d985:	add    %al,(%rax)
+   18001d987:	add    %cl,%cl
+   18001d989:	add    %al,(%rax)
+   18001d98b:	add    %al,(%rdx)
+   18001d98d:	add    %al,(%rax)
+   18001d98f:	add    %al,(%rsi)
+   18001d991:	add    %al,(%rax)
+   18001d993:	add    %bl,(%rbx)
+   18001d995:	add    %al,(%rax)
+   18001d997:	add    %bl,(%rax)
+   18001d999:	add    %al,(%rax)
+   18001d99b:	add    %al,(%rdx)
+   18001d99d:	add    %al,(%rax)
+   18001d99f:	add    %cl,%ah
+   18001d9a1:	add    %al,(%rax)
+   18001d9a3:	add    %al,(%rdx)
+   18001d9a5:	add    %al,(%rax)
+   18001d9a7:	add    %al,(%rdx)
+   18001d9a9:	add    %al,(%rax)
+   18001d9ab:	add    %bl,0x18000000(%rip)        # 0x19801d9b1
+   18001d9b1:	add    %al,(%rax)
+   18001d9b3:	add    %al,(%rcx)
+   18001d9b5:	add    %al,(%rax)
+   18001d9b7:	add    %dl,%cl
+   18001d9b9:	add    %al,(%rax)
+   18001d9bb:	add    %al,(%rdx)
    18001d9bd:	add    %al,(%rax)
-   18001d9bf:	add    %ah,0x0(%rdi)
-   18001d9c2:	jb     0x18001d9c4
-   18001d9c4:	(bad)
-   18001d9c5:	add    %ch,0x0(%rsi)
-   18001d9c8:	je     0x18001d9ca
-   18001d9ca:	pop    %rdi
-   18001d9cb:	add    %dh,0x79(%rax,%rax,1)
-   18001d9cf:	add    %dh,0x0(%rax)
-   18001d9d2:	add    %al,%gs:(%rax)
+   18001d9bf:	add    %ah,(%rdx)
+   18001d9c1:	add    %al,(%rax)
+   18001d9c3:	add    %ah,(%rax)
+   18001d9c5:	add    %al,(%rax)
+   18001d9c7:	add    %bl,(%rbx)
+   18001d9c9:	add    %al,(%rax)
+   18001d9cb:	add    %al,(%rdx)
+   18001d9cd:	add    %al,(%rax)
+   18001d9cf:	add    %dl,%ah
+   18001d9d1:	add    %al,(%rax)
+   18001d9d3:	add    %al,(%rdx)
    18001d9d5:	add    %al,(%rax)
-   18001d9d7:	add    %dh,0x0(%rdx)
-   18001d9da:	add    %ah,%gs:0x69(%rax,%rax,1)
-   18001d9df:	add    %dh,0x0(%rdx)
-   18001d9e2:	add    %ah,%gs:0x0(%rbx)
-   18001d9e6:	je     0x18001d9e8
-   18001d9e8:	pop    %rdi
-   18001d9e9:	add    %dh,0x0(%rbp)
-   18001d9ec:	jb     0x18001d9ee
-   18001d9ee:	imul   $0x0,(%rax),%eax
-   18001d9f4:	add    %al,(%rax)
-   18001d9f6:	add    %al,(%rax)
-   18001d9f8:	jb     0x18001d9fa
-   18001d9fa:	add    %ah,%gs:0x0(%rsi)
-   18001d9fe:	jb     0x18001da00
-   18001da00:	add    %dh,%gs:0x0(%rbx)
-   18001da04:	push   $0x74005f00
-   18001da09:	add    %ch,0x0(%rdi)
-   18001da0c:	imul   $0x65,(%rax),%eax
-   18001da0f:	add    %ch,0x0(%rsi)
-   18001da12:	add    %al,(%rax)
-   18001da14:	add    %al,(%rax)
-   18001da16:	add    %al,(%rax)
-   18001da18:	jb     0x18001da1a
-   18001da1a:	add    %dh,%gs:0x0(%rbx)
-   18001da1e:	jo     0x18001da20
-   18001da20:	outsl  %ds:(%rsi),(%dx)
-   18001da21:	add    %ch,0x0(%rsi)
-   18001da24:	jae    0x18001da26
-   18001da26:	add    %bl,%gs:0x0(%rdi)
-   18001da2a:	je     0x18001da2c
-   18001da2c:	jns    0x18001da2e
-   18001da2e:	jo     0x18001da30
-   18001da30:	add    %al,%gs:(%rax)
-   18001da33:	add    %al,(%rax)
+   18001d9d7:	add    %al,(%rdx)
+   18001d9d9:	add    %al,(%rax)
+   18001d9db:	add    %ah,(%rdx)
+   18001d9dd:	add    %al,(%rax)
+   18001d9df:	add    %bl,(%rbx)
+   18001d9e1:	add    %al,(%rax)
+   18001d9e3:	add    %al,(%rcx)
+   18001d9e5:	add    %al,(%rax)
+   18001d9e7:	add    %bl,%cl
+   18001d9e9:	add    %al,(%rax)
+   18001d9eb:	add    %al,(%rdx)
+   18001d9ed:	add    %al,(%rax)
+   18001d9ef:	add    %ah,(%rdx)
+   18001d9f1:	add    %al,(%rax)
+   18001d9f3:	add    %ah,0x1d000000(%rip)        # 0x19d01d9f9
+   18001d9f9:	add    %al,(%rax)
+   18001d9fb:	add    %al,(%rdx)
+   18001d9fd:	add    %al,(%rax)
+   18001d9ff:	add    %bl,%ah
+   18001da01:	add    %al,(%rax)
+   18001da03:	add    %al,(%rdx)
+   18001da05:	add    %al,(%rax)
+   18001da07:	add    %al,(%rdx)
+   18001da09:	add    %al,(%rax)
+   18001da0b:	add    %ah,(%rdi)
+   18001da0d:	add    %al,(%rax)
+   18001da0f:	add    %bl,0x1000000(%rip)        # 0x18101da15
+   18001da15:	add    %al,(%rax)
+   18001da17:	add    %ah,%cl
+   18001da19:	add    %al,(%rax)
+   18001da1b:	add    %al,(%rdx)
+   18001da1d:	add    %al,(%rax)
+   18001da1f:	add    %ah,(%rdx)
+   18001da21:	add    %al,(%rax)
+   18001da23:	add    %ch,(%rdx)
+   18001da25:	add    %al,(%rax)
+   18001da27:	add    %bl,(%rsi)
+   18001da29:	add    %al,(%rax)
+   18001da2b:	add    %al,(%rdx)
+   18001da2d:	add    %al,(%rax)
+   18001da2f:	add    %ah,%ah
+   18001da31:	add    %al,(%rax)
+   18001da33:	add    %al,(%rdx)
    18001da35:	add    %al,(%rax)
-   18001da37:	add    %dh,0x0(%rbx)
-   18001da3a:	movsxd (%rax),%eax
-   18001da3c:	outsl  %ds:(%rsi),(%dx)
-   18001da3d:	add    %dh,0x0(%rax)
-   18001da40:	add    %al,%gs:(%rax)
-   18001da43:	add    %al,(%rax)
+   18001da37:	add    %al,(%rdx)
+   18001da39:	add    %al,(%rax)
+   18001da3b:	add    %ch,(%rax,%rax,1)
+   18001da3e:	add    %al,(%rax)
+   18001da40:	(bad)
+   18001da41:	add    %al,(%rax)
+   18001da43:	add    %al,(%rcx)
    18001da45:	add    %al,(%rax)
-   18001da47:	add    %dh,0x0(%rbx)
-   18001da4a:	je     0x18001da4c
-   18001da4c:	(bad)
-   18001da4d:	add    %dh,0x65(%rax,%rax,1)
+   18001da47:	add    %ch,%cl
+   18001da49:	add    %al,(%rax)
+   18001da4b:	add    %al,(%rdx)
+   18001da4d:	add    %al,(%rax)
+   18001da4f:	add    %ah,(%rdx)
    18001da51:	add    %al,(%rax)
-   18001da53:	add    %al,(%rax)
+   18001da53:	add    %ch,(%rdi)
    18001da55:	add    %al,(%rax)
-   18001da57:	add    %dh,0x6f(%rax,%rax,1)
-   18001da5b:	add    %ch,0x0(%rbx)
-   18001da5e:	add    %ch,%gs:0x0(%rsi)
-   18001da62:	pop    %rdi
-   18001da63:	add    %dh,0x79(%rax,%rax,1)
-   18001da67:	add    %dh,0x0(%rax)
-   18001da6a:	add    %al,%gs:(%rax)
-	...
+   18001da57:	add    %bl,(%rsi)
+   18001da59:	add    %al,(%rax)
+   18001da5b:	add    %al,(%rdx)
+   18001da5d:	add    %al,(%rax)
+   18001da5f:	add    %ch,%ah
+   18001da61:	add    %al,(%rax)
+   18001da63:	add    %al,(%rdx)
+   18001da65:	add    %al,(%rax)
+   18001da67:	add    %al,(%rdx)
+   18001da69:	add    %al,(%rax)
+   18001da6b:	add    %dh,(%rcx)
+   18001da6d:	add    %al,(%rax)
+   18001da6f:	add    %bl,(%rsi)
+   18001da71:	add    %al,(%rax)
+   18001da73:	add    %al,(%rdx)
    18001da75:	add    %al,(%rax)
-   18001da77:	add    %ah,0x1800021(%rax)
+   18001da77:	add    %dh,%cl
+   18001da79:	add    %al,(%rax)
+   18001da7b:	add    %al,(%rdx)
    18001da7d:	add    %al,(%rax)
-   18001da7f:	add    %dh,0x18001da(%rax)
-   18001da85:	add    %al,(%rax)
-   18001da87:	add    %ah,0x18001dd(%rax)
-   18001da8d:	add    %al,(%rax)
-   18001da8f:	add    %dl,0x5c(%rax)
-   18001da92:	add    %al,0x1(%rax)
-	...
-   18001daa0:	(bad)
-   18001daa1:	loop   0x18001daa4
-   18001daa3:	addb   $0x0,(%rcx)
-	...
-   18001daae:	add    %al,(%rax)
-   18001dab0:	sbb    %al,(%rcx)
-   18001dab2:	add    %al,(%rax)
-   18001dab4:	sldt   (%rax)
-   18001dab7:	add    %ch,(%rax)
-   18001dab9:	add    %eax,(%rax)
-   18001dabb:	add    %cl,(%rax,%rax,1)
-   18001dabe:	add    %al,(%rax)
-   18001dac0:	xor    $0x1,%eax
+   18001da7f:	add    %al,(%rdx)
+   18001da81:	add    %al,(%rax)
+   18001da83:	add    %dh,(%rax,%rax,1)
+   18001da86:	add    %al,(%rax)
+   18001da88:	and    %eax,(%rax)
+   18001da8a:	add    %al,(%rax)
+   18001da8c:	add    (%rax),%al
+   18001da8e:	add    %al,(%rax)
+   18001da90:	testb  $0x0,(%rax)
+   18001da93:	add    %al,(%rdx)
+   18001da95:	add    %al,(%rax)
+   18001da97:	add    %al,(%rdx)
+   18001da99:	add    %al,(%rax)
+   18001da9b:	add    %dh,(%rdi)
+   18001da9d:	add    %al,(%rax)
+   18001da9f:	add    %ah,(%rcx)
+   18001daa1:	add    %al,(%rax)
+   18001daa3:	add    %al,(%rcx)
+   18001daa5:	add    %al,(%rax)
+   18001daa7:	add    %bh,%bl
+   18001daa9:	add    %al,(%rax)
+   18001daab:	add    %al,(%rdx)
+   18001daad:	add    %al,(%rax)
+   18001daaf:	add    %ah,(%rdx)
+   18001dab1:	add    %al,(%rax)
+   18001dab3:	add    %bh,(%rdx)
+   18001dab5:	add    %al,(%rax)
+   18001dab7:	add    %ah,(%rcx)
+   18001dab9:	add    %al,(%rax)
+   18001dabb:	add    %al,(%rdx)
+   18001dabd:	add    %al,(%rax)
+   18001dabf:	add    %bh,%dh
+   18001dac1:	add    %al,(%rax)
+   18001dac3:	add    %al,(%rdx)
    18001dac5:	add    %al,(%rax)
-   18001dac7:	add    %dh,(%rsi)
-   18001dac9:	add    %eax,(%rax)
-   18001dacb:	add    %al,0x3c000000(%rip)        # 0x1bc01dad1
-   18001dad1:	add    %eax,(%rax)
-   18001dad3:	add    %dl,(%rax)
-   18001dad5:	add    %al,(%rax)
-   18001dad7:	add    %cl,0x1(%rbp)
+   18001dac7:	add    %al,(%rdx)
+   18001dac9:	add    %al,(%rax)
+   18001dacb:	add    %bh,(%rax,%rax,1)
+   18001dace:	add    %al,(%rax)
+   18001dad0:	and    %eax,(%rax)
+   18001dad2:	add    %al,(%rax)
+   18001dad4:	add    (%rax),%al
+   18001dad6:	add    %al,(%rax)
+   18001dad8:	add    (%rcx),%eax
    18001dada:	add    %al,(%rax)
-   18001dadc:	or     %eax,(%rax)
+   18001dadc:	add    (%rax),%al
    18001dade:	add    %al,(%rax)
-   18001dae0:	push   %rdi
-   18001dae1:	add    %eax,(%rax)
-   18001dae3:	add    %dl,(%rbx)
+   18001dae0:	add    (%rax),%al
+   18001dae2:	add    %al,(%rax)
+   18001dae4:	(bad)
    18001dae5:	add    %al,(%rax)
-   18001dae7:	add    %ch,0x1(%rbx)
-   18001daea:	add    %al,(%rax)
-   18001daec:	or     $0x0,%al
-   18001daee:	add    %al,(%rax)
-   18001daf0:	js     0x18001daf3
-   18001daf2:	add    %al,(%rax)
-   18001daf4:	and    %al,(%rax)
-   18001daf6:	add    %al,(%rax)
-   18001daf8:	cltd
-   18001daf9:	add    %eax,(%rax)
-   18001dafb:	add    %bl,(%rcx)
-   18001dafd:	add    %al,(%rax)
-   18001daff:	add    %dh,0xc000001(%rbx)
-   18001db05:	add    %al,(%rax)
-   18001db07:	add    %al,%al
-   18001db09:	add    %eax,(%rax)
-   18001db0b:	add    %al,-0x3a000000(%rip)        # 0x14601db11
-   18001db11:	add    %eax,(%rax)
-   18001db13:	add    %dl,(%rbx)
-   18001db15:	add    %al,(%rax)
-   18001db17:	add    %bl,%dl
-   18001db19:	add    %eax,(%rax)
-   18001db1b:	add    %cl,(%rdx)
-   18001db1d:	add    %al,(%rax)
-   18001db1f:	add    %ah,%ch
-   18001db21:	add    %eax,(%rax)
-   18001db23:	add    %dl,(%rbx)
-   18001db25:	add    %al,(%rax)
-   18001db27:	add    %bh,%cl
-   18001db29:	add    %eax,(%rax)
-   18001db2b:	add    %cl,(%rax,%rax,1)
-   18001db2e:	add    %al,(%rax)
-   18001db30:	(bad)
-   18001db31:	add    (%rax),%al
-   18001db33:	add    %dl,(%rdi)
+   18001dae7:	add    %ah,(%rdx)
+   18001dae9:	add    %al,(%rax)
+   18001daeb:	add    %al,(%rdx)
+   18001daed:	add    %al,(%rax)
+   18001daef:	add    %cl,(%rax)
+   18001daf1:	add    %eax,(%rax)
+   18001daf3:	add    %al,(%rdx)
+   18001daf5:	add    %al,(%rax)
+   18001daf7:	add    %al,(%rdx)
+   18001daf9:	add    %al,(%rax)
+   18001dafb:	add    %al,0x0(%rdx)
+   18001dafe:	add    %al,(%rax)
+   18001db00:	and    (%rax),%al
+   18001db02:	add    %al,(%rax)
+   18001db04:	add    %eax,(%rax)
+   18001db06:	add    %al,(%rax)
+   18001db08:	or     $0x2000001,%eax
+   18001db0d:	add    %al,(%rax)
+   18001db0f:	add    %ah,(%rdx)
+   18001db11:	add    %al,(%rax)
+   18001db13:	add    %al,0x0(%rbp)
+   18001db16:	add    %al,(%rax)
+   18001db18:	sub    (%rax),%eax
+   18001db1a:	add    %al,(%rax)
+   18001db1c:	or     (%rax),%al
+   18001db1e:	add    %al,(%rax)
+   18001db20:	add    (%rax),%eax
+   18001db22:	add    %al,(%rax)
+   18001db24:	sub    (%rax),%eax
+   18001db26:	add    %al,(%rax)
+   18001db28:	or     (%rax),%al
+   18001db2a:	add    %al,(%rax)
+   18001db2c:	add    $0x2b000000,%eax
+   18001db31:	add    %al,(%rax)
+   18001db33:	add    %cl,(%rdx)
    18001db35:	add    %al,(%rax)
-   18001db37:	add    %bl,(%rsi)
-   18001db39:	add    (%rax),%al
-   18001db3b:	add    %dl,(%rcx)
+   18001db37:	add    %al,(%rdi)
+   18001db39:	add    %al,(%rax)
+   18001db3b:	add    %ch,(%rbx)
    18001db3d:	add    %al,(%rax)
-   18001db3f:	add    %dh,(%rax)
-   18001db41:	add    (%rax),%al
-   18001db43:	add    %cl,0x3e000000(%rip)        # 0x1be01db49
-   18001db49:	add    (%rax),%al
-   18001db4b:	add    %al,0x44000000(%rip)        # 0x1c401db51
-   18001db51:	add    (%rax),%al
-   18001db53:	add    %dl,(%rax)
+   18001db3f:	add    %cl,(%rdx)
+   18001db41:	add    %al,(%rax)
+   18001db43:	add    %cl,(%rcx)
+   18001db45:	add    %al,(%rax)
+   18001db47:	add    %ch,(%rbx)
+   18001db49:	add    %al,(%rax)
+   18001db4b:	add    %cl,(%rdx)
+   18001db4d:	add    %al,(%rax)
+   18001db4f:	add    %cl,(%rbx)
+   18001db51:	add    %al,(%rax)
+   18001db53:	add    %ch,(%rbx)
    18001db55:	add    %al,(%rax)
-   18001db57:	add    %dl,0x2(%rbp)
-   18001db5a:	add    %al,(%rax)
-   18001db5c:	add    (%rax),%eax
-   18001db5e:	add    %al,(%rax)
-   18001db60:	pop    %rcx
-   18001db61:	add    (%rax),%al
-   18001db63:	add    %bl,0x77000000(%rip)        # 0x1f701db69
-   18001db69:	add    (%rax),%al
-   18001db6b:	add    %al,(%rax,%rax,1)
-   18001db6e:	add    %al,(%rax)
-   18001db70:	jl     0x18001db74
-   18001db72:	add    %al,(%rax)
-   18001db74:	(bad)
-   18001db75:	add    %al,(%rax)
-   18001db77:	add    %dl,0x3000002(%rbx)
-   18001db7d:	add    %al,(%rax)
-   18001db7f:	add    %dl,0xa000002(%rdi)
-   18001db85:	add    %al,(%rax)
-   18001db87:	add    %ah,0x4000002(%rdx)
-   18001db8d:	add    %al,(%rax)
-   18001db8f:	add    %ah,0xe000002(%rdi)
+   18001db57:	add    %dl,(%rax)
+   18001db59:	add    %al,(%rax)
+   18001db5b:	add    %cl,0x2b000000(%rip)        # 0x1ab01db61
+   18001db61:	add    %al,(%rax)
+   18001db63:	add    %cl,(%rdx)
+   18001db65:	add    %al,(%rax)
+   18001db67:	add    %cl,(%rdi)
+   18001db69:	add    %al,(%rax)
+   18001db6b:	add    %ch,(%rbx)
+   18001db6d:	add    %al,(%rax)
+   18001db6f:	add    %dl,(%rcx)
+   18001db71:	add    %al,(%rax)
+   18001db73:	adcb   $0x0,(%rdx)
+   18001db76:	add    %al,(%rax)
+   18001db78:	sub    (%rax),%eax
+   18001db7a:	add    %al,(%rax)
+   18001db7c:	or     (%rax),%al
+   18001db7e:	add    %al,(%rax)
+   18001db80:	or     (%rax),%al
+   18001db82:	add    %al,(%rax)
+   18001db84:	adc    %eax,(%rax)
+   18001db86:	add    %al,(%rax)
+   18001db88:	adc    (%rax),%eax
+   18001db8a:	add    %al,(%rax)
+   18001db8c:	adc    $0x0,%al
+   18001db8e:	add    %al,(%rax)
+   18001db90:	adc    $0x2b000000,%eax
    18001db95:	add    %al,(%rax)
-   18001db97:	add    %dh,0x3000002(%rsi)
+   18001db97:	add    %cl,(%rax)
+   18001db99:	add    %al,(%rax)
+   18001db9b:	add    %dl,(%rdi)
    18001db9d:	add    %al,(%rax)
-   18001db9f:	add    %bh,0x4000002(%rdx)
+   18001db9f:	add    %dl,(%rcx)
+   18001dba1:	add    %al,(%rax)
+   18001dba3:	add    %dl,(%rcx)
    18001dba5:	add    %al,(%rax)
-   18001dba7:	add    %bh,0xf000002(%rdi)
+   18001dba7:	add    %cl,(%rax)
+   18001dba9:	add    %al,(%rax)
+   18001dbab:	add    %bl,(%rcx)
    18001dbad:	add    %al,(%rax)
-   18001dbaf:	add    %cl,%bh
-   18001dbb1:	add    (%rax),%al
-   18001dbb3:	add    %cl,(%rcx)
+   18001dbaf:	add    %bl,(%rdx)
+   18001dbb1:	add    %al,(%rax)
+   18001dbb3:	add    %dl,(%rcx)
    18001dbb5:	add    %al,(%rax)
-   18001dbb7:	add    %bl,%cl
-   18001dbb9:	add    (%rax),%al
-   18001dbbb:	add    %al,(%rbx)
+   18001dbb7:	add    %dl,(%rcx)
+   18001dbb9:	add    %al,(%rax)
+   18001dbbb:	add    %bl,(%rcx)
    18001dbbd:	add    %al,(%rax)
-   18001dbbf:	add    %bl,%ch
-   18001dbc1:	add    (%rax),%al
-   18001dbc3:	add    %cl,(%rsi)
-   18001dbc5:	add    %al,(%rax)
-   18001dbc7:	add    %dl,0x41(%rcx)
-   18001dbca:	(bad)
-   18001dbcf:	movsxd 0x41(%rdi,%rcx,2),%esi
-   18001dbd3:	jne    0x18001dc49
-   18001dbd5:	push   $0x63730032
-   18001dbda:	outsl  %ds:(%rsi),(%dx)
-   18001dbdb:	jo     0x18001dc42
-   18001dbdd:	rex.XB push $0x65676e61
-   18001dbe3:	add    %al,%fs:(%rax)
-   18001dbe6:	jae    0x18001dc4b
-   18001dbe8:	outsl  %ds:(%rsi),(%dx)
-   18001dbe9:	jo     0x18001dc50
-   18001dbeb:	add    %dh,0x73(%rbp)
-   18001dbee:	gs jb  0x18001dc32
-   18001dbf1:	outsb  %gs:(%esi),(%dx)
-   18001dbf4:	je     0x18001dc39
-   18001dbf6:	push   $0x65676e61
-   18001dbfb:	add    %dh,%fs:0x73(%rbp)
-   18001dbff:	gs jb  0x18001dc43
-   18001dc02:	outsb  %gs:(%esi),(%dx)
-   18001dc05:	je     0x18001dc07
-   18001dc07:	jb     0x18001dc6e
-   18001dc09:	jae    0x18001dc7b
-   18001dc0b:	outsl  %ds:(%rsi),(%dx)
-   18001dc0c:	outsb  %ds:(%rsi),(%dx)
-   18001dc0d:	jae    0x18001dc74
-   18001dc0f:	push   %rsp
-   18001dc10:	jns    0x18001dc82
-   18001dc12:	gs rex.XB push $0x65676e61
-   18001dc19:	add    %dh,%fs:0x65(%rdx)
-   18001dc1d:	jae    0x18001dc8f
-   18001dc1f:	outsl  %ds:(%rsi),(%dx)
-   18001dc20:	outsb  %ds:(%rsi),(%dx)
-   18001dc21:	jae    0x18001dc88
-   18001dc23:	push   %rsp
-   18001dc24:	jns    0x18001dc96
-   18001dc26:	add    %ah,%gs:0x6c(%rbx)
-   18001dc2a:	imul   $0x65644974,0x6e(%rbp),%esp
-   18001dc31:	outsb  %ds:(%rsi),(%dx)
-   18001dc32:	je     0x18001dc9d
-   18001dc34:	imul   $0x6853,0x72(%rbp),%sp
-   18001dc3a:	(bad)
-   18001dc3b:	jb     0x18001dca2
-   18001dc3d:	fs rex.WXB
-   18001dc3f:	gs jns 0x18001dc85
-   18001dc42:	push   $0x65676e61
-   18001dc47:	add    %ah,%fs:0x6c(%rbx)
-   18001dc4b:	imul   $0x65644974,0x6e(%rbp),%esp
-   18001dc52:	outsb  %ds:(%rsi),(%dx)
-   18001dc53:	je     0x18001dcbe
-   18001dc55:	imul   $0x6853,0x72(%rbp),%sp
-   18001dc5b:	(bad)
-   18001dc5c:	jb     0x18001dcc3
-   18001dc5e:	fs rex.WXB
-   18001dc60:	gs jns 0x18001dc63
-   18001dc63:	jae    0x18001dcd9
-   18001dc65:	(bad)
-   18001dc66:	je     0x18001dccd
-   18001dc68:	rex.XB push $0x65676e61
-   18001dc6e:	add    %dh,%fs:0x74(%rbx)
-   18001dc72:	(bad)
-   18001dc73:	je     0x18001dcda
-   18001dc75:	add    %ah,0x78(%rbp)
-   18001dc78:	jo     0x18001dce3
-   18001dc7a:	jb     0x18001dcdd
-   18001dc7c:	je     0x18001dce7
-   18001dc7e:	outsl  %ds:(%rsi),(%dx)
-   18001dc7f:	outsb  %ds:(%rsi),(%dx)
-   18001dc80:	rex.B je 0x18001dcc6
-   18001dc83:	push   $0x65676e61
-   18001dc88:	add    %ah,%fs:0x78(%rbp)
-   18001dc8c:	jo     0x18001dcf7
-   18001dc8e:	jb     0x18001dcf1
-   18001dc90:	je     0x18001dcfb
-   18001dc92:	outsl  %ds:(%rsi),(%dx)
-   18001dc93:	outsb  %ds:(%rsi),(%dx)
-   18001dc94:	add    %dh,0x65(%rdx)
-   18001dc97:	data16 jb 0x18001dcff
-   18001dc9a:	jae    0x18001dd04
-   18001dc9c:	push   %rsp
-   18001dc9d:	outsl  %ds:(%rsi),(%dx)
-   18001dc9e:	imul   $0x43,0x6e(%rbp),%esp
-   18001dca2:	push   $0x65676e61
-   18001dca7:	add    %dh,%fs:0x65(%rdx)
-   18001dcab:	data16 jb 0x18001dd13
-   18001dcae:	jae    0x18001dd18
-   18001dcb0:	push   %rsp
-   18001dcb1:	outsl  %ds:(%rsi),(%dx)
-   18001dcb2:	imul   $0x0,0x6e(%rbp),%esp
-   18001dcb6:	jae    0x18001dd2b
-   18001dcb8:	insb   (%dx),%es:(%rdi)
-   18001dcb9:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001dcbb:	outsb  %ds:(%rsi),(%dx)
-   18001dcbc:	imul   $0x6172,0x75(%rdi),%sp
-   18001dcc2:	je     0x18001dd2d
-   18001dcc4:	outsl  %ds:(%rsi),(%dx)
-   18001dcc5:	outsb  %ds:(%rsi),(%dx)
-   18001dcc6:	rex.XB push $0x65676e61
-   18001dccc:	add    %dl,%fs:0x53(%rcx)
-   18001dcd0:	jae    0x18001dd3e
-   18001dcd2:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001dcd4:	outsb  %ds:(%rsi),(%dx)
-   18001dcd5:	imul   $0x6172,0x75(%rdi),%sp
-   18001dcdb:	je     0x18001dd46
-   18001dcdd:	outsl  %ds:(%rsi),(%dx)
-   18001dcde:	outsb  %ds:(%rsi),(%dx)
-   18001dcdf:	add    %ah,0x6f(%rbx)
-   18001dce2:	outsb  %ds:(%rsi),(%dx)
-   18001dce3:	imul   $0x6172,0x75(%rdi),%sp
-   18001dce9:	je     0x18001dd54
-   18001dceb:	outsl  %ds:(%rsi),(%dx)
-   18001dcec:	outsb  %ds:(%rsi),(%dx)
-   18001dced:	add    %ah,0x72(%rbp)
-   18001dcf0:	jb     0x18001dd61
-   18001dcf2:	jb     0x18001dcf4
-   18001dcf4:	gs jb  0x18001dd69
-   18001dcf7:	outsl  %ds:(%rsi),(%dx)
-   18001dcf8:	jb     0x18001dd3e
-   18001dcfa:	gs jae 0x18001dd60
-   18001dcfd:	jb     0x18001dd68
-   18001dcff:	jo     0x18001dd75
-   18001dd01:	imul   $0x69727500,0x6e(%rdi),%ebp
-   18001dd08:	add    %ah,0x75(%rcx)
-   18001dd0b:	je     0x18001dd75
-   18001dd0d:	outsl  %ds:(%rsi),(%dx)
-   18001dd0e:	jb     0x18001dd79
-   18001dd10:	jp     0x18001dd73
-   18001dd12:	je     0x18001dd7d
-   18001dd14:	outsl  %ds:(%rsi),(%dx)
-   18001dd15:	outsb  %ds:(%rsi),(%dx)
-   18001dd16:	rex.XB (bad)
-   18001dd18:	insb   (%dx),%es:(%rdi)
-   18001dd19:	insb   (%dx),%es:(%rdi)
-   18001dd1a:	(bad)
-   18001dd1c:	movsxd 0x52(%rbx),%ebp
-   18001dd1f:	movsxd %gs:0x69(%rbp),%esp
-   18001dd23:	jbe    0x18001dd8a
-   18001dd25:	add    %ah,%fs:0x74(%rcx,%riz,2)
-   18001dd2a:	(bad)
-   18001dd2b:	add    %ah,0x72(%rbx)
-   18001dd2e:	gs (bad)
-   18001dd30:	je     0x18001dd97
-   18001dd32:	rex.B jne 0x18001dda9
-   18001dd35:	push   $0x69746e65
-   18001dd3a:	movsxd 0x74(%rcx),%esp
-   18001dd3d:	gs fs push %rbp
-   18001dd40:	jb     0x18001ddae
-   18001dd42:	add    %dh,0x72(%rbp)
-   18001dd45:	insb   (%dx),%es:(%rdi)
-   18001dd46:	add    %dh,0x61(%rax)
-   18001dd49:	jb     0x18001ddac
-   18001dd4b:	insl   (%dx),%es:(%rdi)
-   18001dd4c:	gs je  0x18001ddb4
-   18001dd4f:	jb     0x18001ddc4
-   18001dd51:	add    %ch,0x65(%rax)
-   18001dd54:	(bad)
-   18001dd55:	add    %dl,%fs:0x4e(%rcx)
-   18001dd59:	gs je  0x18001ddd3
-   18001dd5c:	outsl  %ds:(%rsi),(%dx)
-   18001dd5d:	jb     0x18001ddca
-   18001dd5f:	push   %rdx
-   18001dd60:	gs jo  0x18001ddcf
-   18001dd63:	jns    0x18001dd8f
-   18001dd65:	add    %ah,0x65(%rdi)
-   18001dd68:	je     0x18001dd6a
-   18001dd6a:	jo     0x18001dddb
-   18001dd6c:	jae    0x18001dde2
-   18001dd6e:	add    %dl,0x48(%rcx)
-   18001dd71:	je     0x18001dde7
-   18001dd73:	jo     0x18001ddc2
-   18001dd75:	jne    0x18001dde3
-   18001dd77:	je     0x18001dde2
-   18001dd79:	push   %rax
-   18001dd7a:	(bad)
-   18001dd7b:	jb     0x18001ddf1
-   18001dd7d:	sub    (%rax),%al
-   18001dd7f:	insl   (%dx),%es:(%rdi)
-   18001dd80:	jne    0x18001ddee
-   18001dd82:	je     0x18001dded
-   18001dd84:	push   %rax
-   18001dd85:	(bad)
-   18001dd86:	jb     0x18001ddfc
-   18001dd88:	add    %dh,0x75(%rax)
-   18001dd8b:	je     0x18001dd8d
-   18001dd8d:	fs gs insb (%dx),%es:(%rdi)
-   18001dd90:	gs je  0x18001ddf8
-   18001dd93:	push   %rdx
-   18001dd94:	gs jae 0x18001de06
-   18001dd97:	jne    0x18001de0b
-   18001dd99:	movsxd 0x0(%rbp),%esp
-   18001dd9c:	add    %al,(%rax)
+   18001dbbf:	add    %bl,(%rax,%rax,1)
+   18001dbc2:	add    %al,0x11(%rax)
+   18001dbc8:	or     %al,(%rax)
+   18001dbca:	add    %al,(%rax)
+   18001dbcc:	sbb    %eax,(%rax)
+   18001dbce:	add    %al,(%rax)
+   18001dbd0:	sbb    (%rax),%al
+   18001dbd2:	add    %al,(%rax)
+   18001dbd4:	sbb    $0x0,%al
+   18001dbd6:	add    %al,0x11(%rax)
+   18001dbdc:	sbb    %eax,(%rax)
+   18001dbde:	add    %al,(%rax)
+   18001dbe0:	sbb    $0x0,%al
+   18001dbe2:	add    %al,0x11(%rax)
+   18001dbe8:	or     %al,(%rax)
+   18001dbea:	add    %al,(%rax)
+   18001dbec:	sbb    %eax,(%rax)
+   18001dbee:	add    %al,(%rax)
+   18001dbf0:	sbb    (%rax),%al
+   18001dbf2:	add    %al,(%rax)
+   18001dbf4:	sbb    $0x0,%al
+   18001dbf6:	add    %al,0x11(%rax)
+   18001dbfc:	sbb    %eax,(%rax)
+   18001dbfe:	add    %al,(%rax)
+   18001dc00:	sbb    $0x0,%al
+   18001dc02:	add    %al,0x11(%rax)
+   18001dc08:	or     %al,(%rax)
+   18001dc0a:	add    %al,(%rax)
+   18001dc0c:	sbb    %eax,(%rax)
+   18001dc0e:	add    %al,(%rax)
+   18001dc10:	sbb    (%rax),%al
+   18001dc12:	add    %al,(%rax)
+   18001dc14:	sbb    $0x0,%al
+   18001dc16:	add    %al,0x11(%rax)
+   18001dc1c:	sbb    %eax,(%rax)
+   18001dc1e:	add    %al,(%rax)
+   18001dc20:	sbb    $0x0,%al
+   18001dc22:	add    %al,0x11(%rax)
+   18001dc28:	or     $0x0,%al
+   18001dc2a:	add    %al,(%rax)
+   18001dc2c:	sbb    %eax,(%rax)
+   18001dc2e:	add    %al,(%rax)
+   18001dc30:	(bad)
+   18001dc31:	add    %al,(%rax)
+   18001dc33:	add    %bl,(%rax,%rax,1)
+   18001dc36:	add    %al,0x11(%rax)
+   18001dc3c:	(bad)
+   18001dc3d:	add    %al,(%rax)
+   18001dc3f:	sbbb   $0x0,(%rcx)
+   18001dc42:	add    %al,(%rax)
+   18001dc44:	and    %al,(%rax)
+   18001dc46:	add    %al,(%rax)
+   18001dc48:	sbb    $0x0,%al
+   18001dc4a:	add    %al,0x11(%rax)
+   18001dc50:	or     %al,(%rax)
+   18001dc52:	add    %al,(%rax)
+   18001dc54:	sbb    %eax,(%rax)
+   18001dc56:	add    %al,(%rax)
+   18001dc58:	sbb    (%rax),%al
+   18001dc5a:	add    %al,(%rax)
+   18001dc5c:	sbb    $0x0,%al
+   18001dc5e:	add    %al,0x11(%rax)
+   18001dc64:	sbb    %eax,(%rax)
+   18001dc66:	add    %al,(%rax)
+   18001dc68:	sbb    $0x0,%al
+   18001dc6a:	add    %al,0x11(%rax)
+   18001dc70:	or     $0x0,%al
+   18001dc72:	add    %al,(%rax)
+   18001dc74:	sbb    %eax,(%rax)
+   18001dc76:	add    %al,(%rax)
+   18001dc78:	(bad)
+   18001dc79:	add    %al,(%rax)
+   18001dc7b:	add    %bl,(%rax,%rax,1)
+   18001dc7e:	add    %al,0x11(%rax)
+   18001dc84:	(bad)
+   18001dc85:	add    %al,(%rax)
+   18001dc87:	sbbb   $0x0,(%rcx)
+   18001dc8a:	add    %al,(%rax)
+   18001dc8c:	and    %al,(%rax)
+   18001dc8e:	add    %al,(%rax)
+   18001dc90:	sbb    $0x0,%al
+   18001dc92:	add    %al,0x11(%rax)
+   18001dc98:	or     %al,(%rax)
+   18001dc9a:	add    %al,(%rax)
+   18001dc9c:	sbb    %eax,(%rax)
+   18001dc9e:	add    %al,(%rax)
+   18001dca0:	sbb    (%rax),%al
+   18001dca2:	add    %al,(%rax)
+   18001dca4:	sbb    $0x0,%al
+   18001dca6:	add    %al,0x11(%rax)
+   18001dcac:	sbb    %eax,(%rax)
+   18001dcae:	add    %al,(%rax)
+   18001dcb0:	add    (%rax),%eax
+   18001dcb2:	add    %al,(%rax)
+   18001dcb4:	or     (%rax),%al
+   18001dcb6:	add    %al,(%rax)
+   18001dcb8:	add    0x1(%rcx),%edx
+	...
+   18001dcc3:	add    %al,0xa000000(%rip)        # 0x18a01dcc9
+   18001dcc9:	add    %al,(%rax)
+   18001dccb:	add    %al,(%rbx)
+   18001dccd:	push   %rcx
+   18001dcce:	add    %eax,(%rax)
+   18001dcd0:	add    %eax,(%rax)
+   18001dcd2:	add    %al,(%rax)
+   18001dcd4:	add    %al,(%rax)
+   18001dcd6:	add    %al,(%rax)
+   18001dcd8:	or     %eax,(%rax)
+   18001dcda:	add    %al,(%rax)
+   18001dcdc:	or     (%rax),%al
+   18001dcde:	add    %al,(%rax)
+   18001dce0:	add    0x1(%rcx),%edx
+   18001dce3:	add    %al,(%rbx)
+   18001dce5:	add    %al,(%rax)
+   18001dce7:	add    %al,(%rax)
+   18001dce9:	add    %al,(%rax)
+   18001dceb:	add    %cl,(%rbx)
+   18001dced:	add    %al,(%rax)
+   18001dcef:	add    %cl,(%rdx)
+   18001dcf1:	add    %al,(%rax)
+   18001dcf3:	add    %al,(%rbx)
+   18001dcf5:	push   %rcx
+   18001dcf6:	add    %eax,(%rax)
+   18001dcf8:	add    $0x0,%al
+   18001dcfa:	add    %al,(%rax)
+   18001dcfc:	add    %al,(%rax)
+   18001dcfe:	add    %al,(%rax)
+   18001dd00:	or     $0x10000000,%eax
+   18001dd05:	add    %al,(%rax)
+   18001dd07:	add    %al,(%rcx)
+   18001dd09:	push   %rax
+   18001dd0a:	add    %eax,(%rax)
+   18001dd0c:	add    $0x0,%eax
+   18001dd11:	add    %al,(%rax)
+   18001dd13:	add    %cl,(%rdi)
+   18001dd15:	add    %al,(%rax)
+   18001dd17:	add    %cl,(%rdx)
+   18001dd19:	add    %al,(%rax)
+   18001dd1b:	add    %al,(%rbx)
+   18001dd1d:	push   %rcx
+   18001dd1e:	add    %eax,(%rax)
+   18001dd20:	(bad)
+	...
+   18001dd2d:	add    %al,(%rax)
+   18001dd2f:	add    %ah,0x18002b2(%rax)
+   18001dd35:	add    %al,(%rax)
+   18001dd37:	add    %ah,0x18002b2(%rax)
+   18001dd3d:	add    %al,(%rax)
+   18001dd3f:	add    %ah,0x18002b2(%rax)
+   18001dd45:	add    %al,(%rax)
+   18001dd47:	add    %ah,0x18002b2(%rax)
+   18001dd4d:	add    %al,(%rax)
+   18001dd4f:	add    %dh,0x18002b5(%rax)
+   18001dd55:	add    %al,(%rax)
+   18001dd57:	add    %ah,0x18002b2(%rax)
+   18001dd5d:	add    %al,(%rax)
+   18001dd5f:	add    %ah,(%rax)
+   18001dd61:	mov    $0x2,%dh
+   18001dd63:	addb   $0x0,(%rcx)
+   18001dd66:	add    %al,(%rax)
+   18001dd68:	lock mov $0x2,%bl
+   18001dd6b:	addb   $0x0,(%rcx)
+   18001dd6e:	add    %al,(%rax)
+   18001dd70:	movabs 0xf0000000018002b2,%al
+   18001dd79:	mov    $0x2,%bl
+   18001dd7b:	addb   $0x0,(%rcx)
+   18001dd7e:	add    %al,(%rax)
+   18001dd80:	movabs 0xf0000000018002b2,%al
+   18001dd89:	mov    $0x2,%bl
+   18001dd8b:	addb   $0x0,(%rcx)
+   18001dd8e:	add    %al,(%rax)
+   18001dd90:	movabs 0xf0000000018002b2,%al
+   18001dd99:	mov    $0x2,%bl
+   18001dd9b:	addb   $0x0,(%rcx)
    18001dd9e:	add    %al,(%rax)
-   18001dda0:	or     (%rax),%eax
-	...
+   18001dda0:	movabs 0xf0000000018002b2,%al
+   18001dda9:	mov    $0x2,%bl
+   18001ddab:	addb   $0x0,(%rcx)
    18001ddae:	add    %al,(%rax)
-   18001ddb0:	sbb    (%rax),%al
-   18001ddb2:	add    %al,(%rax)
-   18001ddb4:	(bad)
-   18001ddb5:	add    %al,(%rax)
-   18001ddb7:	add    %al,(%rsi)
-   18001ddb9:	add    %al,(%rax)
-   18001ddbb:	add    %dl,(%rax)
-   18001ddbd:	add    %eax,(%rax)
-	...
-   18001ddd3:	add    %cl,(%rdx)
-   18001ddd5:	add    %al,(%rax)
-   18001ddd7:	add    %al,(%rcx)
-   18001ddd9:	add    %al,(%rax)
-   18001dddb:	add    %al,(%rcx)
-   18001dddd:	add    %al,(%rax)
-   18001dddf:	add    %ch,0x2000000(%rdx)
-   18001dde5:	add    %al,(%rax)
-   18001dde7:	add    %al,(%rsi)
-   18001dde9:	add    %al,(%rax)
-   18001ddeb:	add    %al,(%rdi)
-   18001dded:	add    %al,(%rax)
-   18001ddef:	add    %al,(%rax,%rax,1)
-   18001ddf2:	add    %al,(%rax)
-   18001ddf4:	add    %eax,(%rax)
-   18001ddf6:	add    %al,(%rax)
-   18001ddf8:	lods   %ds:(%rsi),%eax
-   18001ddf9:	add    %al,(%rax)
-   18001ddfb:	add    %al,(%rdx)
-   18001ddfd:	add    %al,(%rax)
-   18001ddff:	add    %al,(%rsi)
-   18001de01:	add    %al,(%rax)
-   18001de03:	add    %cl,(%rcx)
-   18001de05:	add    %al,(%rax)
-   18001de07:	add    %al,(%rsi)
-   18001de09:	add    %al,(%rax)
-   18001de0b:	add    %al,(%rcx)
-   18001de0d:	add    %al,(%rax)
-   18001de0f:	add    %dh,0x2000000(%rax)
-   18001de15:	add    %al,(%rax)
-   18001de17:	add    %al,(%rsi)
-   18001de19:	add    %al,(%rax)
-   18001de1b:	add    %cl,(%rbx)
-   18001de1d:	add    %al,(%rax)
-   18001de1f:	add    %cl,(%rax)
-   18001de21:	add    %al,(%rax)
-   18001de23:	add    %al,(%rcx)
-   18001de25:	add    %al,(%rax)
-   18001de27:	add    %dh,0x2000000(%rbx)
-   18001de2d:	add    %al,(%rax)
-   18001de2f:	add    %al,(%rsi)
-   18001de31:	add    %al,(%rax)
-   18001de33:	add    %cl,0xa000000(%rip)        # 0x18a01de39
-   18001de39:	add    %al,(%rax)
-   18001de3b:	add    %al,(%rcx)
-   18001de3d:	add    %al,(%rax)
-   18001de3f:	add    %dh,0x2000000(%rsi)
-   18001de45:	add    %al,(%rax)
-   18001de47:	add    %al,(%rsi)
-   18001de49:	add    %al,(%rax)
-   18001de4b:	add    %cl,(%rdi)
-   18001de4d:	add    %al,(%rax)
-   18001de4f:	add    %cl,(%rax,%rax,1)
-   18001de52:	add    %al,(%rax)
-   18001de54:	add    %eax,(%rax)
+   18001ddb0:	movabs 0xf0000000018002b2,%al
+   18001ddb9:	mov    $0x2,%bl
+   18001ddbb:	addb   $0x0,(%rcx)
+   18001ddbe:	add    %al,(%rax)
+   18001ddc0:	mov    $0xb5,%al
+   18001ddc2:	add    0x1(%rax),%al
+   18001ddc8:	lock mov $0x2,%bl
+   18001ddcb:	addb   $0x0,(%rcx)
+   18001ddce:	add    %al,(%rax)
+   18001ddd0:	movabs 0xf0000000018002b2,%al
+   18001ddd9:	mov    $0x2,%bl
+   18001dddb:	addb   $0x0,(%rcx)
+   18001ddde:	add    %al,(%rax)
+   18001dde0:	add    %dh,0x18002(%rdi)
+   18001dde6:	add    %al,(%rax)
+   18001dde8:	lock mov $0x2,%bl
+   18001ddeb:	addb   $0x0,(%rcx)
+   18001ddee:	add    %al,(%rax)
+   18001ddf0:	movabs 0xa0000000018002b2,%al
+   18001ddf9:	mov    $0x2,%dl
+   18001ddfb:	addb   $0x0,(%rcx)
+   18001ddfe:	add    %al,(%rax)
+   18001de00:	shlb   $0x0,0x18002(%rcx)
+   18001de07:	add    %dh,%al
+   18001de09:	mov    $0x2,%bl
+   18001de0b:	addb   $0x0,(%rcx)
+   18001de0e:	add    %al,(%rax)
+   18001de10:	loopne 0x18001ddc2
+   18001de12:	add    0x1(%rax),%al
+   18001de18:	shlb   $0x0,0x18002(%rcx)
+   18001de1f:	add    %al,%al
+   18001de21:	mov    $0x2,%cl
+   18001de23:	addb   $0x0,(%rcx)
+   18001de26:	add    %al,(%rax)
+   18001de28:	loopne 0x18001ddda
+   18001de2a:	add    0x1(%rax),%al
+   18001de30:	shlb   $0x0,0x18002(%rcx)
+   18001de37:	add    %al,%al
+   18001de39:	mov    $0x2,%cl
+   18001de3b:	addb   $0x0,(%rcx)
+   18001de3e:	add    %al,(%rax)
+   18001de40:	mov    $0x2,%bpl
+   18001de43:	addb   $0x0,(%rcx)
+   18001de46:	add    %al,(%rax)
+   18001de48:	shlb   $0x0,0x18002(%rcx)
+   18001de4f:	add    %ah,%al
+   18001de51:	mov    $0x2,%al
+   18001de53:	addb   $0x0,(%rcx)
    18001de56:	add    %al,(%rax)
-   18001de58:	mov    $0x2000000,%ecx
-   18001de5d:	add    %al,(%rax)
-   18001de5f:	add    %al,(%rsi)
-   18001de61:	add    %al,(%rax)
-   18001de63:	add    %dl,(%rcx)
-   18001de65:	add    %al,(%rax)
-   18001de67:	add    %cl,(%rsi)
-   18001de69:	add    %al,(%rax)
-   18001de6b:	add    %al,(%rcx)
-   18001de6d:	add    %al,(%rax)
-   18001de6f:	add    %bh,0x20000(%rax,%rax,1)
-   18001de76:	add    %al,(%rax)
-   18001de78:	(bad)
-   18001de79:	add    %al,(%rax)
-   18001de7b:	add    %dl,(%rbx)
-   18001de7d:	add    %al,(%rax)
-   18001de7f:	add    %dl,(%rax)
-   18001de81:	add    %al,(%rax)
-   18001de83:	add    %al,(%rcx)
-   18001de85:	add    %al,(%rax)
-   18001de87:	add    %bh,0x2000000(%rdi)
-   18001de8d:	add    %al,(%rax)
-   18001de8f:	add    %al,(%rsi)
-   18001de91:	add    %al,(%rax)
-   18001de93:	add    %dl,0x13000000(%rip)        # 0x19301de99
-   18001de99:	add    %al,(%rax)
-   18001de9b:	add    %al,(%rbx)
-   18001de9d:	add    %al,(%rax)
-   18001de9f:	add    %al,%dl
-   18001dea1:	add    %al,(%rax)
-   18001dea3:	add    %al,(%rdx)
-   18001dea5:	add    %al,(%rax)
-   18001dea7:	add    %al,(%rsi)
-   18001dea9:	add    %al,(%rax)
-   18001deab:	add    %dl,(%rdi)
-   18001dead:	add    %al,(%rax)
-   18001deaf:	add    %dl,(%rsi)
-   18001deb1:	add    %al,(%rax)
-   18001deb3:	add    %al,(%rcx)
-   18001deb5:	add    %al,(%rax)
-   18001deb7:	add    %cl,%cl
-   18001deb9:	add    %al,(%rax)
-   18001debb:	add    %al,(%rdx)
-   18001debd:	add    %al,(%rax)
-   18001debf:	add    %al,(%rsi)
-   18001dec1:	add    %al,(%rax)
-   18001dec3:	add    %bl,(%rbx)
-   18001dec5:	add    %al,(%rax)
-   18001dec7:	add    %bl,(%rax)
-   18001dec9:	add    %al,(%rax)
-   18001decb:	add    %al,(%rdx)
-   18001decd:	add    %al,(%rax)
-   18001decf:	add    %cl,%ah
-   18001ded1:	add    %al,(%rax)
-   18001ded3:	add    %al,(%rdx)
-   18001ded5:	add    %al,(%rax)
-   18001ded7:	add    %al,(%rdx)
-   18001ded9:	add    %al,(%rax)
-   18001dedb:	add    %bl,0x18000000(%rip)        # 0x19801dee1
-   18001dee1:	add    %al,(%rax)
-   18001dee3:	add    %al,(%rcx)
+   18001de58:	mov    $0x2,%bpl
+   18001de5b:	addb   $0x0,(%rcx)
+   18001de5e:	add    %al,(%rax)
+   18001de60:	shlb   $0x0,0x18002(%rcx)
+   18001de67:	add    %al,-0x4b(%rax)
+   18001de6a:	add    0x1(%rax),%al
+   18001de70:	shlb   $0x0,0x18002(%rcx)
+   18001de77:	add    %ah,%al
+   18001de79:	mov    $0x2,%al
+   18001de7b:	addb   $0x0,(%rcx)
+   18001de7e:	add    %al,(%rax)
+   18001de80:	mov    $0x2,%bpl
+   18001de83:	addb   $0x0,(%rcx)
+   18001de86:	add    %al,(%rax)
+   18001de88:	shlb   $0x0,0x18002(%rcx)
+   18001de8f:	add    %al,-0x4b(%rax)
+   18001de92:	add    0x1(%rax),%al
+   18001de98:	shlb   $0x0,0x18002(%rcx)
+   18001de9f:	add    %ah,%al
+   18001dea1:	mov    $0x2,%al
+   18001dea3:	addb   $0x0,(%rcx)
+   18001dea6:	add    %al,(%rax)
+   18001dea8:	mov    $0x2,%bpl
+   18001deab:	addb   $0x0,(%rcx)
+   18001deae:	add    %al,(%rax)
+   18001deb0:	shlb   $0x0,0x18002(%rcx)
+   18001deb7:	add    %al,-0x4b(%rax)
+   18001deba:	add    0x1(%rax),%al
+   18001dec0:	shlb   $0x0,0x18002(%rcx)
+   18001dec7:	add    %al,(%rax)
+   18001dec9:	mov    $0x2,%al
+   18001decb:	addb   $0x0,(%rcx)
+   18001dece:	add    %al,(%rax)
+   18001ded0:	mov    $0x2,%bpl
+   18001ded3:	addb   $0x0,(%rcx)
+   18001ded6:	add    %al,(%rax)
+   18001ded8:	shlb   $0x0,0x18002(%rcx)
+   18001dedf:	add    %dl,0x18002b6(%rax)
    18001dee5:	add    %al,(%rax)
-   18001dee7:	add    %dl,%cl
-   18001dee9:	add    %al,(%rax)
-   18001deeb:	add    %al,(%rdx)
-   18001deed:	add    %al,(%rax)
-   18001deef:	add    %ah,(%rdx)
-   18001def1:	add    %al,(%rax)
-   18001def3:	add    %ah,(%rax)
-   18001def5:	add    %al,(%rax)
-   18001def7:	add    %bl,(%rbx)
-   18001def9:	add    %al,(%rax)
-   18001defb:	add    %al,(%rdx)
-   18001defd:	add    %al,(%rax)
-   18001deff:	add    %dl,%ah
-   18001df01:	add    %al,(%rax)
-   18001df03:	add    %al,(%rdx)
-   18001df05:	add    %al,(%rax)
-   18001df07:	add    %al,(%rdx)
-   18001df09:	add    %al,(%rax)
-   18001df0b:	add    %ah,(%rdx)
-   18001df0d:	add    %al,(%rax)
-   18001df0f:	add    %bl,(%rbx)
-   18001df11:	add    %al,(%rax)
-   18001df13:	add    %al,(%rcx)
-   18001df15:	add    %al,(%rax)
-   18001df17:	add    %bl,%cl
-   18001df19:	add    %al,(%rax)
-   18001df1b:	add    %al,(%rdx)
-   18001df1d:	add    %al,(%rax)
-   18001df1f:	add    %ah,(%rdx)
-   18001df21:	add    %al,(%rax)
-   18001df23:	add    %ah,0x1d000000(%rip)        # 0x19d01df29
-   18001df29:	add    %al,(%rax)
-   18001df2b:	add    %al,(%rdx)
-   18001df2d:	add    %al,(%rax)
-   18001df2f:	add    %bl,%ah
-   18001df31:	add    %al,(%rax)
-   18001df33:	add    %al,(%rdx)
-   18001df35:	add    %al,(%rax)
-   18001df37:	add    %al,(%rdx)
-   18001df39:	add    %al,(%rax)
-   18001df3b:	add    %ah,(%rdi)
+   18001dee7:	add    %al,-0x4b(%rax)
+   18001deea:	add    0x1(%rax),%al
+   18001def0:	shlb   $0x0,0x18002(%rcx)
+   18001def7:	add    %ah,%al
+   18001def9:	mov    $0x2,%al
+   18001defb:	addb   $0x0,(%rcx)
+   18001defe:	add    %al,(%rax)
+   18001df00:	mov    $0x2,%bpl
+   18001df03:	addb   $0x0,(%rcx)
+   18001df06:	add    %al,(%rax)
+   18001df08:	shlb   $0x0,0x18002(%rcx)
+   18001df0f:	add    %al,-0x4b(%rax)
+   18001df12:	add    0x1(%rax),%al
+   18001df18:	shlb   $0x0,0x18002(%rcx)
+   18001df1f:	add    %al,(%rax)
+   18001df21:	mov    $0x2,%al
+   18001df23:	addb   $0x0,(%rcx)
+   18001df26:	add    %al,(%rax)
+   18001df28:	mov    $0x2,%bpl
+   18001df2b:	addb   $0x0,(%rcx)
+   18001df2e:	add    %al,(%rax)
+   18001df30:	shlb   $0x0,0x18002(%rcx)
+   18001df37:	add    %dl,0x18002b6(%rax)
    18001df3d:	add    %al,(%rax)
-   18001df3f:	add    %bl,0x1000000(%rip)        # 0x18101df45
-   18001df45:	add    %al,(%rax)
-   18001df47:	add    %ah,%cl
-   18001df49:	add    %al,(%rax)
-   18001df4b:	add    %al,(%rdx)
-   18001df4d:	add    %al,(%rax)
-   18001df4f:	add    %ah,(%rdx)
-   18001df51:	add    %al,(%rax)
-   18001df53:	add    %ch,(%rdx)
-   18001df55:	add    %al,(%rax)
-   18001df57:	add    %bl,(%rsi)
-   18001df59:	add    %al,(%rax)
-   18001df5b:	add    %al,(%rdx)
-   18001df5d:	add    %al,(%rax)
-   18001df5f:	add    %ah,%ah
-   18001df61:	add    %al,(%rax)
-   18001df63:	add    %al,(%rdx)
-   18001df65:	add    %al,(%rax)
-   18001df67:	add    %al,(%rdx)
-   18001df69:	add    %al,(%rax)
-   18001df6b:	add    %ch,(%rax,%rax,1)
-   18001df6e:	add    %al,(%rax)
-   18001df70:	(bad)
-   18001df71:	add    %al,(%rax)
-   18001df73:	add    %al,(%rcx)
-   18001df75:	add    %al,(%rax)
-   18001df77:	add    %ch,%cl
-   18001df79:	add    %al,(%rax)
-   18001df7b:	add    %al,(%rdx)
-   18001df7d:	add    %al,(%rax)
-   18001df7f:	add    %ah,(%rdx)
-   18001df81:	add    %al,(%rax)
-   18001df83:	add    %ch,(%rdi)
-   18001df85:	add    %al,(%rax)
-   18001df87:	add    %bl,(%rsi)
+   18001df3f:	add    %al,-0x4b(%rax)
+   18001df42:	add    0x1(%rax),%al
+   18001df48:	shlb   $0x0,0x18002(%rcx)
+   18001df4f:	add    %ah,%al
+   18001df51:	mov    $0x2,%al
+   18001df53:	addb   $0x0,(%rcx)
+   18001df56:	add    %al,(%rax)
+   18001df58:	mov    $0x2,%bpl
+   18001df5b:	addb   $0x0,(%rcx)
+   18001df5e:	add    %al,(%rax)
+   18001df60:	shlb   $0x0,0x18002(%rcx)
+   18001df67:	add    %dl,0x4e(%rcx)
+   18001df6a:	gs je  0x18001dfe4
+   18001df6d:	outsl  %ds:(%rsi),(%dx)
+   18001df6e:	jb     0x18001dfdb
+   18001df70:	push   %rdx
+   18001df71:	gs jo  0x18001dfe0
+   18001df74:	jns    0x18001dfa0
+   18001df76:	add    %al,(%rax)
+   18001df78:	push   %rcx
+   18001df79:	push   %rbx
+   18001df7a:	jae    0x18001dfe8
+   18001df7c:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001df7e:	outsb  %ds:(%rsi),(%dx)
+   18001df7f:	imul   $0x6172,0x75(%rdi),%sp
+   18001df85:	je     0x18001dff0
+   18001df87:	outsl  %ds:(%rsi),(%dx)
+   18001df88:	outsb  %ds:(%rsi),(%dx)
    18001df89:	add    %al,(%rax)
-   18001df8b:	add    %al,(%rdx)
+   18001df8b:	add    %al,(%rax)
    18001df8d:	add    %al,(%rax)
-   18001df8f:	add    %ch,%ah
-   18001df91:	add    %al,(%rax)
-   18001df93:	add    %al,(%rdx)
-   18001df95:	add    %al,(%rax)
-   18001df97:	add    %al,(%rdx)
-   18001df99:	add    %al,(%rax)
-   18001df9b:	add    %dh,(%rcx)
+   18001df8f:	add    %dl,0x44(%rcx)
+   18001df92:	(bad)
+   18001df93:	je     0x18001dffa
+   18001df95:	push   %rsp
+   18001df96:	imul   $0x0,0x65(%rbp),%ebp
    18001df9d:	add    %al,(%rax)
-   18001df9f:	add    %bl,(%rsi)
-   18001dfa1:	add    %al,(%rax)
-   18001dfa3:	add    %al,(%rdx)
-   18001dfa5:	add    %al,(%rax)
-   18001dfa7:	add    %dh,%cl
-   18001dfa9:	add    %al,(%rax)
-   18001dfab:	add    %al,(%rdx)
-   18001dfad:	add    %al,(%rax)
-   18001dfaf:	add    %al,(%rdx)
-   18001dfb1:	add    %al,(%rax)
-   18001dfb3:	add    %dh,(%rax,%rax,1)
-   18001dfb6:	add    %al,(%rax)
-   18001dfb8:	and    %eax,(%rax)
-   18001dfba:	add    %al,(%rax)
-   18001dfbc:	add    (%rax),%al
-   18001dfbe:	add    %al,(%rax)
-   18001dfc0:	testb  $0x0,(%rax)
-   18001dfc3:	add    %al,(%rdx)
-   18001dfc5:	add    %al,(%rax)
-   18001dfc7:	add    %al,(%rdx)
-   18001dfc9:	add    %al,(%rax)
-   18001dfcb:	add    %dh,(%rdi)
-   18001dfcd:	add    %al,(%rax)
-   18001dfcf:	add    %ah,(%rcx)
+   18001df9f:	add    %dl,0x41(%rcx)
+   18001dfa2:	(bad)
+   18001dfa7:	movsxd 0x41(%rdi,%rcx,2),%esi
+   18001dfab:	jne    0x18001e021
+   18001dfad:	push   $0x48510032
+   18001dfb2:	je     0x18001e028
+   18001dfb4:	jo     0x18001e003
+   18001dfb6:	jne    0x18001e024
+   18001dfb8:	je     0x18001e023
+   18001dfba:	push   %rax
+   18001dfbb:	(bad)
+   18001dfbc:	jb     0x18001e032
+   18001dfbe:	sub    (%rax),%al
+   18001dfc0:	push   %rcx
+   18001dfc1:	push   %rbx
+   18001dfc2:	jae    0x18001e030
+   18001dfc4:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001dfc6:	outsb  %ds:(%rsi),(%dx)
+   18001dfc7:	imul   $0x6172,0x75(%rdi),%sp
+   18001dfcd:	je     0x18001e038
+   18001dfcf:	outsl  %ds:(%rsi),(%dx)
+   18001dfd0:	outsb  %ds:(%rsi),(%dx)
    18001dfd1:	add    %al,(%rax)
-   18001dfd3:	add    %al,(%rcx)
+   18001dfd3:	add    %al,(%rax)
    18001dfd5:	add    %al,(%rax)
-   18001dfd7:	add    %bh,%bl
-   18001dfd9:	add    %al,(%rax)
-   18001dfdb:	add    %al,(%rdx)
-   18001dfdd:	add    %al,(%rax)
-   18001dfdf:	add    %ah,(%rdx)
-   18001dfe1:	add    %al,(%rax)
-   18001dfe3:	add    %bh,(%rdx)
-   18001dfe5:	add    %al,(%rax)
-   18001dfe7:	add    %ah,(%rcx)
-   18001dfe9:	add    %al,(%rax)
-   18001dfeb:	add    %al,(%rdx)
-   18001dfed:	add    %al,(%rax)
-   18001dfef:	add    %bh,%dh
-   18001dff1:	add    %al,(%rax)
-   18001dff3:	add    %al,(%rdx)
-   18001dff5:	add    %al,(%rax)
-   18001dff7:	add    %al,(%rdx)
-   18001dff9:	add    %al,(%rax)
-   18001dffb:	add    %bh,(%rax,%rax,1)
-   18001dffe:	add    %al,(%rax)
-   18001e000:	and    %eax,(%rax)
-   18001e002:	add    %al,(%rax)
-   18001e004:	add    (%rax),%al
+   18001dfd7:	add    %ah,0x0(%rcx)
+   18001dfda:	movsxd (%rax),%eax
+   18001dfdc:	movsxd (%rax),%eax
+   18001dfde:	add    %dh,%gs:0x0(%rbx)
+   18001dfe2:	jae    0x18001dfe4
+   18001dfe4:	pop    %rdi
+   18001dfe5:	add    %dh,0x6f(%rax,%rax,1)
+   18001dfe9:	add    %ch,0x0(%rbx)
+   18001dfec:	add    %ch,%gs:0x0(%rsi)
+	...
+   18001dff8:	(bad)
+   18001dff9:	add    %dh,0x0(%rax)
+   18001dffc:	imul   $0x6b005f,(%rax),%eax
+   18001e002:	add    %bh,%gs:0x0(%rcx)
    18001e006:	add    %al,(%rax)
-   18001e008:	add    (%rcx),%eax
-   18001e00a:	add    %al,(%rax)
-   18001e00c:	add    (%rax),%al
-   18001e00e:	add    %al,(%rax)
-   18001e010:	add    (%rax),%al
-   18001e012:	add    %al,(%rax)
-   18001e014:	(bad)
-   18001e015:	add    %al,(%rax)
-   18001e017:	add    %ah,(%rdx)
-   18001e019:	add    %al,(%rax)
-   18001e01b:	add    %al,(%rdx)
+   18001e008:	movsxd (%rax),%eax
+   18001e00a:	insb   (%dx),%es:(%rdi)
+   18001e00b:	add    %ch,0x0(%rcx)
+   18001e00e:	add    %ch,%gs:0x0(%rsi)
+   18001e012:	je     0x18001e014
+   18001e014:	pop    %rdi
+   18001e015:	add    %ch,0x0(%rcx)
+   18001e018:	add    %al,%fs:(%rax)
+   18001e01b:	add    %al,(%rax)
    18001e01d:	add    %al,(%rax)
-   18001e01f:	add    %cl,(%rax)
-   18001e021:	add    %eax,(%rax)
-   18001e023:	add    %al,(%rdx)
-   18001e025:	add    %al,(%rax)
-   18001e027:	add    %al,(%rdx)
-   18001e029:	add    %al,(%rax)
-   18001e02b:	add    %al,0x0(%rdx)
-   18001e02e:	add    %al,(%rax)
-   18001e030:	and    (%rax),%al
-   18001e032:	add    %al,(%rax)
-   18001e034:	add    %eax,(%rax)
-   18001e036:	add    %al,(%rax)
-   18001e038:	or     $0x2000001,%eax
+   18001e01f:	add    %ah,0x0(%rbx)
+   18001e022:	insb   (%dx),%es:(%rdi)
+   18001e023:	add    %ch,0x0(%rcx)
+   18001e026:	add    %ch,%gs:0x0(%rsi)
+   18001e02a:	je     0x18001e02c
+   18001e02c:	pop    %rdi
+   18001e02d:	add    %dh,0x0(%rbx)
+   18001e030:	add    %ah,%gs:0x0(%rbx)
+   18001e034:	jb     0x18001e036
+   18001e036:	add    %dh,%gs:0x0(%rax,%rax,1)
+   18001e03b:	add    %al,(%rax)
    18001e03d:	add    %al,(%rax)
-   18001e03f:	add    %ah,(%rdx)
-   18001e041:	add    %al,(%rax)
-   18001e043:	add    %al,0x0(%rbp)
-   18001e046:	add    %al,(%rax)
-   18001e048:	sub    (%rax),%eax
-   18001e04a:	add    %al,(%rax)
-   18001e04c:	or     (%rax),%al
-   18001e04e:	add    %al,(%rax)
-   18001e050:	add    (%rax),%eax
-   18001e052:	add    %al,(%rax)
-   18001e054:	sub    (%rax),%eax
-   18001e056:	add    %al,(%rax)
-   18001e058:	or     (%rax),%al
+   18001e03f:	add    %ah,0x0(%rbx)
+   18001e042:	outsl  %ds:(%rsi),(%dx)
+   18001e043:	add    %ah,0x65(%rax,%rax,1)
+	...
+   18001e04f:	add    %ah,0x0(%rbp)
+   18001e052:	jb     0x18001e054
+   18001e054:	jb     0x18001e056
+   18001e056:	outsl  %ds:(%rsi),(%dx)
+   18001e057:	add    %dh,0x0(%rdx)
    18001e05a:	add    %al,(%rax)
-   18001e05c:	add    $0x2b000000,%eax
-   18001e061:	add    %al,(%rax)
-   18001e063:	add    %cl,(%rdx)
-   18001e065:	add    %al,(%rax)
-   18001e067:	add    %al,(%rdi)
-   18001e069:	add    %al,(%rax)
-   18001e06b:	add    %ch,(%rbx)
-   18001e06d:	add    %al,(%rax)
-   18001e06f:	add    %cl,(%rdx)
-   18001e071:	add    %al,(%rax)
-   18001e073:	add    %cl,(%rcx)
-   18001e075:	add    %al,(%rax)
-   18001e077:	add    %ch,(%rbx)
-   18001e079:	add    %al,(%rax)
-   18001e07b:	add    %cl,(%rdx)
-   18001e07d:	add    %al,(%rax)
-   18001e07f:	add    %cl,(%rbx)
-   18001e081:	add    %al,(%rax)
-   18001e083:	add    %ch,(%rbx)
-   18001e085:	add    %al,(%rax)
-   18001e087:	add    %dl,(%rax)
-   18001e089:	add    %al,(%rax)
-   18001e08b:	add    %cl,0x2b000000(%rip)        # 0x1ab01e091
-   18001e091:	add    %al,(%rax)
-   18001e093:	add    %cl,(%rdx)
-   18001e095:	add    %al,(%rax)
-   18001e097:	add    %cl,(%rdi)
-   18001e099:	add    %al,(%rax)
-   18001e09b:	add    %ch,(%rbx)
-   18001e09d:	add    %al,(%rax)
-   18001e09f:	add    %dl,(%rcx)
-   18001e0a1:	add    %al,(%rax)
-   18001e0a3:	adcb   $0x0,(%rdx)
-   18001e0a6:	add    %al,(%rax)
-   18001e0a8:	sub    (%rax),%eax
-   18001e0aa:	add    %al,(%rax)
-   18001e0ac:	or     (%rax),%al
-   18001e0ae:	add    %al,(%rax)
-   18001e0b0:	or     (%rax),%al
-   18001e0b2:	add    %al,(%rax)
-   18001e0b4:	adc    %eax,(%rax)
-   18001e0b6:	add    %al,(%rax)
-   18001e0b8:	adc    (%rax),%eax
-   18001e0ba:	add    %al,(%rax)
-   18001e0bc:	adc    $0x0,%al
-   18001e0be:	add    %al,(%rax)
-   18001e0c0:	adc    $0x2b000000,%eax
-   18001e0c5:	add    %al,(%rax)
-   18001e0c7:	add    %cl,(%rax)
-   18001e0c9:	add    %al,(%rax)
-   18001e0cb:	add    %dl,(%rdi)
+   18001e05c:	add    %al,(%rax)
+   18001e05e:	add    %al,(%rax)
+   18001e060:	add    %dh,%gs:0x0(%rdx)
+   18001e064:	jb     0x18001e066
+   18001e066:	outsl  %ds:(%rsi),(%dx)
+   18001e067:	add    %dh,0x0(%rdx)
+   18001e06a:	pop    %rdi
+   18001e06b:	add    %ah,0x65(%rax,%rax,1)
+   18001e06f:	add    %dh,0x0(%rbx)
+   18001e072:	movsxd (%rax),%eax
+   18001e074:	jb     0x18001e076
+   18001e076:	imul   $0x740070,(%rax),%eax
+   18001e07c:	imul   $0x6e006f,(%rax),%eax
+   18001e082:	add    %al,(%rax)
+   18001e084:	add    %al,(%rax)
+   18001e086:	add    %al,(%rax)
+   18001e088:	add    %dh,%gs:0x0(%rdx)
+   18001e08c:	jb     0x18001e08e
+   18001e08e:	outsl  %ds:(%rsi),(%dx)
+   18001e08f:	add    %dh,0x0(%rdx)
+   18001e092:	pop    %rdi
+   18001e093:	add    %dh,0x0(%rbp)
+   18001e096:	jb     0x18001e098
+   18001e098:	imul   $0x0,(%rax),%eax
+   18001e09e:	add    %al,(%rax)
+   18001e0a0:	add    %bh,%gs:0x0(%rax)
+   18001e0a4:	jo     0x18001e0a6
+   18001e0a6:	imul   $0x650072,(%rax),%eax
+   18001e0ac:	jae    0x18001e0ae
+   18001e0ae:	pop    %rdi
+   18001e0af:	add    %ch,0x0(%rcx)
+   18001e0b2:	outsb  %ds:(%rsi),(%dx)
+   18001e0b3:	add    %al,(%rax)
+   18001e0b5:	add    %al,(%rax)
+   18001e0b7:	add    %ah,0x0(%rdi)
+   18001e0ba:	jb     0x18001e0bc
+   18001e0bc:	(bad)
+   18001e0bd:	add    %ch,0x0(%rsi)
+   18001e0c0:	je     0x18001e0c2
+   18001e0c2:	pop    %rdi
+   18001e0c3:	add    %dh,0x79(%rax,%rax,1)
+   18001e0c7:	add    %dh,0x0(%rax)
+   18001e0ca:	add    %al,%gs:(%rax)
    18001e0cd:	add    %al,(%rax)
-   18001e0cf:	add    %dl,(%rcx)
-   18001e0d1:	add    %al,(%rax)
-   18001e0d3:	add    %dl,(%rcx)
-   18001e0d5:	add    %al,(%rax)
-   18001e0d7:	add    %cl,(%rax)
-   18001e0d9:	add    %al,(%rax)
-   18001e0db:	add    %bl,(%rcx)
-   18001e0dd:	add    %al,(%rax)
-   18001e0df:	add    %bl,(%rdx)
-   18001e0e1:	add    %al,(%rax)
-   18001e0e3:	add    %dl,(%rcx)
-   18001e0e5:	add    %al,(%rax)
-   18001e0e7:	add    %dl,(%rcx)
-   18001e0e9:	add    %al,(%rax)
-   18001e0eb:	add    %bl,(%rcx)
-   18001e0ed:	add    %al,(%rax)
-   18001e0ef:	add    %bl,(%rax,%rax,1)
-   18001e0f2:	add    %al,0x11(%rax)
-   18001e0f8:	or     %al,(%rax)
-   18001e0fa:	add    %al,(%rax)
-   18001e0fc:	sbb    %eax,(%rax)
-   18001e0fe:	add    %al,(%rax)
-   18001e100:	sbb    (%rax),%al
-   18001e102:	add    %al,(%rax)
-   18001e104:	sbb    $0x0,%al
-   18001e106:	add    %al,0x11(%rax)
-   18001e10c:	sbb    %eax,(%rax)
+   18001e0cf:	add    %dh,0x0(%rdx)
+   18001e0d2:	add    %ah,%gs:0x69(%rax,%rax,1)
+   18001e0d7:	add    %dh,0x0(%rdx)
+   18001e0da:	add    %ah,%gs:0x0(%rbx)
+   18001e0de:	je     0x18001e0e0
+   18001e0e0:	pop    %rdi
+   18001e0e1:	add    %dh,0x0(%rbp)
+   18001e0e4:	jb     0x18001e0e6
+   18001e0e6:	imul   $0x0,(%rax),%eax
+   18001e0ec:	add    %al,(%rax)
+   18001e0ee:	add    %al,(%rax)
+   18001e0f0:	jb     0x18001e0f2
+   18001e0f2:	add    %ah,%gs:0x0(%rsi)
+   18001e0f6:	jb     0x18001e0f8
+   18001e0f8:	add    %dh,%gs:0x0(%rbx)
+   18001e0fc:	push   $0x74005f00
+   18001e101:	add    %ch,0x0(%rdi)
+   18001e104:	imul   $0x65,(%rax),%eax
+   18001e107:	add    %ch,0x0(%rsi)
+   18001e10a:	add    %al,(%rax)
+   18001e10c:	add    %al,(%rax)
    18001e10e:	add    %al,(%rax)
-   18001e110:	sbb    $0x0,%al
-   18001e112:	add    %al,0x11(%rax)
-   18001e118:	or     %al,(%rax)
-   18001e11a:	add    %al,(%rax)
-   18001e11c:	sbb    %eax,(%rax)
-   18001e11e:	add    %al,(%rax)
-   18001e120:	sbb    (%rax),%al
-   18001e122:	add    %al,(%rax)
-   18001e124:	sbb    $0x0,%al
-   18001e126:	add    %al,0x11(%rax)
-   18001e12c:	sbb    %eax,(%rax)
-   18001e12e:	add    %al,(%rax)
-   18001e130:	sbb    $0x0,%al
-   18001e132:	add    %al,0x11(%rax)
-   18001e138:	or     %al,(%rax)
-   18001e13a:	add    %al,(%rax)
-   18001e13c:	sbb    %eax,(%rax)
-   18001e13e:	add    %al,(%rax)
-   18001e140:	sbb    (%rax),%al
-   18001e142:	add    %al,(%rax)
-   18001e144:	sbb    $0x0,%al
-   18001e146:	add    %al,0x11(%rax)
-   18001e14c:	sbb    %eax,(%rax)
-   18001e14e:	add    %al,(%rax)
-   18001e150:	sbb    $0x0,%al
-   18001e152:	add    %al,0x11(%rax)
-   18001e158:	or     $0x0,%al
-   18001e15a:	add    %al,(%rax)
-   18001e15c:	sbb    %eax,(%rax)
-   18001e15e:	add    %al,(%rax)
-   18001e160:	(bad)
-   18001e161:	add    %al,(%rax)
-   18001e163:	add    %bl,(%rax,%rax,1)
-   18001e166:	add    %al,0x11(%rax)
-   18001e16c:	(bad)
-   18001e16d:	add    %al,(%rax)
-   18001e16f:	sbbb   $0x0,(%rcx)
-   18001e172:	add    %al,(%rax)
-   18001e174:	and    %al,(%rax)
-   18001e176:	add    %al,(%rax)
-   18001e178:	sbb    $0x0,%al
-   18001e17a:	add    %al,0x11(%rax)
-   18001e180:	or     %al,(%rax)
-   18001e182:	add    %al,(%rax)
-   18001e184:	sbb    %eax,(%rax)
-   18001e186:	add    %al,(%rax)
-   18001e188:	sbb    (%rax),%al
-   18001e18a:	add    %al,(%rax)
-   18001e18c:	sbb    $0x0,%al
-   18001e18e:	add    %al,0x11(%rax)
-   18001e194:	sbb    %eax,(%rax)
-   18001e196:	add    %al,(%rax)
-   18001e198:	sbb    $0x0,%al
-   18001e19a:	add    %al,0x11(%rax)
-   18001e1a0:	or     $0x0,%al
-   18001e1a2:	add    %al,(%rax)
-   18001e1a4:	sbb    %eax,(%rax)
-   18001e1a6:	add    %al,(%rax)
-   18001e1a8:	(bad)
-   18001e1a9:	add    %al,(%rax)
-   18001e1ab:	add    %bl,(%rax,%rax,1)
-   18001e1ae:	add    %al,0x11(%rax)
-   18001e1b4:	(bad)
-   18001e1b5:	add    %al,(%rax)
-   18001e1b7:	sbbb   $0x0,(%rcx)
-   18001e1ba:	add    %al,(%rax)
-   18001e1bc:	and    %al,(%rax)
+   18001e110:	jb     0x18001e112
+   18001e112:	add    %dh,%gs:0x0(%rbx)
+   18001e116:	jo     0x18001e118
+   18001e118:	outsl  %ds:(%rsi),(%dx)
+   18001e119:	add    %ch,0x0(%rsi)
+   18001e11c:	jae    0x18001e11e
+   18001e11e:	add    %bl,%gs:0x0(%rdi)
+   18001e122:	je     0x18001e124
+   18001e124:	jns    0x18001e126
+   18001e126:	jo     0x18001e128
+   18001e128:	add    %al,%gs:(%rax)
+   18001e12b:	add    %al,(%rax)
+   18001e12d:	add    %al,(%rax)
+   18001e12f:	add    %dh,0x0(%rbx)
+   18001e132:	movsxd (%rax),%eax
+   18001e134:	outsl  %ds:(%rsi),(%dx)
+   18001e135:	add    %dh,0x0(%rax)
+   18001e138:	add    %al,%gs:(%rax)
+   18001e13b:	add    %al,(%rax)
+   18001e13d:	add    %al,(%rax)
+   18001e13f:	add    %dh,0x0(%rbx)
+   18001e142:	je     0x18001e144
+   18001e144:	(bad)
+   18001e145:	add    %dh,0x65(%rax,%rax,1)
+   18001e149:	add    %al,(%rax)
+   18001e14b:	add    %al,(%rax)
+   18001e14d:	add    %al,(%rax)
+   18001e14f:	add    %dh,0x6f(%rax,%rax,1)
+   18001e153:	add    %ch,0x0(%rbx)
+   18001e156:	add    %ch,%gs:0x0(%rsi)
+   18001e15a:	pop    %rdi
+   18001e15b:	add    %dh,0x79(%rax,%rax,1)
+   18001e15f:	add    %dh,0x0(%rax)
+   18001e162:	add    %al,%gs:(%rax)
+	...
+   18001e175:	add    %al,(%rax)
+   18001e177:	add    %ah,0x1800021(%rax)
+   18001e17d:	add    %al,(%rax)
+   18001e17f:	add    %dh,0x18001e1(%rax)
+   18001e185:	add    %al,(%rax)
+   18001e187:	add    %dh,-0x28(%rax)
+   18001e18a:	add    %eax,0x1(%rax)
+   18001e190:	push   %rax
+   18001e191:	pop    %rsp
+   18001e192:	add    %al,0x1(%rax)
+	...
+   18001e1a0:	xor    %bl,%ch
+   18001e1a2:	add    %eax,0x1(%rax)
+	...
+   18001e1b0:	sbb    %al,(%rcx)
+   18001e1b2:	add    %al,(%rax)
+   18001e1b4:	sldt   (%rax)
+   18001e1b7:	add    %ch,(%rax)
+   18001e1b9:	add    %eax,(%rax)
+   18001e1bb:	add    %cl,(%rax,%rax,1)
    18001e1be:	add    %al,(%rax)
-   18001e1c0:	sbb    $0x0,%al
-   18001e1c2:	add    %al,0x11(%rax)
-   18001e1c8:	or     %al,(%rax)
-   18001e1ca:	add    %al,(%rax)
-   18001e1cc:	sbb    %eax,(%rax)
-   18001e1ce:	add    %al,(%rax)
-   18001e1d0:	sbb    (%rax),%al
-   18001e1d2:	add    %al,(%rax)
-   18001e1d4:	sbb    $0x0,%al
-   18001e1d6:	add    %al,0x11(%rax)
-   18001e1dc:	sbb    %eax,(%rax)
+   18001e1c0:	xor    $0x1,%eax
+   18001e1c5:	add    %al,(%rax)
+   18001e1c7:	add    %dh,(%rsi)
+   18001e1c9:	add    %eax,(%rax)
+   18001e1cb:	add    %al,0x3c000000(%rip)        # 0x1bc01e1d1
+   18001e1d1:	add    %eax,(%rax)
+   18001e1d3:	add    %dl,(%rax)
+   18001e1d5:	add    %al,(%rax)
+   18001e1d7:	add    %cl,0x1(%rbp)
+   18001e1da:	add    %al,(%rax)
+   18001e1dc:	or     %eax,(%rax)
    18001e1de:	add    %al,(%rax)
-   18001e1e0:	add    (%rax),%eax
-   18001e1e2:	add    %al,(%rax)
-   18001e1e4:	or     (%rax),%al
-   18001e1e6:	add    %al,(%rax)
-   18001e1e8:	add    0x1(%rcx),%edx
-	...
-   18001e1f3:	add    %al,0xa000000(%rip)        # 0x18a01e1f9
-   18001e1f9:	add    %al,(%rax)
-   18001e1fb:	add    %al,(%rbx)
-   18001e1fd:	push   %rcx
-   18001e1fe:	add    %eax,(%rax)
-   18001e200:	add    %eax,(%rax)
-   18001e202:	add    %al,(%rax)
-   18001e204:	add    %al,(%rax)
-   18001e206:	add    %al,(%rax)
-   18001e208:	or     %eax,(%rax)
-   18001e20a:	add    %al,(%rax)
-   18001e20c:	or     (%rax),%al
-   18001e20e:	add    %al,(%rax)
-   18001e210:	add    0x1(%rcx),%edx
-   18001e213:	add    %al,(%rbx)
+   18001e1e0:	push   %rdi
+   18001e1e1:	add    %eax,(%rax)
+   18001e1e3:	add    %dl,(%rbx)
+   18001e1e5:	add    %al,(%rax)
+   18001e1e7:	add    %ch,0x1(%rbx)
+   18001e1ea:	add    %al,(%rax)
+   18001e1ec:	or     $0x0,%al
+   18001e1ee:	add    %al,(%rax)
+   18001e1f0:	js     0x18001e1f3
+   18001e1f2:	add    %al,(%rax)
+   18001e1f4:	and    %al,(%rax)
+   18001e1f6:	add    %al,(%rax)
+   18001e1f8:	cltd
+   18001e1f9:	add    %eax,(%rax)
+   18001e1fb:	add    %bl,(%rcx)
+   18001e1fd:	add    %al,(%rax)
+   18001e1ff:	add    %dh,0xc000001(%rbx)
+   18001e205:	add    %al,(%rax)
+   18001e207:	add    %al,%al
+   18001e209:	add    %eax,(%rax)
+   18001e20b:	add    %al,-0x3a000000(%rip)        # 0x14601e211
+   18001e211:	add    %eax,(%rax)
+   18001e213:	add    %dl,(%rbx)
    18001e215:	add    %al,(%rax)
-   18001e217:	add    %al,(%rax)
-   18001e219:	add    %al,(%rax)
-   18001e21b:	add    %cl,(%rbx)
+   18001e217:	add    %bl,%dl
+   18001e219:	add    %eax,(%rax)
+   18001e21b:	add    %cl,(%rdx)
    18001e21d:	add    %al,(%rax)
-   18001e21f:	add    %cl,(%rdx)
-   18001e221:	add    %al,(%rax)
-   18001e223:	add    %al,(%rbx)
-   18001e225:	push   %rcx
-   18001e226:	add    %eax,(%rax)
-   18001e228:	add    $0x0,%al
-   18001e22a:	add    %al,(%rax)
-   18001e22c:	add    %al,(%rax)
+   18001e21f:	add    %ah,%ch
+   18001e221:	add    %eax,(%rax)
+   18001e223:	add    %dl,(%rbx)
+   18001e225:	add    %al,(%rax)
+   18001e227:	add    %bh,%cl
+   18001e229:	add    %eax,(%rax)
+   18001e22b:	add    %cl,(%rax,%rax,1)
    18001e22e:	add    %al,(%rax)
-   18001e230:	or     $0x10000000,%eax
+   18001e230:	(bad)
+   18001e231:	add    (%rax),%al
+   18001e233:	add    %dl,(%rdi)
    18001e235:	add    %al,(%rax)
-   18001e237:	add    %al,(%rcx)
-   18001e239:	push   %rax
-   18001e23a:	add    %eax,(%rax)
-   18001e23c:	add    $0x0,%eax
-   18001e241:	add    %al,(%rax)
-   18001e243:	add    %cl,(%rdi)
-   18001e245:	add    %al,(%rax)
-   18001e247:	add    %cl,(%rdx)
-   18001e249:	add    %al,(%rax)
-   18001e24b:	add    %al,(%rbx)
-   18001e24d:	push   %rcx
-   18001e24e:	add    %eax,(%rax)
-   18001e250:	(bad)
-	...
-   18001e25d:	add    %al,(%rax)
-   18001e25f:	add    %ah,0x18002b2(%rax)
-   18001e265:	add    %al,(%rax)
-   18001e267:	add    %ah,0x18002b2(%rax)
-   18001e26d:	add    %al,(%rax)
-   18001e26f:	add    %ah,0x18002b2(%rax)
+   18001e237:	add    %bl,(%rsi)
+   18001e239:	add    (%rax),%al
+   18001e23b:	add    %dl,(%rcx)
+   18001e23d:	add    %al,(%rax)
+   18001e23f:	add    %dh,(%rax)
+   18001e241:	add    (%rax),%al
+   18001e243:	add    %cl,0x3e000000(%rip)        # 0x1be01e249
+   18001e249:	add    (%rax),%al
+   18001e24b:	add    %al,0x44000000(%rip)        # 0x1c401e251
+   18001e251:	add    (%rax),%al
+   18001e253:	add    %dl,(%rax)
+   18001e255:	add    %al,(%rax)
+   18001e257:	add    %dl,0x2(%rbp)
+   18001e25a:	add    %al,(%rax)
+   18001e25c:	add    (%rax),%eax
+   18001e25e:	add    %al,(%rax)
+   18001e260:	pop    %rcx
+   18001e261:	add    (%rax),%al
+   18001e263:	add    %bl,0x77000000(%rip)        # 0x1f701e269
+   18001e269:	add    (%rax),%al
+   18001e26b:	add    %al,(%rax,%rax,1)
+   18001e26e:	add    %al,(%rax)
+   18001e270:	jl     0x18001e274
+   18001e272:	add    %al,(%rax)
+   18001e274:	(bad)
    18001e275:	add    %al,(%rax)
-   18001e277:	add    %ah,0x18002b2(%rax)
+   18001e277:	add    %dl,0x3000002(%rbx)
    18001e27d:	add    %al,(%rax)
-   18001e27f:	add    %dh,0x18002b5(%rax)
+   18001e27f:	add    %dl,0xa000002(%rdi)
    18001e285:	add    %al,(%rax)
-   18001e287:	add    %ah,0x18002b2(%rax)
+   18001e287:	add    %ah,0x4000002(%rdx)
    18001e28d:	add    %al,(%rax)
-   18001e28f:	add    %ah,(%rax)
-   18001e291:	mov    $0x2,%dh
-   18001e293:	addb   $0x0,(%rcx)
-   18001e296:	add    %al,(%rax)
-   18001e298:	lock mov $0x2,%bl
-   18001e29b:	addb   $0x0,(%rcx)
-   18001e29e:	add    %al,(%rax)
-   18001e2a0:	movabs 0xf0000000018002b2,%al
-   18001e2a9:	mov    $0x2,%bl
-   18001e2ab:	addb   $0x0,(%rcx)
-   18001e2ae:	add    %al,(%rax)
-   18001e2b0:	movabs 0xf0000000018002b2,%al
-   18001e2b9:	mov    $0x2,%bl
-   18001e2bb:	addb   $0x0,(%rcx)
-   18001e2be:	add    %al,(%rax)
-   18001e2c0:	movabs 0xf0000000018002b2,%al
-   18001e2c9:	mov    $0x2,%bl
-   18001e2cb:	addb   $0x0,(%rcx)
-   18001e2ce:	add    %al,(%rax)
-   18001e2d0:	movabs 0xf0000000018002b2,%al
-   18001e2d9:	mov    $0x2,%bl
-   18001e2db:	addb   $0x0,(%rcx)
-   18001e2de:	add    %al,(%rax)
-   18001e2e0:	movabs 0xf0000000018002b2,%al
-   18001e2e9:	mov    $0x2,%bl
-   18001e2eb:	addb   $0x0,(%rcx)
-   18001e2ee:	add    %al,(%rax)
-   18001e2f0:	mov    $0xb5,%al
-   18001e2f2:	add    0x1(%rax),%al
-   18001e2f8:	lock mov $0x2,%bl
-   18001e2fb:	addb   $0x0,(%rcx)
-   18001e2fe:	add    %al,(%rax)
-   18001e300:	movabs 0xf0000000018002b2,%al
-   18001e309:	mov    $0x2,%bl
-   18001e30b:	addb   $0x0,(%rcx)
-   18001e30e:	add    %al,(%rax)
-   18001e310:	add    %dh,0x18002(%rdi)
-   18001e316:	add    %al,(%rax)
-   18001e318:	lock mov $0x2,%bl
-   18001e31b:	addb   $0x0,(%rcx)
-   18001e31e:	add    %al,(%rax)
-   18001e320:	movabs 0xa0000000018002b2,%al
-   18001e329:	mov    $0x2,%dl
-   18001e32b:	addb   $0x0,(%rcx)
-   18001e32e:	add    %al,(%rax)
-   18001e330:	shlb   $0x0,0x18002(%rcx)
-   18001e337:	add    %dh,%al
-   18001e339:	mov    $0x2,%bl
-   18001e33b:	addb   $0x0,(%rcx)
-   18001e33e:	add    %al,(%rax)
-   18001e340:	loopne 0x18001e2f2
-   18001e342:	add    0x1(%rax),%al
-   18001e348:	shlb   $0x0,0x18002(%rcx)
-   18001e34f:	add    %al,%al
-   18001e351:	mov    $0x2,%cl
-   18001e353:	addb   $0x0,(%rcx)
-   18001e356:	add    %al,(%rax)
-   18001e358:	loopne 0x18001e30a
-   18001e35a:	add    0x1(%rax),%al
-   18001e360:	shlb   $0x0,0x18002(%rcx)
-   18001e367:	add    %al,%al
-   18001e369:	mov    $0x2,%cl
-   18001e36b:	addb   $0x0,(%rcx)
-   18001e36e:	add    %al,(%rax)
-   18001e370:	mov    $0x2,%bpl
-   18001e373:	addb   $0x0,(%rcx)
-   18001e376:	add    %al,(%rax)
-   18001e378:	shlb   $0x0,0x18002(%rcx)
-   18001e37f:	add    %ah,%al
-   18001e381:	mov    $0x2,%al
-   18001e383:	addb   $0x0,(%rcx)
-   18001e386:	add    %al,(%rax)
-   18001e388:	mov    $0x2,%bpl
-   18001e38b:	addb   $0x0,(%rcx)
-   18001e38e:	add    %al,(%rax)
-   18001e390:	shlb   $0x0,0x18002(%rcx)
-   18001e397:	add    %al,-0x4b(%rax)
-   18001e39a:	add    0x1(%rax),%al
-   18001e3a0:	shlb   $0x0,0x18002(%rcx)
-   18001e3a7:	add    %ah,%al
-   18001e3a9:	mov    $0x2,%al
-   18001e3ab:	addb   $0x0,(%rcx)
-   18001e3ae:	add    %al,(%rax)
-   18001e3b0:	mov    $0x2,%bpl
-   18001e3b3:	addb   $0x0,(%rcx)
-   18001e3b6:	add    %al,(%rax)
-   18001e3b8:	shlb   $0x0,0x18002(%rcx)
-   18001e3bf:	add    %al,-0x4b(%rax)
-   18001e3c2:	add    0x1(%rax),%al
-   18001e3c8:	shlb   $0x0,0x18002(%rcx)
-   18001e3cf:	add    %ah,%al
-   18001e3d1:	mov    $0x2,%al
-   18001e3d3:	addb   $0x0,(%rcx)
-   18001e3d6:	add    %al,(%rax)
-   18001e3d8:	mov    $0x2,%bpl
-   18001e3db:	addb   $0x0,(%rcx)
-   18001e3de:	add    %al,(%rax)
-   18001e3e0:	shlb   $0x0,0x18002(%rcx)
-   18001e3e7:	add    %al,-0x4b(%rax)
-   18001e3ea:	add    0x1(%rax),%al
-   18001e3f0:	shlb   $0x0,0x18002(%rcx)
-   18001e3f7:	add    %al,(%rax)
-   18001e3f9:	mov    $0x2,%al
-   18001e3fb:	addb   $0x0,(%rcx)
-   18001e3fe:	add    %al,(%rax)
-   18001e400:	mov    $0x2,%bpl
-   18001e403:	addb   $0x0,(%rcx)
-   18001e406:	add    %al,(%rax)
-   18001e408:	shlb   $0x0,0x18002(%rcx)
-   18001e40f:	add    %dl,0x18002b6(%rax)
-   18001e415:	add    %al,(%rax)
-   18001e417:	add    %al,-0x4b(%rax)
-   18001e41a:	add    0x1(%rax),%al
-   18001e420:	shlb   $0x0,0x18002(%rcx)
-   18001e427:	add    %ah,%al
-   18001e429:	mov    $0x2,%al
-   18001e42b:	addb   $0x0,(%rcx)
-   18001e42e:	add    %al,(%rax)
-   18001e430:	mov    $0x2,%bpl
-   18001e433:	addb   $0x0,(%rcx)
-   18001e436:	add    %al,(%rax)
-   18001e438:	shlb   $0x0,0x18002(%rcx)
-   18001e43f:	add    %al,-0x4b(%rax)
-   18001e442:	add    0x1(%rax),%al
-   18001e448:	shlb   $0x0,0x18002(%rcx)
-   18001e44f:	add    %al,(%rax)
-   18001e451:	mov    $0x2,%al
-   18001e453:	addb   $0x0,(%rcx)
-   18001e456:	add    %al,(%rax)
-   18001e458:	mov    $0x2,%bpl
-   18001e45b:	addb   $0x0,(%rcx)
-   18001e45e:	add    %al,(%rax)
-   18001e460:	shlb   $0x0,0x18002(%rcx)
-   18001e467:	add    %dl,0x18002b6(%rax)
-   18001e46d:	add    %al,(%rax)
-   18001e46f:	add    %al,-0x4b(%rax)
-   18001e472:	add    0x1(%rax),%al
-   18001e478:	shlb   $0x0,0x18002(%rcx)
-   18001e47f:	add    %ah,%al
-   18001e481:	mov    $0x2,%al
-   18001e483:	addb   $0x0,(%rcx)
-   18001e486:	add    %al,(%rax)
-   18001e488:	mov    $0x2,%bpl
-   18001e48b:	addb   $0x0,(%rcx)
-   18001e48e:	add    %al,(%rax)
-   18001e490:	shlb   $0x0,0x18002(%rcx)
-   18001e497:	add    %bh,0x18001fd(%rax)
-   18001e49d:	add    %al,(%rax)
-   18001e49f:	add    %ah,(%rax)
-   18001e4a1:	jbe    0x18001e4a3
-   18001e4a3:	addb   $0x0,(%rcx)
-   18001e4a6:	add    %al,(%rax)
-   18001e4a8:	and    %bh,0x0(%rbp)
+   18001e28f:	add    %ah,0xe000002(%rdi)
+   18001e295:	add    %al,(%rax)
+   18001e297:	add    %dh,0x3000002(%rsi)
+   18001e29d:	add    %al,(%rax)
+   18001e29f:	add    %bh,0x4000002(%rdx)
+   18001e2a5:	add    %al,(%rax)
+   18001e2a7:	add    %bh,0xf000002(%rdi)
+   18001e2ad:	add    %al,(%rax)
+   18001e2af:	add    %cl,%bh
+   18001e2b1:	add    (%rax),%al
+   18001e2b3:	add    %cl,(%rcx)
+   18001e2b5:	add    %al,(%rax)
+   18001e2b7:	add    %bl,%cl
+   18001e2b9:	add    (%rax),%al
+   18001e2bb:	add    %al,(%rbx)
+   18001e2bd:	add    %al,(%rax)
+   18001e2bf:	add    %bl,%ch
+   18001e2c1:	add    (%rax),%al
+   18001e2c3:	add    %cl,(%rsi)
+   18001e2c5:	add    %al,(%rax)
+   18001e2c7:	add    %dl,0x41(%rcx)
+   18001e2ca:	(bad)
+   18001e2cf:	movsxd 0x41(%rdi,%rcx,2),%esi
+   18001e2d3:	jne    0x18001e349
+   18001e2d5:	push   $0x63730032
+   18001e2da:	outsl  %ds:(%rsi),(%dx)
+   18001e2db:	jo     0x18001e342
+   18001e2dd:	rex.XB push $0x65676e61
+   18001e2e3:	add    %al,%fs:(%rax)
+   18001e2e6:	jae    0x18001e34b
+   18001e2e8:	outsl  %ds:(%rsi),(%dx)
+   18001e2e9:	jo     0x18001e350
+   18001e2eb:	add    %dh,0x73(%rbp)
+   18001e2ee:	gs jb  0x18001e332
+   18001e2f1:	outsb  %gs:(%esi),(%dx)
+   18001e2f4:	je     0x18001e339
+   18001e2f6:	push   $0x65676e61
+   18001e2fb:	add    %dh,%fs:0x73(%rbp)
+   18001e2ff:	gs jb  0x18001e343
+   18001e302:	outsb  %gs:(%esi),(%dx)
+   18001e305:	je     0x18001e307
+   18001e307:	jb     0x18001e36e
+   18001e309:	jae    0x18001e37b
+   18001e30b:	outsl  %ds:(%rsi),(%dx)
+   18001e30c:	outsb  %ds:(%rsi),(%dx)
+   18001e30d:	jae    0x18001e374
+   18001e30f:	push   %rsp
+   18001e310:	jns    0x18001e382
+   18001e312:	gs rex.XB push $0x65676e61
+   18001e319:	add    %dh,%fs:0x65(%rdx)
+   18001e31d:	jae    0x18001e38f
+   18001e31f:	outsl  %ds:(%rsi),(%dx)
+   18001e320:	outsb  %ds:(%rsi),(%dx)
+   18001e321:	jae    0x18001e388
+   18001e323:	push   %rsp
+   18001e324:	jns    0x18001e396
+   18001e326:	add    %ah,%gs:0x6c(%rbx)
+   18001e32a:	imul   $0x65644974,0x6e(%rbp),%esp
+   18001e331:	outsb  %ds:(%rsi),(%dx)
+   18001e332:	je     0x18001e39d
+   18001e334:	imul   $0x6853,0x72(%rbp),%sp
+   18001e33a:	(bad)
+   18001e33b:	jb     0x18001e3a2
+   18001e33d:	fs rex.WXB
+   18001e33f:	gs jns 0x18001e385
+   18001e342:	push   $0x65676e61
+   18001e347:	add    %ah,%fs:0x6c(%rbx)
+   18001e34b:	imul   $0x65644974,0x6e(%rbp),%esp
+   18001e352:	outsb  %ds:(%rsi),(%dx)
+   18001e353:	je     0x18001e3be
+   18001e355:	imul   $0x6853,0x72(%rbp),%sp
+   18001e35b:	(bad)
+   18001e35c:	jb     0x18001e3c3
+   18001e35e:	fs rex.WXB
+   18001e360:	gs jns 0x18001e363
+   18001e363:	jae    0x18001e3d9
+   18001e365:	(bad)
+   18001e366:	je     0x18001e3cd
+   18001e368:	rex.XB push $0x65676e61
+   18001e36e:	add    %dh,%fs:0x74(%rbx)
+   18001e372:	(bad)
+   18001e373:	je     0x18001e3da
+   18001e375:	add    %ah,0x78(%rbp)
+   18001e378:	jo     0x18001e3e3
+   18001e37a:	jb     0x18001e3dd
+   18001e37c:	je     0x18001e3e7
+   18001e37e:	outsl  %ds:(%rsi),(%dx)
+   18001e37f:	outsb  %ds:(%rsi),(%dx)
+   18001e380:	rex.B je 0x18001e3c6
+   18001e383:	push   $0x65676e61
+   18001e388:	add    %ah,%fs:0x78(%rbp)
+   18001e38c:	jo     0x18001e3f7
+   18001e38e:	jb     0x18001e3f1
+   18001e390:	je     0x18001e3fb
+   18001e392:	outsl  %ds:(%rsi),(%dx)
+   18001e393:	outsb  %ds:(%rsi),(%dx)
+   18001e394:	add    %dh,0x65(%rdx)
+   18001e397:	data16 jb 0x18001e3ff
+   18001e39a:	jae    0x18001e404
+   18001e39c:	push   %rsp
+   18001e39d:	outsl  %ds:(%rsi),(%dx)
+   18001e39e:	imul   $0x43,0x6e(%rbp),%esp
+   18001e3a2:	push   $0x65676e61
+   18001e3a7:	add    %dh,%fs:0x65(%rdx)
+   18001e3ab:	data16 jb 0x18001e413
+   18001e3ae:	jae    0x18001e418
+   18001e3b0:	push   %rsp
+   18001e3b1:	outsl  %ds:(%rsi),(%dx)
+   18001e3b2:	imul   $0x0,0x6e(%rbp),%esp
+   18001e3b6:	jae    0x18001e42b
+   18001e3b8:	insb   (%dx),%es:(%rdi)
+   18001e3b9:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001e3bb:	outsb  %ds:(%rsi),(%dx)
+   18001e3bc:	imul   $0x6172,0x75(%rdi),%sp
+   18001e3c2:	je     0x18001e42d
+   18001e3c4:	outsl  %ds:(%rsi),(%dx)
+   18001e3c5:	outsb  %ds:(%rsi),(%dx)
+   18001e3c6:	rex.XB push $0x65676e61
+   18001e3cc:	add    %dl,%fs:0x53(%rcx)
+   18001e3d0:	jae    0x18001e43e
+   18001e3d2:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001e3d4:	outsb  %ds:(%rsi),(%dx)
+   18001e3d5:	imul   $0x6172,0x75(%rdi),%sp
+   18001e3db:	je     0x18001e446
+   18001e3dd:	outsl  %ds:(%rsi),(%dx)
+   18001e3de:	outsb  %ds:(%rsi),(%dx)
+   18001e3df:	add    %ah,0x6f(%rbx)
+   18001e3e2:	outsb  %ds:(%rsi),(%dx)
+   18001e3e3:	imul   $0x6172,0x75(%rdi),%sp
+   18001e3e9:	je     0x18001e454
+   18001e3eb:	outsl  %ds:(%rsi),(%dx)
+   18001e3ec:	outsb  %ds:(%rsi),(%dx)
+   18001e3ed:	add    %ah,0x72(%rbp)
+   18001e3f0:	jb     0x18001e461
+   18001e3f2:	jb     0x18001e3f4
+   18001e3f4:	gs jb  0x18001e469
+   18001e3f7:	outsl  %ds:(%rsi),(%dx)
+   18001e3f8:	jb     0x18001e43e
+   18001e3fa:	gs jae 0x18001e460
+   18001e3fd:	jb     0x18001e468
+   18001e3ff:	jo     0x18001e475
+   18001e401:	imul   $0x69727500,0x6e(%rdi),%ebp
+   18001e408:	add    %ah,0x75(%rcx)
+   18001e40b:	je     0x18001e475
+   18001e40d:	outsl  %ds:(%rsi),(%dx)
+   18001e40e:	jb     0x18001e479
+   18001e410:	jp     0x18001e473
+   18001e412:	je     0x18001e47d
+   18001e414:	outsl  %ds:(%rsi),(%dx)
+   18001e415:	outsb  %ds:(%rsi),(%dx)
+   18001e416:	rex.XB (bad)
+   18001e418:	insb   (%dx),%es:(%rdi)
+   18001e419:	insb   (%dx),%es:(%rdi)
+   18001e41a:	(bad)
+   18001e41c:	movsxd 0x52(%rbx),%ebp
+   18001e41f:	movsxd %gs:0x69(%rbp),%esp
+   18001e423:	jbe    0x18001e48a
+   18001e425:	add    %ah,%fs:0x74(%rcx,%riz,2)
+   18001e42a:	(bad)
+   18001e42b:	add    %ah,0x72(%rbx)
+   18001e42e:	gs (bad)
+   18001e430:	je     0x18001e497
+   18001e432:	rex.B jne 0x18001e4a9
+   18001e435:	push   $0x69746e65
+   18001e43a:	movsxd 0x74(%rcx),%esp
+   18001e43d:	gs fs push %rbp
+   18001e440:	jb     0x18001e4ae
+   18001e442:	add    %dh,0x72(%rbp)
+   18001e445:	insb   (%dx),%es:(%rdi)
+   18001e446:	add    %dh,0x61(%rax)
+   18001e449:	jb     0x18001e4ac
+   18001e44b:	insl   (%dx),%es:(%rdi)
+   18001e44c:	gs je  0x18001e4b4
+   18001e44f:	jb     0x18001e4c4
+   18001e451:	add    %ch,0x65(%rax)
+   18001e454:	(bad)
+   18001e455:	add    %dl,%fs:0x4e(%rcx)
+   18001e459:	gs je  0x18001e4d3
+   18001e45c:	outsl  %ds:(%rsi),(%dx)
+   18001e45d:	jb     0x18001e4ca
+   18001e45f:	push   %rdx
+   18001e460:	gs jo  0x18001e4cf
+   18001e463:	jns    0x18001e48f
+   18001e465:	add    %ah,0x65(%rdi)
+   18001e468:	je     0x18001e46a
+   18001e46a:	jo     0x18001e4db
+   18001e46c:	jae    0x18001e4e2
+   18001e46e:	add    %dl,0x48(%rcx)
+   18001e471:	je     0x18001e4e7
+   18001e473:	jo     0x18001e4c2
+   18001e475:	jne    0x18001e4e3
+   18001e477:	je     0x18001e4e2
+   18001e479:	push   %rax
+   18001e47a:	(bad)
+   18001e47b:	jb     0x18001e4f1
+   18001e47d:	sub    (%rax),%al
+   18001e47f:	insl   (%dx),%es:(%rdi)
+   18001e480:	jne    0x18001e4ee
+   18001e482:	je     0x18001e4ed
+   18001e484:	push   %rax
+   18001e485:	(bad)
+   18001e486:	jb     0x18001e4fc
+   18001e488:	add    %dh,0x75(%rax)
+   18001e48b:	je     0x18001e48d
+   18001e48d:	fs gs insb (%dx),%es:(%rdi)
+   18001e490:	gs je  0x18001e4f8
+   18001e493:	push   %rdx
+   18001e494:	gs jae 0x18001e506
+   18001e497:	jne    0x18001e50b
+   18001e499:	movsxd 0x0(%rbp),%esp
+   18001e49c:	add    %al,(%rax)
+   18001e49e:	add    %al,(%rax)
+   18001e4a0:	mov    $0x18001fd,%eax
+   18001e4a5:	add    %al,(%rax)
+   18001e4a7:	add    %ah,(%rax)
+   18001e4a9:	jbe    0x18001e4ab
    18001e4ab:	addb   $0x0,(%rcx)
    18001e4ae:	add    %al,(%rax)
-   18001e4b0:	cmpb   $0x1,-0x80(%rax,%rax,1)
-   18001e4b5:	add    %al,(%rax)
-   18001e4b7:	add    %dl,0x180006b(%rax)
+   18001e4b0:	and    %bh,0x0(%rbp)
+   18001e4b3:	addb   $0x0,(%rcx)
+   18001e4b6:	add    %al,(%rax)
+   18001e4b8:	cmpb   $0x1,-0x80(%rax,%rax,1)
    18001e4bd:	add    %al,(%rax)
-   18001e4bf:	add    %dh,0x1800192(%rax)
+   18001e4bf:	add    %dl,0x180006b(%rax)
    18001e4c5:	add    %al,(%rax)
-   18001e4c7:	add    %al,%al
-   18001e4c9:	xchg   %eax,%edx
-   18001e4ca:	add    %eax,0x1(%rax)
-   18001e4d0:	loopne 0x18001e464
+   18001e4c7:	add    %dh,0x1800192(%rax)
+   18001e4cd:	add    %al,(%rax)
+   18001e4cf:	add    %al,%al
+   18001e4d1:	xchg   %eax,%edx
    18001e4d2:	add    %eax,0x1(%rax)
-   18001e4d8:	jo     0x18001e46c
+   18001e4d8:	loopne 0x18001e46c
    18001e4da:	add    %eax,0x1(%rax)
-   18001e4e0:	nop
-   18001e4e1:	xchg   %eax,%edx
+   18001e4e0:	jo     0x18001e474
    18001e4e2:	add    %eax,0x1(%rax)
-   18001e4e8:	adcb   $0x0,0x18001(%rdx)
-   18001e4ef:	add    %ah,0x1800192(%rax)
-   18001e4f5:	add    %al,(%rax)
-   18001e4f7:	add    %dl,0x1800074(%rax)
+   18001e4e8:	nop
+   18001e4e9:	xchg   %eax,%edx
+   18001e4ea:	add    %eax,0x1(%rax)
+   18001e4f0:	adcb   $0x0,0x18001(%rdx)
+   18001e4f7:	add    %ah,0x1800192(%rax)
    18001e4fd:	add    %al,(%rax)
-   18001e4ff:	add    %dh,0x73(%rax)
-   18001e502:	add    %al,0x1(%rax)
-   18001e508:	rex jbe 0x18001e50b
-   18001e50b:	addb   $0x0,(%rcx)
-   18001e50e:	add    %al,(%rax)
-   18001e510:	loopne 0x18001e58b
-   18001e512:	add    %al,0x1(%rax)
-   18001e518:	adc    %dh,0x0(%rcx)
-   18001e51b:	addb   $0x0,(%rcx)
-   18001e51e:	add    %al,(%rax)
-   18001e520:	loopne 0x18001e59a
-   18001e522:	add    %al,0x1(%rax)
-   18001e528:	rex movsb %ds:(%rsi),%es:(%rdi)
-   18001e52a:	add    %eax,0x1(%rax)
-   18001e530:	lock push %rbp
-   18001e532:	add    %al,0x1(%rax)
-   18001e538:	shrb   0x0(%rbp)
-   18001e53b:	addb   $0x0,(%rcx)
-   18001e53e:	add    %al,(%rax)
-   18001e540:	shlb   $0x80,0x0(%rdi)
-   18001e544:	add    %eax,(%rax)
+   18001e4ff:	add    %dl,0x1800074(%rax)
+   18001e505:	add    %al,(%rax)
+   18001e507:	add    %dh,0x73(%rax)
+   18001e50a:	add    %al,0x1(%rax)
+   18001e510:	rex jbe 0x18001e513
+   18001e513:	addb   $0x0,(%rcx)
+   18001e516:	add    %al,(%rax)
+   18001e518:	loopne 0x18001e593
+   18001e51a:	add    %al,0x1(%rax)
+   18001e520:	adc    %dh,0x0(%rcx)
+   18001e523:	addb   $0x0,(%rcx)
+   18001e526:	add    %al,(%rax)
+   18001e528:	loopne 0x18001e5a2
+   18001e52a:	add    %al,0x1(%rax)
+   18001e530:	rex movsb %ds:(%rsi),%es:(%rdi)
+   18001e532:	add    %eax,0x1(%rax)
+   18001e538:	lock push %rbp
+   18001e53a:	add    %al,0x1(%rax)
+   18001e540:	shrb   0x0(%rbp)
+   18001e543:	addb   $0x0,(%rcx)
    18001e546:	add    %al,(%rax)
-   18001e548:	movabs 0x6000000001800076,%al
-   18001e551:	jnp    0x18001e553
-   18001e553:	addb   $0x0,(%rcx)
-   18001e556:	add    %al,(%rax)
-   18001e558:	rex jp 0x18001e55b
+   18001e548:	shlb   $0x80,0x0(%rdi)
+   18001e54c:	add    %eax,(%rax)
+   18001e54e:	add    %al,(%rax)
+   18001e550:	movabs 0x6000000001800076,%al
+   18001e559:	jnp    0x18001e55b
    18001e55b:	addb   $0x0,(%rcx)
    18001e55e:	add    %al,(%rax)
-   18001e560:	sub    %bh,%ch
-   18001e562:	add    %eax,0x1(%rax)
-   18001e568:	subb   $0x1,-0x80(%rax,%rax,1)
-   18001e56d:	add    %al,(%rax)
-   18001e56f:	add    %dl,%al
-   18001e571:	xchg   %eax,%edx
-   18001e572:	add    %eax,0x1(%rax)
-   18001e578:	jno    0x18001e5ee
-   18001e57a:	outsb  %ds:(%rsi),(%dx)
-   18001e57c:	gs je  0x18001e5f6
-   18001e57f:	outsl  %ds:(%rsi),(%dx)
-   18001e580:	jb     0x18001e5ed
-   18001e582:	(bad)
-   18001e583:	jne    0x18001e5f9
-   18001e585:	push   $0x75616f2e
-   18001e58a:	je     0x18001e5f4
-   18001e58c:	xor    (%rax),%al
-   18001e58e:	add    %al,(%rax)
-   18001e590:	push   %rcx
-   18001e591:	add    %dh,0x4f(%rax,%rax,1)
-   18001e595:	add    %al,0x0(%rcx)
-   18001e598:	jne    0x18001e59a
-   18001e59a:	je     0x18001e59c
-   18001e59c:	push   $0x31002f00
-   18001e5a1:	add    %ch,(%rsi)
-   18001e5a3:	add    %dh,(%rax)
-   18001e5a5:	add    %ah,(%rax)
-   18001e5a7:	add    %ch,(%rax)
-   18001e5a9:	add    %ch,(%rbx)
-   18001e5ab:	add    %ch,0x0(%rax)
-   18001e5ae:	je     0x18001e5b0
-   18001e5b0:	je     0x18001e5b2
-   18001e5b2:	jo     0x18001e5b4
-   18001e5b4:	jae    0x18001e5b6
-   18001e5b6:	cmp    (%rax),%al
-   18001e5b8:	(bad)
-   18001e5b9:	add    %ch,(%rdi)
-   18001e5bb:	add    %dh,0x0(%rdi)
-   18001e5be:	ja     0x18001e5c0
-   18001e5c0:	ja     0x18001e5c2
-   18001e5c2:	cs add %dh,0x0(%rcx)
-   18001e5c6:	je     0x18001e5c8
-   18001e5c8:	cs add %ch,0x0(%rcx)
-   18001e5cc:	outsl  %ds:(%rsi),(%dx)
-   18001e5cd:	add    %ch,(%rcx)
-	...
-   18001e5d7:	add    %al,0x0(%rdx)
-   18001e5da:	add    %ah,%gs:0x0(%rcx)
-   18001e5de:	jb     0x18001e5e0
-   18001e5e0:	add    %dh,%gs:0x0(%rdx)
-   18001e5e4:	and    %al,(%rax)
-   18001e5e6:	and    $0x3100,%eax
-   18001e5eb:	add    %al,(%rax)
-   18001e5ed:	add    %al,(%rax)
-   18001e5ef:	add    %al,0x75(%rcx)
-   18001e5f2:	je     0x18001e65c
-   18001e5f4:	outsl  %ds:(%rsi),(%dx)
-   18001e5f5:	jb     0x18001e660
-   18001e5f7:	jp     0x18001e65a
-   18001e5f9:	je     0x18001e664
-   18001e5fb:	outsl  %ds:(%rsi),(%dx)
-   18001e5fc:	outsb  %ds:(%rsi),(%dx)
+   18001e560:	rex jp 0x18001e563
+   18001e563:	addb   $0x0,(%rcx)
+   18001e566:	add    %al,(%rax)
+   18001e568:	sub    %bh,%ch
+   18001e56a:	add    %eax,0x1(%rax)
+   18001e570:	subb   $0x1,-0x80(%rax,%rax,1)
+   18001e575:	add    %al,(%rax)
+   18001e577:	add    %dl,%al
+   18001e579:	xchg   %eax,%edx
+   18001e57a:	add    %eax,0x1(%rax)
+   18001e580:	jno    0x18001e5f6
+   18001e582:	outsb  %ds:(%rsi),(%dx)
+   18001e584:	gs je  0x18001e5fe
+   18001e587:	outsl  %ds:(%rsi),(%dx)
+   18001e588:	jb     0x18001e5f5
+   18001e58a:	(bad)
+   18001e58b:	jne    0x18001e601
+   18001e58d:	push   $0x75616f2e
+   18001e592:	je     0x18001e5fc
+   18001e594:	xor    (%rax),%al
+	...
+   18001e59e:	add    %al,(%rax)
+   18001e5a0:	push   %rcx
+   18001e5a1:	add    %dh,0x4f(%rax,%rax,1)
+   18001e5a5:	add    %al,0x0(%rcx)
+   18001e5a8:	jne    0x18001e5aa
+   18001e5aa:	je     0x18001e5ac
+   18001e5ac:	push   $0x31002f00
+   18001e5b1:	add    %ch,(%rsi)
+   18001e5b3:	add    %dh,(%rax)
+   18001e5b5:	add    %ah,(%rax)
+   18001e5b7:	add    %ch,(%rax)
+   18001e5b9:	add    %ch,(%rbx)
+   18001e5bb:	add    %ch,0x0(%rax)
+   18001e5be:	je     0x18001e5c0
+   18001e5c0:	je     0x18001e5c2
+   18001e5c2:	jo     0x18001e5c4
+   18001e5c4:	jae    0x18001e5c6
+   18001e5c6:	cmp    (%rax),%al
+   18001e5c8:	(bad)
+   18001e5c9:	add    %ch,(%rdi)
+   18001e5cb:	add    %dh,0x0(%rdi)
+   18001e5ce:	ja     0x18001e5d0
+   18001e5d0:	ja     0x18001e5d2
+   18001e5d2:	cs add %dh,0x0(%rcx)
+   18001e5d6:	je     0x18001e5d8
+   18001e5d8:	cs add %ch,0x0(%rcx)
+   18001e5dc:	outsl  %ds:(%rsi),(%dx)
+   18001e5dd:	add    %ch,(%rcx)
+	...
+   18001e5e7:	add    %al,0x0(%rdx)
+   18001e5ea:	add    %ah,%gs:0x0(%rcx)
+   18001e5ee:	jb     0x18001e5f0
+   18001e5f0:	add    %dh,%gs:0x0(%rdx)
+   18001e5f4:	and    %al,(%rax)
+   18001e5f6:	and    $0x3100,%eax
+   18001e5fb:	add    %al,(%rax)
    18001e5fd:	add    %al,(%rax)
-   18001e5ff:	add    %al,0x6d(%rbp)
-   18001e602:	jo     0x18001e678
-   18001e604:	jns    0x18001e626
-   18001e606:	(bad)
-   18001e607:	movsxd 0x65(%rbx),%esp
-   18001e60a:	jae    0x18001e67f
-   18001e60c:	and    %dh,0x6b(%rdi,%rbp,2)
-   18001e610:	outsb  %gs:(%rsi),(%dx)
-	...
-   18001e61e:	add    %al,(%rax)
-   18001e620:	push   %rcx
-   18001e621:	push   %rbx
-   18001e622:	jae    0x18001e690
-   18001e624:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001e626:	outsb  %ds:(%rsi),(%dx)
-   18001e627:	imul   $0x6172,0x75(%rdi),%sp
-   18001e62d:	je     0x18001e698
-   18001e62f:	outsl  %ds:(%rsi),(%dx)
-   18001e630:	rex incb (%rcx)
-   18001e633:	addb   $0x0,(%rcx)
-   18001e636:	add    %al,(%rax)
-   18001e638:	rex (bad)
-   18001e63a:	add    %al,0x1(%rax)
-   18001e640:	(bad)
-   18001e641:	add    %al,0x1(%r8)
-   18001e648:	and    %al,0x0(%rax)
-   18001e64b:	addb   $0x0,(%rcx)
-   18001e64e:	add    %al,(%rax)
-   18001e650:	and    %al,0x180(%rax,%rax,1)
-   18001e657:	add    %dh,0x1800192(%rax)
-   18001e65d:	add    %al,(%rax)
-   18001e65f:	add    %al,%al
-   18001e661:	xchg   %eax,%edx
-   18001e662:	add    %eax,0x1(%rax)
-   18001e668:	loopne 0x18001e5fc
-   18001e66a:	add    %eax,0x1(%rax)
-   18001e670:	jo     0x18001e604
+   18001e5ff:	add    %al,0x75(%rcx)
+   18001e602:	je     0x18001e66c
+   18001e604:	outsl  %ds:(%rsi),(%dx)
+   18001e605:	jb     0x18001e670
+   18001e607:	jp     0x18001e66a
+   18001e609:	je     0x18001e674
+   18001e60b:	outsl  %ds:(%rsi),(%dx)
+   18001e60c:	outsb  %ds:(%rsi),(%dx)
+   18001e60d:	add    %al,(%rax)
+   18001e60f:	add    %al,0x6d(%rbp)
+   18001e612:	jo     0x18001e688
+   18001e614:	jns    0x18001e636
+   18001e616:	(bad)
+   18001e617:	movsxd 0x65(%rbx),%esp
+   18001e61a:	jae    0x18001e68f
+   18001e61c:	and    %dh,0x6b(%rdi,%rbp,2)
+   18001e620:	outsb  %gs:(%rsi),(%dx)
+	...
+   18001e62e:	add    %al,(%rax)
+   18001e630:	push   %rcx
+   18001e631:	push   %rbx
+   18001e632:	jae    0x18001e6a0
+   18001e634:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001e636:	outsb  %ds:(%rsi),(%dx)
+   18001e637:	imul   $0x6172,0x75(%rdi),%sp
+   18001e63d:	je     0x18001e6a8
+   18001e63f:	outsl  %ds:(%rsi),(%dx)
+   18001e640:	rex incb (%rcx)
+   18001e643:	addb   $0x0,(%rcx)
+   18001e646:	add    %al,(%rax)
+   18001e648:	rex (bad)
+   18001e64a:	add    %al,0x1(%rax)
+   18001e650:	(bad)
+   18001e651:	add    %al,0x1(%r8)
+   18001e658:	and    %al,0x0(%rax)
+   18001e65b:	addb   $0x0,(%rcx)
+   18001e65e:	add    %al,(%rax)
+   18001e660:	and    %al,0x180(%rax,%rax,1)
+   18001e667:	add    %dh,0x1800192(%rax)
+   18001e66d:	add    %al,(%rax)
+   18001e66f:	add    %al,%al
+   18001e671:	xchg   %eax,%edx
    18001e672:	add    %eax,0x1(%rax)
-   18001e678:	nop
-   18001e679:	xchg   %eax,%edx
+   18001e678:	loopne 0x18001e60c
    18001e67a:	add    %eax,0x1(%rax)
-   18001e680:	adcb   $0x0,0x18001(%rdx)
-   18001e687:	add    %ah,0x1800192(%rax)
-   18001e68d:	add    %al,(%rax)
-   18001e68f:	add    %al,-0x5c(%rax)
-   18001e692:	add    %eax,0x1(%rax)
-   18001e698:	rex movsb %ds:(%rsi),%es:(%rdi)
-   18001e69a:	add    %eax,0x1(%rax)
-   18001e6a0:	jno    0x18001e716
-   18001e6a2:	outsb  %ds:(%rsi),(%dx)
-   18001e6a4:	gs je  0x18001e71e
-   18001e6a7:	outsl  %ds:(%rsi),(%dx)
-   18001e6a8:	jb     0x18001e715
-   18001e6aa:	(bad)
-   18001e6ab:	jne    0x18001e721
-   18001e6ad:	push   $0x7065722e
-   18001e6b2:	insb   (%dx),%es:(%rdi)
-   18001e6b3:	jns    0x18001e71d
-   18001e6b5:	(bad)
-   18001e6b6:	outsb  %ds:(%rsi),(%dx)
-   18001e6b7:	fs insb (%dx),%es:(%rdi)
-   18001e6b9:	gs jb  0x18001e6bc
-   18001e6bc:	add    %al,(%rax)
-   18001e6be:	add    %al,(%rax)
-   18001e6c0:	outsl  %ds:(%rsi),(%dx)
-   18001e6c1:	add    %ah,0x0(%rcx)
-   18001e6c4:	jne    0x18001e6c6
-   18001e6c6:	je     0x18001e6c8
-   18001e6c8:	push   $0x63005f00
-   18001e6cd:	add    %ah,0x0(%rcx)
-   18001e6d0:	insb   (%dx),%es:(%rdi)
-   18001e6d1:	add    %ch,0x62(%rax,%rax,1)
-   18001e6d5:	add    %ah,0x0(%rcx)
-   18001e6d8:	movsxd (%rax),%eax
-   18001e6da:	imul   $0x0,(%rax),%eax
-   18001e6dd:	add    %al,(%rax)
-   18001e6df:	add    %ch,0x0(%rdi)
-   18001e6e2:	(bad)
-   18001e6e3:	add    %dh,0x0(%rbp)
-   18001e6e6:	je     0x18001e6e8
-   18001e6e8:	push   $0x63005f00
-   18001e6ed:	add    %ah,0x0(%rcx)
-   18001e6f0:	insb   (%dx),%es:(%rdi)
-   18001e6f1:	add    %ch,0x62(%rax,%rax,1)
-   18001e6f5:	add    %ah,0x0(%rcx)
-   18001e6f8:	movsxd (%rax),%eax
-   18001e6fa:	imul   $0x5f,(%rax),%eax
-   18001e6fd:	add    %ah,0x0(%rbx)
-   18001e700:	outsl  %ds:(%rsi),(%dx)
-   18001e701:	add    %ch,0x0(%rsi)
-   18001e704:	data16 add %ch,0x0(%rcx)
-   18001e708:	jb     0x18001e70a
-   18001e70a:	insl   (%dx),%es:(%rdi)
-   18001e70b:	add    %ah,0x0(%rbp)
-   18001e70e:	add    %al,%fs:(%rax)
-   18001e711:	add    %al,(%rax)
-   18001e713:	add    %al,(%rax)
-   18001e715:	add    %al,(%rax)
-   18001e717:	add    %ch,0x0(%rdi)
-   18001e71a:	(bad)
-   18001e71b:	add    %dh,0x0(%rbp)
-   18001e71e:	je     0x18001e720
-   18001e720:	push   $0x63005f00
-   18001e725:	add    %ch,0x0(%rdi)
-   18001e728:	outsb  %ds:(%rsi),(%dx)
-   18001e729:	add    %dh,0x0(%rbx)
-   18001e72c:	jne    0x18001e72e
-   18001e72e:	insl   (%dx),%es:(%rdi)
-   18001e72f:	add    %ah,0x0(%rbp)
-   18001e732:	jb     0x18001e734
-   18001e734:	pop    %rdi
-   18001e735:	add    %ch,0x0(%rbx)
-   18001e738:	add    %bh,%gs:0x0(%rcx)
-   18001e73c:	add    %al,(%rax)
-   18001e73e:	add    %al,(%rax)
-   18001e740:	outsl  %ds:(%rsi),(%dx)
-   18001e741:	add    %ah,0x0(%rcx)
-   18001e744:	jne    0x18001e746
-   18001e746:	je     0x18001e748
-   18001e748:	push   $0x6e005f00
-   18001e74d:	add    %ch,0x0(%rdi)
-   18001e750:	outsb  %ds:(%rsi),(%dx)
-   18001e751:	add    %ah,0x0(%rbx)
-   18001e754:	add    %al,%gs:(%rax)
-   18001e757:	add    %ch,0x0(%rdi)
-   18001e75a:	(bad)
-   18001e75b:	add    %dh,0x0(%rbp)
-   18001e75e:	je     0x18001e760
-   18001e760:	push   $0x73005f00
-   18001e765:	add    %ch,0x0(%rcx)
-   18001e768:	add    %ch,0x0(%esi)
-   18001e76c:	(bad)
-   18001e76d:	add    %dh,0x75(%rax,%rax,1)
-   18001e771:	add    %dh,0x0(%rdx)
-   18001e774:	add    %al,%gs:(%rax)
-   18001e777:	add    %ch,0x0(%rdi)
-   18001e77a:	(bad)
-   18001e77b:	add    %dh,0x0(%rbp)
-   18001e77e:	je     0x18001e780
-   18001e780:	push   $0x73005f00
-   18001e785:	add    %ch,0x0(%rcx)
-   18001e788:	add    %ch,0x0(%esi)
-   18001e78c:	(bad)
-   18001e78d:	add    %dh,0x75(%rax,%rax,1)
-   18001e791:	add    %dh,0x0(%rdx)
-   18001e794:	add    %bl,%gs:0x0(%rdi)
-   18001e798:	insl   (%dx),%es:(%rdi)
-   18001e799:	add    %ah,0x0(%rbp)
-   18001e79c:	je     0x18001e79e
-   18001e79e:	push   $0x64006f00
-   18001e7a3:	add    %al,(%rax)
-   18001e7a5:	add    %al,(%rax)
-   18001e7a7:	add    %ch,0x0(%rdi)
-   18001e7aa:	(bad)
-   18001e7ab:	add    %dh,0x0(%rbp)
-   18001e7ae:	je     0x18001e7b0
-   18001e7b0:	push   $0x74005f00
-   18001e7b5:	add    %ch,0x0(%rcx)
-   18001e7b8:	insl   (%dx),%es:(%rdi)
-   18001e7b9:	add    %ah,0x0(%rbp)
-   18001e7bc:	jae    0x18001e7be
+   18001e680:	jo     0x18001e614
+   18001e682:	add    %eax,0x1(%rax)
+   18001e688:	nop
+   18001e689:	xchg   %eax,%edx
+   18001e68a:	add    %eax,0x1(%rax)
+   18001e690:	adcb   $0x0,0x18001(%rdx)
+   18001e697:	add    %ah,0x1800192(%rax)
+   18001e69d:	add    %al,(%rax)
+   18001e69f:	add    %al,-0x5c(%rax)
+   18001e6a2:	add    %eax,0x1(%rax)
+   18001e6a8:	rex movsb %ds:(%rsi),%es:(%rdi)
+   18001e6aa:	add    %eax,0x1(%rax)
+   18001e6b0:	jno    0x18001e726
+   18001e6b2:	outsb  %ds:(%rsi),(%dx)
+   18001e6b4:	gs je  0x18001e72e
+   18001e6b7:	outsl  %ds:(%rsi),(%dx)
+   18001e6b8:	jb     0x18001e725
+   18001e6ba:	(bad)
+   18001e6bb:	jne    0x18001e731
+   18001e6bd:	push   $0x7065722e
+   18001e6c2:	insb   (%dx),%es:(%rdi)
+   18001e6c3:	jns    0x18001e72d
+   18001e6c5:	(bad)
+   18001e6c6:	outsb  %ds:(%rsi),(%dx)
+   18001e6c7:	fs insb (%dx),%es:(%rdi)
+   18001e6c9:	gs jb  0x18001e6cc
+   18001e6cc:	add    %al,(%rax)
+   18001e6ce:	add    %al,(%rax)
+   18001e6d0:	outsl  %ds:(%rsi),(%dx)
+   18001e6d1:	add    %ah,0x0(%rcx)
+   18001e6d4:	jne    0x18001e6d6
+   18001e6d6:	je     0x18001e6d8
+   18001e6d8:	push   $0x63005f00
+   18001e6dd:	add    %ah,0x0(%rcx)
+   18001e6e0:	insb   (%dx),%es:(%rdi)
+   18001e6e1:	add    %ch,0x62(%rax,%rax,1)
+   18001e6e5:	add    %ah,0x0(%rcx)
+   18001e6e8:	movsxd (%rax),%eax
+   18001e6ea:	imul   $0x0,(%rax),%eax
+   18001e6ed:	add    %al,(%rax)
+   18001e6ef:	add    %ch,0x0(%rdi)
+   18001e6f2:	(bad)
+   18001e6f3:	add    %dh,0x0(%rbp)
+   18001e6f6:	je     0x18001e6f8
+   18001e6f8:	push   $0x63005f00
+   18001e6fd:	add    %ah,0x0(%rcx)
+   18001e700:	insb   (%dx),%es:(%rdi)
+   18001e701:	add    %ch,0x62(%rax,%rax,1)
+   18001e705:	add    %ah,0x0(%rcx)
+   18001e708:	movsxd (%rax),%eax
+   18001e70a:	imul   $0x5f,(%rax),%eax
+   18001e70d:	add    %ah,0x0(%rbx)
+   18001e710:	outsl  %ds:(%rsi),(%dx)
+   18001e711:	add    %ch,0x0(%rsi)
+   18001e714:	data16 add %ch,0x0(%rcx)
+   18001e718:	jb     0x18001e71a
+   18001e71a:	insl   (%dx),%es:(%rdi)
+   18001e71b:	add    %ah,0x0(%rbp)
+   18001e71e:	add    %al,%fs:(%rax)
+   18001e721:	add    %al,(%rax)
+   18001e723:	add    %al,(%rax)
+   18001e725:	add    %al,(%rax)
+   18001e727:	add    %ch,0x0(%rdi)
+   18001e72a:	(bad)
+   18001e72b:	add    %dh,0x0(%rbp)
+   18001e72e:	je     0x18001e730
+   18001e730:	push   $0x63005f00
+   18001e735:	add    %ch,0x0(%rdi)
+   18001e738:	outsb  %ds:(%rsi),(%dx)
+   18001e739:	add    %dh,0x0(%rbx)
+   18001e73c:	jne    0x18001e73e
+   18001e73e:	insl   (%dx),%es:(%rdi)
+   18001e73f:	add    %ah,0x0(%rbp)
+   18001e742:	jb     0x18001e744
+   18001e744:	pop    %rdi
+   18001e745:	add    %ch,0x0(%rbx)
+   18001e748:	add    %bh,%gs:0x0(%rcx)
+   18001e74c:	add    %al,(%rax)
+   18001e74e:	add    %al,(%rax)
+   18001e750:	outsl  %ds:(%rsi),(%dx)
+   18001e751:	add    %ah,0x0(%rcx)
+   18001e754:	jne    0x18001e756
+   18001e756:	je     0x18001e758
+   18001e758:	push   $0x6e005f00
+   18001e75d:	add    %ch,0x0(%rdi)
+   18001e760:	outsb  %ds:(%rsi),(%dx)
+   18001e761:	add    %ah,0x0(%rbx)
+   18001e764:	add    %al,%gs:(%rax)
+   18001e767:	add    %ch,0x0(%rdi)
+   18001e76a:	(bad)
+   18001e76b:	add    %dh,0x0(%rbp)
+   18001e76e:	je     0x18001e770
+   18001e770:	push   $0x73005f00
+   18001e775:	add    %ch,0x0(%rcx)
+   18001e778:	add    %ch,0x0(%esi)
+   18001e77c:	(bad)
+   18001e77d:	add    %dh,0x75(%rax,%rax,1)
+   18001e781:	add    %dh,0x0(%rdx)
+   18001e784:	add    %al,%gs:(%rax)
+   18001e787:	add    %ch,0x0(%rdi)
+   18001e78a:	(bad)
+   18001e78b:	add    %dh,0x0(%rbp)
+   18001e78e:	je     0x18001e790
+   18001e790:	push   $0x73005f00
+   18001e795:	add    %ch,0x0(%rcx)
+   18001e798:	add    %ch,0x0(%esi)
+   18001e79c:	(bad)
+   18001e79d:	add    %dh,0x75(%rax,%rax,1)
+   18001e7a1:	add    %dh,0x0(%rdx)
+   18001e7a4:	add    %bl,%gs:0x0(%rdi)
+   18001e7a8:	insl   (%dx),%es:(%rdi)
+   18001e7a9:	add    %ah,0x0(%rbp)
+   18001e7ac:	je     0x18001e7ae
+   18001e7ae:	push   $0x64006f00
+   18001e7b3:	add    %al,(%rax)
+   18001e7b5:	add    %al,(%rax)
+   18001e7b7:	add    %ch,0x0(%rdi)
+   18001e7ba:	(bad)
+   18001e7bb:	add    %dh,0x0(%rbp)
    18001e7be:	je     0x18001e7c0
-   18001e7c0:	(bad)
-   18001e7c1:	add    %ch,0x0(%rbp)
-   18001e7c4:	jo     0x18001e7c6
-   18001e7c6:	add    %al,(%rax)
-   18001e7c8:	outsl  %ds:(%rsi),(%dx)
-   18001e7c9:	add    %ah,0x0(%rcx)
-   18001e7cc:	jne    0x18001e7ce
+   18001e7c0:	push   $0x74005f00
+   18001e7c5:	add    %ch,0x0(%rcx)
+   18001e7c8:	insl   (%dx),%es:(%rdi)
+   18001e7c9:	add    %ah,0x0(%rbp)
+   18001e7cc:	jae    0x18001e7ce
    18001e7ce:	je     0x18001e7d0
-   18001e7d0:	push   $0x74005f00
-   18001e7d5:	add    %ch,0x0(%rdi)
-   18001e7d8:	imul   $0x65,(%rax),%eax
-   18001e7db:	add    %ch,0x0(%rsi)
-   18001e7de:	add    %al,(%rax)
-   18001e7e0:	outsl  %ds:(%rsi),(%dx)
-   18001e7e1:	add    %ah,0x0(%rcx)
-   18001e7e4:	jne    0x18001e7e6
-   18001e7e6:	je     0x18001e7e8
-   18001e7e8:	push   $0x74005f00
-   18001e7ed:	add    %ch,0x0(%rdi)
-   18001e7f0:	imul   $0x65,(%rax),%eax
-   18001e7f3:	add    %ch,0x0(%rsi)
-   18001e7f6:	pop    %rdi
-   18001e7f7:	add    %dh,0x0(%rbx)
-   18001e7fa:	add    %ah,%gs:0x0(%rbx)
-   18001e7fe:	jb     0x18001e800
-   18001e800:	add    %dh,%gs:0x0(%rax,%rax,1)
-   18001e805:	add    %al,(%rax)
-   18001e807:	add    %ch,0x0(%rdi)
-   18001e80a:	(bad)
-   18001e80b:	add    %dh,0x0(%rbp)
-   18001e80e:	je     0x18001e810
-   18001e810:	push   $0x76005f00
-   18001e815:	add    %ah,0x0(%rbp)
-   18001e818:	jb     0x18001e81a
-   18001e81a:	imul   $0x690066,(%rax),%eax
-   18001e820:	add    %dh,%gs:0x0(%rdx)
-   18001e824:	add    %al,(%rax)
-   18001e826:	add    %al,(%rax)
-   18001e828:	outsl  %ds:(%rsi),(%dx)
-   18001e829:	add    %ah,0x0(%rcx)
-   18001e82c:	jne    0x18001e82e
-   18001e82e:	je     0x18001e830
-   18001e830:	push   $0x76005f00
-   18001e835:	add    %ah,0x0(%rbp)
-   18001e838:	jb     0x18001e83a
-   18001e83a:	jae    0x18001e83c
-   18001e83c:	imul   $0x6e006f,(%rax),%eax
-   18001e842:	add    %al,(%rax)
-   18001e844:	add    %al,(%rax)
-   18001e846:	add    %al,(%rax)
-   18001e848:	push   %rax
-   18001e849:	incl   (%rcx)
-   18001e84b:	addb   $0x0,(%rcx)
-   18001e84e:	add    %al,(%rax)
-   18001e850:	(bad)
-   18001e851:	(bad)
-   18001e852:	add    %al,0x1(%rax)
-   18001e858:	mov    $0x41,%al
-   18001e85a:	add    %al,0x1(%rax)
-   18001e860:	movabs 0x7000000001800040,%al
-   18001e869:	xchg   %eax,%esp
+   18001e7d0:	(bad)
+   18001e7d1:	add    %ch,0x0(%rbp)
+   18001e7d4:	jo     0x18001e7d6
+   18001e7d6:	add    %al,(%rax)
+   18001e7d8:	outsl  %ds:(%rsi),(%dx)
+   18001e7d9:	add    %ah,0x0(%rcx)
+   18001e7dc:	jne    0x18001e7de
+   18001e7de:	je     0x18001e7e0
+   18001e7e0:	push   $0x74005f00
+   18001e7e5:	add    %ch,0x0(%rdi)
+   18001e7e8:	imul   $0x65,(%rax),%eax
+   18001e7eb:	add    %ch,0x0(%rsi)
+   18001e7ee:	add    %al,(%rax)
+   18001e7f0:	outsl  %ds:(%rsi),(%dx)
+   18001e7f1:	add    %ah,0x0(%rcx)
+   18001e7f4:	jne    0x18001e7f6
+   18001e7f6:	je     0x18001e7f8
+   18001e7f8:	push   $0x74005f00
+   18001e7fd:	add    %ch,0x0(%rdi)
+   18001e800:	imul   $0x65,(%rax),%eax
+   18001e803:	add    %ch,0x0(%rsi)
+   18001e806:	pop    %rdi
+   18001e807:	add    %dh,0x0(%rbx)
+   18001e80a:	add    %ah,%gs:0x0(%rbx)
+   18001e80e:	jb     0x18001e810
+   18001e810:	add    %dh,%gs:0x0(%rax,%rax,1)
+   18001e815:	add    %al,(%rax)
+   18001e817:	add    %ch,0x0(%rdi)
+   18001e81a:	(bad)
+   18001e81b:	add    %dh,0x0(%rbp)
+   18001e81e:	je     0x18001e820
+   18001e820:	push   $0x76005f00
+   18001e825:	add    %ah,0x0(%rbp)
+   18001e828:	jb     0x18001e82a
+   18001e82a:	imul   $0x690066,(%rax),%eax
+   18001e830:	add    %dh,%gs:0x0(%rdx)
+   18001e834:	add    %al,(%rax)
+   18001e836:	add    %al,(%rax)
+   18001e838:	outsl  %ds:(%rsi),(%dx)
+   18001e839:	add    %ah,0x0(%rcx)
+   18001e83c:	jne    0x18001e83e
+   18001e83e:	je     0x18001e840
+   18001e840:	push   $0x76005f00
+   18001e845:	add    %ah,0x0(%rbp)
+   18001e848:	jb     0x18001e84a
+   18001e84a:	jae    0x18001e84c
+   18001e84c:	imul   $0x6e006f,(%rax),%eax
+   18001e852:	add    %al,(%rax)
+   18001e854:	add    %al,(%rax)
+   18001e856:	add    %al,(%rax)
+   18001e858:	push   %rax
+   18001e859:	incl   (%rcx)
+   18001e85b:	addb   $0x0,(%rcx)
+   18001e85e:	add    %al,(%rax)
+   18001e860:	(bad)
+   18001e861:	(bad)
+   18001e862:	add    %al,0x1(%rax)
+   18001e868:	mov    $0x41,%al
    18001e86a:	add    %al,0x1(%rax)
-   18001e870:	mov    $0x92,%al
-   18001e872:	add    %eax,0x1(%rax)
-   18001e878:	rclb   $0x0,0x18001(%rdx)
-   18001e87f:	add    %ah,%al
-   18001e881:	xchg   %eax,%edx
+   18001e870:	movabs 0x7000000001800040,%al
+   18001e879:	xchg   %eax,%esp
+   18001e87a:	add    %al,0x1(%rax)
+   18001e880:	mov    $0x92,%al
    18001e882:	add    %eax,0x1(%rax)
-   18001e888:	jo     0x18001e81c
-   18001e88a:	add    %eax,0x1(%rax)
-   18001e890:	nop
+   18001e888:	rclb   $0x0,0x18001(%rdx)
+   18001e88f:	add    %ah,%al
    18001e891:	xchg   %eax,%edx
    18001e892:	add    %eax,0x1(%rax)
-   18001e898:	adcb   $0x0,0x18001(%rdx)
-   18001e89f:	add    %ah,0x1800192(%rax)
-   18001e8a5:	add    %al,(%rax)
-   18001e8a7:	add    %dh,%al
-   18001e8a9:	mov    $0x0,%dl
-   18001e8ab:	addb   $0x0,(%rcx)
-   18001e8ae:	add    %al,(%rax)
-   18001e8b0:	xor    %ch,0x18000(%rsi)
-   18001e8b6:	add    %al,(%rax)
-   18001e8b8:	loopne 0x18001e874
-   18001e8ba:	add    %al,0x1(%rax)
-   18001e8c0:	adc    %al,%bl
-   18001e8c2:	add    %al,0x1(%rax)
-   18001e8c8:	and    %ah,0x18000(%rsi)
-   18001e8ce:	add    %al,(%rax)
-   18001e8d0:	nop
-   18001e8d1:	mov    $0x18000,%esp
-   18001e8d6:	add    %al,(%rax)
-   18001e8d8:	movabs 0xf0000000018000af,%al
-   18001e8e1:	push   %rbp
-   18001e8e2:	add    %al,0x1(%rax)
-   18001e8e8:	push   %rcx
-   18001e8e9:	rex.WRX
-   18001e8ea:	gs je  0x18001e964
-   18001e8ed:	outsl  %ds:(%rsi),(%dx)
-   18001e8ee:	jb     0x18001e95b
-   18001e8f0:	push   %rdx
-   18001e8f1:	gs jo  0x18001e960
-   18001e8f4:	jns    0x18001e930
-   18001e8f6:	cmp    0x65(%rsi),%cl
-   18001e8f9:	je     0x18001e972
-   18001e8fb:	outsl  %ds:(%rsi),(%dx)
-   18001e8fc:	jb     0x18001e969
-   18001e8fe:	rex.RB jb 0x18001e973
-   18001e901:	outsl  %ds:(%rsi),(%dx)
-   18001e902:	jb     0x18001e904
-   18001e904:	add    %al,(%rax)
-   18001e906:	add    %al,(%rax)
-   18001e908:	sar    $0x1,%dh
-   18001e90b:	addb   $0x0,(%rcx)
-   18001e90e:	add    %al,(%rax)
-   18001e910:	rex xchg %eax,%esi
-   18001e912:	add    %al,0x1(%rax)
-   18001e918:	rclb   0x18001(%rdx)
+   18001e898:	jo     0x18001e82c
+   18001e89a:	add    %eax,0x1(%rax)
+   18001e8a0:	nop
+   18001e8a1:	xchg   %eax,%edx
+   18001e8a2:	add    %eax,0x1(%rax)
+   18001e8a8:	adcb   $0x0,0x18001(%rdx)
+   18001e8af:	add    %ah,0x1800192(%rax)
+   18001e8b5:	add    %al,(%rax)
+   18001e8b7:	add    %dh,%al
+   18001e8b9:	mov    $0x0,%dl
+   18001e8bb:	addb   $0x0,(%rcx)
+   18001e8be:	add    %al,(%rax)
+   18001e8c0:	xor    %ch,0x18000(%rsi)
+   18001e8c6:	add    %al,(%rax)
+   18001e8c8:	loopne 0x18001e884
+   18001e8ca:	add    %al,0x1(%rax)
+   18001e8d0:	adc    %al,%bl
+   18001e8d2:	add    %al,0x1(%rax)
+   18001e8d8:	and    %ah,0x18000(%rsi)
+   18001e8de:	add    %al,(%rax)
+   18001e8e0:	nop
+   18001e8e1:	mov    $0x18000,%esp
+   18001e8e6:	add    %al,(%rax)
+   18001e8e8:	movabs 0xf0000000018000af,%al
+   18001e8f1:	push   %rbp
+   18001e8f2:	add    %al,0x1(%rax)
+   18001e8f8:	push   %rcx
+   18001e8f9:	rex.WRX
+   18001e8fa:	gs je  0x18001e974
+   18001e8fd:	outsl  %ds:(%rsi),(%dx)
+   18001e8fe:	jb     0x18001e96b
+   18001e900:	push   %rdx
+   18001e901:	gs jo  0x18001e970
+   18001e904:	jns    0x18001e940
+   18001e906:	cmp    0x65(%rsi),%cl
+   18001e909:	je     0x18001e982
+   18001e90b:	outsl  %ds:(%rsi),(%dx)
+   18001e90c:	jb     0x18001e979
+   18001e90e:	rex.RB jb 0x18001e983
+   18001e911:	outsl  %ds:(%rsi),(%dx)
+   18001e912:	jb     0x18001e914
+   18001e914:	add    %al,(%rax)
+   18001e916:	add    %al,(%rax)
+   18001e918:	sar    $0x1,%dh
+   18001e91b:	addb   $0x0,(%rcx)
    18001e91e:	add    %al,(%rax)
-   18001e920:	jno    0x18001e996
-   18001e922:	outsb  %ds:(%rsi),(%dx)
-   18001e924:	gs je  0x18001e99e
-   18001e927:	outsl  %ds:(%rsi),(%dx)
-   18001e928:	jb     0x18001e995
-   18001e92a:	(bad)
-   18001e92b:	jne    0x18001e9a1
-   18001e92d:	push   $0x75616f2e
-   18001e932:	je     0x18001e99c
-   18001e934:	xor    %eax,(%rax)
-   18001e936:	add    %al,(%rax)
-   18001e938:	xor    %eax,(%rax)
-   18001e93a:	cs add %dh,(%rax)
-   18001e93d:	add    %al,(%rax)
-   18001e93f:	add    %dl,0x4f(%rcx)
-   18001e942:	rex.B jne 0x18001e9b9
-   18001e945:	push   $0x533a3a31
-   18001e94a:	imul   $0x72757461,0x6e(%rdi),%esp
-   18001e951:	gs rex.WRB
-   18001e953:	gs je  0x18001e9be
-   18001e956:	outsl  %ds:(%rsi),(%dx)
-   18001e957:	add    %al,%fs:(%rax)
-   18001e95a:	add    %al,(%rax)
-   18001e95c:	add    %al,(%rax)
-   18001e95e:	add    %al,(%rax)
-   18001e960:	push   %rcx
-   18001e961:	rex.WRX
-   18001e962:	gs je  0x18001e9dc
-   18001e965:	outsl  %ds:(%rsi),(%dx)
-   18001e966:	jb     0x18001e9d3
-   18001e968:	movsxd 0x65(%r11),%esp
-   18001e96c:	jae    0x18001e9e1
-   18001e96e:	rex.WRB (bad)
-   18001e970:	outsb  %ds:(%rsi),(%dx)
-   18001e971:	(bad)
-   18001e972:	addr32 gs jb 0x18001e996
-   18001e976:	outsb  %ds:(%rsi),(%dx)
-   18001e977:	outsl  %ds:(%rsi),(%dx)
-   18001e978:	je     0x18001e99a
-   18001e97a:	(bad)
-   18001e97b:	jbe    0x18001e9de
-   18001e97d:	imul   $0x656c,0x62(%rcx,%riz,2),%ebp
-   18001e985:	add    %al,(%rax)
-   18001e987:	add    %dl,0x65(%rdx)
-   18001e98a:	jno    0x18001ea01
-   18001e98c:	gs jae 0x18001ea03
-   18001e98f:	and    %dl,0x72(%rbp)
-   18001e992:	insb   (%dx),%es:(%rdi)
-   18001e993:	and    %ch,0x6f(%rsi)
-   18001e996:	je     0x18001e9b8
-   18001e998:	jae    0x18001e9ff
-   18001e99a:	je     0x18001e99c
-   18001e99c:	add    %al,(%rax)
-   18001e99e:	add    %al,(%rax)
-   18001e9a0:	rex.WRXB jo 0x18001ea08
-   18001e9a3:	jb     0x18001ea06
-   18001e9a5:	je     0x18001ea10
-   18001e9a7:	outsl  %ds:(%rsi),(%dx)
-   18001e9a8:	outsb  %ds:(%rsi),(%dx)
-   18001e9a9:	and    %ch,0x6f(%rsi)
-   18001e9ac:	je     0x18001e9ce
-   18001e9ae:	jae    0x18001ea25
-   18001e9b0:	jo     0x18001ea22
-   18001e9b2:	outsl  %ds:(%rsi),(%dx)
-   18001e9b3:	jb     0x18001ea29
-   18001e9b5:	gs add %ch,%fs:0x0(%rdi)
-   18001e9ba:	(bad)
-   18001e9bb:	add    %dh,0x0(%rbp)
-   18001e9be:	je     0x18001e9c0
-   18001e9c0:	push   $0x5f00
-   18001e9c5:	add    %al,(%rax)
-   18001e9c7:	add    %dl,0x0(%rax)
-   18001e9ca:	rex.WR add %r8b,0x0(%rcx)
-   18001e9ce:	rex.WB add %cl,0x0(%r14)
-   18001e9d2:	push   %rsp
-   18001e9d3:	add    %al,0x0(%rbp)
-   18001e9d6:	pop    %rax
-   18001e9d7:	add    %dl,0x0(%rax,%rax,1)
-   18001e9db:	add    %al,(%rax)
-   18001e9dd:	add    %al,(%rax)
-   18001e9df:	add    %cl,0x0(%rax)
-   18001e9e2:	rex.WRB add %r8b,0x0(%r9)
-   18001e9e6:	rex.XB add %bpl,0x48005300(%rip)        # 0x1c8023ced
-   18001e9ed:	add    %al,0x0(%rcx)
-   18001e9f0:	xor    %eax,(%rax)
-   18001e9f2:	add    %al,(%rax)
-   18001e9f4:	add    %al,(%rax)
-   18001e9f6:	add    %al,(%rax)
-   18001e9f8:	push   %rdx
-   18001e9f9:	push   %rbx
-   18001e9fa:	rex.B sub $0x31414853,%eax
-   18001ea00:	and    %dh,0x69(%rbx)
-   18001ea03:	outsb  %ds:(%esi),(%dx)
-   18001ea05:	(bad)
-   18001ea06:	je     0x18001ea7d
-   18001ea08:	jb     0x18001ea6f
-   18001ea0a:	and    %ch,0x65(%rbp)
-   18001ea0d:	je     0x18001ea77
-   18001ea0f:	outsl  %ds:(%rsi),(%dx)
-   18001ea10:	and    %ch,%fs:0x6f(%rsi)
-   18001ea14:	je     0x18001ea36
-   18001ea16:	jae    0x18001ea8d
-   18001ea18:	jo     0x18001ea8a
-   18001ea1a:	outsl  %ds:(%rsi),(%dx)
-   18001ea1b:	jb     0x18001ea91
-   18001ea1d:	gs add %dl,%fs:0x0(%rdx)
-   18001ea22:	push   %rbx
-   18001ea23:	add    %al,0x0(%rcx)
-   18001ea26:	sub    $0x48005300,%eax
-   18001ea2b:	add    %al,0x0(%rcx)
-   18001ea2e:	xor    %eax,(%rax)
-	...
-   18001ea38:	rex.WB outsb %ds:(%rsi),(%dx)
-   18001ea3a:	jbe    0x18001ea9d
-   18001ea3c:	insb   (%dx),%es:(%rdi)
-   18001ea3d:	imul   $0x616e6769,0x73(%rax,%riz,1),%esp
-   18001ea45:	je     0x18001eabc
-   18001ea47:	jb     0x18001eaae
-   18001ea49:	and    %ch,0x65(%rbp)
-   18001ea4c:	je     0x18001eab6
-   18001ea4e:	outsl  %ds:(%rsi),(%dx)
-   18001ea4f:	add    %al,%fs:(%rax)
-	...
-   18001ea5e:	add    %al,(%rax)
-   18001ea60:	push   %rcx
-   18001ea61:	rex.WRXB
-   18001ea62:	rex.B jne 0x18001ead9
-   18001ea65:	push   $0x69725031
-   18001ea6a:	jbe    0x18001eacd
-   18001ea6c:	je     0x18001ead3
-   18001ea6e:	cmp    (%rdx),%bh
-   18001ea70:	outsb  %gs:(%esi),(%dx)
-   18001ea73:	gs jb  0x18001ead7
-   18001ea76:	je     0x18001eadd
-   18001ea78:	push   %rbx
-   18001ea79:	imul   $0x72757461,0x6e(%rdi),%esp
-   18001ea80:	cmp    %gs:(%rax),%ah
-   18001ea83:	push   %rbx
-   18001ea84:	imul   $0x72757461,0x6e(%rdi),%esp
-   18001ea8b:	and    %ch,%gs:0x65(%rbp)
-   18001ea8f:	je     0x18001eaf9
-   18001ea91:	outsl  %ds:(%rsi),(%dx)
-   18001ea92:	and    %ch,%fs:0x6f(%rsi)
-   18001ea96:	je     0x18001eab8
-   18001ea98:	jae    0x18001eb0f
-   18001ea9a:	jo     0x18001eb0c
-   18001ea9c:	outsl  %ds:(%rsi),(%dx)
-   18001ea9d:	jb     0x18001eb13
-   18001ea9f:	gs add %al,%fs:(%rax)
-   18001eaa3:	add    %dl,0x4f(%rax)
-   18001eaa6:	push   %rbx
-   18001eaa7:	push   %rsp
-	...
-   18001eab0:	(bad)
-   18001eab1:	jo     0x18001eb23
-   18001eab3:	insb   (%dx),%es:(%rdi)
-   18001eab4:	imul   $0x6e6f6974,0x61(%rbx),%esp
-   18001eabb:	(bad)
-   18001eabc:	js     0x18001eaeb
-   18001eabe:	ja     0x18001eb37
-   18001eac0:	ja     0x18001eaef
-   18001eac2:	outsw  %ds:(%rsi),(%dx)
-   18001eac4:	jb     0x18001eb33
-   18001eac6:	sub    $0x656c7275,%eax
-   18001eacb:	outsb  %ds:(%rsi),(%dx)
-   18001eacc:	movsxd 0x64(%rdi),%ebp
-   18001eacf:	gs add %al,%fs:(%rax)
-   18001ead3:	add    %al,(%rax)
-   18001ead5:	add    %al,(%rax)
-   18001ead7:	add    %cl,0x0(%rdi)
-   18001eada:	add    %sil,0x0(%r13)
-   18001eade:	je     0x18001eae0
-   18001eae0:	push   $0x2000
+   18001e920:	rex xchg %eax,%esi
+   18001e922:	add    %al,0x1(%rax)
+   18001e928:	rclb   0x18001(%rdx)
+   18001e92e:	add    %al,(%rax)
+   18001e930:	jno    0x18001e9a6
+   18001e932:	outsb  %ds:(%rsi),(%dx)
+   18001e934:	gs je  0x18001e9ae
+   18001e937:	outsl  %ds:(%rsi),(%dx)
+   18001e938:	jb     0x18001e9a5
+   18001e93a:	(bad)
+   18001e93b:	jne    0x18001e9b1
+   18001e93d:	push   $0x75616f2e
+   18001e942:	je     0x18001e9ac
+   18001e944:	xor    %eax,(%rax)
+   18001e946:	add    %al,(%rax)
+   18001e948:	xor    %eax,(%rax)
+   18001e94a:	cs add %dh,(%rax)
+   18001e94d:	add    %al,(%rax)
+   18001e94f:	add    %dl,0x4f(%rcx)
+   18001e952:	rex.B jne 0x18001e9c9
+   18001e955:	push   $0x533a3a31
+   18001e95a:	imul   $0x72757461,0x6e(%rdi),%esp
+   18001e961:	gs rex.WRB
+   18001e963:	gs je  0x18001e9ce
+   18001e966:	outsl  %ds:(%rsi),(%dx)
+   18001e967:	add    %al,%fs:(%rax)
+   18001e96a:	add    %al,(%rax)
+   18001e96c:	add    %al,(%rax)
+   18001e96e:	add    %al,(%rax)
+   18001e970:	push   %rcx
+   18001e971:	rex.WRX
+   18001e972:	gs je  0x18001e9ec
+   18001e975:	outsl  %ds:(%rsi),(%dx)
+   18001e976:	jb     0x18001e9e3
+   18001e978:	movsxd 0x65(%r11),%esp
+   18001e97c:	jae    0x18001e9f1
+   18001e97e:	rex.WRB (bad)
+   18001e980:	outsb  %ds:(%rsi),(%dx)
+   18001e981:	(bad)
+   18001e982:	addr32 gs jb 0x18001e9a6
+   18001e986:	outsb  %ds:(%rsi),(%dx)
+   18001e987:	outsl  %ds:(%rsi),(%dx)
+   18001e988:	je     0x18001e9aa
+   18001e98a:	(bad)
+   18001e98b:	jbe    0x18001e9ee
+   18001e98d:	imul   $0x656c,0x62(%rcx,%riz,2),%ebp
+   18001e995:	add    %al,(%rax)
+   18001e997:	add    %dl,0x65(%rdx)
+   18001e99a:	jno    0x18001ea11
+   18001e99c:	gs jae 0x18001ea13
+   18001e99f:	and    %dl,0x72(%rbp)
+   18001e9a2:	insb   (%dx),%es:(%rdi)
+   18001e9a3:	and    %ch,0x6f(%rsi)
+   18001e9a6:	je     0x18001e9c8
+   18001e9a8:	jae    0x18001ea0f
+   18001e9aa:	je     0x18001e9ac
+   18001e9ac:	add    %al,(%rax)
+   18001e9ae:	add    %al,(%rax)
+   18001e9b0:	rex.WRXB jo 0x18001ea18
+   18001e9b3:	jb     0x18001ea16
+   18001e9b5:	je     0x18001ea20
+   18001e9b7:	outsl  %ds:(%rsi),(%dx)
+   18001e9b8:	outsb  %ds:(%rsi),(%dx)
+   18001e9b9:	and    %ch,0x6f(%rsi)
+   18001e9bc:	je     0x18001e9de
+   18001e9be:	jae    0x18001ea35
+   18001e9c0:	jo     0x18001ea32
+   18001e9c2:	outsl  %ds:(%rsi),(%dx)
+   18001e9c3:	jb     0x18001ea39
+   18001e9c5:	gs add %ch,%fs:0x0(%rdi)
+   18001e9ca:	(bad)
+   18001e9cb:	add    %dh,0x0(%rbp)
+   18001e9ce:	je     0x18001e9d0
+   18001e9d0:	push   $0x5f00
+   18001e9d5:	add    %al,(%rax)
+   18001e9d7:	add    %dl,0x0(%rax)
+   18001e9da:	rex.WR add %r8b,0x0(%rcx)
+   18001e9de:	rex.WB add %cl,0x0(%r14)
+   18001e9e2:	push   %rsp
+   18001e9e3:	add    %al,0x0(%rbp)
+   18001e9e6:	pop    %rax
+   18001e9e7:	add    %dl,0x0(%rax,%rax,1)
+   18001e9eb:	add    %al,(%rax)
+   18001e9ed:	add    %al,(%rax)
+   18001e9ef:	add    %cl,0x0(%rax)
+   18001e9f2:	rex.WRB add %r8b,0x0(%r9)
+   18001e9f6:	rex.XB add %bpl,0x48005300(%rip)        # 0x1c8023cfd
+   18001e9fd:	add    %al,0x0(%rcx)
+   18001ea00:	xor    %eax,(%rax)
+   18001ea02:	add    %al,(%rax)
+   18001ea04:	add    %al,(%rax)
+   18001ea06:	add    %al,(%rax)
+   18001ea08:	push   %rdx
+   18001ea09:	push   %rbx
+   18001ea0a:	rex.B sub $0x31414853,%eax
+   18001ea10:	and    %dh,0x69(%rbx)
+   18001ea13:	outsb  %ds:(%esi),(%dx)
+   18001ea15:	(bad)
+   18001ea16:	je     0x18001ea8d
+   18001ea18:	jb     0x18001ea7f
+   18001ea1a:	and    %ch,0x65(%rbp)
+   18001ea1d:	je     0x18001ea87
+   18001ea1f:	outsl  %ds:(%rsi),(%dx)
+   18001ea20:	and    %ch,%fs:0x6f(%rsi)
+   18001ea24:	je     0x18001ea46
+   18001ea26:	jae    0x18001ea9d
+   18001ea28:	jo     0x18001ea9a
+   18001ea2a:	outsl  %ds:(%rsi),(%dx)
+   18001ea2b:	jb     0x18001eaa1
+   18001ea2d:	gs add %dl,%fs:0x0(%rdx)
+   18001ea32:	push   %rbx
+   18001ea33:	add    %al,0x0(%rcx)
+   18001ea36:	sub    $0x48005300,%eax
+   18001ea3b:	add    %al,0x0(%rcx)
+   18001ea3e:	xor    %eax,(%rax)
+	...
+   18001ea48:	rex.WB outsb %ds:(%rsi),(%dx)
+   18001ea4a:	jbe    0x18001eaad
+   18001ea4c:	insb   (%dx),%es:(%rdi)
+   18001ea4d:	imul   $0x616e6769,0x73(%rax,%riz,1),%esp
+   18001ea55:	je     0x18001eacc
+   18001ea57:	jb     0x18001eabe
+   18001ea59:	and    %ch,0x65(%rbp)
+   18001ea5c:	je     0x18001eac6
+   18001ea5e:	outsl  %ds:(%rsi),(%dx)
+   18001ea5f:	add    %al,%fs:(%rax)
+	...
+   18001ea6e:	add    %al,(%rax)
+   18001ea70:	push   %rcx
+   18001ea71:	rex.WRXB
+   18001ea72:	rex.B jne 0x18001eae9
+   18001ea75:	push   $0x69725031
+   18001ea7a:	jbe    0x18001eadd
+   18001ea7c:	je     0x18001eae3
+   18001ea7e:	cmp    (%rdx),%bh
+   18001ea80:	outsb  %gs:(%esi),(%dx)
+   18001ea83:	gs jb  0x18001eae7
+   18001ea86:	je     0x18001eaed
+   18001ea88:	push   %rbx
+   18001ea89:	imul   $0x72757461,0x6e(%rdi),%esp
+   18001ea90:	cmp    %gs:(%rax),%ah
+   18001ea93:	push   %rbx
+   18001ea94:	imul   $0x72757461,0x6e(%rdi),%esp
+   18001ea9b:	and    %ch,%gs:0x65(%rbp)
+   18001ea9f:	je     0x18001eb09
+   18001eaa1:	outsl  %ds:(%rsi),(%dx)
+   18001eaa2:	and    %ch,%fs:0x6f(%rsi)
+   18001eaa6:	je     0x18001eac8
+   18001eaa8:	jae    0x18001eb1f
+   18001eaaa:	jo     0x18001eb1c
+   18001eaac:	outsl  %ds:(%rsi),(%dx)
+   18001eaad:	jb     0x18001eb23
+   18001eaaf:	gs add %al,%fs:(%rax)
+   18001eab3:	add    %dl,0x4f(%rax)
+   18001eab6:	push   %rbx
+   18001eab7:	push   %rsp
+	...
+   18001eac0:	(bad)
+   18001eac1:	jo     0x18001eb33
+   18001eac3:	insb   (%dx),%es:(%rdi)
+   18001eac4:	imul   $0x6e6f6974,0x61(%rbx),%esp
+   18001eacb:	(bad)
+   18001eacc:	js     0x18001eafb
+   18001eace:	ja     0x18001eb47
+   18001ead0:	ja     0x18001eaff
+   18001ead2:	outsw  %ds:(%rsi),(%dx)
+   18001ead4:	jb     0x18001eb43
+   18001ead6:	sub    $0x656c7275,%eax
+   18001eadb:	outsb  %ds:(%rsi),(%dx)
+   18001eadc:	movsxd 0x64(%rdi),%ebp
+   18001eadf:	gs add %al,%fs:(%rax)
+   18001eae3:	add    %al,(%rax)
    18001eae5:	add    %al,(%rax)
-   18001eae7:	add    %ch,(%rax,%rax,1)
-   18001eaea:	add    %al,(%rax)
-   18001eaec:	cmp    $0x25000022,%eax
-   18001eaf1:	jae    0x18001eb13
-   18001eaf3:	outsb  %ds:(%rsi),(%dx)
-   18001eaf4:	outsl  %ds:(%rsi),(%dx)
-   18001eaf5:	je     0x18001eb17
-   18001eaf7:	outsw  %ds:(%rsi),(%dx)
-   18001eaf9:	jne    0x18001eb69
-   18001eafb:	and    %ch,%fs:0x6e(%rcx)
-   18001eaff:	and    %dh,0x65(%rax,%rbp,2)
-   18001eb03:	and    %ah,0x61(%rbx)
-   18001eb06:	insb   (%dx),%es:(%rdi)
-   18001eb07:	insb   (%dx),%es:(%rdi)
-   18001eb08:	(bad)
-   18001eb0a:	movsxd 0x0(%rbx),%ebp
-   18001eb0d:	add    %al,(%rax)
-   18001eb0f:	add    %dh,0x65(%rdx)
-   18001eb12:	jno    0x18001eb89
-   18001eb14:	gs jae 0x18001eb8b
-   18001eb17:	push   %rsp
-   18001eb18:	outsl  %ds:(%rsi),(%dx)
-   18001eb19:	imul   $0x55,0x6e(%rbp),%esp
-   18001eb1d:	jb     0x18001eb8b
-   18001eb1f:	and    %ch,0x73(%rcx)
-   18001eb22:	and    %ah,0x6d(%rbp)
-   18001eb25:	jo     0x18001eb9b
-   18001eb27:	jns    0x18001eb29
-   18001eb29:	add    %al,(%rax)
-   18001eb2b:	add    %al,(%rax)
-   18001eb2d:	add    %al,(%rax)
-   18001eb2f:	add    %ah,0x75(%rcx)
-   18001eb32:	je     0x18001eb9c
-   18001eb34:	outsl  %ds:(%rsi),(%dx)
-   18001eb35:	jb     0x18001eba0
-   18001eb37:	jp     0x18001eb9a
-   18001eb39:	je     0x18001eba4
-   18001eb3b:	outsl  %ds:(%rsi),(%dx)
-   18001eb3c:	outsb  %ds:(%rsi),(%dx)
-   18001eb3d:	rex.RXB jb 0x18001eba1
-   18001eb40:	outsb  %ds:(%rsi),(%dx)
-   18001eb41:	je     0x18001eb98
-   18001eb43:	jb     0x18001ebb1
-   18001eb45:	and    %ch,0x73(%rcx)
-   18001eb48:	and    %ah,0x6d(%rbp)
-   18001eb4b:	jo     0x18001ebc1
-   18001eb4d:	jns    0x18001eb4f
-   18001eb4f:	add    %al,0x6c(%rcx)
-   18001eb52:	jb     0x18001ebb9
-   18001eb54:	(bad)
-   18001eb55:	fs jns 0x18001eb78
-   18001eb58:	(bad)
-   18001eb59:	jne    0x18001ebcf
-   18001eb5b:	push   $0x69746e65
-   18001eb60:	movsxd 0x74(%rcx),%esp
-   18001eb63:	gs add %al,%fs:(%rax)
-	...
-   18001eb6f:	add    %dl,0x4e(%rcx)
-   18001eb72:	gs je  0x18001ebec
-   18001eb75:	outsl  %ds:(%rsi),(%dx)
-   18001eb76:	jb     0x18001ebe3
-   18001eb78:	push   %rdx
-   18001eb79:	gs jo  0x18001ebe8
-   18001eb7c:	jns    0x18001ebb8
-   18001eb7e:	cmp    0x71(%rsi),%cl
-   18001eb81:	je     0x18001ebb1
-   18001eb83:	outsb  %ds:(%rsi),(%dx)
-   18001eb84:	gs je  0x18001ebfe
-   18001eb87:	outsl  %ds:(%rsi),(%dx)
-   18001eb88:	jb     0x18001ebf5
-   18001eb8a:	(bad)
-   18001eb8b:	jne    0x18001ec01
-   18001eb8d:	push   $0x75616f2e
-   18001eb92:	je     0x18001ebfc
-   18001eb94:	xor    %ebp,(%rsi)
-   18001eb96:	jae    0x18001ec01
-   18001eb98:	outsb  %ds:(%esi),(%dx)
+   18001eae7:	add    %cl,0x0(%rdi)
+   18001eaea:	add    %sil,0x0(%r13)
+   18001eaee:	je     0x18001eaf0
+   18001eaf0:	push   $0x2000
+   18001eaf5:	add    %al,(%rax)
+   18001eaf7:	add    %ch,(%rax,%rax,1)
+   18001eafa:	add    %al,(%rax)
+   18001eafc:	cmp    $0x25000022,%eax
+   18001eb01:	jae    0x18001eb23
+   18001eb03:	outsb  %ds:(%rsi),(%dx)
+   18001eb04:	outsl  %ds:(%rsi),(%dx)
+   18001eb05:	je     0x18001eb27
+   18001eb07:	outsw  %ds:(%rsi),(%dx)
+   18001eb09:	jne    0x18001eb79
+   18001eb0b:	and    %ch,%fs:0x6e(%rcx)
+   18001eb0f:	and    %dh,0x65(%rax,%rbp,2)
+   18001eb13:	and    %ah,0x61(%rbx)
+   18001eb16:	insb   (%dx),%es:(%rdi)
+   18001eb17:	insb   (%dx),%es:(%rdi)
+   18001eb18:	(bad)
+   18001eb1a:	movsxd 0x0(%rbx),%ebp
+   18001eb1d:	add    %al,(%rax)
+   18001eb1f:	add    %dh,0x65(%rdx)
+   18001eb22:	jno    0x18001eb99
+   18001eb24:	gs jae 0x18001eb9b
+   18001eb27:	push   %rsp
+   18001eb28:	outsl  %ds:(%rsi),(%dx)
+   18001eb29:	imul   $0x55,0x6e(%rbp),%esp
+   18001eb2d:	jb     0x18001eb9b
+   18001eb2f:	and    %ch,0x73(%rcx)
+   18001eb32:	and    %ah,0x6d(%rbp)
+   18001eb35:	jo     0x18001ebab
+   18001eb37:	jns    0x18001eb39
+   18001eb39:	add    %al,(%rax)
+   18001eb3b:	add    %al,(%rax)
+   18001eb3d:	add    %al,(%rax)
+   18001eb3f:	add    %ah,0x75(%rcx)
+   18001eb42:	je     0x18001ebac
+   18001eb44:	outsl  %ds:(%rsi),(%dx)
+   18001eb45:	jb     0x18001ebb0
+   18001eb47:	jp     0x18001ebaa
+   18001eb49:	je     0x18001ebb4
+   18001eb4b:	outsl  %ds:(%rsi),(%dx)
+   18001eb4c:	outsb  %ds:(%rsi),(%dx)
+   18001eb4d:	rex.RXB jb 0x18001ebb1
+   18001eb50:	outsb  %ds:(%rsi),(%dx)
+   18001eb51:	je     0x18001eba8
+   18001eb53:	jb     0x18001ebc1
+   18001eb55:	and    %ch,0x73(%rcx)
+   18001eb58:	and    %ah,0x6d(%rbp)
+   18001eb5b:	jo     0x18001ebd1
+   18001eb5d:	jns    0x18001eb5f
+   18001eb5f:	add    %al,0x6c(%rcx)
+   18001eb62:	jb     0x18001ebc9
+   18001eb64:	(bad)
+   18001eb65:	fs jns 0x18001eb88
+   18001eb68:	(bad)
+   18001eb69:	jne    0x18001ebdf
+   18001eb6b:	push   $0x69746e65
+   18001eb70:	movsxd 0x74(%rcx),%esp
+   18001eb73:	gs add %al,%fs:(%rax)
+	...
+   18001eb7f:	add    %dl,0x4e(%rcx)
+   18001eb82:	gs je  0x18001ebfc
+   18001eb85:	outsl  %ds:(%rsi),(%dx)
+   18001eb86:	jb     0x18001ebf3
+   18001eb88:	push   %rdx
+   18001eb89:	gs jo  0x18001ebf8
+   18001eb8c:	jns    0x18001ebc8
+   18001eb8e:	cmp    0x71(%rsi),%cl
+   18001eb91:	je     0x18001ebc1
+   18001eb93:	outsb  %ds:(%rsi),(%dx)
+   18001eb94:	gs je  0x18001ec0e
+   18001eb97:	outsl  %ds:(%rsi),(%dx)
+   18001eb98:	jb     0x18001ec05
    18001eb9a:	(bad)
-   18001eb9b:	je     0x18001ec12
-   18001eb9d:	jb     0x18001ec04
-   18001eb9f:	add    %cl,0x45(%rax)
-   18001eba2:	rex.B
-   18001eba3:	add    %r8b,(%rax)
-   18001eba6:	add    %al,(%rax)
-   18001eba8:	rex.RXB
-   18001eba9:	rex.RB push %r12
-   18001ebab:	add    %dl,0x55(%rax)
-   18001ebae:	push   %rsp
-   18001ebaf:	add    %al,0x4c(%rbp,%rax,2)
-   18001ebb3:	rex.RB push %r12
-   18001ebb5:	add    %r8b,(%r8)
-	...
-   18001ebc0:	push   %rcx
-   18001ebc1:	rex.WRXB
-   18001ebc2:	rex.B jne 0x18001ec39
-   18001ebc5:	push   $0x67695331
-   18001ebca:	outsb  %ds:(%rsi),(%dx)
-   18001ebcb:	(bad)
-   18001ebcc:	je     0x18001ec43
-   18001ebce:	jb     0x18001ec35
-   18001ebd0:	cmp    (%rax),%ah
-   18001ebd2:	rex.W je 0x18001ec49
-   18001ebd5:	jo     0x18001ec29
-   18001ebd7:	gs jno 0x18001ec4f
-   18001ebda:	gs jae 0x18001ec51
-   18001ebdd:	rex.WRB
-   18001ebde:	gs je  0x18001ec49
-   18001ebe1:	outsl  %ds:(%rsi),(%dx)
-   18001ebe2:	cmp    %fs:(%rdx),%bh
-   18001ebe5:	rex.XB jne 0x18001ec5b
-   18001ebe8:	je     0x18001ec59
-   18001ebea:	insl   (%dx),%es:(%rdi)
-   18001ebeb:	and    %dh,0x65(%rdx)
-   18001ebee:	jno    0x18001ec65
-   18001ebf0:	imul   $0x68742073,0x65(%rdx),%esi
-   18001ebf7:	and    %dh,%gs:0x65(%rsi)
-   18001ebfb:	jb     0x18001ec5f
-   18001ebfd:	and    %dh,0x20(%rdi,%rbp,2)
-   18001ec01:	(bad)
-   18001ec03:	and    %dh,0x65(%rbx)
-   18001ec06:	je     0x18001ec28
-   18001ec08:	jbe    0x18001ec73
-   18001ec0a:	(bad)
-   18001ec0b:	and    %dh,0x65(%rbx)
-   18001ec0e:	je     0x18001ec53
-   18001ec10:	jne    0x18001ec85
-   18001ec12:	je     0x18001ec83
-   18001ec14:	insl   (%dx),%es:(%rdi)
-   18001ec15:	rex.WRB
-   18001ec16:	gs je  0x18001ec81
-   18001ec19:	outsl  %ds:(%rsi),(%dx)
-   18001ec1a:	fs push %rbx
-   18001ec1c:	je     0x18001ec90
-   18001ec1e:	imul   $0x0,0x67(%rsi),%ebp
-   18001ec25:	add    %al,(%rax)
-   18001ec27:	add    %dl,0x4f(%rcx)
-   18001ec2a:	rex.B jne 0x18001eca1
-   18001ec2d:	push   $0x67695331
-   18001ec32:	outsb  %ds:(%rsi),(%dx)
-   18001ec33:	(bad)
-   18001ec34:	je     0x18001ecab
-   18001ec36:	jb     0x18001ec9d
-   18001ec38:	cmp    (%rax),%ah
-   18001ec3a:	rex.W je 0x18001ecb1
-   18001ec3d:	jo     0x18001ec91
-   18001ec3f:	gs jno 0x18001ecb7
-   18001ec42:	gs jae 0x18001ecb9
-   18001ec45:	rex.WRB
-   18001ec46:	gs je  0x18001ecb1
-   18001ec49:	outsl  %ds:(%rsi),(%dx)
-   18001ec4a:	and    %ch,%fs:0x6f(%rsi)
-   18001ec4e:	je     0x18001ec70
-   18001ec50:	jae    0x18001ecc7
-   18001ec52:	jo     0x18001ecc4
-   18001ec54:	outsl  %ds:(%rsi),(%dx)
-   18001ec55:	jb     0x18001eccb
-   18001ec57:	gs add %al,%fs:(%rax)
-   18001ec5b:	add    %ah,(%rsi)
-   18001ec5d:	add    %al,(%rax)
-   18001ec5f:	add    %ah,0x70(%rbp,%rsi,2)
-   18001ec63:	insb   (%dx),%es:(%rdi)
-   18001ec64:	imul   $0x20646574,0x61(%rbx),%esp
-   18001ec6b:	imul   $0x20,0x79(%rbp),%esp
-   18001ec6f:	and    $0x73,%eax
-   18001ec74:	cmp    $0x52000000,%eax
-   18001ec79:	push   %rbx
-   18001ec7a:	rex.B sub $0x31414853,%eax
-   18001ec80:	and    %dh,0x69(%rbx)
-   18001ec83:	outsb  %ds:(%esi),(%dx)
-   18001ec85:	imul   $0x74656d20,0x67(%rsi),%ebp
-   18001ec8c:	push   $0x6e20646f
-   18001ec91:	outsl  %ds:(%rsi),(%dx)
-   18001ec92:	je     0x18001ecb4
-   18001ec94:	jae    0x18001ed0b
-   18001ec96:	jo     0x18001ed08
-   18001ec98:	outsl  %ds:(%rsi),(%dx)
-   18001ec99:	jb     0x18001ed0f
-   18001ec9b:	gs add %al,%fs:(%rax)
-   18001ec9f:	add    %dh,(%rax)
-   18001eca1:	add    %al,(%rax)
-   18001eca3:	add    %bl,(%rax,%rax,1)
-   18001eca6:	add    %al,(%rax)
-   18001eca8:	rex.WRB add %r8b,(%r8)
-   18001ecab:	add    %dl,0x63000000(%rip)        # 0x1e301ecb1
+   18001eb9b:	jne    0x18001ec11
+   18001eb9d:	push   $0x75616f2e
+   18001eba2:	je     0x18001ec0c
+   18001eba4:	xor    %ebp,(%rsi)
+   18001eba6:	jae    0x18001ec11
+   18001eba8:	outsb  %ds:(%esi),(%dx)
+   18001ebaa:	(bad)
+   18001ebab:	je     0x18001ec22
+   18001ebad:	jb     0x18001ec14
+   18001ebaf:	add    %cl,0x45(%rax)
+   18001ebb2:	rex.B
+   18001ebb3:	add    %r8b,(%rax)
+   18001ebb6:	add    %al,(%rax)
+   18001ebb8:	rex.RXB
+   18001ebb9:	rex.RB push %r12
+   18001ebbb:	add    %dl,0x55(%rax)
+   18001ebbe:	push   %rsp
+   18001ebbf:	add    %al,0x4c(%rbp,%rax,2)
+   18001ebc3:	rex.RB push %r12
+   18001ebc5:	add    %r8b,(%r8)
+	...
+   18001ebd0:	push   %rcx
+   18001ebd1:	rex.WRXB
+   18001ebd2:	rex.B jne 0x18001ec49
+   18001ebd5:	push   $0x67695331
+   18001ebda:	outsb  %ds:(%rsi),(%dx)
+   18001ebdb:	(bad)
+   18001ebdc:	je     0x18001ec53
+   18001ebde:	jb     0x18001ec45
+   18001ebe0:	cmp    (%rax),%ah
+   18001ebe2:	rex.W je 0x18001ec59
+   18001ebe5:	jo     0x18001ec39
+   18001ebe7:	gs jno 0x18001ec5f
+   18001ebea:	gs jae 0x18001ec61
+   18001ebed:	rex.WRB
+   18001ebee:	gs je  0x18001ec59
+   18001ebf1:	outsl  %ds:(%rsi),(%dx)
+   18001ebf2:	cmp    %fs:(%rdx),%bh
+   18001ebf5:	rex.XB jne 0x18001ec6b
+   18001ebf8:	je     0x18001ec69
+   18001ebfa:	insl   (%dx),%es:(%rdi)
+   18001ebfb:	and    %dh,0x65(%rdx)
+   18001ebfe:	jno    0x18001ec75
+   18001ec00:	imul   $0x68742073,0x65(%rdx),%esi
+   18001ec07:	and    %dh,%gs:0x65(%rsi)
+   18001ec0b:	jb     0x18001ec6f
+   18001ec0d:	and    %dh,0x20(%rdi,%rbp,2)
+   18001ec11:	(bad)
+   18001ec13:	and    %dh,0x65(%rbx)
+   18001ec16:	je     0x18001ec38
+   18001ec18:	jbe    0x18001ec83
+   18001ec1a:	(bad)
+   18001ec1b:	and    %dh,0x65(%rbx)
+   18001ec1e:	je     0x18001ec63
+   18001ec20:	jne    0x18001ec95
+   18001ec22:	je     0x18001ec93
+   18001ec24:	insl   (%dx),%es:(%rdi)
+   18001ec25:	rex.WRB
+   18001ec26:	gs je  0x18001ec91
+   18001ec29:	outsl  %ds:(%rsi),(%dx)
+   18001ec2a:	fs push %rbx
+   18001ec2c:	je     0x18001eca0
+   18001ec2e:	imul   $0x0,0x67(%rsi),%ebp
+   18001ec35:	add    %al,(%rax)
+   18001ec37:	add    %dl,0x4f(%rcx)
+   18001ec3a:	rex.B jne 0x18001ecb1
+   18001ec3d:	push   $0x67695331
+   18001ec42:	outsb  %ds:(%rsi),(%dx)
+   18001ec43:	(bad)
+   18001ec44:	je     0x18001ecbb
+   18001ec46:	jb     0x18001ecad
+   18001ec48:	cmp    (%rax),%ah
+   18001ec4a:	rex.W je 0x18001ecc1
+   18001ec4d:	jo     0x18001eca1
+   18001ec4f:	gs jno 0x18001ecc7
+   18001ec52:	gs jae 0x18001ecc9
+   18001ec55:	rex.WRB
+   18001ec56:	gs je  0x18001ecc1
+   18001ec59:	outsl  %ds:(%rsi),(%dx)
+   18001ec5a:	and    %ch,%fs:0x6f(%rsi)
+   18001ec5e:	je     0x18001ec80
+   18001ec60:	jae    0x18001ecd7
+   18001ec62:	jo     0x18001ecd4
+   18001ec64:	outsl  %ds:(%rsi),(%dx)
+   18001ec65:	jb     0x18001ecdb
+   18001ec67:	gs add %al,%fs:(%rax)
+   18001ec6b:	add    %ah,(%rsi)
+   18001ec6d:	add    %al,(%rax)
+   18001ec6f:	add    %ah,0x70(%rbp,%rsi,2)
+   18001ec73:	insb   (%dx),%es:(%rdi)
+   18001ec74:	imul   $0x20646574,0x61(%rbx),%esp
+   18001ec7b:	imul   $0x20,0x79(%rbp),%esp
+   18001ec7f:	and    $0x73,%eax
+   18001ec84:	cmp    $0x52000000,%eax
+   18001ec89:	push   %rbx
+   18001ec8a:	rex.B sub $0x31414853,%eax
+   18001ec90:	and    %dh,0x69(%rbx)
+   18001ec93:	outsb  %ds:(%esi),(%dx)
+   18001ec95:	imul   $0x74656d20,0x67(%rsi),%ebp
+   18001ec9c:	push   $0x6e20646f
+   18001eca1:	outsl  %ds:(%rsi),(%dx)
+   18001eca2:	je     0x18001ecc4
+   18001eca4:	jae    0x18001ed1b
+   18001eca6:	jo     0x18001ed18
+   18001eca8:	outsl  %ds:(%rsi),(%dx)
+   18001eca9:	jb     0x18001ed1f
+   18001ecab:	gs add %al,%fs:(%rax)
+   18001ecaf:	add    %dh,(%rax)
    18001ecb1:	add    %al,(%rax)
-   18001ecb3:	add    %al,(%rax)
-   18001ecb5:	add    %al,(%rax)
-   18001ecb7:	add    %ah,0x0(%rax,%rax,1)
-   18001ecbb:	add    %cl,(%rsi)
-   18001ecbd:	add    %al,(%rax)
-   18001ecbf:	add    %dh,0x0(%rbx)
-   18001ecc2:	add    %al,(%rax)
-   18001ecc4:	add    $0x79000000,%eax
-   18001ecc9:	add    %al,(%rax)
-   18001eccb:	add    %dl,(%rdx)
+   18001ecb3:	add    %bl,(%rax,%rax,1)
+   18001ecb6:	add    %al,(%rax)
+   18001ecb8:	rex.WRB add %r8b,(%r8)
+   18001ecbb:	add    %dl,0x63000000(%rip)        # 0x1e301ecc1
+   18001ecc1:	add    %al,(%rax)
+   18001ecc3:	add    %al,(%rax)
+   18001ecc5:	add    %al,(%rax)
+   18001ecc7:	add    %ah,0x0(%rax,%rax,1)
+   18001eccb:	add    %cl,(%rsi)
    18001eccd:	add    %al,(%rax)
-   18001eccf:	add    %dl,0x4f(%rcx)
-   18001ecd2:	rex.B jne 0x18001ed49
-   18001ecd5:	push   $0x74754132
-   18001ecda:	push   $0x7a69726f
-   18001ecdf:	(bad)
-   18001ece0:	je     0x18001ed4b
-   18001ece2:	outsl  %ds:(%rsi),(%dx)
-   18001ece3:	outsb  %ds:(%rsi),(%dx)
-   18001ece4:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001ece6:	fs gs rex.RX insb (%dx),%es:(%rdi)
-   18001ecea:	outsl  %ds:(%rsi),(%dx)
-   18001eceb:	ja     0x18001eced
-   18001eced:	(bad)
-   18001ecee:	movsxd 0x65(%rbx),%esp
-   18001ecf1:	jae    0x18001ed66
-   18001ecf3:	push   %rsp
-   18001ecf4:	outsl  %ds:(%rsi),(%dx)
-   18001ecf5:	imul   $0x55,0x6e(%rbp),%esp
-   18001ecf9:	jb     0x18001ed67
-   18001ecfb:	rex.XB push $0x65676e61
-   18001ed01:	add    %al,%fs:(%rax)
-   18001ed04:	(bad)
-   18001ed05:	movsxd 0x65(%rbx),%esp
-   18001ed08:	jae    0x18001ed7d
-   18001ed0a:	push   %rsp
-   18001ed0b:	outsl  %ds:(%rsi),(%dx)
-   18001ed0c:	imul   $0x55,0x6e(%rbp),%esp
-   18001ed10:	jb     0x18001ed7e
-   18001ed12:	add    %ah,0x72(%rdi)
-   18001ed15:	(bad)
-   18001ed16:	outsb  %ds:(%rsi),(%dx)
-   18001ed17:	je     0x18001ed19
-   18001ed19:	jb     0x18001ed80
-   18001ed1b:	data16 jb 0x18001ed83
-   18001ed1e:	jae    0x18001ed88
-   18001ed20:	movsxd 0x65(%r11),%esp
-   18001ed24:	jae    0x18001ed99
-   18001ed26:	push   %rsp
-   18001ed27:	outsl  %ds:(%rsi),(%dx)
-   18001ed28:	imul   $0x0,0x6e(%rbp),%esp
-   18001ed2c:	add    %al,(%rax)
-   18001ed2e:	add    %al,(%rax)
-   18001ed30:	or     (%rax),%eax
-	...
+   18001eccf:	add    %dh,0x0(%rbx)
+   18001ecd2:	add    %al,(%rax)
+   18001ecd4:	add    $0x79000000,%eax
+   18001ecd9:	add    %al,(%rax)
+   18001ecdb:	add    %dl,(%rdx)
+   18001ecdd:	add    %al,(%rax)
+   18001ecdf:	add    %dl,0x4f(%rcx)
+   18001ece2:	rex.B jne 0x18001ed59
+   18001ece5:	push   $0x74754132
+   18001ecea:	push   $0x7a69726f
+   18001ecef:	(bad)
+   18001ecf0:	je     0x18001ed5b
+   18001ecf2:	outsl  %ds:(%rsi),(%dx)
+   18001ecf3:	outsb  %ds:(%rsi),(%dx)
+   18001ecf4:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001ecf6:	fs gs rex.RX insb (%dx),%es:(%rdi)
+   18001ecfa:	outsl  %ds:(%rsi),(%dx)
+   18001ecfb:	ja     0x18001ecfd
+   18001ecfd:	(bad)
+   18001ecfe:	movsxd 0x65(%rbx),%esp
+   18001ed01:	jae    0x18001ed76
+   18001ed03:	push   %rsp
+   18001ed04:	outsl  %ds:(%rsi),(%dx)
+   18001ed05:	imul   $0x55,0x6e(%rbp),%esp
+   18001ed09:	jb     0x18001ed77
+   18001ed0b:	rex.XB push $0x65676e61
+   18001ed11:	add    %al,%fs:(%rax)
+   18001ed14:	(bad)
+   18001ed15:	movsxd 0x65(%rbx),%esp
+   18001ed18:	jae    0x18001ed8d
+   18001ed1a:	push   %rsp
+   18001ed1b:	outsl  %ds:(%rsi),(%dx)
+   18001ed1c:	imul   $0x55,0x6e(%rbp),%esp
+   18001ed20:	jb     0x18001ed8e
+   18001ed22:	add    %ah,0x72(%rdi)
+   18001ed25:	(bad)
+   18001ed26:	outsb  %ds:(%rsi),(%dx)
+   18001ed27:	je     0x18001ed29
+   18001ed29:	jb     0x18001ed90
+   18001ed2b:	data16 jb 0x18001ed93
+   18001ed2e:	jae    0x18001ed98
+   18001ed30:	movsxd 0x65(%r11),%esp
+   18001ed34:	jae    0x18001eda9
+   18001ed36:	push   %rsp
+   18001ed37:	outsl  %ds:(%rsi),(%dx)
+   18001ed38:	imul   $0x0,0x6e(%rbp),%esp
+   18001ed3c:	add    %al,(%rax)
    18001ed3e:	add    %al,(%rax)
-   18001ed40:	add    (%rax),%eax
-   18001ed42:	add    %al,(%rax)
-   18001ed44:	(bad)
-   18001ed45:	add    %al,(%rax)
-   18001ed47:	add    %al,(%rcx)
-   18001ed49:	add    %al,(%rax)
-   18001ed4b:	add    %ah,0x0(%rip)        # 0x18001ed51
-	...
-   18001ed61:	add    %al,(%rax)
-   18001ed63:	add    %al,(%rcx)
-   18001ed65:	add    %al,(%rax)
-   18001ed67:	add    %al,(%rcx)
-   18001ed69:	add    %al,(%rax)
-   18001ed6b:	add    %al,(%rcx)
-   18001ed6d:	add    %al,(%rax)
-   18001ed6f:	add    %ah,(%rax)
+   18001ed40:	or     (%rax),%eax
+	...
+   18001ed4e:	add    %al,(%rax)
+   18001ed50:	add    (%rax),%eax
+   18001ed52:	add    %al,(%rax)
+   18001ed54:	(bad)
+   18001ed55:	add    %al,(%rax)
+   18001ed57:	add    %al,(%rcx)
+   18001ed59:	add    %al,(%rax)
+   18001ed5b:	add    %ah,0x0(%rip)        # 0x18001ed61
+	...
    18001ed71:	add    %al,(%rax)
-   18001ed73:	add    %al,(%rdx)
+   18001ed73:	add    %al,(%rcx)
    18001ed75:	add    %al,(%rax)
-   18001ed77:	add    %al,(%rsi)
+   18001ed77:	add    %al,(%rcx)
    18001ed79:	add    %al,(%rax)
-   18001ed7b:	add    %al,(%rdx)
+   18001ed7b:	add    %al,(%rcx)
    18001ed7d:	add    %al,(%rax)
-   18001ed7f:	add    %al,(%rax,%rax,1)
-   18001ed82:	add    %al,(%rax)
-   18001ed84:	add    %al,(%rax)
-   18001ed86:	add    %al,(%rax)
-   18001ed88:	and    (%rax),%eax
-   18001ed8a:	add    %al,(%rax)
-   18001ed8c:	add    (%rax),%al
-   18001ed8e:	add    %al,(%rax)
-   18001ed90:	or     (%rax),%al
+   18001ed7f:	add    %ah,(%rax)
+   18001ed81:	add    %al,(%rax)
+   18001ed83:	add    %al,(%rdx)
+   18001ed85:	add    %al,(%rax)
+   18001ed87:	add    %al,(%rsi)
+   18001ed89:	add    %al,(%rax)
+   18001ed8b:	add    %al,(%rdx)
+   18001ed8d:	add    %al,(%rax)
+   18001ed8f:	add    %al,(%rax,%rax,1)
    18001ed92:	add    %al,(%rax)
-   18001ed94:	add    $0x0,%al
+   18001ed94:	add    %al,(%rax)
    18001ed96:	add    %al,(%rax)
-   18001ed98:	add    $0x0,%eax
-   18001ed9d:	add    %al,(%rax)
-   18001ed9f:	add    %ah,(%rax,%rax,1)
+   18001ed98:	and    (%rax),%eax
+   18001ed9a:	add    %al,(%rax)
+   18001ed9c:	add    (%rax),%al
+   18001ed9e:	add    %al,(%rax)
+   18001eda0:	or     (%rax),%al
    18001eda2:	add    %al,(%rax)
-   18001eda4:	add    (%rax),%al
+   18001eda4:	add    $0x0,%al
    18001eda6:	add    %al,(%rax)
-   18001eda8:	or     (%rax),%al
-   18001edaa:	add    %al,(%rax)
-   18001edac:	add    $0x2b000000,%eax
-   18001edb1:	add    %al,(%rax)
-   18001edb3:	add    %dl,(%rcx)
-   18001edb5:	add    %al,(%rax)
-   18001edb7:	add    %al,(%rbx)
-   18001edb9:	add    %al,(%rax)
-   18001edbb:	add    %ch,(%rbx)
-   18001edbd:	add    %al,(%rax)
-   18001edbf:	add    %ch,(%rbx)
+   18001eda8:	add    $0x0,%eax
+   18001edad:	add    %al,(%rax)
+   18001edaf:	add    %ah,(%rax,%rax,1)
+   18001edb2:	add    %al,(%rax)
+   18001edb4:	add    (%rax),%al
+   18001edb6:	add    %al,(%rax)
+   18001edb8:	or     (%rax),%al
+   18001edba:	add    %al,(%rax)
+   18001edbc:	add    $0x2b000000,%eax
    18001edc1:	add    %al,(%rax)
-   18001edc3:	add    %al,(%rbx)
+   18001edc3:	add    %dl,(%rcx)
    18001edc5:	add    %al,(%rax)
-   18001edc7:	add    %dl,(%rcx)
+   18001edc7:	add    %al,(%rbx)
    18001edc9:	add    %al,(%rax)
-   18001edcb:	add    %al,(%rbx)
-   18001edcd:	push   %rcx
-   18001edce:	add    %eax,(%rax)
-	...
-   18001ede0:	shlb   $0x0,0x18002(%rcx)
-   18001ede7:	add    %dl,%al
-   18001ede9:	mov    $0x2,%bh
-   18001edeb:	addb   $0x0,(%rcx)
-   18001edee:	add    %al,(%rax)
-   18001edf0:	lock mov $0x2,%bl
-   18001edf3:	addb   $0x0,(%rcx)
-   18001edf6:	add    %al,(%rax)
-   18001edf8:	shlb   $0x0,0x18002(%rcx)
-   18001edff:	add    %dh,%al
-   18001ee01:	mov    $0x2,%bl
+   18001edcb:	add    %ch,(%rbx)
+   18001edcd:	add    %al,(%rax)
+   18001edcf:	add    %ch,(%rbx)
+   18001edd1:	add    %al,(%rax)
+   18001edd3:	add    %al,(%rbx)
+   18001edd5:	add    %al,(%rax)
+   18001edd7:	add    %dl,(%rcx)
+   18001edd9:	add    %al,(%rax)
+   18001eddb:	add    %al,(%rbx)
+   18001eddd:	push   %rcx
+   18001edde:	add    %eax,(%rax)
+	...
+   18001edf0:	shlb   $0x0,0x18002(%rcx)
+   18001edf7:	add    %dl,%al
+   18001edf9:	mov    $0x2,%bh
+   18001edfb:	addb   $0x0,(%rcx)
+   18001edfe:	add    %al,(%rax)
+   18001ee00:	lock mov $0x2,%bl
    18001ee03:	addb   $0x0,(%rcx)
    18001ee06:	add    %al,(%rax)
-   18001ee08:	lock mov $0x2,%bl
-   18001ee0b:	addb   $0x0,(%rcx)
-   18001ee0e:	add    %al,(%rax)
-   18001ee10:	push   %rcx
-   18001ee11:	rex.WRXB
-   18001ee12:	rex.B jne 0x18001ee89
-   18001ee15:	push   $0x74754132
-   18001ee1a:	push   $0x7a69726f
-   18001ee1f:	(bad)
-   18001ee20:	je     0x18001ee8b
-   18001ee22:	outsl  %ds:(%rsi),(%dx)
-   18001ee23:	outsb  %ds:(%rsi),(%dx)
-   18001ee24:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001ee26:	fs gs rex.RX insb (%dx),%es:(%rdi)
-   18001ee2a:	outsl  %ds:(%rsi),(%dx)
-   18001ee2b:	ja     0x18001ee2d
-	...
-   18001ee35:	add    %al,(%rax)
-   18001ee37:	add    %dl,%al
-   18001ee39:	pop    %rbx
-   18001ee3a:	add    %al,0x1(%rax)
-   18001ee40:	movabs 0x30000000018001ec,%al
-   18001ee49:	in     (%dx),%eax
-   18001ee4a:	add    %eax,0x1(%rax)
-   18001ee50:	and    %cl,(%rdi)
+   18001ee08:	shlb   $0x0,0x18002(%rcx)
+   18001ee0f:	add    %dh,%al
+   18001ee11:	mov    $0x2,%bl
+   18001ee13:	addb   $0x0,(%rcx)
+   18001ee16:	add    %al,(%rax)
+   18001ee18:	lock mov $0x2,%bl
+   18001ee1b:	addb   $0x0,(%rcx)
+   18001ee1e:	add    %al,(%rax)
+   18001ee20:	push   %rcx
+   18001ee21:	rex.WRXB
+   18001ee22:	rex.B jne 0x18001ee99
+   18001ee25:	push   $0x74754132
+   18001ee2a:	push   $0x7a69726f
+   18001ee2f:	(bad)
+   18001ee30:	je     0x18001ee9b
+   18001ee32:	outsl  %ds:(%rsi),(%dx)
+   18001ee33:	outsb  %ds:(%rsi),(%dx)
+   18001ee34:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001ee36:	fs gs rex.RX insb (%dx),%es:(%rdi)
+   18001ee3a:	outsl  %ds:(%rsi),(%dx)
+   18001ee3b:	ja     0x18001ee3d
+	...
+   18001ee45:	add    %al,(%rax)
+   18001ee47:	add    %dl,%al
+   18001ee49:	pop    %rbx
+   18001ee4a:	add    %al,0x1(%rax)
+   18001ee50:	mov    $0xec,%al
    18001ee52:	add    %eax,0x1(%rax)
-	...
-   18001ee60:	loopne 0x18001ee4f
-   18001ee62:	add    %eax,0x1(%rax)
-	...
-   18001ee70:	jo     0x18001ee72
-   18001ee72:	add    0x1(%rax),%al
-   18001ee78:	add    %dh,0x18001(%rip)        # 0x180036e7f
-   18001ee7e:	add    %al,(%rax)
-   18001ee80:	shlb   $0x0,0x18001(%rip)        # 0x180036e88
-   18001ee87:	add    %ah,(%rax)
-   18001ee89:	xor    $0x18001,%eax
+   18001ee58:	rex in (%dx),%eax
+   18001ee5a:	add    %eax,0x1(%rax)
+   18001ee60:	(bad)
+   18001ee61:	sgdt   0x1(%rax)
+	...
+   18001ee70:	lock in (%dx),%eax
+   18001ee72:	add    %eax,0x1(%rax)
+	...
+   18001ee80:	jo     0x18001ee82
+   18001ee82:	add    0x1(%rax),%al
+   18001ee88:	add    %dh,0x18001(%rip)        # 0x180036e8f
    18001ee8e:	add    %al,(%rax)
-   18001ee90:	add    %dl,(%rdi)
-   18001ee92:	add    %eax,0x1(%rax)
-   18001ee98:	mov    $0x92,%al
-   18001ee9a:	add    %eax,0x1(%rax)
-   18001eea0:	rclb   $0x0,0x18001(%rdx)
-   18001eea7:	add    %ah,%al
-   18001eea9:	xchg   %eax,%edx
+   18001ee90:	shlb   $0x0,0x18001(%rip)        # 0x180036e98
+   18001ee97:	add    %ah,(%rax)
+   18001ee99:	xor    $0x18001,%eax
+   18001ee9e:	add    %al,(%rax)
+   18001eea0:	add    %dl,(%rdi)
+   18001eea2:	add    %eax,0x1(%rax)
+   18001eea8:	mov    $0x92,%al
    18001eeaa:	add    %eax,0x1(%rax)
-   18001eeb0:	jo     0x18001ee44
-   18001eeb2:	add    %eax,0x1(%rax)
-   18001eeb8:	nop
+   18001eeb0:	rclb   $0x0,0x18001(%rdx)
+   18001eeb7:	add    %ah,%al
    18001eeb9:	xchg   %eax,%edx
    18001eeba:	add    %eax,0x1(%rax)
-   18001eec0:	adcb   $0x0,0x18001(%rdx)
-   18001eec7:	add    %ah,0x1800192(%rax)
-   18001eecd:	add    %al,(%rax)
-   18001eecf:	add    %dl,0x1800074(%rax)
-   18001eed5:	add    %al,(%rax)
-   18001eed7:	add    %dh,0x73(%rax)
-   18001eeda:	add    %al,0x1(%rax)
-   18001eee0:	rex jbe 0x18001eee3
-   18001eee3:	addb   $0x0,(%rcx)
-   18001eee6:	add    %al,(%rax)
-   18001eee8:	loopne 0x18001ef63
+   18001eec0:	jo     0x18001ee54
+   18001eec2:	add    %eax,0x1(%rax)
+   18001eec8:	nop
+   18001eec9:	xchg   %eax,%edx
+   18001eeca:	add    %eax,0x1(%rax)
+   18001eed0:	adcb   $0x0,0x18001(%rdx)
+   18001eed7:	add    %ah,0x1800192(%rax)
+   18001eedd:	add    %al,(%rax)
+   18001eedf:	add    %dl,0x1800074(%rax)
+   18001eee5:	add    %al,(%rax)
+   18001eee7:	add    %dh,0x73(%rax)
    18001eeea:	add    %al,0x1(%rax)
-   18001eef0:	adc    %dh,0x0(%rcx)
+   18001eef0:	rex jbe 0x18001eef3
    18001eef3:	addb   $0x0,(%rcx)
    18001eef6:	add    %al,(%rax)
-   18001eef8:	loopne 0x18001ef72
+   18001eef8:	loopne 0x18001ef73
    18001eefa:	add    %al,0x1(%rax)
-   18001ef00:	adc    %ch,(%rdi)
-   18001ef02:	add    %eax,0x1(%rax)
-   18001ef08:	adc    %cl,0x1(%rax)
-   18001ef0b:	addb   $0x0,(%rcx)
-   18001ef0e:	add    %al,(%rax)
-   18001ef10:	shrb   0x0(%rbp)
-   18001ef13:	addb   $0x0,(%rcx)
-   18001ef16:	add    %al,(%rax)
-   18001ef18:	shlb   $0x80,0x0(%rdi)
-   18001ef1c:	add    %eax,(%rax)
+   18001ef00:	adc    %dh,0x0(%rcx)
+   18001ef03:	addb   $0x0,(%rcx)
+   18001ef06:	add    %al,(%rax)
+   18001ef08:	loopne 0x18001ef82
+   18001ef0a:	add    %al,0x1(%rax)
+   18001ef10:	adc    %ch,(%rdi)
+   18001ef12:	add    %eax,0x1(%rax)
+   18001ef18:	adc    %cl,0x1(%rax)
+   18001ef1b:	addb   $0x0,(%rcx)
    18001ef1e:	add    %al,(%rax)
-   18001ef20:	movabs 0x6000000001800076,%al
-   18001ef29:	jnp    0x18001ef2b
-   18001ef2b:	addb   $0x0,(%rcx)
+   18001ef20:	shrb   0x0(%rbp)
+   18001ef23:	addb   $0x0,(%rcx)
+   18001ef26:	add    %al,(%rax)
+   18001ef28:	shlb   $0x80,0x0(%rdi)
+   18001ef2c:	add    %eax,(%rax)
    18001ef2e:	add    %al,(%rax)
-   18001ef30:	rex jp 0x18001ef33
-   18001ef33:	addb   $0x0,(%rcx)
-   18001ef36:	add    %al,(%rax)
-   18001ef38:	fdivr  %st(7),%st
-   18001ef3a:	add    %eax,0x1(%rax)
-   18001ef40:	add    %bl,(%rax)
-   18001ef42:	add    %eax,0x1(%rax)
-   18001ef48:	rclb   0x18001(%rdx)
-   18001ef4e:	add    %al,(%rax)
-   18001ef50:	push   %rbp
-   18001ef51:	outsb  %ds:(%rsi),(%dx)
-   18001ef52:	gs js  0x18001efc5
-   18001ef55:	movsxd %gs:0x64(%rbp,%riz,2),%esi
-   18001ef5a:	and    %ah,0x61(%rbx)
-   18001ef5d:	insb   (%dx),%es:(%rdi)
-   18001ef5e:	insb   (%dx),%es:(%rdi)
-   18001ef5f:	add    %al,0x75(%rcx)
-   18001ef62:	je     0x18001efcc
-   18001ef64:	outsb  %gs:(%rsi),(%dx)
-   18001ef66:	je     0x18001efd1
-   18001ef68:	movsxd 0x74(%rcx),%esp
-   18001ef6b:	imul   $0x6f727245,0x6e(%rdi),%ebp
-   18001ef72:	jb     0x18001efae
-   18001ef74:	and    %ah,0x73252873(%rip)        # 0x1f32717ed
-   18001ef7a:	sub    %edi,(%rdx)
-   18001ef7c:	and    %ah,0x75410073(%rip)        # 0x1f542eff5
-   18001ef82:	je     0x18001efec
-   18001ef84:	outsb  %gs:(%rsi),(%dx)
-   18001ef86:	je     0x18001eff1
-   18001ef88:	movsxd 0x74(%rcx),%esp
-   18001ef8b:	imul   $0x6f727245,0x6e(%rdi),%ebp
-   18001ef92:	jb     0x18001efce
-   18001ef94:	and    %al,0x6f(%rbx)
-   18001ef97:	fs and %ch,%gs:0x6f(%rsi)
-   18001ef9c:	je     0x18001efbe
-   18001ef9e:	jb     0x18001f005
-   18001efa0:	movsxd 0x69(%rbp),%esp
-   18001efa3:	jbe    0x18001f00a
-   18001efa5:	add    %al,%fs:(%rax)
-   18001efa8:	push   %rbx
-   18001efa9:	je     0x18001f00c
-   18001efab:	je     0x18001f012
-   18001efad:	and    %ch,0x6f(%rsi)
-   18001efb0:	je     0x18001efd2
-   18001efb2:	jb     0x18001f019
-   18001efb4:	movsxd 0x69(%rbp),%esp
-   18001efb7:	jbe    0x18001f01e
-   18001efb9:	add    %al,%fs:(%rax)
-   18001efbc:	add    %al,(%rax)
-   18001efbe:	add    %al,(%rax)
-   18001efc0:	push   %rbx
-   18001efc1:	je     0x18001f024
-   18001efc3:	je     0x18001f02a
-   18001efc5:	and    %ch,0x69(%rbp)
-   18001efc8:	jae    0x18001f037
-   18001efca:	(bad)
-   18001efcb:	je     0x18001f030
-   18001efcd:	push   $0x72450000
-   18001efd2:	jb     0x18001f043
-   18001efd4:	jb     0x18001f010
-   18001efd6:	and    %ah,0x73(%rip)        # 0x18001f04f
-   18001efdc:	add    %al,(%rax)
-   18001efde:	add    %al,(%rax)
-   18001efe0:	movsxd 0x65(%r11),%esp
-   18001efe4:	jae    0x18001f059
-   18001efe6:	and    %dh,0x6b(%rdi,%rbp,2)
-   18001efea:	outsb  %gs:(%rsi),(%dx)
-   18001efec:	and    %ch,0x6f(%rsi)
-   18001efef:	je     0x18001f011
-   18001eff1:	jb     0x18001f058
-   18001eff3:	movsxd 0x69(%rbp),%esp
-   18001eff6:	jbe    0x18001f05d
-   18001eff8:	add    %al,%fs:(%rax)
-   18001effb:	add    %al,(%rax)
-   18001effd:	add    %al,(%rax)
-   18001efff:	add    %cl,0x6f(%rsi)
-   18001f002:	and    %ah,0x75(%rcx)
-   18001f005:	je     0x18001f06f
-   18001f007:	outsb  %gs:(%rsi),(%dx)
-   18001f009:	je     0x18001f074
-   18001f00b:	movsxd 0x74(%rcx),%esp
-   18001f00e:	and    %dl,%gs:0x72(%rbp)
-   18001f012:	insb   (%dx),%es:(%rdi)
-   18001f013:	and    %dh,0x65(%rbx)
-   18001f016:	je     0x18001f018
-   18001f018:	rex.WRX outsl %ds:(%rsi),(%dx)
-   18001f01a:	and    %dh,0x65(%rdx)
-   18001f01d:	jno    0x18001f094
-   18001f01f:	gs jae 0x18001f096
-   18001f022:	and    %ah,0x63(%rcx)
-   18001f025:	movsxd 0x73(%rbp),%esp
-   18001f028:	jae    0x18001f04a
-   18001f02a:	je     0x18001f09b
-   18001f02c:	imul   $0x20,0x6e(%rbp),%esp
-   18001f030:	push   %rbp
-   18001f031:	jb     0x18001f09f
-   18001f033:	and    %dh,0x65(%rbx)
-   18001f036:	je     0x18001f038
-   18001f038:	rex.XB (bad)
-   18001f03a:	outsb  %ds:(%rsi),(%dx)
-   18001f03b:	outsb  %ds:(%rsi),(%dx)
-   18001f03c:	outsl  %ds:(%rsi),(%dx)
-   18001f03d:	je     0x18001f05f
-   18001f03f:	jb     0x18001f0a6
-   18001f041:	data16 jb 0x18001f0a9
-   18001f044:	jae    0x18001f0ae
-   18001f046:	and    %ah,0x63(%rcx)
-   18001f049:	movsxd 0x73(%rbp),%esp
-   18001f04c:	jae    0x18001f06e
-   18001f04e:	je     0x18001f0bf
-   18001f050:	imul   $0x2e,0x6e(%rbp),%esp
-   18001f054:	and    %al,0x6d(%rbp)
-   18001f057:	jo     0x18001f0cd
-   18001f059:	jns    0x18001f07b
-   18001f05b:	jb     0x18001f0c2
-   18001f05d:	data16 jb 0x18001f0c5
-   18001f060:	jae    0x18001f0ca
-   18001f062:	and    %dh,0x6b(%rdi,%rbp,2)
-   18001f066:	outsb  %gs:(%rsi),(%dx)
-	...
-   18001f070:	rex.XB (bad)
-   18001f072:	outsb  %ds:(%rsi),(%dx)
-   18001f073:	outsb  %ds:(%rsi),(%dx)
-   18001f074:	outsl  %ds:(%rsi),(%dx)
-   18001f075:	je     0x18001f097
-   18001f077:	jb     0x18001f0de
-   18001f079:	data16 jb 0x18001f0e1
-   18001f07c:	jae    0x18001f0e6
-   18001f07e:	and    %ah,0x63(%rcx)
-   18001f081:	movsxd 0x73(%rbp),%esp
-   18001f084:	jae    0x18001f0a6
-   18001f086:	je     0x18001f0f7
-   18001f088:	imul   $0x2e,0x6e(%rbp),%esp
-   18001f08c:	and    %dl,0x65(%rdx)
-   18001f08f:	data16 jb 0x18001f0f7
-   18001f092:	jae    0x18001f0fc
-   18001f094:	and    %al,0x63(%rcx)
-   18001f097:	movsxd 0x73(%rbp),%esp
-   18001f09a:	jae    0x18001f0bc
-   18001f09c:	push   %rsp
-   18001f09d:	outsl  %ds:(%rsi),(%dx)
-   18001f09e:	imul   $0x20,0x6e(%rbp),%esp
-   18001f0a2:	imul   $0x65726c61,0x20(%rbx),%esi
-   18001f0a9:	(bad)
-   18001f0aa:	fs jns 0x18001f0cd
-   18001f0ad:	imul   $0x676f7270,0x20(%rsi),%ebp
-   18001f0b4:	jb     0x18001f11b
-   18001f0b6:	jae    0x18001f12b
-	...
-   18001f0c0:	rex.RXB
-   18001f0c1:	outsb  %gs:(%rsi),(%dx)
-   18001f0c3:	gs jb  0x18001f127
-   18001f0c6:	je     0x18001f12d
-   18001f0c8:	and    %dl,%fs:0x52(%rbp)
-   18001f0cc:	rex.WR cmp (%rax),%r12b
-   18001f0cf:	and    $0x73,%eax
-   18001f0d4:	add    %al,(%rax)
-   18001f0d6:	add    %al,(%rax)
-   18001f0d8:	(bad)
-   18001f0d9:	add    %dh,0x0(%rbp)
-   18001f0dc:	je     0x18001f0de
-   18001f0de:	push   $0x72006f00
-   18001f0e3:	add    %ch,0x0(%rcx)
-   18001f0e6:	jp     0x18001f0e8
+   18001ef30:	movabs 0x6000000001800076,%al
+   18001ef39:	jnp    0x18001ef3b
+   18001ef3b:	addb   $0x0,(%rcx)
+   18001ef3e:	add    %al,(%rax)
+   18001ef40:	rex jp 0x18001ef43
+   18001ef43:	addb   $0x0,(%rcx)
+   18001ef46:	add    %al,(%rax)
+   18001ef48:	fdivr  %st(7),%st
+   18001ef4a:	add    %eax,0x1(%rax)
+   18001ef50:	add    %bl,(%rax)
+   18001ef52:	add    %eax,0x1(%rax)
+   18001ef58:	rclb   0x18001(%rdx)
+   18001ef5e:	add    %al,(%rax)
+   18001ef60:	push   %rbp
+   18001ef61:	outsb  %ds:(%rsi),(%dx)
+   18001ef62:	gs js  0x18001efd5
+   18001ef65:	movsxd %gs:0x64(%rbp,%riz,2),%esi
+   18001ef6a:	and    %ah,0x61(%rbx)
+   18001ef6d:	insb   (%dx),%es:(%rdi)
+   18001ef6e:	insb   (%dx),%es:(%rdi)
+   18001ef6f:	add    %al,0x75(%rcx)
+   18001ef72:	je     0x18001efdc
+   18001ef74:	outsb  %gs:(%rsi),(%dx)
+   18001ef76:	je     0x18001efe1
+   18001ef78:	movsxd 0x74(%rcx),%esp
+   18001ef7b:	imul   $0x6f727245,0x6e(%rdi),%ebp
+   18001ef82:	jb     0x18001efbe
+   18001ef84:	and    %ah,0x73252873(%rip)        # 0x1f32717fd
+   18001ef8a:	sub    %edi,(%rdx)
+   18001ef8c:	and    %ah,0x75410073(%rip)        # 0x1f542f005
+   18001ef92:	je     0x18001effc
+   18001ef94:	outsb  %gs:(%rsi),(%dx)
+   18001ef96:	je     0x18001f001
+   18001ef98:	movsxd 0x74(%rcx),%esp
+   18001ef9b:	imul   $0x6f727245,0x6e(%rdi),%ebp
+   18001efa2:	jb     0x18001efde
+   18001efa4:	and    %al,0x6f(%rbx)
+   18001efa7:	fs and %ch,%gs:0x6f(%rsi)
+   18001efac:	je     0x18001efce
+   18001efae:	jb     0x18001f015
+   18001efb0:	movsxd 0x69(%rbp),%esp
+   18001efb3:	jbe    0x18001f01a
+   18001efb5:	add    %al,%fs:(%rax)
+   18001efb8:	push   %rbx
+   18001efb9:	je     0x18001f01c
+   18001efbb:	je     0x18001f022
+   18001efbd:	and    %ch,0x6f(%rsi)
+   18001efc0:	je     0x18001efe2
+   18001efc2:	jb     0x18001f029
+   18001efc4:	movsxd 0x69(%rbp),%esp
+   18001efc7:	jbe    0x18001f02e
+   18001efc9:	add    %al,%fs:(%rax)
+   18001efcc:	add    %al,(%rax)
+   18001efce:	add    %al,(%rax)
+   18001efd0:	push   %rbx
+   18001efd1:	je     0x18001f034
+   18001efd3:	je     0x18001f03a
+   18001efd5:	and    %ch,0x69(%rbp)
+   18001efd8:	jae    0x18001f047
+   18001efda:	(bad)
+   18001efdb:	je     0x18001f040
+   18001efdd:	push   $0x72450000
+   18001efe2:	jb     0x18001f053
+   18001efe4:	jb     0x18001f020
+   18001efe6:	and    %ah,0x73(%rip)        # 0x18001f05f
+   18001efec:	add    %al,(%rax)
+   18001efee:	add    %al,(%rax)
+   18001eff0:	movsxd 0x65(%r11),%esp
+   18001eff4:	jae    0x18001f069
+   18001eff6:	and    %dh,0x6b(%rdi,%rbp,2)
+   18001effa:	outsb  %gs:(%rsi),(%dx)
+   18001effc:	and    %ch,0x6f(%rsi)
+   18001efff:	je     0x18001f021
+   18001f001:	jb     0x18001f068
+   18001f003:	movsxd 0x69(%rbp),%esp
+   18001f006:	jbe    0x18001f06d
+   18001f008:	add    %al,%fs:(%rax)
+   18001f00b:	add    %al,(%rax)
+   18001f00d:	add    %al,(%rax)
+   18001f00f:	add    %cl,0x6f(%rsi)
+   18001f012:	and    %ah,0x75(%rcx)
+   18001f015:	je     0x18001f07f
+   18001f017:	outsb  %gs:(%rsi),(%dx)
+   18001f019:	je     0x18001f084
+   18001f01b:	movsxd 0x74(%rcx),%esp
+   18001f01e:	and    %dl,%gs:0x72(%rbp)
+   18001f022:	insb   (%dx),%es:(%rdi)
+   18001f023:	and    %dh,0x65(%rbx)
+   18001f026:	je     0x18001f028
+   18001f028:	rex.WRX outsl %ds:(%rsi),(%dx)
+   18001f02a:	and    %dh,0x65(%rdx)
+   18001f02d:	jno    0x18001f0a4
+   18001f02f:	gs jae 0x18001f0a6
+   18001f032:	and    %ah,0x63(%rcx)
+   18001f035:	movsxd 0x73(%rbp),%esp
+   18001f038:	jae    0x18001f05a
+   18001f03a:	je     0x18001f0ab
+   18001f03c:	imul   $0x20,0x6e(%rbp),%esp
+   18001f040:	push   %rbp
+   18001f041:	jb     0x18001f0af
+   18001f043:	and    %dh,0x65(%rbx)
+   18001f046:	je     0x18001f048
+   18001f048:	rex.XB (bad)
+   18001f04a:	outsb  %ds:(%rsi),(%dx)
+   18001f04b:	outsb  %ds:(%rsi),(%dx)
+   18001f04c:	outsl  %ds:(%rsi),(%dx)
+   18001f04d:	je     0x18001f06f
+   18001f04f:	jb     0x18001f0b6
+   18001f051:	data16 jb 0x18001f0b9
+   18001f054:	jae    0x18001f0be
+   18001f056:	and    %ah,0x63(%rcx)
+   18001f059:	movsxd 0x73(%rbp),%esp
+   18001f05c:	jae    0x18001f07e
+   18001f05e:	je     0x18001f0cf
+   18001f060:	imul   $0x2e,0x6e(%rbp),%esp
+   18001f064:	and    %al,0x6d(%rbp)
+   18001f067:	jo     0x18001f0dd
+   18001f069:	jns    0x18001f08b
+   18001f06b:	jb     0x18001f0d2
+   18001f06d:	data16 jb 0x18001f0d5
+   18001f070:	jae    0x18001f0da
+   18001f072:	and    %dh,0x6b(%rdi,%rbp,2)
+   18001f076:	outsb  %gs:(%rsi),(%dx)
+	...
+   18001f080:	rex.XB (bad)
+   18001f082:	outsb  %ds:(%rsi),(%dx)
+   18001f083:	outsb  %ds:(%rsi),(%dx)
+   18001f084:	outsl  %ds:(%rsi),(%dx)
+   18001f085:	je     0x18001f0a7
+   18001f087:	jb     0x18001f0ee
+   18001f089:	data16 jb 0x18001f0f1
+   18001f08c:	jae    0x18001f0f6
+   18001f08e:	and    %ah,0x63(%rcx)
+   18001f091:	movsxd 0x73(%rbp),%esp
+   18001f094:	jae    0x18001f0b6
+   18001f096:	je     0x18001f107
+   18001f098:	imul   $0x2e,0x6e(%rbp),%esp
+   18001f09c:	and    %dl,0x65(%rdx)
+   18001f09f:	data16 jb 0x18001f107
+   18001f0a2:	jae    0x18001f10c
+   18001f0a4:	and    %al,0x63(%rcx)
+   18001f0a7:	movsxd 0x73(%rbp),%esp
+   18001f0aa:	jae    0x18001f0cc
+   18001f0ac:	push   %rsp
+   18001f0ad:	outsl  %ds:(%rsi),(%dx)
+   18001f0ae:	imul   $0x20,0x6e(%rbp),%esp
+   18001f0b2:	imul   $0x65726c61,0x20(%rbx),%esi
+   18001f0b9:	(bad)
+   18001f0ba:	fs jns 0x18001f0dd
+   18001f0bd:	imul   $0x676f7270,0x20(%rsi),%ebp
+   18001f0c4:	jb     0x18001f12b
+   18001f0c6:	jae    0x18001f13b
+	...
+   18001f0d0:	rex.RXB
+   18001f0d1:	outsb  %gs:(%rsi),(%dx)
+   18001f0d3:	gs jb  0x18001f137
+   18001f0d6:	je     0x18001f13d
+   18001f0d8:	and    %dl,%fs:0x52(%rbp)
+   18001f0dc:	rex.WR cmp (%rax),%r12b
+   18001f0df:	and    $0x73,%eax
+   18001f0e4:	add    %al,(%rax)
+   18001f0e6:	add    %al,(%rax)
    18001f0e8:	(bad)
-   18001f0e9:	add    %dh,0x69(%rax,%rax,1)
-   18001f0ed:	add    %ch,0x0(%rdi)
-   18001f0f0:	outsb  %ds:(%rsi),(%dx)
-   18001f0f1:	add    %bl,0x0(%rdi)
-   18001f0f4:	movsxd (%rax),%eax
-   18001f0f6:	outsl  %ds:(%rsi),(%dx)
-   18001f0f7:	add    %ah,0x65(%rax,%rax,1)
-   18001f0fb:	add    %al,(%rax)
-   18001f0fd:	add    %al,(%rax)
-   18001f0ff:	add    %cl,0x6e(%rcx)
-   18001f102:	jbe    0x18001f165
-   18001f104:	insb   (%dx),%es:(%rdi)
-   18001f105:	imul   $0x203a4c52,0x55(%rax,%riz,1),%esp
-   18001f10d:	and    $0x80073,%eax
-   18001f112:	add    %al,(%rax)
-   18001f114:	sbb    $0x0,%al
-   18001f116:	add    %al,(%rax)
-   18001f118:	push   %rcx
-   18001f119:	rex.WRXB
-   18001f11a:	rex.B jne 0x18001f191
-   18001f11d:	push   $0x70747448
-   18001f122:	push   %rbx
-   18001f123:	gs jb  0x18001f19c
-   18001f126:	gs jb  0x18001f17b
-   18001f129:	gs jo  0x18001f198
-   18001f12c:	jns    0x18001f176
-   18001f12e:	(bad)
-   18001f12f:	outsb  %ds:(%rsi),(%dx)
-   18001f130:	fs insb (%dx),%es:(%rdi)
-   18001f132:	gs jb  0x18001f135
-   18001f135:	add    %al,(%rax)
-   18001f137:	add    %cl,(%rbx)
-	...
-   18001f175:	add    %al,(%rax)
-   18001f177:	add    %al,-0x48(%rax)
-   18001f17a:	add    0x1(%rax),%al
-   18001f180:	push   %rcx
-   18001f181:	rex.WRXB
-   18001f182:	rex.B jne 0x18001f1f9
-   18001f185:	push   $0x70747448
-   18001f18a:	push   %rbx
-   18001f18b:	gs jb  0x18001f204
-   18001f18e:	gs jb  0x18001f1e3
-   18001f191:	gs jo  0x18001f200
-   18001f194:	jns    0x18001f1de
-   18001f196:	(bad)
-   18001f197:	outsb  %ds:(%rsi),(%dx)
-   18001f198:	fs insb (%dx),%es:(%rdi)
-   18001f19a:	gs jb  0x18001f19d
-	...
-   18001f1a5:	add    %al,(%rax)
-   18001f1a7:	add    %dh,0x180014a(%rax)
-   18001f1ad:	add    %al,(%rax)
-   18001f1af:	add    %dl,(%rax)
-   18001f1b1:	int1
-   18001f1b2:	add    %eax,0x1(%rax)
-   18001f1b8:	cmp    %dh,%cl
-   18001f1ba:	add    %eax,0x1(%rax)
-   18001f1c0:	rorb   $0x80,0x1(%rdx)
-   18001f1c4:	add    %eax,(%rax)
-	...
-   18001f1ce:	add    %al,(%rax)
-   18001f1d0:	js     0x18001f1c3
-   18001f1d2:	add    %eax,0x1(%rax)
-	...
-   18001f1e0:	add    %al,(%rcx)
-   18001f1e2:	add    0x1(%rax),%al
-   18001f1e8:	xor    %dh,0x1(%rbx)
-   18001f1eb:	addb   $0x0,(%rcx)
-   18001f1ee:	add    %al,(%rax)
-   18001f1f0:	jo     0x18001f265
-   18001f1f2:	add    %eax,0x1(%rax)
-   18001f1f8:	(bad)
-   18001f1f9:	jae    0x18001f1fc
+   18001f0e9:	add    %dh,0x0(%rbp)
+   18001f0ec:	je     0x18001f0ee
+   18001f0ee:	push   $0x72006f00
+   18001f0f3:	add    %ch,0x0(%rcx)
+   18001f0f6:	jp     0x18001f0f8
+   18001f0f8:	(bad)
+   18001f0f9:	add    %dh,0x69(%rax,%rax,1)
+   18001f0fd:	add    %ch,0x0(%rdi)
+   18001f100:	outsb  %ds:(%rsi),(%dx)
+   18001f101:	add    %bl,0x0(%rdi)
+   18001f104:	movsxd (%rax),%eax
+   18001f106:	outsl  %ds:(%rsi),(%dx)
+   18001f107:	add    %ah,0x65(%rax,%rax,1)
+   18001f10b:	add    %al,(%rax)
+   18001f10d:	add    %al,(%rax)
+   18001f10f:	add    %cl,0x6e(%rcx)
+   18001f112:	jbe    0x18001f175
+   18001f114:	insb   (%dx),%es:(%rdi)
+   18001f115:	imul   $0x203a4c52,0x55(%rax,%riz,1),%esp
+   18001f11d:	and    $0x80073,%eax
+   18001f122:	add    %al,(%rax)
+   18001f124:	sbb    $0x0,%al
+   18001f126:	add    %al,(%rax)
+   18001f128:	push   %rcx
+   18001f129:	rex.WRXB
+   18001f12a:	rex.B jne 0x18001f1a1
+   18001f12d:	push   $0x70747448
+   18001f132:	push   %rbx
+   18001f133:	gs jb  0x18001f1ac
+   18001f136:	gs jb  0x18001f18b
+   18001f139:	gs jo  0x18001f1a8
+   18001f13c:	jns    0x18001f186
+   18001f13e:	(bad)
+   18001f13f:	outsb  %ds:(%rsi),(%dx)
+   18001f140:	fs insb (%dx),%es:(%rdi)
+   18001f142:	gs jb  0x18001f145
+   18001f145:	add    %al,(%rax)
+   18001f147:	add    %cl,(%rbx)
+	...
+   18001f185:	add    %al,(%rax)
+   18001f187:	add    %al,-0x48(%rax)
+   18001f18a:	add    0x1(%rax),%al
+   18001f190:	push   %rcx
+   18001f191:	rex.WRXB
+   18001f192:	rex.B jne 0x18001f209
+   18001f195:	push   $0x70747448
+   18001f19a:	push   %rbx
+   18001f19b:	gs jb  0x18001f214
+   18001f19e:	gs jb  0x18001f1f3
+   18001f1a1:	gs jo  0x18001f210
+   18001f1a4:	jns    0x18001f1ee
+   18001f1a6:	(bad)
+   18001f1a7:	outsb  %ds:(%rsi),(%dx)
+   18001f1a8:	fs insb (%dx),%es:(%rdi)
+   18001f1aa:	gs jb  0x18001f1ad
+	...
+   18001f1b5:	add    %al,(%rax)
+   18001f1b7:	add    %dh,0x180014a(%rax)
+   18001f1bd:	add    %al,(%rax)
+   18001f1bf:	add    %ah,(%rax)
+   18001f1c1:	int1
+   18001f1c2:	add    %eax,0x1(%rax)
+   18001f1c8:	rex.W int1
+   18001f1ca:	add    %eax,0x1(%rax)
+   18001f1d0:	rorb   $0x80,0x1(%rdx)
+   18001f1d4:	add    %eax,(%rax)
+	...
+   18001f1de:	add    %al,(%rax)
+   18001f1e0:	mov    %dh,%cl
+   18001f1e2:	add    %eax,0x1(%rax)
+	...
+   18001f1f0:	add    %al,(%rcx)
+   18001f1f2:	add    0x1(%rax),%al
+   18001f1f8:	xor    %dh,0x1(%rbx)
    18001f1fb:	addb   $0x0,(%rcx)
    18001f1fe:	add    %al,(%rax)
-   18001f200:	nop
-   18001f201:	pop    %rax
+   18001f200:	jo     0x18001f275
    18001f202:	add    %eax,0x1(%rax)
-   18001f208:	mov    $0x92,%al
-   18001f20a:	add    %eax,0x1(%rax)
-   18001f210:	rclb   $0x0,0x18001(%rdx)
-   18001f217:	add    %ah,%al
-   18001f219:	xchg   %eax,%edx
+   18001f208:	(bad)
+   18001f209:	jae    0x18001f20c
+   18001f20b:	addb   $0x0,(%rcx)
+   18001f20e:	add    %al,(%rax)
+   18001f210:	nop
+   18001f211:	pop    %rax
+   18001f212:	add    %eax,0x1(%rax)
+   18001f218:	mov    $0x92,%al
    18001f21a:	add    %eax,0x1(%rax)
-   18001f220:	jo     0x18001f1b4
-   18001f222:	add    %eax,0x1(%rax)
-   18001f228:	nop
+   18001f220:	rclb   $0x0,0x18001(%rdx)
+   18001f227:	add    %ah,%al
    18001f229:	xchg   %eax,%edx
    18001f22a:	add    %eax,0x1(%rax)
-   18001f230:	adcb   $0x0,0x18001(%rdx)
-   18001f237:	add    %ah,0x1800192(%rax)
-   18001f23d:	add    %al,(%rax)
-   18001f23f:	add    %ah,0x67(%rax)
-   18001f242:	add    %eax,0x1(%rax)
-   18001f248:	addb   $0x0,0x18001(%rbx)
-   18001f24f:	add    %al,0x61(%rbx)
-   18001f252:	insb   (%dx),%es:(%rdi)
-   18001f253:	insb   (%dx),%es:(%rdi)
-   18001f254:	(bad)
-   18001f256:	movsxd 0x20(%rbx),%ebp
-   18001f259:	jb     0x18001f2c0
-   18001f25b:	movsxd 0x69(%rbp),%esp
-   18001f25e:	jbe    0x18001f2c5
-   18001f260:	fs and %al,%fs:0x65(%rsi)
-   18001f265:	gs insb (%dx),%es:(%rdi)
-   18001f267:	and    %ah,0x72(%rsi)
-   18001f26a:	gs and %dh,%gs:0x20(%rdi,%rbp,2)
-   18001f270:	movsxd 0x73(%rdi,%rbp,2),%ebp
-   18001f274:	and    %dh,%gs:0x69(%rax,%rbp,2)
-   18001f279:	jae    0x18001f29b
-   18001f27b:	jo     0x18001f2de
-   18001f27d:	gs add %al,%gs:(%eax)
-   18001f282:	add    %al,(%rax)
-   18001f284:	add    %al,(%rax)
-   18001f286:	add    %al,(%rax)
-   18001f288:	rex.WB outsb %ds:(%rsi),(%dx)
-   18001f28a:	jbe    0x18001f2ed
-   18001f28c:	insb   (%dx),%es:(%rdi)
-   18001f28d:	imul   $0x6f687465,0x4d(%rax,%riz,1),%esp
-   18001f295:	add    %al,%fs:(%rax)
+   18001f230:	jo     0x18001f1c4
+   18001f232:	add    %eax,0x1(%rax)
+   18001f238:	nop
+   18001f239:	xchg   %eax,%edx
+   18001f23a:	add    %eax,0x1(%rax)
+   18001f240:	adcb   $0x0,0x18001(%rdx)
+   18001f247:	add    %ah,0x1800192(%rax)
+   18001f24d:	add    %al,(%rax)
+   18001f24f:	add    %ah,0x67(%rax)
+   18001f252:	add    %eax,0x1(%rax)
+   18001f258:	addb   $0x0,0x18001(%rbx)
+   18001f25f:	add    %al,0x61(%rbx)
+   18001f262:	insb   (%dx),%es:(%rdi)
+   18001f263:	insb   (%dx),%es:(%rdi)
+   18001f264:	(bad)
+   18001f266:	movsxd 0x20(%rbx),%ebp
+   18001f269:	jb     0x18001f2d0
+   18001f26b:	movsxd 0x69(%rbp),%esp
+   18001f26e:	jbe    0x18001f2d5
+   18001f270:	fs and %al,%fs:0x65(%rsi)
+   18001f275:	gs insb (%dx),%es:(%rdi)
+   18001f277:	and    %ah,0x72(%rsi)
+   18001f27a:	gs and %dh,%gs:0x20(%rdi,%rbp,2)
+   18001f280:	movsxd 0x73(%rdi,%rbp,2),%ebp
+   18001f284:	and    %dh,%gs:0x69(%rax,%rbp,2)
+   18001f289:	jae    0x18001f2ab
+   18001f28b:	jo     0x18001f2ee
+   18001f28d:	gs add %al,%gs:(%eax)
+   18001f292:	add    %al,(%rax)
+   18001f294:	add    %al,(%rax)
+   18001f296:	add    %al,(%rax)
    18001f298:	rex.WB outsb %ds:(%rsi),(%dx)
    18001f29a:	jbe    0x18001f2fd
    18001f29c:	insb   (%dx),%es:(%rdi)
-   18001f29d:	imul   $0x4c52,0x55(%rax,%riz,1),%esp
-   18001f2a5:	add    %al,(%rax)
-   18001f2a7:	add    %cl,0x6e(%rcx)
+   18001f29d:	imul   $0x6f687465,0x4d(%rax,%riz,1),%esp
+   18001f2a5:	add    %al,%fs:(%rax)
+   18001f2a8:	rex.WB outsb %ds:(%rsi),(%dx)
    18001f2aa:	jbe    0x18001f30d
    18001f2ac:	insb   (%dx),%es:(%rdi)
-   18001f2ad:	imul   $0x75746174,0x53(%rax,%riz,1),%esp
-   18001f2b5:	jae    0x18001f2b7
+   18001f2ad:	imul   $0x4c52,0x55(%rax,%riz,1),%esp
+   18001f2b5:	add    %al,(%rax)
    18001f2b7:	add    %cl,0x6e(%rcx)
    18001f2ba:	jbe    0x18001f31d
    18001f2bc:	insb   (%dx),%es:(%rdi)
-   18001f2bd:	imul   $0x65646165,0x48(%rax,%riz,1),%esp
-   18001f2c5:	jb     0x18001f2c7
-   18001f2c7:	add    %ch,(%rdi)
-   18001f2c9:	add    %al,(%rax)
-   18001f2cb:	add    %al,(%rax)
-   18001f2cd:	add    %al,(%rax)
-   18001f2cf:	add    %cl,0x6e(%rcx)
-   18001f2d2:	jbe    0x18001f335
-   18001f2d4:	insb   (%dx),%es:(%rdi)
-   18001f2d5:	imul   $0x65757165,0x72(%rax,%riz,1),%esp
-   18001f2dd:	jae    0x18001f353
-   18001f2df:	cmp    (%rax),%ah
-   18001f2e1:	and    $0x73,%eax
-   18001f2e6:	add    %al,(%rax)
-   18001f2e8:	cmp    $0x2f,%al
-   18001f2ea:	(bad)
-   18001f2eb:	outsl  %ds:(%rsi),(%dx)
-   18001f2ec:	fs jns 0x18001f32d
-   18001f2ef:	cmp    $0x2f,%al
-   18001f2f1:	push   $0x3e6c6d74
+   18001f2bd:	imul   $0x75746174,0x53(%rax,%riz,1),%esp
+   18001f2c5:	jae    0x18001f2c7
+   18001f2c7:	add    %cl,0x6e(%rcx)
+   18001f2ca:	jbe    0x18001f32d
+   18001f2cc:	insb   (%dx),%es:(%rdi)
+   18001f2cd:	imul   $0x65646165,0x48(%rax,%riz,1),%esp
+   18001f2d5:	jb     0x18001f2d7
+   18001f2d7:	add    %ch,(%rdi)
+   18001f2d9:	add    %al,(%rax)
+   18001f2db:	add    %al,(%rax)
+   18001f2dd:	add    %al,(%rax)
+   18001f2df:	add    %cl,0x6e(%rcx)
+   18001f2e2:	jbe    0x18001f345
+   18001f2e4:	insb   (%dx),%es:(%rdi)
+   18001f2e5:	imul   $0x65757165,0x72(%rax,%riz,1),%esp
+   18001f2ed:	jae    0x18001f363
+   18001f2ef:	cmp    (%rax),%ah
+   18001f2f1:	and    $0x73,%eax
    18001f2f6:	add    %al,(%rax)
    18001f2f8:	cmp    $0x2f,%al
-   18001f2fa:	je     0x18001f365
-   18001f2fc:	je     0x18001f36a
-   18001f2fe:	gs ds cmp $0x2f,%al
-   18001f302:	push   $0x3e646165
-   18001f307:	cmp    $0x62,%al
-   18001f309:	outsl  %ds:(%rsi),(%dx)
-   18001f30a:	fs jns 0x18001f34b
-   18001f30d:	add    %al,(%rax)
-   18001f30f:	add    %bh,(%rax,%rbp,2)
-   18001f312:	je     0x18001f381
-   18001f314:	insb   (%dx),%es:(%rdi)
-   18001f315:	ds cmp $0x68,%al
-   18001f318:	gs (bad)
-   18001f31a:	fs ds cmp $0x74,%al
-   18001f31e:	imul   $0xa0d003e,0x65(%rsp,%rbp,2),%esi
-   18001f326:	or     $0xa,%eax
-   18001f32b:	add    %al,(%rax)
-   18001f32d:	add    %al,(%rax)
-   18001f32f:	add    %cl,0x54(%rax)
-   18001f332:	push   %rsp
-   18001f333:	push   %rax
-   18001f334:	(bad)
-   18001f335:	xor    %ebp,(%rsi)
-   18001f337:	xor    %ah,(%rax)
-   18001f339:	xor    (%rax),%dh
-   18001f33b:	xor    %ah,(%rax)
-   18001f33d:	rex.WRXB
-   18001f33e:	rex.WXB and %cl,0x6e6f430a(%rip)        # 0x1ee71364f
-   18001f345:	je     0x18001f3ac
-   18001f347:	outsb  %ds:(%rsi),(%dx)
-   18001f348:	je     0x18001f377
-   18001f34a:	push   %rsp
-   18001f34b:	jns    0x18001f3bd
-   18001f34d:	cmp    %gs:(%rax),%ah
-   18001f350:	je     0x18001f3b7
-   18001f352:	js     0x18001f3c8
-   18001f354:	(bad)
-   18001f355:	push   $0x3b6c6d74
-   18001f35a:	and    %ah,0x68(%rbx)
-   18001f35d:	(bad)
-   18001f35e:	jb     0x18001f3d3
-   18001f360:	gs je  0x18001f3a0
-   18001f363:	and    0x74(%rbp),%dh
-   18001f366:	sub    $0x2238,%ax
-   18001f36a:	or     $0x6e6f430a,%eax
-   18001f36f:	je     0x18001f3d6
-   18001f371:	outsb  %ds:(%rsi),(%dx)
-   18001f372:	je     0x18001f3a1
-   18001f374:	rex.WR
-   18001f375:	outsb  %gs:(%rsi),(%dx)
-   18001f377:	addr32 je 0x18001f3e2
-   18001f37a:	cmp    (%rax),%ah
-   18001f37c:	add    %al,(%rax)
-   18001f37e:	add    %al,(%rax)
-   18001f380:	rex.WB outsb %ds:(%rsi),(%dx)
-   18001f382:	jbe    0x18001f3e5
-   18001f384:	insb   (%dx),%es:(%rdi)
-   18001f385:	imul   $0x61726570,0x6f(%rax,%riz,1),%esp
-   18001f38d:	je     0x18001f3f8
-   18001f38f:	outsl  %ds:(%rsi),(%dx)
-   18001f390:	outsb  %ds:(%rsi),(%dx)
-   18001f391:	and    %ah,0x73(%rip)        # 0x18001f40a
-   18001f397:	add    %cl,0x6e(%rcx)
-   18001f39a:	jbe    0x18001f3fd
-   18001f39c:	insb   (%dx),%es:(%rdi)
-   18001f39d:	imul   $0x70204c52,0x55(%rax,%riz,1),%esp
-   18001f3a5:	(bad)
-   18001f3a6:	je     0x18001f410
-   18001f3a8:	and    %ah,0x73(%rip)        # 0x18001f421
-   18001f3ae:	add    %al,(%rax)
-   18001f3b0:	push   $0x74007400
-   18001f3b5:	add    %dh,0x0(%rax)
-   18001f3b8:	cmp    (%rax),%al
-   18001f3ba:	(bad)
-   18001f3bb:	add    %ch,(%rdi)
-   18001f3bd:	add    %dh,(%rcx)
-   18001f3bf:	add    %dh,(%rdx)
-   18001f3c1:	add    %dh,(%rdi)
-   18001f3c3:	add    %ch,(%rsi)
-   18001f3c5:	add    %dh,(%rax)
-   18001f3c7:	add    %ch,(%rsi)
-   18001f3c9:	add    %dh,(%rax)
-   18001f3cb:	add    %ch,(%rsi)
+   18001f2fa:	(bad)
+   18001f2fb:	outsl  %ds:(%rsi),(%dx)
+   18001f2fc:	fs jns 0x18001f33d
+   18001f2ff:	cmp    $0x2f,%al
+   18001f301:	push   $0x3e6c6d74
+   18001f306:	add    %al,(%rax)
+   18001f308:	cmp    $0x2f,%al
+   18001f30a:	je     0x18001f375
+   18001f30c:	je     0x18001f37a
+   18001f30e:	gs ds cmp $0x2f,%al
+   18001f312:	push   $0x3e646165
+   18001f317:	cmp    $0x62,%al
+   18001f319:	outsl  %ds:(%rsi),(%dx)
+   18001f31a:	fs jns 0x18001f35b
+   18001f31d:	add    %al,(%rax)
+   18001f31f:	add    %bh,(%rax,%rbp,2)
+   18001f322:	je     0x18001f391
+   18001f324:	insb   (%dx),%es:(%rdi)
+   18001f325:	ds cmp $0x68,%al
+   18001f328:	gs (bad)
+   18001f32a:	fs ds cmp $0x74,%al
+   18001f32e:	imul   $0xa0d003e,0x65(%rsp,%rbp,2),%esi
+   18001f336:	or     $0xa,%eax
+   18001f33b:	add    %al,(%rax)
+   18001f33d:	add    %al,(%rax)
+   18001f33f:	add    %cl,0x54(%rax)
+   18001f342:	push   %rsp
+   18001f343:	push   %rax
+   18001f344:	(bad)
+   18001f345:	xor    %ebp,(%rsi)
+   18001f347:	xor    %ah,(%rax)
+   18001f349:	xor    (%rax),%dh
+   18001f34b:	xor    %ah,(%rax)
+   18001f34d:	rex.WRXB
+   18001f34e:	rex.WXB and %cl,0x6e6f430a(%rip)        # 0x1ee71365f
+   18001f355:	je     0x18001f3bc
+   18001f357:	outsb  %ds:(%rsi),(%dx)
+   18001f358:	je     0x18001f387
+   18001f35a:	push   %rsp
+   18001f35b:	jns    0x18001f3cd
+   18001f35d:	cmp    %gs:(%rax),%ah
+   18001f360:	je     0x18001f3c7
+   18001f362:	js     0x18001f3d8
+   18001f364:	(bad)
+   18001f365:	push   $0x3b6c6d74
+   18001f36a:	and    %ah,0x68(%rbx)
+   18001f36d:	(bad)
+   18001f36e:	jb     0x18001f3e3
+   18001f370:	gs je  0x18001f3b0
+   18001f373:	and    0x74(%rbp),%dh
+   18001f376:	sub    $0x2238,%ax
+   18001f37a:	or     $0x6e6f430a,%eax
+   18001f37f:	je     0x18001f3e6
+   18001f381:	outsb  %ds:(%rsi),(%dx)
+   18001f382:	je     0x18001f3b1
+   18001f384:	rex.WR
+   18001f385:	outsb  %gs:(%rsi),(%dx)
+   18001f387:	addr32 je 0x18001f3f2
+   18001f38a:	cmp    (%rax),%ah
+   18001f38c:	add    %al,(%rax)
+   18001f38e:	add    %al,(%rax)
+   18001f390:	rex.WB outsb %ds:(%rsi),(%dx)
+   18001f392:	jbe    0x18001f3f5
+   18001f394:	insb   (%dx),%es:(%rdi)
+   18001f395:	imul   $0x61726570,0x6f(%rax,%riz,1),%esp
+   18001f39d:	je     0x18001f408
+   18001f39f:	outsl  %ds:(%rsi),(%dx)
+   18001f3a0:	outsb  %ds:(%rsi),(%dx)
+   18001f3a1:	and    %ah,0x73(%rip)        # 0x18001f41a
+   18001f3a7:	add    %cl,0x6e(%rcx)
+   18001f3aa:	jbe    0x18001f40d
+   18001f3ac:	insb   (%dx),%es:(%rdi)
+   18001f3ad:	imul   $0x70204c52,0x55(%rax,%riz,1),%esp
+   18001f3b5:	(bad)
+   18001f3b6:	je     0x18001f420
+   18001f3b8:	and    %ah,0x73(%rip)        # 0x18001f431
+   18001f3be:	add    %al,(%rax)
+   18001f3c0:	push   $0x74007400
+   18001f3c5:	add    %dh,0x0(%rax)
+   18001f3c8:	cmp    (%rax),%al
+   18001f3ca:	(bad)
+   18001f3cb:	add    %ch,(%rdi)
    18001f3cd:	add    %dh,(%rcx)
-   18001f3cf:	add    %bh,(%rdx)
-   18001f3d1:	add    %al,(%rax)
-   18001f3d3:	add    %al,(%rax)
-   18001f3d5:	add    %al,(%rax)
-   18001f3d7:	add    %cl,0x6e(%rcx)
-   18001f3da:	jbe    0x18001f43d
-   18001f3dc:	insb   (%dx),%es:(%rdi)
-   18001f3dd:	imul   $0x25204c52,0x55(%rax,%riz,1),%esp
-   18001f3e5:	jae    0x18001f3e7
-   18001f3e7:	add    %cl,0xa(%rip)        # 0x18001f3f7
-   18001f3ed:	add    %al,(%rax)
-   18001f3ef:	add    %cl,0x6e(%rcx)
-   18001f3f2:	jbe    0x18001f455
-   18001f3f4:	insb   (%dx),%es:(%rdi)
-   18001f3f5:	imul   $0x69737265,0x76(%rax,%riz,1),%esp
-   18001f3fd:	outsl  %ds:(%rsi),(%dx)
-   18001f3fe:	outsb  %ds:(%rsi),(%dx)
-   18001f3ff:	add    %ch,0x74(%rax)
-   18001f402:	je     0x18001f474
-   18001f404:	cmp    (%rdi),%ch
-   18001f406:	(bad)
-   18001f407:	xor    %esi,(%rdx)
-   18001f409:	(bad)
-   18001f40a:	cs xor %ch,(%rsi)
-   18001f40d:	xor    %ch,(%rsi)
-   18001f40f:	xor    %edi,(%rdx)
-   18001f411:	and    $0x32252f31,%eax
-	...
-   18001f426:	add    %al,(%rax)
-   18001f428:	add    %ah,(%rdx)
-   18001f42a:	add    %al,0x1(%rax)
-   18001f430:	(bad)
-   18001f431:	hlt
-   18001f432:	add    %eax,0x1(%rax)
-   18001f438:	xor    $0x1,%ah
-   18001f43b:	addb   $0x0,(%rcx)
-   18001f43e:	add    %al,(%rax)
-   18001f440:	rorb   $0x80,0x1(%rdx)
-   18001f444:	add    %eax,(%rax)
-	...
-   18001f44e:	add    %al,(%rax)
-   18001f450:	shl    $0x1,%ah
-   18001f453:	addb   $0x0,(%rcx)
+   18001f3cf:	add    %dh,(%rdx)
+   18001f3d1:	add    %dh,(%rdi)
+   18001f3d3:	add    %ch,(%rsi)
+   18001f3d5:	add    %dh,(%rax)
+   18001f3d7:	add    %ch,(%rsi)
+   18001f3d9:	add    %dh,(%rax)
+   18001f3db:	add    %ch,(%rsi)
+   18001f3dd:	add    %dh,(%rcx)
+   18001f3df:	add    %bh,(%rdx)
+   18001f3e1:	add    %al,(%rax)
+   18001f3e3:	add    %al,(%rax)
+   18001f3e5:	add    %al,(%rax)
+   18001f3e7:	add    %cl,0x6e(%rcx)
+   18001f3ea:	jbe    0x18001f44d
+   18001f3ec:	insb   (%dx),%es:(%rdi)
+   18001f3ed:	imul   $0x25204c52,0x55(%rax,%riz,1),%esp
+   18001f3f5:	jae    0x18001f3f7
+   18001f3f7:	add    %cl,0xa(%rip)        # 0x18001f407
+   18001f3fd:	add    %al,(%rax)
+   18001f3ff:	add    %cl,0x6e(%rcx)
+   18001f402:	jbe    0x18001f465
+   18001f404:	insb   (%dx),%es:(%rdi)
+   18001f405:	imul   $0x69737265,0x76(%rax,%riz,1),%esp
+   18001f40d:	outsl  %ds:(%rsi),(%dx)
+   18001f40e:	outsb  %ds:(%rsi),(%dx)
+   18001f40f:	add    %ch,0x74(%rax)
+   18001f412:	je     0x18001f484
+   18001f414:	cmp    (%rdi),%ch
+   18001f416:	(bad)
+   18001f417:	xor    %esi,(%rdx)
+   18001f419:	(bad)
+   18001f41a:	cs xor %ch,(%rsi)
+   18001f41d:	xor    %ch,(%rsi)
+   18001f41f:	xor    %edi,(%rdx)
+   18001f421:	and    $0x32252f31,%eax
+	...
+   18001f436:	add    %al,(%rax)
+   18001f438:	add    %ah,(%rdx)
+   18001f43a:	add    %al,0x1(%rax)
+   18001f440:	jo     0x18001f436
+   18001f442:	add    %eax,0x1(%rax)
+   18001f448:	nop
+   18001f449:	hlt
+   18001f44a:	add    %eax,0x1(%rax)
+   18001f450:	rorb   $0x80,0x1(%rdx)
+   18001f454:	add    %eax,(%rax)
 	...
    18001f45e:	add    %al,(%rax)
-   18001f460:	or     %al,(%rax)
-   18001f462:	add    %al,(%rax)
-   18001f464:	adc    $0x51000000,%eax
-   18001f469:	rex.WRXB
-   18001f46a:	rex.B jne 0x18001f4e1
-   18001f46d:	push   $0x52626f4f
-   18001f472:	gs jo  0x18001f4e1
-   18001f475:	jns    0x18001f4bf
-   18001f477:	(bad)
-   18001f478:	outsb  %ds:(%rsi),(%dx)
-   18001f479:	fs insb (%dx),%es:(%rdi)
-   18001f47b:	gs jb  0x18001f47e
-   18001f47e:	add    %al,(%rax)
-   18001f480:	or     (%rax),%eax
-	...
-   18001f4be:	add    %al,(%rax)
-   18001f4c0:	mov    $0xb8,%al
-   18001f4c2:	add    0x1(%rax),%al
-   18001f4c8:	push   %rcx
-   18001f4c9:	rex.WRXB
-   18001f4ca:	rex.B jne 0x18001f541
-   18001f4cd:	push   $0x52626f4f
-   18001f4d2:	gs jo  0x18001f541
-   18001f4d5:	jns    0x18001f51f
-   18001f4d7:	(bad)
-   18001f4d8:	outsb  %ds:(%rsi),(%dx)
-   18001f4d9:	fs insb (%dx),%es:(%rdi)
-   18001f4db:	gs jb  0x18001f4de
-   18001f4de:	add    %al,(%rax)
-   18001f4e0:	lock add %eax,(%rdx)
-   18001f4e3:	addb   $0x0,(%rcx)
-   18001f4e6:	add    %al,(%rax)
-   18001f4e8:	(bad)
-   18001f4e9:	addl   $0xffffff80,(%rcx)
-   18001f4ec:	add    %eax,(%rax)
+   18001f460:	shl    %ah
+   18001f462:	add    %eax,0x1(%rax)
+	...
+   18001f470:	or     %al,(%rax)
+   18001f472:	add    %al,(%rax)
+   18001f474:	adc    $0x51000000,%eax
+   18001f479:	rex.WRXB
+   18001f47a:	rex.B jne 0x18001f4f1
+   18001f47d:	push   $0x52626f4f
+   18001f482:	gs jo  0x18001f4f1
+   18001f485:	jns    0x18001f4cf
+   18001f487:	(bad)
+   18001f488:	outsb  %ds:(%rsi),(%dx)
+   18001f489:	fs insb (%dx),%es:(%rdi)
+   18001f48b:	gs jb  0x18001f48e
+   18001f48e:	add    %al,(%rax)
+   18001f490:	or     (%rax),%eax
+	...
+   18001f4ce:	add    %al,(%rax)
+   18001f4d0:	mov    $0xb8,%al
+   18001f4d2:	add    0x1(%rax),%al
+   18001f4d8:	push   %rcx
+   18001f4d9:	rex.WRXB
+   18001f4da:	rex.B jne 0x18001f551
+   18001f4dd:	push   $0x52626f4f
+   18001f4e2:	gs jo  0x18001f551
+   18001f4e5:	jns    0x18001f52f
+   18001f4e7:	(bad)
+   18001f4e8:	outsb  %ds:(%rsi),(%dx)
+   18001f4e9:	fs insb (%dx),%es:(%rdi)
+   18001f4eb:	gs jb  0x18001f4ee
    18001f4ee:	add    %al,(%rax)
-   18001f4f0:	rclb   0x18001(%rcx)
+   18001f4f0:	lock add %eax,(%rdx)
+   18001f4f3:	addb   $0x0,(%rcx)
    18001f4f6:	add    %al,(%rax)
-   18001f4f8:	rclb   $0x0,0x18001(%rcx)
-   18001f4ff:	add    %dh,(%rax)
-   18001f501:	(bad)
-   18001f502:	add    %eax,0x1(%rax)
-   18001f508:	mov    $0x92,%al
-   18001f50a:	add    %eax,0x1(%rax)
-   18001f510:	rclb   $0x0,0x18001(%rdx)
-   18001f517:	add    %ah,%al
-   18001f519:	xchg   %eax,%edx
+   18001f4f8:	(bad)
+   18001f4f9:	addl   $0xffffff80,(%rcx)
+   18001f4fc:	add    %eax,(%rax)
+   18001f4fe:	add    %al,(%rax)
+   18001f500:	rclb   0x18001(%rcx)
+   18001f506:	add    %al,(%rax)
+   18001f508:	rclb   $0x0,0x18001(%rcx)
+   18001f50f:	add    %dh,(%rax)
+   18001f511:	(bad)
+   18001f512:	add    %eax,0x1(%rax)
+   18001f518:	mov    $0x92,%al
    18001f51a:	add    %eax,0x1(%rax)
-   18001f520:	jo     0x18001f4b4
-   18001f522:	add    %eax,0x1(%rax)
-   18001f528:	nop
+   18001f520:	rclb   $0x0,0x18001(%rdx)
+   18001f527:	add    %ah,%al
    18001f529:	xchg   %eax,%edx
    18001f52a:	add    %eax,0x1(%rax)
-   18001f530:	adcb   $0x0,0x18001(%rdx)
-   18001f537:	add    %ah,0x1800192(%rax)
-   18001f53d:	add    %al,(%rax)
-   18001f53f:	add    %dh,%al
-   18001f541:	(bad)
-   18001f542:	add    %eax,0x1(%rax)
-   18001f548:	addb   $0x0,0x18001(%rbx)
-   18001f54f:	add    %ch,0x0(%rdi)
-   18001f552:	outsl  %ds:(%rsi),(%dx)
-   18001f553:	add    %ah,0x0(%rdx)
-   18001f556:	add    %al,(%rax)
-   18001f558:	and    $0x73,%eax
-   18001f55d:	add    %al,(%rax)
-   18001f55f:	add    %al,0x6d(%rbp)
-   18001f562:	jo     0x18001f5d8
-   18001f564:	jns    0x18001f586
-   18001f566:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001f568:	outsb  %ds:(%rsi),(%dx)
-   18001f569:	je     0x18001f5d0
-   18001f56b:	outsb  %ds:(%rsi),(%dx)
-   18001f56c:	je     0x18001f59b
-   18001f56e:	je     0x18001f5e9
-   18001f570:	jo     0x18001f5d7
-   18001f572:	and    %ch,0x65(%rax)
-   18001f575:	(bad)
-   18001f576:	fs gs jb 0x18001f57a
-   18001f57a:	add    %al,(%rax)
-   18001f57c:	add    %al,(%rax)
-   18001f57e:	add    %al,(%rax)
-   18001f580:	je     0x18001f582
-   18001f582:	add    %bh,%gs:0x0(%rax)
-   18001f586:	je     0x18001f588
-   18001f588:	(bad)
-   18001f589:	add    %ch,0x0(%rax)
-   18001f58c:	je     0x18001f58e
-   18001f58e:	insl   (%dx),%es:(%rdi)
-   18001f58f:	add    %ch,0x0(%rax,%rax,1)
-   18001f593:	add    %al,(%rax)
-   18001f595:	add    %al,(%rax)
-   18001f597:	add    %cl,0x6f(%rsi)
-   18001f59a:	and    %dh,0x65(%rdx)
-   18001f59d:	movsxd 0x69(%rbp),%esp
-   18001f5a0:	jbe    0x18001f607
-   18001f5a2:	and    %ah,%fs:0x74(%rcx,%riz,2)
-   18001f5a7:	(bad)
-	...
-   18001f5b0:	je     0x18001f5b2
-   18001f5b2:	add    %bh,%gs:0x0(%rax)
-   18001f5b6:	je     0x18001f5b8
-   18001f5b8:	(bad)
-   18001f5b9:	add    %ch,0x0(%rdx)
-   18001f5bc:	(bad)
-   18001f5bd:	add    %dh,0x0(%rsi)
-   18001f5c0:	(bad)
-   18001f5c1:	add    %dh,0x0(%rbx)
-   18001f5c4:	movsxd (%rax),%eax
-   18001f5c6:	jb     0x18001f5c8
-   18001f5c8:	imul   $0x740070,(%rax),%eax
-   18001f5ce:	add    %al,(%rax)
-   18001f5d0:	push   %rdx
-   18001f5d1:	movsxd %gs:0x69(%rbp),%esp
-   18001f5d5:	jbe    0x18001f63c
-   18001f5d7:	and    %ah,%fs:0x74(%rcx,%riz,2)
-   18001f5dc:	(bad)
-   18001f5dd:	and    %ch,0x73(%rcx)
-   18001f5e0:	and    %ch,0x6f(%rsi)
-   18001f5e3:	je     0x18001f605
-   18001f5e5:	(bad)
-   18001f5e6:	and    %cl,0x53(%rdx)
-   18001f5e9:	rex.WRXB
-   18001f5ea:	rex.WRX and %r13b,0x62(%rdi)
-   18001f5ee:	push   $0x65
-   18001f5f0:	movsxd 0x20(%rdx,%rdi,1),%esi
-   18001f5f4:	and    $0x52000073,%eax
-   18001f5f9:	movsxd %gs:0x69(%rbp),%esp
-   18001f5fd:	jbe    0x18001f664
-   18001f5ff:	and    %ah,%fs:0x6d(%rbp)
-   18001f603:	jo     0x18001f679
-   18001f605:	jns    0x18001f627
-   18001f607:	rex.WX push %rbx
-   18001f609:	rex.WRXB
-   18001f60a:	rex.WRX and %r13b,0x62(%rdi)
-   18001f60e:	push   $0x65
-   18001f610:	movsxd 0x20(%rdx,%rdi,1),%esi
-   18001f614:	and    $0x55000073,%eax
-   18001f619:	outsb  %ds:(%rsi),(%dx)
-   18001f61a:	imul   $0x77,0x6f(%rsi),%ebp
-   18001f61e:	outsb  %ds:(%rsi),(%dx)
-   18001f61f:	and    %al,0x6f(%rbx)
-   18001f622:	outsb  %ds:(%rsi),(%dx)
-   18001f623:	je     0x18001f68a
-   18001f625:	outsb  %ds:(%rsi),(%dx)
-   18001f626:	je     0x18001f655
-   18001f628:	je     0x18001f6a3
-   18001f62a:	jo     0x18001f691
-   18001f62c:	cmp    (%rax),%ah
-   18001f62e:	and    $0x73,%eax
-   18001f633:	add    %al,(%rax)
-   18001f635:	add    %al,(%rax)
-   18001f637:	add    %bl,(%rax)
-   18001f639:	add    (%rdx),%al
-   18001f63b:	addb   $0x0,(%rcx)
-   18001f63e:	add    %al,(%rax)
-   18001f640:	add    %dl,0x18001(%rbx)
-	...
+   18001f530:	jo     0x18001f4c4
+   18001f532:	add    %eax,0x1(%rax)
+   18001f538:	nop
+   18001f539:	xchg   %eax,%edx
+   18001f53a:	add    %eax,0x1(%rax)
+   18001f540:	adcb   $0x0,0x18001(%rdx)
+   18001f547:	add    %ah,0x1800192(%rax)
+   18001f54d:	add    %al,(%rax)
+   18001f54f:	add    %dh,%al
+   18001f551:	(bad)
+   18001f552:	add    %eax,0x1(%rax)
+   18001f558:	addb   $0x0,0x18001(%rbx)
+   18001f55f:	add    %ch,0x0(%rdi)
+   18001f562:	outsl  %ds:(%rsi),(%dx)
+   18001f563:	add    %ah,0x0(%rdx)
+   18001f566:	add    %al,(%rax)
+   18001f568:	and    $0x73,%eax
+   18001f56d:	add    %al,(%rax)
+   18001f56f:	add    %al,0x6d(%rbp)
+   18001f572:	jo     0x18001f5e8
+   18001f574:	jns    0x18001f596
+   18001f576:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001f578:	outsb  %ds:(%rsi),(%dx)
+   18001f579:	je     0x18001f5e0
+   18001f57b:	outsb  %ds:(%rsi),(%dx)
+   18001f57c:	je     0x18001f5ab
+   18001f57e:	je     0x18001f5f9
+   18001f580:	jo     0x18001f5e7
+   18001f582:	and    %ch,0x65(%rax)
+   18001f585:	(bad)
+   18001f586:	fs gs jb 0x18001f58a
+   18001f58a:	add    %al,(%rax)
+   18001f58c:	add    %al,(%rax)
+   18001f58e:	add    %al,(%rax)
+   18001f590:	je     0x18001f592
+   18001f592:	add    %bh,%gs:0x0(%rax)
+   18001f596:	je     0x18001f598
+   18001f598:	(bad)
+   18001f599:	add    %ch,0x0(%rax)
+   18001f59c:	je     0x18001f59e
+   18001f59e:	insl   (%dx),%es:(%rdi)
+   18001f59f:	add    %ch,0x0(%rax,%rax,1)
+   18001f5a3:	add    %al,(%rax)
+   18001f5a5:	add    %al,(%rax)
+   18001f5a7:	add    %cl,0x6f(%rsi)
+   18001f5aa:	and    %dh,0x65(%rdx)
+   18001f5ad:	movsxd 0x69(%rbp),%esp
+   18001f5b0:	jbe    0x18001f617
+   18001f5b2:	and    %ah,%fs:0x74(%rcx,%riz,2)
+   18001f5b7:	(bad)
+	...
+   18001f5c0:	je     0x18001f5c2
+   18001f5c2:	add    %bh,%gs:0x0(%rax)
+   18001f5c6:	je     0x18001f5c8
+   18001f5c8:	(bad)
+   18001f5c9:	add    %ch,0x0(%rdx)
+   18001f5cc:	(bad)
+   18001f5cd:	add    %dh,0x0(%rsi)
+   18001f5d0:	(bad)
+   18001f5d1:	add    %dh,0x0(%rbx)
+   18001f5d4:	movsxd (%rax),%eax
+   18001f5d6:	jb     0x18001f5d8
+   18001f5d8:	imul   $0x740070,(%rax),%eax
+   18001f5de:	add    %al,(%rax)
+   18001f5e0:	push   %rdx
+   18001f5e1:	movsxd %gs:0x69(%rbp),%esp
+   18001f5e5:	jbe    0x18001f64c
+   18001f5e7:	and    %ah,%fs:0x74(%rcx,%riz,2)
+   18001f5ec:	(bad)
+   18001f5ed:	and    %ch,0x73(%rcx)
+   18001f5f0:	and    %ch,0x6f(%rsi)
+   18001f5f3:	je     0x18001f615
+   18001f5f5:	(bad)
+   18001f5f6:	and    %cl,0x53(%rdx)
+   18001f5f9:	rex.WRXB
+   18001f5fa:	rex.WRX and %r13b,0x62(%rdi)
+   18001f5fe:	push   $0x65
+   18001f600:	movsxd 0x20(%rdx,%rdi,1),%esi
+   18001f604:	and    $0x52000073,%eax
+   18001f609:	movsxd %gs:0x69(%rbp),%esp
+   18001f60d:	jbe    0x18001f674
+   18001f60f:	and    %ah,%fs:0x6d(%rbp)
+   18001f613:	jo     0x18001f689
+   18001f615:	jns    0x18001f637
+   18001f617:	rex.WX push %rbx
+   18001f619:	rex.WRXB
+   18001f61a:	rex.WRX and %r13b,0x62(%rdi)
+   18001f61e:	push   $0x65
+   18001f620:	movsxd 0x20(%rdx,%rdi,1),%esi
+   18001f624:	and    $0x55000073,%eax
+   18001f629:	outsb  %ds:(%rsi),(%dx)
+   18001f62a:	imul   $0x77,0x6f(%rsi),%ebp
+   18001f62e:	outsb  %ds:(%rsi),(%dx)
+   18001f62f:	and    %al,0x6f(%rbx)
+   18001f632:	outsb  %ds:(%rsi),(%dx)
+   18001f633:	je     0x18001f69a
+   18001f635:	outsb  %ds:(%rsi),(%dx)
+   18001f636:	je     0x18001f665
+   18001f638:	je     0x18001f6b3
+   18001f63a:	jo     0x18001f6a1
+   18001f63c:	cmp    (%rax),%ah
+   18001f63e:	and    $0x73,%eax
+   18001f643:	add    %al,(%rax)
+   18001f645:	add    %al,(%rax)
+   18001f647:	add    %bl,(%rax)
+   18001f649:	add    (%rdx),%al
+   18001f64b:	addb   $0x0,(%rcx)
    18001f64e:	add    %al,(%rax)
-   18001f650:	(bad)
-   18001f651:	add    %dh,0x0(%rax)
-   18001f654:	imul   $0x6d002d,(%rax),%eax
-   18001f65a:	jae    0x18001f65c
-   18001f65c:	sub    $0x69007700,%eax
-   18001f661:	add    %ch,0x0(%rsi)
-   18001f664:	sub    $0x6f006300,%eax
-   18001f669:	add    %dh,0x0(%rdx)
-   18001f66c:	add    %ch,%gs:0x79007300(%rip)        # 0x1f9026973
-   18001f673:	add    %ch,0x0(%rsi)
-   18001f676:	movsxd (%rax),%eax
-   18001f678:	push   $0x6c002d00
-   18001f67d:	add    %dh,(%rcx)
-   18001f67f:	add    %ch,0x2d003200(%rip)        # 0x1ad022885
-   18001f685:	add    %dh,(%rax)
-   18001f687:	add    %ch,(%rsi)
-   18001f689:	add    %ah,0x6c(%rax,%rax,1)
-   18001f68d:	add    %ch,0x0(%rax,%rax,1)
-   18001f691:	add    %al,(%rax)
-   18001f693:	add    %al,(%rax)
-   18001f695:	add    %al,(%rax)
-   18001f697:	add    %ch,0x0(%rbx)
-   18001f69a:	add    %dh,%gs:0x0(%rdx)
-   18001f69e:	outsb  %ds:(%rsi),(%dx)
-   18001f69f:	add    %ah,0x0(%rbp)
-   18001f6a2:	insb   (%dx),%es:(%rdi)
-   18001f6a3:	add    %dh,(%rbx)
-   18001f6a5:	add    %dh,(%rdx)
-   18001f6a7:	add    %ch,(%rsi)
-   18001f6a9:	add    %ah,0x6c(%rax,%rax,1)
-   18001f6ad:	add    %ch,0x0(%rax,%rax,1)
-   18001f6b1:	add    %al,(%rax)
-   18001f6b3:	add    %al,(%rax)
-   18001f6b5:	add    %al,(%rax)
-   18001f6b7:	add    %dl,0x6c(%rbx)
-   18001f6ba:	gs gs jo 0x18001f701
-   18001f6be:	outsl  %ds:(%rsi),(%dx)
-   18001f6bf:	outsb  %ds:(%rsi),(%dx)
-   18001f6c0:	imul   $0x7261566e,%fs:0x6f(%rcx,%rbp,2),%esi
-   18001f6c9:	imul   $0x5343656c,0x62(%rcx),%esp
-	...
-   18001f6d8:	push   %rdi
-   18001f6d9:	(bad)
-   18001f6da:	imul   $0x6c,0x41(%rbp),%esp
-   18001f6de:	insb   (%dx),%es:(%rdi)
-   18001f6df:	rex.XB outsl %ds:(%rsi),(%dx)
-   18001f6e1:	outsb  %ds:(%rsi),(%dx)
-   18001f6e2:	imul   $0x7261566e,%fs:0x6f(%rcx,%rbp,2),%esi
-   18001f6eb:	imul   $0x656c,0x62(%rcx),%esp
-	...
-   18001f6fe:	add    %al,(%rax)
-   18001f700:	(bad)
-   18001f701:	(bad)
-   18001f702:	(bad)
-   18001f703:	(bad)
-   18001f704:	(bad)
-   18001f705:	(bad)
-   18001f706:	(bad)
-   18001f707:	(bad)
-   18001f708:	(bad)
-   18001f709:	(bad)
-   18001f70a:	(bad)
-   18001f70b:	(bad)
-   18001f70c:	(bad)
-   18001f70d:	(bad)
-   18001f70e:	(bad)
-   18001f70f:	incl   (%rax)
-   18001f711:	add    %al,(%rax)
-   18001f713:	add    %al,(%rax)
-   18001f715:	add    %al,(%rax)
-   18001f717:	add    %ah,0x61(%rdx)
-   18001f71a:	and    %ah,%fs:0x6c(%rcx)
-   18001f71e:	insb   (%dx),%es:(%rdi)
-   18001f71f:	outsl  %ds:(%rsi),(%dx)
-   18001f720:	movsxd 0x74(%rcx),%esp
-   18001f723:	imul   $0xd3e00000,0x6e(%rdi),%ebp
-   18001f72a:	add    0x1(%rax),%al
-   18001f730:	adc    $0x2,%ah
-   18001f733:	addb   $0x0,(%rcx)
-   18001f736:	add    %al,(%rax)
-   18001f738:	add    %al,(%rax)
-   18001f73a:	add    %al,(%rax)
-   18001f73c:	movsl  %ds:(%rsi),%es:(%rdi)
-   18001f73d:	mov    $0x69,%dh
-   18001f73f:	add    %al,%fs:(%rax)
-   18001f742:	add    %al,(%rax)
-   18001f744:	add    (%rax),%al
+   18001f650:	add    %dl,0x18001(%rbx)
+	...
+   18001f65e:	add    %al,(%rax)
+   18001f660:	(bad)
+   18001f661:	add    %dh,0x0(%rax)
+   18001f664:	imul   $0x6d002d,(%rax),%eax
+   18001f66a:	jae    0x18001f66c
+   18001f66c:	sub    $0x69007700,%eax
+   18001f671:	add    %ch,0x0(%rsi)
+   18001f674:	sub    $0x6f006300,%eax
+   18001f679:	add    %dh,0x0(%rdx)
+   18001f67c:	add    %ch,%gs:0x79007300(%rip)        # 0x1f9026983
+   18001f683:	add    %ch,0x0(%rsi)
+   18001f686:	movsxd (%rax),%eax
+   18001f688:	push   $0x6c002d00
+   18001f68d:	add    %dh,(%rcx)
+   18001f68f:	add    %ch,0x2d003200(%rip)        # 0x1ad022895
+   18001f695:	add    %dh,(%rax)
+   18001f697:	add    %ch,(%rsi)
+   18001f699:	add    %ah,0x6c(%rax,%rax,1)
+   18001f69d:	add    %ch,0x0(%rax,%rax,1)
+   18001f6a1:	add    %al,(%rax)
+   18001f6a3:	add    %al,(%rax)
+   18001f6a5:	add    %al,(%rax)
+   18001f6a7:	add    %ch,0x0(%rbx)
+   18001f6aa:	add    %dh,%gs:0x0(%rdx)
+   18001f6ae:	outsb  %ds:(%rsi),(%dx)
+   18001f6af:	add    %ah,0x0(%rbp)
+   18001f6b2:	insb   (%dx),%es:(%rdi)
+   18001f6b3:	add    %dh,(%rbx)
+   18001f6b5:	add    %dh,(%rdx)
+   18001f6b7:	add    %ch,(%rsi)
+   18001f6b9:	add    %ah,0x6c(%rax,%rax,1)
+   18001f6bd:	add    %ch,0x0(%rax,%rax,1)
+   18001f6c1:	add    %al,(%rax)
+   18001f6c3:	add    %al,(%rax)
+   18001f6c5:	add    %al,(%rax)
+   18001f6c7:	add    %dl,0x6c(%rbx)
+   18001f6ca:	gs gs jo 0x18001f711
+   18001f6ce:	outsl  %ds:(%rsi),(%dx)
+   18001f6cf:	outsb  %ds:(%rsi),(%dx)
+   18001f6d0:	imul   $0x7261566e,%fs:0x6f(%rcx,%rbp,2),%esi
+   18001f6d9:	imul   $0x5343656c,0x62(%rcx),%esp
+	...
+   18001f6e8:	push   %rdi
+   18001f6e9:	(bad)
+   18001f6ea:	imul   $0x6c,0x41(%rbp),%esp
+   18001f6ee:	insb   (%dx),%es:(%rdi)
+   18001f6ef:	rex.XB outsl %ds:(%rsi),(%dx)
+   18001f6f1:	outsb  %ds:(%rsi),(%dx)
+   18001f6f2:	imul   $0x7261566e,%fs:0x6f(%rcx,%rbp,2),%esi
+   18001f6fb:	imul   $0x656c,0x62(%rcx),%esp
+	...
+   18001f70e:	add    %al,(%rax)
+   18001f710:	(bad)
+   18001f711:	(bad)
+   18001f712:	(bad)
+   18001f713:	(bad)
+   18001f714:	(bad)
+   18001f715:	(bad)
+   18001f716:	(bad)
+   18001f717:	(bad)
+   18001f718:	(bad)
+   18001f719:	(bad)
+   18001f71a:	(bad)
+   18001f71b:	(bad)
+   18001f71c:	(bad)
+   18001f71d:	(bad)
+   18001f71e:	(bad)
+   18001f71f:	incl   (%rax)
+   18001f721:	add    %al,(%rax)
+   18001f723:	add    %al,(%rax)
+   18001f725:	add    %al,(%rax)
+   18001f727:	add    %ah,0x61(%rdx)
+   18001f72a:	and    %ah,%fs:0x6c(%rcx)
+   18001f72e:	insb   (%dx),%es:(%rdi)
+   18001f72f:	outsl  %ds:(%rsi),(%dx)
+   18001f730:	movsxd 0x74(%rcx),%esp
+   18001f733:	imul   $0xd3e00000,0x6e(%rdi),%ebp
+   18001f73a:	add    0x1(%rax),%al
+   18001f740:	adc    $0x2,%ah
+   18001f743:	addb   $0x0,(%rcx)
    18001f746:	add    %al,(%rax)
-   18001f748:	push   %rdi
-   18001f749:	add    %al,(%rax)
-   18001f74b:	add    %dh,%al
-   18001f74d:	(bad)
-   18001f74e:	add    (%rax),%al
-   18001f750:	lock hlt
-   18001f752:	add    %eax,(%rax)
-   18001f754:	add    %al,(%rax)
-   18001f756:	add    %al,(%rax)
-   18001f758:	movsl  %ds:(%rsi),%es:(%rdi)
-   18001f759:	mov    $0x69,%dh
-   18001f75b:	add    %al,%fs:(%rax)
-   18001f75e:	add    %al,(%rax)
-   18001f760:	or     $0x0,%al
-   18001f762:	add    %al,(%rax)
-   18001f764:	adc    $0x0,%al
+   18001f748:	add    %al,(%rax)
+   18001f74a:	add    %al,(%rax)
+   18001f74c:	xchg   %eax,%ebx
+   18001f74d:	test   %esp,0x64(%rdi)
+   18001f753:	add    %al,(%rdx)
+   18001f755:	add    %al,(%rax)
+   18001f757:	add    %dl,0x0(%rdi)
+   18001f75a:	add    %al,(%rax)
+   18001f75c:	lock (bad)
+   18001f75e:	add    (%rax),%al
+   18001f760:	lock hlt
+   18001f762:	add    %eax,(%rax)
+   18001f764:	add    %al,(%rax)
    18001f766:	add    %al,(%rax)
-   18001f768:	rex.W (bad)
-   18001f76a:	add    (%rax),%al
-   18001f76c:	rex.W cmc
-   18001f76e:	add    %eax,(%rax)
-   18001f770:	add    %al,(%rax)
+   18001f768:	xchg   %eax,%ebx
+   18001f769:	test   %esp,0x64(%rdi)
+   18001f76f:	add    %cl,(%rax,%rax,1)
    18001f772:	add    %al,(%rax)
-   18001f774:	movsl  %ds:(%rsi),%es:(%rdi)
-   18001f775:	mov    $0x69,%dh
-   18001f777:	add    %al,%fs:(%rax)
-   18001f77a:	add    %al,(%rax)
-   18001f77c:	or     $0x84000000,%eax
-   18001f781:	add    (%rax),%eax
-   18001f783:	add    %bl,0x2(%rdi,%rax,1)
-   18001f787:	add    %bl,0x1(%rbp,%rsi,8)
-   18001f78b:	add    %al,(%rax)
-   18001f78d:	add    %al,(%rax)
-   18001f78f:	add    %bh,(%rax)
-   18001f791:	add    %eax,(%rax)
-	...
-   18001f7e7:	add    %ch,(%rax)
-   18001f7e9:	mov    $0x18002,%ecx
-	...
-   18001f7fe:	add    %al,(%rax)
-   18001f800:	js     0x18001f7bc
-   18001f802:	add    %eax,0x1(%rax)
-   18001f808:	mov    %bh,0x18001(%rdx)
-   18001f80e:	add    %al,(%rax)
-   18001f810:	fdivrs 0x18001(%rbx)
-   18001f816:	add    %al,(%rax)
-   18001f818:	xchg   %eax,%edx
-   18001f819:	add    %eax,(%rax)
-   18001f81b:	add    %al,(%rax)
-   18001f81d:	add    %al,(%rax)
-   18001f81f:	add    %al,(%rax)
-   18001f821:	jne    0x18001f824
-   18001f823:	adc    %al,(%rax)
+   18001f774:	adc    $0x0,%al
+   18001f776:	add    %al,(%rax)
+   18001f778:	rex.W (bad)
+   18001f77a:	add    (%rax),%al
+   18001f77c:	rex.W cmc
+   18001f77e:	add    %eax,(%rax)
+   18001f780:	add    %al,(%rax)
+   18001f782:	add    %al,(%rax)
+   18001f784:	xchg   %eax,%ebx
+   18001f785:	test   %esp,0x64(%rdi)
+   18001f78b:	add    %cl,-0x7c000000(%rip)        # 0x10401f791
+   18001f791:	add    (%rax),%eax
+   18001f793:	add    %bl,0x2(%rdi,%rax,1)
+   18001f797:	add    %bl,0x1(%rbp,%rsi,8)
+   18001f79b:	add    %al,(%rax)
+   18001f79d:	add    %al,(%rax)
+   18001f79f:	add    %bh,(%rax)
+   18001f7a1:	add    %eax,(%rax)
 	...
+   18001f7f7:	add    %ch,(%rax)
+   18001f7f9:	mov    $0x18002,%ecx
+	...
+   18001f80e:	add    %al,(%rax)
+   18001f810:	js     0x18001f7cc
+   18001f812:	add    %eax,0x1(%rax)
+   18001f818:	mov    %bh,0x18001(%rdx)
+   18001f81e:	add    %al,(%rax)
+   18001f820:	fdivrs 0x18001(%rbx)
+   18001f826:	add    %al,(%rax)
+   18001f828:	xchg   %eax,%edx
+   18001f829:	add    %eax,(%rax)
+   18001f82b:	add    %al,(%rax)
    18001f82d:	add    %al,(%rax)
-   18001f82f:	add    %dh,0x18001(%rbx,%rax,8)
-   18001f836:	add    %al,(%rax)
-   18001f838:	(bad)
-	...
-   18001f88d:	add    %al,(%rax)
-   18001f88f:	add    %cl,0x18002(%rdx,%rax,1)
-	...
-   18001f8a6:	add    %al,(%rax)
-   18001f8a8:	cmpb   $0x0,0x18001(%rdx)
-   18001f8af:	add    %dl,0x18001ba(%rax)
-   18001f8b5:	add    %al,(%rax)
-   18001f8b7:	add    %bl,0x18001ba(%rax)
-   18001f8bd:	add    %al,(%rax)
-   18001f8bf:	add    %dh,(%rax)
-   18001f8c1:	roll   %cl,(%rdx)
-   18001f8c3:	addb   $0x0,(%rcx)
+   18001f82f:	add    %al,(%rax)
+   18001f831:	jne    0x18001f834
+   18001f833:	adc    %al,(%rax)
+	...
+   18001f83d:	add    %al,(%rax)
+   18001f83f:	add    %dh,0x18001(%rbx,%rax,8)
+   18001f846:	add    %al,(%rax)
+   18001f848:	(bad)
+	...
+   18001f89d:	add    %al,(%rax)
+   18001f89f:	add    %cl,0x18002(%rdx,%rax,1)
+	...
+   18001f8b6:	add    %al,(%rax)
+   18001f8b8:	cmpb   $0x0,0x18001(%rdx)
+   18001f8bf:	add    %dl,0x18001ba(%rax)
+   18001f8c5:	add    %al,(%rax)
+   18001f8c7:	add    %bl,0x18001ba(%rax)
+   18001f8cd:	add    %al,(%rax)
+   18001f8cf:	add    %dh,(%rax)
+   18001f8d1:	roll   %cl,(%rdx)
+   18001f8d3:	addb   $0x0,(%rcx)
 	...
    18001f8fe:	add    %al,(%rax)
    18001f900:	add    %cl,(%rbx)
    18001f902:	add    0x1(%rax),%al
    18001f908:	or     %cl,(%rbx)
    18001f90a:	add    0x1(%rax),%al
    18001f910:	adc    $0x2,%bl
@@ -44279,26 +44267,26 @@
    1800206e8:	push   %rax
    1800206e9:	cmpsb  %es:(%rdi),%ds:(%rsi)
    1800206ea:	add    %eax,(%rax)
    1800206ec:	(bad)
    1800206ed:	add    (%rax),%al
    1800206ef:	add    %dl,0x53(%rdx)
    1800206f2:	rex.R push %rbx
-   1800206f4:	sub    %edi,%ecx
-   1800206f6:	sbb    (%rax,%rbx,1),%bh
-   1800206f9:	(bad)
-   1800206fa:	in     $0x4e,%al
-   1800206fc:	lods   %ds:(%rsi),%al
-   1800206fd:	(bad)
-   1800206fe:	or     $0x6b,%al
-   180020700:	rex.XB ret $0x985
-   180020704:	add    %eax,(%rax)
-   180020706:	add    %al,(%rax)
-   180020708:	cmp    0x73(%r13,%r10,2),%bl
-   18002070d:	gs jb  0x180020783
+   1800206f4:	movsb  %ds:(%rsi),%es:(%rdi)
+   1800206f5:	hlt
+   1800206f6:	pop    %rbp
+   1800206f7:	lahf
+   1800206f8:	rex.RX mov $0x35804374,%ebx
+   1800206fe:	int    $0x42
+   180020700:	fmull  0x15c(%rdx,%rdx,4)
+   180020707:	add    %al,0x3a(%rbx)
+   18002070a:	pop    %rsp
+   18002070b:	push   %rbp
+   18002070c:	jae    0x180020773
+   18002070e:	jb     0x180020783
    180020710:	pop    %rsp
    180020711:	jno    0x180020787
    180020713:	pop    %rsp
    180020714:	ja     0x180020785
    180020716:	jb     0x180020783
    180020718:	pop    %rsp
    180020719:	jno    0x18002078f
@@ -46824,23 +46812,23 @@
    180021e94:	(bad)
    180021e95:	xor    %eax,(%rcx)
    180021e97:	add    %ch,(%rax)
    180021e99:	(bad)
    180021e9a:	add    (%rax),%al
    180021e9c:	and    %eax,0x34050002(%rip)        # 0x1b4071ea4
    180021ea2:	(bad)
-   180021ea3:	add    %ah,(%rax)
-   180021ea5:	sgdt   (%rax)
-   180021ea8:	scas   %es:(%rdi),%eax
+   180021ea3:	add    %ah,0xf(%rax)
+   180021ea6:	add    %eax,(%rax)
+   180021ea8:	out    %eax,(%dx)
    180021ea9:	sgdt   (%rax)
    180021eac:	sbb    %cl,0x210002(%rip)        # 0x180231eb4
    180021eb2:	add    %al,(%rax)
-   180021eb4:	and    %cl,(%rdi)
-   180021eb6:	add    %eax,(%rax)
-   180021eb8:	scas   %es:(%rdi),%eax
+   180021eb4:	(bad)
+   180021eb5:	sgdt   (%rax)
+   180021eb8:	out    %eax,(%dx)
    180021eb9:	sgdt   (%rax)
    180021ebc:	sbb    %cl,0x10010002(%rip)        # 0x190031ec4
    180021ec2:	or     %al,(%rax)
    180021ec4:	adc    %dh,0xc521000(,%rcx,1)
    180021ecb:	lock or %al,%ah
    180021ece:	or     %dh,0x7(%rax)
    180021ed1:	(bad)
@@ -47992,23 +47980,26 @@
    180022999:	push   %rsp
    18002299a:	add    %eax,(%rax)
    18002299c:	rex
    18002299d:	rex.RXB add %r8b,(%r8)
    1800229a0:	shl    $0x0,%dh
    1800229a3:	add    %al,(%rax)
    1800229a5:	out    %eax,$0x0
-   1800229a7:	add    %ah,-0x5ffffe1c(%rax)
+   1800229a7:	add    %ch,-0x5ffffe1c(%rax)
    1800229ad:	(bad)
    1800229ae:	add    %eax,(%rax)
-   1800229b0:	cmp    %ah,%dh
-   1800229b2:	add    %eax,(%rax)
-   1800229b4:	push   %rax
-   1800229b5:	call   0x16e7a29bb
+   1800229b0:	rex.W out %al,$0x1
+   1800229b3:	add    %ah,-0x18(%rax)
+   1800229b6:	add    %eax,(%rax)
+   1800229b8:	mov    %ch,%dh
    1800229ba:	add    %eax,(%rax)
-   1800229bc:	call   0x168022bb2
+   1800229bc:	clc
+   1800229bd:	int1
+   1800229be:	add    %eax,(%rax)
+   1800229c0:	clc
    1800229c1:	hlt
    1800229c2:	add    %eax,(%rax)
    1800229c4:	push   %rax
    1800229c5:	insb   (%dx),%es:(%rdi)
    1800229c6:	add    %al,(%rax)
    1800229c8:	loopne 0x180022a01
    1800229ca:	add    %al,(%rax)
@@ -48172,16 +48163,16 @@
    180022b79:	pop    %rsp
    180022b7a:	add    %al,(%rax)
    180022b7c:	loopne 0x180022ba0
    180022b7e:	add    %al,(%rax)
    180022b80:	add    %bl,(%rsi)
    180022b82:	add    %al,(%rax)
    180022b84:	rex sub %eax,(%rax)
-   180022b87:	add    %ah,(%rax)
-   180022b89:	sgdt   (%rax)
+   180022b87:	add    %ah,0xf(%rax)
+   180022b8a:	add    %eax,(%rax)
    180022b8c:	rorb   $0x0,0x1(%rdx)
    180022b90:	rorb   $0x0,0x1(%rdx)
    180022b94:	adc    %dh,(%rsi)
    180022b96:	add    %eax,(%rax)
    180022b98:	jo     0x180022c17
    180022b9a:	add    %al,(%rax)
    180022b9c:	movabs 0x600000423000007d,%al
@@ -48270,24 +48261,27 @@
    180022c69:	rex.X add %al,(%rax)
    180022c6c:	and    %al,-0x7d800000(%rdx)
    180022c72:	add    %al,(%rax)
    180022c74:	mov    $0x82,%al
    180022c76:	add    %al,(%rax)
    180022c78:	loopne 0x180022bfc
    180022c7a:	add    %al,(%rax)
-   180022c7c:	jo     0x180022c58
+   180022c7c:	jo     0x180022c5f
    180022c7e:	add    %eax,(%rax)
    180022c80:	lock movb $0x0,(%rcx)
    180022c84:	and    %al,%ah
    180022c86:	add    %eax,(%rax)
    180022c88:	rex rolb %cl,(%rcx)
-   180022c8b:	add    %dh,(%rax)
-   180022c8d:	out    %al,(%dx)
+   180022c8b:	add    %al,-0x12(%rax)
    180022c8e:	add    %eax,(%rax)
-   180022c90:	movabs 0x900001f4200001f1,%al
+   180022c90:	mov    $0xf1,%al
+   180022c92:	add    %eax,(%rax)
+   180022c94:	xor    %dh,%ah
+   180022c96:	add    %eax,(%rax)
+   180022c98:	nop
    180022c99:	pop    %rdx
    180022c9a:	add    %al,(%rax)
    180022c9c:	adc    %al,0x0(%rbx)
    180022c9f:	add    %dl,%al
    180022ca1:	or     %al,(%rcx)
    180022ca3:	add    %ah,%al
    180022ca5:	or     %al,(%rcx)
@@ -57382,16 +57376,15 @@
    180027970:	add    $0xab,%al
    180027972:	add    (%rax),%al
    180027974:	add    %al,(%rax)
    180027976:	add    %al,(%rax)
    180027978:	sbb    %ch,0x2(%rbx)
 	...
    180027986:	add    %al,(%rax)
-   180027988:	(bad)
-   180027989:	add    $0x7465733f,%eax
+   180027988:	ss add $0x7465733f,%eax
    18002798e:	rex.W
    18002798f:	gs (bad)
    180027991:	fs gs jb 0x1800279d5
    180027995:	push   %rcx
    180027996:	rex.WRX
    180027997:	gs je  0x180027a11
    18002799a:	outsl  %ds:(%rsi),(%dx)
@@ -57559,15 +57552,15 @@
    180027ac7:	gs je  0x180027b2b
    180027aca:	rex.WRXB (bad)
    180027acc:	push   $0x65
    180027ace:	movsxd 0x40(%rax,%rax,2),%esi
    180027ad2:	pop    %rax
    180027ad3:	pop    %rdx
    180027ad4:	add    %al,(%rax)
-   180027ad6:	pop    %rdx
+   180027ad6:	pop    %rcx
    180027ad7:	add    $0x3f,%al
    180027ad9:	jno    0x180027b4f
    180027adb:	pop    %rdi
    180027adc:	insl   (%dx),%es:(%rdi)
    180027add:	gs je  0x180027b41
    180027ae0:	movsxd 0x6c(%rcx),%esp
    180027ae3:	insb   (%dx),%es:(%rdi)
@@ -57599,15 +57592,15 @@
    180027b11:	movsxd 0x40(%rax,%rax,2),%esi
    180027b15:	rex.W push %rax
    180027b17:	rex.RB
    180027b18:	push   %r8
    180027b1a:	rex.RB
    180027b1b:	pop    %r8
    180027b1d:	rex pop %rdx
-   180027b1f:	add    %dh,0x4(%rdx)
+   180027b1f:	add    %dh,0x4(%rcx)
    180027b22:	(bad)
    180027b23:	jno    0x180027b99
    180027b25:	pop    %rdi
    180027b26:	insl   (%dx),%es:(%rdi)
    180027b27:	gs je  0x180027b8b
    180027b2a:	movsxd 0x73(%rcx),%esp
    180027b2d:	je     0x180027b6f
@@ -57630,15 +57623,17 @@
    180027b4c:	pop    %r8
    180027b4e:	push   %rax
    180027b4f:	rex.RB
    180027b50:	rex.X
    180027b51:	rex.R
    180027b52:	rex pop %rdx
    180027b54:	add    %al,(%rax)
-   180027b56:	xor    $0x75733f06,%eax
+   180027b56:	xor    $0x6,%al
+   180027b58:	(bad)
+   180027b59:	jae    0x180027bd0
    180027b5b:	jo     0x180027bcd
    180027b5d:	outsl  %ds:(%rsi),(%dx)
    180027b5e:	jb     0x180027bd4
    180027b60:	gs fs push %rbx
    180027b63:	movsxd 0x65(%rax),%ebp
    180027b66:	insl   (%dx),%es:(%rdi)
    180027b67:	gs jae 0x180027baa
@@ -57662,15 +57657,17 @@
    180027b89:	and    $0x51,%al
    180027b8b:	imul   $0x53515640,0x74(%rbx),%r14
    180027b93:	je     0x180027c07
    180027b95:	imul   $0x40404040,0x67(%rsi),%ebp
    180027b9c:	pop    %rax
    180027b9d:	pop    %rdx
    180027b9e:	add    %al,(%rax)
-   180027ba0:	adc    $0x74733f06,%eax
+   180027ba0:	adc    $0x6,%al
+   180027ba2:	(bad)
+   180027ba3:	jae    0x180027c19
    180027ba5:	(bad)
    180027ba6:	je     0x180027c11
    180027ba8:	movsxd 0x65(%rbp),%ecx
    180027bab:	je     0x180027c0e
    180027bad:	rex.WRXB (bad)
    180027baf:	push   $0x65
    180027bb1:	movsxd 0x51(%rax,%rax,2),%esi
@@ -57683,18 +57680,15 @@
    180027bc0:	jns    0x180027c02
    180027bc2:	rex xor 0x51(%rbp),%dl
    180027bc6:	rex.WRB
    180027bc7:	gs je  0x180027c2b
    180027bca:	rex.WRXB (bad)
    180027bcc:	push   $0x65
    180027bce:	movsxd 0x40(%rax,%rax,2),%esi
-   180027bd2:	rex.X add %al,(%rsi)
-   180027bd5:	(bad)
-   180027bd6:	(bad)
-   180027bd7:	jae    0x180027c4d
+   180027bd2:	rex.X add %al,0x74733f06(%rip)        # 0x1f475badf
    180027bd9:	(bad)
    180027bda:	je     0x180027c45
    180027bdc:	movsxd 0x65(%rbp),%ecx
    180027bdf:	je     0x180027c42
    180027be1:	rex.WRXB (bad)
    180027be3:	push   $0x65
    180027be5:	movsxd 0x51(%rax,%rax,2),%esi
@@ -57742,15 +57736,15 @@
    180027c3c:	rex
    180027c3d:	rex push %rcx
    180027c3f:	rex.RB
    180027c40:	rex.B
    180027c41:	rex.B
    180027c42:	rex pop %rax
    180027c44:	pop    %rdx
-   180027c45:	add    %cl,%bl
+   180027c45:	add    %cl,%dl
    180027c47:	add    $0x7465733f,%eax
    180027c4c:	push   %rbp
    180027c4d:	jb     0x180027cbb
    180027c4f:	rex push %rcx
    180027c51:	rex.WRX
    180027c52:	gs je  0x180027ccc
    180027c55:	outsl  %ds:(%rsi),(%dx)
@@ -57769,15 +57763,15 @@
    180027c6a:	push   %rcx
    180027c6b:	push   %rbp
    180027c6c:	jb     0x180027cda
    180027c6e:	rex
    180027c6f:	rex
    180027c70:	rex pop %rdx
    180027c72:	add    %al,(%rax)
-   180027c74:	xchg   %eax,%esp
+   180027c74:	xchg   %eax,%ebx
    180027c75:	add    $0x7465733f,%eax
    180027c7a:	push   %rdx
    180027c7b:	(bad)
    180027c7c:	ja     0x180027cc6
    180027c7e:	gs (bad)
    180027c80:	fs gs jb 0x180027cc4
    180027c84:	push   %rcx
@@ -57903,15 +57897,15 @@
    180027d5d:	rex.WRX
    180027d5e:	rex.B
    180027d5f:	rex.RB
    180027d60:	rex.X push %rsi
    180027d62:	xor    %al,0x40(%rax)
    180027d65:	pop    %rdx
    180027d66:	add    %al,(%rax)
-   180027d68:	rex.RB add $0x3f,%al
+   180027d68:	rex.R add $0x3f,%al
    180027d6b:	jno    0x180027dbf
    180027d6d:	imul   $0x6f4e7265,%gs:0x74(%ebx),%esi
    180027d76:	jb     0x180027de5
    180027d78:	(bad)
    180027d79:	insb   (%dx),%es:(%rdi)
    180027d7a:	imul   $0x74654d64,0x65(%rdx),%edi
    180027d81:	(bad)
@@ -58330,15 +58324,16 @@
    180028065:	rex.X push %rsi
    180028067:	push   %rcx
    180028068:	push   %rbp
    180028069:	jb     0x1800280d7
    18002806b:	rex
    18002806c:	rex
    18002806d:	rex pop %rdx
-   18002806f:	add    %ah,0x6c72753f(%rsi,%rax,1)
+   18002806f:	add    %ah,0x72753f06(%rbx)
+   180028075:	insb   (%dx),%es:(%rdi)
    180028076:	rex push %rcx
    180028078:	rex.WRX
    180028079:	gs je  0x1800280f3
    18002807c:	outsl  %ds:(%rsi),(%dx)
    18002807d:	jb     0x1800280ea
    18002807f:	push   %rdx
    180028080:	gs jno 0x1800280f8
@@ -58414,16 +58409,15 @@
    180028104:	jb     0x180028171
    180028106:	rex.RB jb 0x18002817b
    180028109:	outsl  %ds:(%rsi),(%dx)
    18002810a:	jb     0x18002814c
    18002810c:	xor    %eax,0x40(%rax)
    18002810f:	pop    %rdx
    180028110:	add    %al,(%rax)
-   180028112:	(bad)
-   180028113:	add    $0x3f,%al
+   180028112:	ds add $0x3f,%al
    180028115:	jno    0x180028169
    180028117:	imul   $0x6f4e7265,%gs:0x74(%ebx),%esi
    180028120:	jb     0x18002818f
    180028122:	(bad)
    180028123:	insb   (%dx),%es:(%rdi)
    180028124:	imul   $0x74654d64,0x65(%rdx),%edi
    18002812b:	(bad)
@@ -58455,15 +58449,15 @@
    180028155:	push   %rcx
    180028156:	rex.X jns 0x1800281cd
    180028159:	gs rex.B jb 0x1800281cf
    18002815d:	(bad)
    18002815e:	jns    0x1800281a0
    180028160:	rex
    180028161:	rex pop %rdx
-   180028163:	add    %bh,0x65733f05(%rax)
+   180028163:	add    %dh,0x65733f05(%rdi)
    180028169:	je     0x1800281be
    18002816b:	jae    0x1800281d9
    18002816d:	rex.XB outsl %ds:(%rsi),(%dx)
    18002816f:	outsb  %ds:(%rsi),(%dx)
    180028170:	imul   $0x6172,0x75(%rdi),%sp
    180028176:	je     0x1800281e1
    180028178:	outsl  %ds:(%rsi),(%dx)
@@ -58554,15 +58548,15 @@
    180028220:	rex.B jne 0x180028297
    180028223:	push   $0x69746e65
    180028228:	movsxd 0x74(%rcx),%esp
    18002822b:	outsl  %ds:(%rsi),(%dx)
    18002822c:	jb     0x18002826e
    18002822e:	rex
    18002822f:	rex pop %rdx
-   180028231:	add    %ah,0x72753f06(%rbx)
+   180028231:	add    %ah,0x72753f06(%rdx)
    180028237:	insb   (%dx),%es:(%rdi)
    180028238:	rex push %rcx
    18002823a:	rex.WRX
    18002823b:	gs je  0x1800282b5
    18002823e:	outsl  %ds:(%rsi),(%dx)
    18002823f:	jb     0x1800282ac
    180028241:	push   %rdx
@@ -58575,15 +58569,15 @@
    18002824d:	push   %r14
    18002824f:	push   %rcx
    180028250:	push   %rbp
    180028251:	jb     0x1800282bf
    180028253:	rex
    180028254:	rex pop %rax
    180028256:	pop    %rdx
-   180028257:	add    %cl,%ch
+   180028257:	add    %cl,%ah
    180028259:	add    $0x7465733f,%eax
    18002825e:	push   %rbp
    18002825f:	jae    0x1800282c6
    180028261:	jb     0x1800282a3
    180028263:	push   %rcx
    180028264:	rex.B jne 0x1800282db
    180028267:	push   $0x69746e65
@@ -58597,15 +58591,15 @@
    180028278:	rex.B
    180028279:	rex.RB
    18002827a:	rex.X push %rsi
    18002827c:	push   %rcx
    18002827d:	push   %rbx
    18002827e:	je     0x1800282f2
    180028280:	imul   $0x5a404040,0x67(%rsi),%ebp
-   180028287:	add    %ch,0x5(%rbx)
+   180028287:	add    %ch,0x5(%rdx)
    18002828a:	(bad)
    18002828b:	jae    0x1800282f2
    18002828d:	je     0x1800282df
    18002828f:	(bad)
    180028290:	jae    0x180028305
    180028292:	ja     0x180028303
    180028294:	jb     0x1800282fa
@@ -58622,15 +58616,15 @@
    1800282ac:	rex.B
    1800282ad:	rex.RB
    1800282ae:	rex.X push %rsi
    1800282b0:	push   %rcx
    1800282b1:	push   %rbx
    1800282b2:	je     0x180028326
    1800282b4:	imul   $0x5a404040,0x67(%rsi),%ebp
-   1800282bb:	add    %cl,(%rbx)
+   1800282bb:	add    %cl,(%rdx)
    1800282bd:	(bad)
    1800282be:	(bad)
    1800282bf:	jae    0x180028335
    1800282c1:	(bad)
    1800282c2:	je     0x18002832d
    1800282c4:	movsxd 0x65(%rbp),%ecx
    1800282c7:	je     0x18002832a
@@ -58789,15 +58783,15 @@
    180028413:	gs jb  0x180028456
    180028416:	rex push %rcx
    180028418:	rex.RB
    180028419:	rex.X
    18002841a:	pop    %r15
    18002841c:	rex.WRX pop %rax
    18002841e:	pop    %rdx
-   18002841f:	add    %bl,%bh
+   18002841f:	add    %bl,%dh
    180028421:	add    $0x3f,%al
    180028423:	jae    0x18002848a
    180028425:	jb     0x18002849d
    180028427:	gs jb  0x18002847a
    18002842a:	outsl  %ds:(%rsi),(%dx)
    18002842b:	jb     0x1800284a1
    18002842d:	rex push %rcx
@@ -58828,15 +58822,15 @@
    18002845e:	rex push %rcx
    180028460:	rex.RB
    180028461:	rex.B
    180028462:	pop    %r8
    180028464:	pop    %rax
    180028465:	pop    %rdx
    180028466:	add    %al,(%rax)
-   180028468:	add    %eax,(%rsi)
+   180028468:	add    %al,(%rsi)
    18002846a:	(bad)
    18002846b:	jae    0x1800284e1
    18002846d:	(bad)
    18002846e:	je     0x1800284d9
    180028470:	movsxd 0x65(%rbp),%ecx
    180028473:	je     0x1800284d6
    180028475:	rex.WRXB (bad)
@@ -58848,15 +58842,15 @@
    18002848a:	je     0x1800284cc
    18002848c:	rex xor 0x51(%rbp),%dl
    180028490:	rex.WRB
    180028491:	gs je  0x1800284f5
    180028494:	rex.WRXB (bad)
    180028496:	push   $0x65
    180028498:	movsxd 0x40(%rax,%rax,2),%esi
-   18002849c:	rex.X add %bl,(%rcx)
+   18002849c:	rex.X add %bl,(%rax)
    18002849f:	(bad)
    1800284a0:	(bad)
    1800284a1:	jae    0x180028517
    1800284a3:	(bad)
    1800284a4:	je     0x18002850f
    1800284a6:	movsxd 0x65(%rbp),%ecx
    1800284a9:	je     0x18002850c
@@ -58969,15 +58963,15 @@
    180028579:	movsxd 0x40(%rax,%rax,2),%esi
    18002857d:	xor    0x51(%rbp),%dl
    180028580:	rex.WRB
    180028581:	gs je  0x1800285e5
    180028584:	rex.WRXB (bad)
    180028586:	push   $0x65
    180028588:	movsxd 0x40(%rax,%rax,2),%esi
-   18002858c:	rex.X add %cl,(%rdx)
+   18002858c:	rex.X add %cl,(%rbx)
    18002858f:	or     (%rdi),%bh
    180028591:	movsxd 0x6d(%rdi),%ebp
    180028594:	jo     0x1800285f7
    180028596:	jb     0x1800285fd
    180028598:	rex.WRB
    180028599:	gs insl (%dx),%es:(%rdi)
    18002859b:	outsl  %ds:(%rsi),(%dx)
@@ -59061,32 +59055,30 @@
    18002862b:	rex and $0x24,%al
    18002862e:	push   %rcx
    18002862f:	rex.RB
    180028630:	push   %r14
    180028632:	xor    %al,0x40(%rax)
    180028635:	pop    %rdx
    180028636:	add    %al,(%rax)
-   180028638:	adcb   $0x3f,(%rsi)
-   18002863b:	jb     0x1800286a2
-   18002863d:	jae    0x1800286a4
-   18002863f:	jb     0x1800286b7
+   180028638:	adcl   $0x7365723f,(%rsi)
+   18002863e:	gs jb  0x1800286b7
    180028641:	gs rex push %rcx
    180028644:	rex.X jns 0x1800286bb
    180028647:	gs rex.B jb 0x1800286bd
    18002864b:	(bad)
    18002864c:	jns    0x18002868e
    18002864e:	rex push %rcx
    180028650:	rex.RB
    180028651:	rex.B
    180028652:	pop    %r8
    180028654:	pop    %rdi
    180028655:	rex.WX
    180028656:	rex pop %rdx
    180028658:	add    %al,(%rax)
-   18002865a:	(bad)
+   18002865a:	fwait
    18002865b:	or     (%rdi),%edi
    18002865d:	fs (bad)
    18002865f:	je     0x1800286c2
    180028661:	rex push %rcx
    180028663:	rex.X jns 0x1800286da
    180028666:	gs rex.B jb 0x1800286dc
    18002866a:	(bad)
@@ -59096,15 +59088,15 @@
    180028670:	rex.X
    180028671:	push   %r8
    180028673:	rex.RB
    180028674:	rex.X
    180028675:	rex.R pop %rax
    180028677:	pop    %rdx
    180028678:	add    %al,(%rax)
-   18002867a:	add    %cl,(%rax)
+   18002867a:	add    %ecx,(%rax)
    18002867c:	(bad)
    18002867d:	(bad)
    18002867e:	jo     0x1800286f0
    180028680:	outsb  %gs:(%rsi),(%dx)
    180028682:	fs rex push %rcx
    180028685:	rex.X jns 0x1800286fc
    180028688:	gs rex.B jb 0x1800286fe
@@ -59119,31 +59111,29 @@
    180028696:	push   %r14
    180028698:	xor    %eax,0x50(%rax)
    18002869b:	rex.RB
    18002869c:	rex.X
    18002869d:	rex.R
    18002869e:	rex pop %rdx
    1800286a0:	add    %al,(%rax)
-   1800286a2:	and    $0x19,%al
-   1800286a4:	(bad)
-   1800286a5:	jae    0x180028710
+   1800286a2:	and    $0x69733f19,%eax
    1800286a7:	jp     0x18002870e
    1800286a9:	rex push %rcx
    1800286ab:	rex.X jns 0x180028722
    1800286ae:	gs rex.B jb 0x180028724
    1800286b2:	(bad)
    1800286b3:	jns    0x1800286f5
    1800286b5:	rex push %rcx
    1800286b7:	rex.RB
    1800286b8:	rex.X
    1800286b9:	pop    %r15
    1800286bb:	rex.WX pop %rax
    1800286bd:	pop    %rdx
    1800286be:	add    %al,(%rax)
-   1800286c0:	adc    %dil,(%r15)
+   1800286c0:	rex.X adc %dil,(%rdi)
    1800286c3:	imul   $0x406c6c75,0x4e(%rbx),%esi
    1800286ca:	push   %rcx
    1800286cb:	rex.X jns 0x180028742
    1800286ce:	gs rex.B jb 0x180028744
    1800286d2:	(bad)
    1800286d3:	jns    0x180028715
    1800286d5:	rex push %rcx
@@ -59205,15 +59195,15 @@
    180028735:	push   %rcx
    180028736:	rex.X jns 0x1800287ad
    180028739:	gs rex.B jb 0x1800287af
    18002873d:	(bad)
    18002873e:	jns    0x180028780
    180028740:	rex
    180028741:	rex pop %rdx
-   180028743:	add    %cl,0x6c633f09(%rdx)
+   180028743:	add    %cl,0x6c633f09(%rbx)
    180028749:	(bad)
    18002874a:	jae    0x1800287bf
    18002874c:	rex.WRX (bad)
    18002874e:	insl   (%dx),%es:(%rdi)
    18002874f:	gs rex push %rcx
    180028752:	rex.WRB
    180028753:	gs je  0x1800287b7
@@ -59246,15 +59236,15 @@
    180028784:	push   %rcx
    180028785:	push   %rbx
    180028786:	je     0x1800287fa
    180028788:	imul   $0x45504040,0x67(%rsi),%ebp
    18002878f:	rex.X
    180028790:	xor    %r9b,0x40(%rax)
    180028794:	pop    %rdx
-   180028795:	add    %cl,0x63613f07(%rcx)
+   180028795:	add    %cl,0x63613f07(%rdx)
    18002879b:	je     0x180028806
    18002879d:	jbe    0x180028800
    18002879f:	je     0x180028806
    1800287a1:	rex push %rcx
    1800287a3:	rex.WRB
    1800287a4:	gs je  0x180028808
    1800287a7:	rex.WRXB (bad)
@@ -59275,15 +59265,15 @@
    1800287c3:	xor    %eax,0x48(%rax)
    1800287c6:	push   %rax
    1800287c7:	rex.RB
    1800287c8:	push   %r8
    1800287ca:	rex.RB
    1800287cb:	pop    %r8
    1800287cd:	rex pop %rdx
-   1800287cf:	add    %dl,(%rcx)
+   1800287cf:	add    %dl,(%rdx)
    1800287d1:	or     (%rdi),%bh
    1800287d3:	movsxd 0x6d(%rdi),%ebp
    1800287d6:	jo     0x180028839
    1800287d8:	jb     0x18002883f
    1800287da:	push   %rbx
    1800287db:	je     0x18002884f
    1800287dd:	imul   $0x74514073,0x67(%rsi),%ebp
@@ -59376,15 +59366,15 @@
    180028894:	xor    %al,0x24(%rax)
    180028897:	and    $0x51,%al
    180028899:	rex.RB
    18002889a:	push   %r14
    18002889c:	xor    %al,0x40(%rax)
    18002889f:	pop    %rdx
    1800288a0:	add    %al,(%rax)
-   1800288a2:	movsl  %ds:(%rsi),%es:(%rdi)
+   1800288a2:	cmpsb  %es:(%rdi),%ds:(%rsi)
    1800288a3:	or     (%rdi),%edi
    1800288a5:	fs (bad)
    1800288a7:	je     0x18002890a
    1800288a9:	rex push %rcx
    1800288ab:	push   %rbx
    1800288ac:	je     0x180028920
    1800288ae:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -59393,15 +59383,15 @@
    1800288b8:	rex.RB
    1800288b9:	rex.X push %rsi
    1800288bb:	push   %rcx
    1800288bc:	rex.XB push $0x40407261
    1800288c2:	pop    %rax
    1800288c3:	pop    %rdx
    1800288c4:	add    %al,(%rax)
-   1800288c6:	push   %rdx
+   1800288c6:	push   %rbx
    1800288c7:	adc    %bh,(%rdi)
    1800288c9:	imul   $0x406c6c75,0x4e(%rbx),%esi
    1800288d0:	push   %rcx
    1800288d1:	push   %rbx
    1800288d2:	je     0x180028946
    1800288d4:	imul   $0x45514040,0x67(%rsi),%ebp
    1800288db:	rex.X
@@ -59653,15 +59643,15 @@
    180028a72:	xor    $0x53,%al
    180028a74:	je     0x180028ad7
    180028a76:	je     0x180028aed
    180028a78:	jae    0x180028aba
    180028a7a:	xor    %eax,0x58(%rax)
    180028a7d:	pop    %rdx
    180028a7e:	add    %al,(%rax)
-   180028a80:	mov    $0x18,%ah
+   180028a80:	mov    $0x18,%ch
    180028a82:	(bad)
    180028a83:	jae    0x180028aea
    180028a85:	je     0x180028ada
    180028a87:	je     0x180028aea
    180028a89:	je     0x180028b00
    180028a8b:	jae    0x180028acd
    180028a8d:	push   %rcx
@@ -59680,15 +59670,15 @@
    180028aa0:	xor    $0x53,%al
    180028aa2:	je     0x180028b05
    180028aa4:	je     0x180028b1b
    180028aa6:	jae    0x180028ae8
    180028aa8:	xor    %eax,0x40(%rax)
    180028aab:	pop    %rdx
    180028aac:	add    %al,(%rax)
-   180028aae:	xchg   %eax,%esp
+   180028aae:	xchg   %eax,%ebp
    180028aaf:	(bad)
    180028ab0:	(bad)
    180028ab1:	jb     0x180028b18
    180028ab3:	jae    0x180028b1a
    180028ab5:	je     0x180028b0a
    180028ab7:	je     0x180028b1a
    180028ab9:	je     0x180028b30
@@ -59744,15 +59734,15 @@
    180028b0a:	rex.B
    180028b0b:	rex.B
    180028b0c:	rex.B
    180028b0d:	rex.RB
    180028b0e:	push   %r14
    180028b10:	xor    %al,0x48(%rax)
    180028b13:	rex pop %rdx
-   180028b15:	add    %al,%dl
+   180028b15:	add    %al,%bl
    180028b17:	(bad)
    180028b19:	imul   $0x63697665,0x44(%rbx),%esi
    180028b20:	gs push %rsp
    180028b22:	jb     0x180028b85
    180028b24:	outsb  %ds:(%rsi),(%dx)
    180028b25:	jae    0x180028b88
    180028b27:	movsxd 0x6f(%rcx,%rbp,2),%esi
@@ -59770,15 +59760,15 @@
    180028b3f:	rex
    180028b40:	rex push %rcx
    180028b42:	rex.RB
    180028b43:	rex.X
    180028b44:	pop    %r15
    180028b46:	rex.WRX pop %rax
    180028b48:	pop    %rdx
-   180028b49:	add    %bl,%bl
+   180028b49:	add    %bl,%ah
    180028b4b:	adc    $0x6765723f,%eax
    180028b50:	imul   $0x6f4e7265,0x74(%rbx),%esi
    180028b57:	jb     0x180028bc6
    180028b59:	(bad)
    180028b5a:	insb   (%dx),%es:(%rdi)
    180028b5b:	imul   $0x70795464,0x65(%rdx),%edi
    180028b62:	gs fs gs rex push %cx
@@ -59797,29 +59787,29 @@
    180028b7d:	gs rex.B jb 0x180028bf3
    180028b81:	(bad)
    180028b82:	jns    0x180028bc4
    180028b84:	rex push %rsi
    180028b86:	xor    %eax,0x40(%rax)
    180028b89:	pop    %rdx
    180028b8a:	add    %al,(%rax)
-   180028b8c:	mov    $0x64693f0e,%ebp
+   180028b8c:	mov    $0x64693f0e,%esi
    180028b91:	rex push %rcx
    180028b93:	rex.WRB
    180028b94:	gs je  0x180028bf8
    180028b97:	push   %rsp
    180028b98:	jns    0x180028c0a
    180028b9a:	gs rex
    180028b9c:	rex push %rcx
    180028b9e:	rex.RB
    180028b9f:	rex.X
    180028ba0:	rex.B
    180028ba1:	rex.W
    180028ba2:	rex.W
    180028ba3:	rex pop %rdx
-   180028ba5:	add    %bl,0xc(%rdi)
+   180028ba5:	add    %ah,0xc(%rax)
    180028ba8:	(bad)
    180028ba9:	fs jns 0x180028c1a
    180028bac:	(bad)
    180028bad:	insl   (%dx),%es:(%rdi)
    180028bae:	imul   $0x4f617465,0x4d(%rbx),%esp
    180028bb5:	(bad)
    180028bb6:	push   $0x65
@@ -59839,15 +59829,15 @@
    180028bd1:	rex.WRB
    180028bd2:	gs je  0x180028c36
    180028bd5:	rex.WRXB (bad)
    180028bd7:	push   $0x65
    180028bd9:	movsxd 0x40(%rax,%rax,2),%esi
    180028bdd:	pop    %rax
    180028bde:	pop    %rdx
-   180028bdf:	add    %cl,(%rdi)
+   180028bdf:	add    %dl,(%rax)
    180028be1:	adc    $0x5f74713f,%eax
    180028be6:	insl   (%dx),%es:(%rdi)
    180028be7:	gs je  0x180028c4b
    180028bea:	movsxd 0x73(%rcx),%esp
    180028bed:	je     0x180028c2f
    180028bef:	push   %rcx
    180028bf0:	rex.WRXB (bad)
@@ -59861,15 +59851,15 @@
    180028bfe:	pop    %r8
    180028c00:	push   %rax
    180028c01:	rex.RB
    180028c02:	rex.X
    180028c03:	rex.R
    180028c04:	rex pop %rdx
    180028c06:	add    %al,(%rax)
-   180028c08:	ficoml (%rdi,%rdi,1)
+   180028c08:	fistl  (%rdi,%rdi,1)
    180028c0b:	jno    0x180028c81
    180028c0d:	pop    %rdi
    180028c0e:	insl   (%dx),%es:(%rdi)
    180028c0f:	gs je  0x180028c73
    180028c12:	movsxd 0x6c(%rcx),%esp
    180028c15:	insb   (%dx),%es:(%rdi)
    180028c16:	rex push %rcx
@@ -60031,15 +60021,15 @@
    180028d46:	rex push %rcx
    180028d48:	rex.RB
    180028d49:	rex.B
    180028d4a:	rex.B
    180028d4b:	rex pop %rax
    180028d4d:	pop    %rdx
    180028d4e:	add    %al,(%rax)
-   180028d50:	mov    $0x14,%cl
+   180028d50:	mov    $0x14,%dl
    180028d52:	(bad)
    180028d53:	jno    0x180028dc9
    180028d55:	pop    %rdi
    180028d56:	push   %rcx
    180028d57:	rex.WRB
    180028d58:	gs je  0x180028dbc
    180028d5b:	rex.RB outsb %ds:(%rsi),(%dx)
@@ -60137,15 +60127,15 @@
    180028dfe:	rex.RB
    180028dff:	push   %r14
    180028e01:	xor    %al,0x41(%rax)
    180028e04:	rex.RB
    180028e05:	rex.X push %rsi
    180028e07:	xor    %al,0x40(%rax)
    180028e0a:	pop    %rdx
-   180028e0b:	add    %bl,0x64713f14(%rdi)
+   180028e0b:	add    %ah,0x64713f14(%rax)
    180028e11:	(bad)
    180028e17:	insb   (%dx),%es:(%rdi)
    180028e18:	jo     0x180028e7f
    180028e1a:	jb     0x180028e5c
    180028e1c:	push   %rcx
    180028e1d:	push   %rsi
    180028e1e:	(bad)
@@ -60162,15 +60152,15 @@
    180028e2d:	push   %rcx
    180028e2e:	rex.R
    180028e2f:	(bad)
    180028e35:	push   %rsi
    180028e36:	xor    0x40(%rax),%al
    180028e39:	pop    %rdx
    180028e3a:	add    %al,(%rax)
-   180028e3c:	rorb   %cl,(%rdi,%rdi,1)
+   180028e3c:	rorl   %cl,(%rdi,%rdi,1)
    180028e3f:	gs jno 0x180028eb7
    180028e42:	(bad)
    180028e43:	insb   (%dx),%es:(%rdi)
    180028e44:	jae    0x180028e86
    180028e46:	push   %rcx
    180028e47:	push   %rsi
    180028e48:	(bad)
@@ -60247,15 +60237,15 @@
    180028eb5:	(bad)
    180028eb6:	jb     0x180028f21
    180028eb8:	(bad)
    180028eb9:	outsb  %ds:(%rsi),(%dx)
    180028eba:	je     0x180028efc
    180028ebc:	rex
    180028ebd:	rex pop %rdx
-   180028ebf:	add    %dl,%bh
+   180028ebf:	add    %bl,%al
    180028ec1:	or     (%rdi),%edi
    180028ec3:	fs gs (bad)
    180028ec6:	insb   (%dx),%es:(%rdi)
    180028ec7:	insb   (%dx),%es:(%rdi)
    180028ec8:	outsl  %ds:(%rsi),(%dx)
    180028ec9:	movsxd 0x74(%rcx),%esp
    180028ecc:	gs rex push %rcx
@@ -60290,17 +60280,16 @@
    180028f01:	push   %r14
    180028f03:	xor    %al,0x24(%rax)
    180028f06:	and    $0x51,%al
    180028f08:	rex.RB
    180028f09:	push   %r14
    180028f0b:	xor    %al,0x40(%rax)
    180028f0e:	pop    %rdx
-   180028f0f:	add    %bh,%bh
-   180028f11:	(bad)
-   180028f12:	(bad)
+   180028f0f:	add    %al,(%rax)
+   180028f11:	or     %bh,(%rdi)
    180028f13:	(bad)
    180028f14:	jo     0x180028f86
    180028f16:	outsb  %gs:(%rsi),(%dx)
    180028f18:	fs rex push %rcx
    180028f1b:	rex.X jns 0x180028f92
    180028f1e:	gs rex.B jb 0x180028f94
    180028f22:	(bad)
@@ -60393,15 +60382,15 @@
    180028fc4:	rex.RB
    180028fc5:	push   %r14
    180028fc7:	xor    %al,0x41(%rax)
    180028fca:	rex.RB
    180028fcb:	rex.X push %rsi
    180028fcd:	xor    %al,0x40(%rax)
    180028fd0:	pop    %rdx
-   180028fd1:	add    %bh,0x18(%rax)
+   180028fd1:	add    %bh,0x18(%rcx)
    180028fd4:	(bad)
    180028fd5:	jae    0x18002903c
    180028fd7:	je     0x18002902a
    180028fd9:	jne    0x180029040
    180028fdb:	jb     0x180029056
    180028fdd:	rex push %rcx
    180028fdf:	push   %rbp
@@ -60448,15 +60437,15 @@
    180029020:	movsxd 0x40(%rax,%rax,2),%esi
    180029024:	push   %rbp
    180029025:	rex.RB
    180029026:	rex.B
    180029027:	rex.B
    180029028:	rex pop %rax
    18002902a:	pop    %rdx
-   18002902b:	add    %bh,0x13(%rsi)
+   18002902b:	add    %bh,0x13(%rdi)
    18002902e:	(bad)
    18002902f:	jo     0x180029092
    180029031:	jb     0x180029098
    180029033:	outsb  %ds:(%rsi),(%dx)
    180029034:	je     0x180029076
    180029036:	push   %rcx
    180029037:	rex.WRXB (bad)
@@ -60488,16 +60477,18 @@
    180029068:	movsxd 0x72(%rax,%rdx,2),%esi
    18002906c:	imul   $0x40406574,0x61(%rsi),%esi
    180029073:	push   %rax
    180029074:	rex.RB
    180029075:	push   %r14
    180029077:	xor    %al,0x40(%rax)
    18002907a:	pop    %rdx
-   18002907b:	add    %bh,0x65673f0e(%rip)        # 0x1e569cf8f
-   180029081:	je     0x1800290c4
+   18002907b:	add    %bh,(%rsi)
+   18002907d:	(bad)
+   18002907e:	(bad)
+   18002907f:	addr32 gs je 0x1800290c4
    180029083:	outsb  %ds:(%rsi),(%dx)
    180029084:	fs push %rdx
    180029086:	gs data16 rex
    180029089:	rex.RB js 0x180029100
    18002908c:	gs jb  0x1800290fd
    18002908f:	(bad)
    180029090:	insb   (%dx),%es:(%rdi)
@@ -60693,15 +60684,15 @@
    18002920e:	push   %rsp
    18002920f:	imul   $0x45514040,0x65(%rbp),%ebp
    180029216:	rex.X
    180029217:	pop    %r15
    180029219:	rex.WX pop %rax
    18002921b:	pop    %rdx
    18002921c:	add    %al,(%rax)
-   18002921e:	or     (%rbx),%cl
+   18002921e:	or     (%rbx),%ecx
    180029220:	(bad)
    180029221:	movsxd 0x72(%rbp),%esi
    180029224:	jb     0x18002928b
    180029226:	outsb  %ds:(%rsi),(%dx)
    180029227:	je     0x18002926d
    180029229:	(bad)
    18002922a:	je     0x180029291
@@ -60783,15 +60774,15 @@
    1800292c4:	push   %rbp
    1800292c5:	jb     0x180029333
    1800292c7:	rex
    1800292c8:	rex
    1800292c9:	rex
    1800292ca:	rex
    1800292cb:	rex pop %rdx
-   1800292cd:	add    %al,%ch
+   1800292cd:	add    %al,%dh
    1800292cf:	(bad)
    1800292d0:	(bad)
    1800292d1:	(bad)
    1800292d2:	fs fs push %rcx
    1800292d5:	jne    0x18002933c
    1800292d7:	jb     0x180029352
    1800292d9:	rex.WB je 0x180029341
@@ -60828,15 +60819,15 @@
    180029311:	je     0x180029353
    180029313:	rex push %rcx
    180029315:	rex.RB
    180029316:	rex.B
    180029317:	rex.B
    180029318:	rex pop %rax
    18002931a:	pop    %rdx
-   18002931b:	add    %ah,(%rdi)
+   18002931b:	add    %ch,(%rax)
    18002931d:	(bad)
    18002931e:	(bad)
    18002931f:	data16 jb 0x180029391
    180029322:	insl   (%dx),%es:(%rdi)
    180029323:	push   %rsi
    180029324:	(bad)
    180029325:	jb     0x180029390
@@ -60893,15 +60884,15 @@
    180029383:	outsb  %ds:(%rsi),(%dx)
    180029384:	rex.RX outsl %ds:(%rsi),(%dx)
    180029386:	jb     0x1800293f5
    180029388:	(bad)
    180029389:	je     0x1800293cb
    18002938b:	xor    %eax,0x40(%rax)
    18002938e:	pop    %rdx
-   18002938f:	add    %bh,0x9(%rax)
+   18002938f:	add    %bh,0x9(%rcx)
    180029392:	(bad)
    180029393:	movsxd 0x69(%rax),%ebp
    180029396:	insb   (%dx),%es:(%rdi)
    180029397:	fs rex.RB jbe 0x180029400
    18002939b:	outsb  %ds:(%rsi),(%dx)
    18002939c:	je     0x1800293de
    18002939e:	push   %rcx
@@ -60918,15 +60909,15 @@
    1800293b0:	push   %rcx
    1800293b1:	rex.XB push $0x45646c69
    1800293b7:	jbe    0x18002941e
    1800293b9:	outsb  %ds:(%rsi),(%dx)
    1800293ba:	je     0x1800293fc
    1800293bc:	rex
    1800293bd:	rex pop %rdx
-   1800293bf:	add    %dh,(%rdi)
+   1800293bf:	add    %bh,(%rax)
    1800293c1:	or     (%rdi),%bh
    1800293c3:	movsxd 0x6e(%rdi),%ebp
    1800293c6:	outsb  %ds:(%rsi),(%dx)
    1800293c7:	movsxd %gs:0x6f(%rsi,%rcx,2),%esi
    1800293cc:	je     0x180029437
    1800293ce:	data16 jns 0x180029411
    1800293d1:	push   %rcx
@@ -60946,15 +60937,15 @@
    1800293e8:	rex.WRB
    1800293e9:	gs je  0x180029454
    1800293ec:	outsl  %ds:(%rsi),(%dx)
    1800293ed:	fs rex
    1800293ef:	rex
    1800293f0:	rex pop %rdx
    1800293f2:	add    %al,(%rax)
-   1800293f4:	sub    %cl,(%rbx)
+   1800293f4:	sub    %ecx,(%rbx)
    1800293f6:	(bad)
    1800293f7:	movsxd 0x73(%rbp),%esi
    1800293fa:	je     0x18002946b
    1800293fc:	insl   (%dx),%es:(%rdi)
    1800293fd:	rex.RB jbe 0x180029465
    180029400:	outsb  %ds:(%rsi),(%dx)
    180029401:	je     0x180029443
@@ -60971,20 +60962,18 @@
    180029413:	push   %r14
    180029415:	push   %rcx
    180029416:	rex.RB jbe 0x18002947e
    180029419:	outsb  %ds:(%rsi),(%dx)
    18002941a:	je     0x18002945c
    18002941c:	rex
    18002941d:	rex pop %rdx
-   18002941f:	add    %dh,0x69643f0c(%rip)        # 0x1e966d331
-   180029425:	jae    0x18002948a
-   180029427:	outsl  %ds:(%rsi),(%dx)
-   180029428:	outsb  %ds:(%rsi),(%dx)
-   180029429:	outsb  %ds:(%rsi),(%dx)
-   18002942a:	movsxd %gs:0x6f(%rsi,%rcx,2),%esi
+   18002941f:	add    %dh,(%rsi)
+   180029421:	or     $0x3f,%al
+   180029423:	imul   $0x656e6e6f,%fs:0x63(%rbx),%esi
+   18002942b:	movsxd 0x6f(%rsi,%rcx,2),%esi
    18002942f:	je     0x18002949a
    180029431:	data16 jns 0x180029474
    180029434:	push   %rcx
    180029435:	rex.WRXB (bad)
    180029437:	push   $0x65
    180029439:	movsxd 0x40(%rax,%rax,2),%esi
    18002943d:	rex.WRB
@@ -60999,17 +60988,16 @@
    180029448:	gs je  0x1800294ac
    18002944b:	rex.WRB
    18002944c:	gs je  0x1800294b7
    18002944f:	outsl  %ds:(%rsi),(%dx)
    180029450:	fs rex
    180029452:	rex
    180029453:	rex pop %rdx
-   180029455:	add    %bh,%bh
-   180029457:	or     $0x3f,%al
-   180029459:	gs jbe 0x1800294c1
+   180029455:	add    %al,(%rax)
+   180029457:	or     $0x6576653f,%eax
    18002945c:	outsb  %ds:(%rsi),(%dx)
    18002945d:	je     0x18002949f
    18002945f:	push   %rcx
    180029460:	rex.WRXB (bad)
    180029462:	push   $0x65
    180029464:	movsxd 0x40(%rax,%rax,2),%esi
    180029468:	push   %rbp
@@ -61022,16 +61010,15 @@
    180029472:	push   %rcx
    180029473:	rex.RB jbe 0x1800294db
    180029476:	outsb  %ds:(%rsi),(%dx)
    180029477:	je     0x1800294b9
    180029479:	rex
    18002947a:	rex pop %rdx
    18002947c:	add    %al,(%rax)
-   18002947e:	prefetch (%rdi)
-   180029481:	gs jbe 0x1800294e9
+   18002947e:	adc    %cl,0x6576653f(%rip)        # 0x1e578f9c3
    180029484:	outsb  %ds:(%rsi),(%dx)
    180029485:	je     0x1800294cd
    180029487:	imul   $0x4f514072,0x65(%rsp,%rsi,2),%ebp
    18002948f:	(bad)
    180029490:	push   $0x65
    180029492:	movsxd 0x40(%rax,%rax,2),%esi
    180029496:	push   %rbp
@@ -61047,17 +61034,15 @@
    1800294a6:	push   %rcx
    1800294a7:	rex.RB jbe 0x18002950f
    1800294aa:	outsb  %ds:(%rsi),(%dx)
    1800294ab:	je     0x1800294ed
    1800294ad:	rex
    1800294ae:	rex pop %rdx
    1800294b0:	add    %al,(%rax)
-   1800294b2:	mov    $0xd,%bh
-   1800294b4:	(bad)
-   1800294b5:	data16 insb (%dx),%es:(%rdi)
+   1800294b2:	mov    $0x6c663f0d,%eax
    1800294b7:	(bad)
    1800294b8:	addr32 jae 0x180029501
    1800294bb:	outsl  %ds:(%rsi),(%dx)
    1800294bc:	jb     0x180029502
    1800294be:	jne    0x18002952d
    1800294c0:	jo     0x18002952b
    1800294c2:	outsb  %ds:(%rsi),(%dx)
@@ -61153,15 +61138,15 @@
    18002958e:	pop    %r8
    180029590:	push   %rax
    180029591:	rex.RB
    180029592:	rex.X
    180029593:	rex.R pop %rdx
    180029595:	pop    %rdx
    180029596:	add    %al,(%rax)
-   180029598:	xchg   %eax,%ebx
+   180029598:	xchg   %eax,%esp
    180029599:	adc    %edi,(%rdi)
    18002959b:	insb   (%dx),%es:(%rdi)
    18002959c:	outsb  %gs:(%rsi),(%dx)
    18002959e:	addr32 je 0x180029609
    1800295a1:	rex.W
    1800295a2:	gs insb (%dx),%es:(%rdi)
    1800295a4:	jo     0x18002960b
@@ -61197,16 +61182,18 @@
    1800295e3:	rex push %rax
    1800295e5:	rex.RB
    1800295e6:	rex.X
    1800295e7:	rex.R pop %rdi
    1800295e9:	rex.WX
    1800295ea:	rex pop %rdx
    1800295ec:	add    %al,(%rax)
-   1800295ee:	xor    $0x72613f08,%eax
-   1800295f3:	addr32 rex push %rcx
+   1800295ee:	ss or  %bh,(%rdi)
+   1800295f1:	(bad)
+   1800295f2:	jb     0x18002965b
+   1800295f4:	rex push %rcx
    1800295f6:	push   %rbx
    1800295f7:	je     0x18002966b
    1800295f9:	imul   $0x45514040,0x67(%rsi),%ebp
    180029600:	rex.X
    180029601:	rex.B (bad)
    180029603:	push   %r14
    180029605:	xor    %eax,0x41(%rax)
@@ -61234,16 +61221,18 @@
    180029635:	push   %rcx
    180029636:	rex.X jns 0x1800296ad
    180029639:	gs rex.B jb 0x1800296af
    18002963d:	(bad)
    18002963e:	jns    0x180029680
    180029640:	rex pop %rax
    180029642:	pop    %rdx
-   180029643:	add    %ah,0x72663f0e(%rip)        # 0x1f268d557
-   180029649:	outsl  %ds:(%rsi),(%dx)
+   180029643:	add    %ah,(%rsi)
+   180029645:	(bad)
+   180029646:	(bad)
+   180029647:	data16 jb 0x1800296b9
    18002964a:	insl   (%dx),%es:(%rdi)
    18002964b:	push   %rbp
    18002964c:	je     0x1800296b4
    18002964e:	cmp    %al,0x51(%rax)
    180029651:	push   %rbx
    180029652:	je     0x1800296c6
    180029654:	imul   $0x41534040,0x67(%rsi),%ebp
@@ -61252,15 +61241,15 @@
    18002965e:	xor    %eax,0x56(%rax)
    180029661:	push   %rcx
    180029662:	rex.X jns 0x1800296d9
    180029665:	gs rex.B jb 0x1800296db
    180029669:	(bad)
    18002966a:	jns    0x1800296c2
    18002966c:	imul   $0x5a404040,0x77(%rbp),%esp
-   180029673:	add    %bl,(%rdx)
+   180029673:	add    %bl,(%rbx)
    180029675:	adc    (%rdi),%edi
    180029677:	outsb  %ds:(%rsi),(%dx)
    180029678:	outsl  %ds:(%rsi),(%dx)
    180029679:	jb     0x1800296e8
    18002967b:	(bad)
    18002967c:	insb   (%dx),%es:(%rdi)
    18002967d:	imul   $0x70795464,0x65(%rdx),%edi
@@ -61301,15 +61290,15 @@
    1800296c9:	push   %rcx
    1800296ca:	rex.RB
    1800296cb:	rex.B
    1800296cc:	rex.B
    1800296cd:	rex pop %rax
    1800296cf:	pop    %rdx
    1800296d0:	add    %al,(%rax)
-   1800296d2:	xor    (%rdx),%ecx
+   1800296d2:	xor    $0xa,%al
    1800296d4:	(bad)
    1800296d5:	movsxd 0x6e(%rdi),%ebp
    1800296d8:	outsb  %ds:(%rsi),(%dx)
    1800296d9:	movsxd %gs:0x6d(%rcx,%rcx,2),%esi
    1800296de:	jo     0x18002974c
    1800296e0:	rex push %rcx
    1800296e2:	rex.WRXB (bad)
@@ -61433,15 +61422,15 @@
    1800297c6:	xor    %al,0x24(%rax)
    1800297c9:	and    $0x51,%al
    1800297cb:	rex.RB
    1800297cc:	push   %r14
    1800297ce:	xor    %al,0x40(%rax)
    1800297d1:	pop    %rdx
    1800297d2:	add    %al,(%rax)
-   1800297d4:	(bad)
+   1800297d4:	iret
    1800297d5:	or     $0x3f,%al
    1800297d7:	gs jno 0x18002984f
    1800297da:	(bad)
    1800297db:	insb   (%dx),%es:(%rdi)
    1800297dc:	jae    0x18002981e
    1800297de:	push   %rcx
    1800297df:	rex.R (bad)
@@ -61452,15 +61441,15 @@
    1800297ec:	pop    %r15
    1800297ee:	rex.WRX
    1800297ef:	rex.B
    1800297f0:	rex.RB
    1800297f1:	rex.X push %rsi
    1800297f3:	xor    %eax,0x40(%rax)
    1800297f6:	pop    %rdx
-   1800297f7:	add    %cl,%al
+   1800297f7:	add    %cl,%cl
    1800297f9:	adc    (%rdi),%edi
    1800297fb:	jo     0x18002986f
    1800297fd:	movsxd %gs:0x64(%rbp),%esp
    180029801:	gs jae 0x180029844
    180029804:	push   %rcx
    180029805:	rex.R (bad)
    180029807:	je     0x18002986e
@@ -61543,15 +61532,15 @@
    180029899:	rex.RB
    18002989a:	rex.X push %rsi
    18002989c:	push   %rcx
    18002989d:	rex.R (bad)
    18002989f:	je     0x180029906
    1800298a1:	push   %rsp
    1800298a2:	imul   $0x5a404040,0x65(%rbp),%ebp
-   1800298a9:	add    %ch,0x15(%rsi)
+   1800298a9:	add    %ch,0x15(%rdi)
    1800298ac:	(bad)
    1800298ad:	jno    0x180029924
    1800298af:	gs jb  0x18002992b
    1800298b2:	rex push %rcx
    1800298b4:	push   %rbp
    1800298b5:	jb     0x180029923
    1800298b7:	rex
@@ -61587,15 +61576,15 @@
    1800298f0:	push   %rbp
    1800298f1:	jb     0x18002995f
    1800298f3:	rex
    1800298f4:	rex
    1800298f5:	rex
    1800298f6:	rex
    1800298f7:	rex pop %rdx
-   1800298f9:	add    %ah,(%rdx)
+   1800298f9:	add    %ah,(%rbx)
    1800298fb:	adc    %edi,(%rdi)
    1800298fd:	imul   $0x696e7261,0x57(%rbx),%esi
    180029904:	outsb  %ds:(%rsi),(%dx)
    180029905:	rex.RB outsb %ds:(%esi),(%dx)
    180029908:	(bad)
    180029909:	(bad)
    18002990a:	insb   (%dx),%es:(%rdi)
@@ -61664,16 +61653,16 @@
    180029984:	rex.B
    180029985:	rex push %rax
    180029987:	rex.RB
    180029988:	rex.X
    180029989:	rex.R
    18002998a:	rex.W xor %al,0x5a(%rax)
    18002998e:	add    %al,(%rax)
-   180029990:	cmp    $0x61663f0d,%eax
-   180029995:	je     0x1800299f8
+   180029990:	ds or  $0x7461663f,%eax
+   180029996:	(bad)
    180029997:	insb   (%dx),%es:(%rdi)
    180029998:	rex push %rcx
    18002999a:	rex.WRB
    18002999b:	gs jae 0x180029a11
    18002999e:	(bad)
    18002999f:	rex.WR outsl %gs:(%esi),(%dx)
    1800299a3:	addr32 addr32 gs jb 0x1800299e8
@@ -61683,15 +61672,15 @@
    1800299ac:	pop    %r8
    1800299ae:	push   %rax
    1800299af:	rex.RB
    1800299b0:	rex.X
    1800299b1:	rex.R pop %rdx
    1800299b3:	pop    %rdx
    1800299b4:	add    %al,(%rax)
-   1800299b6:	out    %al,(%dx)
+   1800299b6:	out    %eax,(%dx)
    1800299b7:	(bad)
    1800299b8:	(bad)
    1800299b9:	(bad)
    1800299ba:	insb   (%dx),%es:(%rdi)
    1800299bb:	insb   (%dx),%es:(%rdi)
    1800299bc:	outsl  %ds:(%rsi),(%dx)
    1800299bd:	movsxd 0x74(%rcx),%esp
@@ -61722,15 +61711,16 @@
    1800299ea:	imul   $0x6974704f,0x6e(%rdi),%ebp
    1800299f1:	outsl  %ds:(%rsi),(%dx)
    1800299f2:	outsb  %ds:(%rsi),(%dx)
    1800299f3:	rex xor %eax,0x40(%rax)
    1800299f7:	pop    %rdx
    1800299f8:	add    %al,(%rax)
    1800299fa:	(bad)
-   1800299fb:	adc    $0x6165723f,%eax
+   1800299fd:	jb     0x180029a64
+   1800299ff:	(bad)
    180029a00:	insb   (%dx),%es:(%rdi)
    180029a01:	insb   (%dx),%es:(%rdi)
    180029a02:	outsl  %ds:(%rsi),(%dx)
    180029a03:	movsxd 0x74(%rcx),%esp
    180029a06:	gs push %rbp
    180029a08:	outsb  %ds:(%rsi),(%dx)
    180029a09:	(bad)
@@ -61774,15 +61764,15 @@
    180029a55:	outsl  %ds:(%rsi),(%dx)
    180029a56:	movsxd 0x74(%rcx),%esp
    180029a59:	imul   $0x6974704f,0x6e(%rdi),%ebp
    180029a60:	outsl  %ds:(%rsi),(%dx)
    180029a61:	outsb  %ds:(%rsi),(%dx)
    180029a62:	rex xor %eax,0x40(%rax)
    180029a66:	pop    %rdx
-   180029a67:	add    %al,0xa(%rsi)
+   180029a67:	add    %al,0xa(%rdi)
    180029a6a:	(bad)
    180029a6b:	movsxd 0x6e(%rdi),%ebp
    180029a6e:	jae    0x180029ae4
    180029a70:	rex.R (bad)
    180029a72:	je     0x180029ad5
    180029a74:	rex push %rcx
    180029a76:	rex.X jns 0x180029aed
@@ -61829,15 +61819,15 @@
    180029ace:	(bad)
    180029acf:	jns    0x180029b11
    180029ad1:	rex
    180029ad2:	rex
    180029ad3:	rex
    180029ad4:	rex pop %rdx
    180029ad6:	add    %al,(%rax)
-   180029ad8:	rex.WRX or %r15,(%rdi)
+   180029ad8:	rex.WRXB or %r15,(%r15)
    180029adb:	movsxd 0x73(%rcx),%esp
    180029ade:	je     0x180029b20
    180029ae0:	push   %rcx
    180029ae1:	rex.WRB
    180029ae2:	gs je  0x180029b46
    180029ae5:	rex.WRXB (bad)
    180029ae7:	push   $0x65
@@ -61920,69 +61910,69 @@
    180029b77:	je     0x180029be2
    180029b79:	outsb  %ds:(%rsi),(%dx)
    180029b7a:	xor    %eax,0x68(%rbx)
    180029b7d:	(bad)
    180029b7e:	jb     0x180029bc0
    180029b80:	rex
    180029b81:	rex pop %rdx
-   180029b83:	add    %bl,0x7365723f(%rsi,%rdx,1)
-   180029b8a:	imul   $0x74535140,0x65(%rdx),%edi
-   180029b91:	jb     0x180029bfc
-   180029b93:	outsb  %ds:(%rsi),(%dx)
-   180029b94:	addr32 rex
-   180029b96:	rex push %rcx
-   180029b98:	rex.RB
+   180029b83:	add    %bl,0x65723f16(%rbp)
+   180029b89:	jae    0x180029bf4
+   180029b8b:	jp     0x180029bf2
+   180029b8d:	rex push %rcx
+   180029b8f:	push   %rbx
+   180029b90:	je     0x180029c04
+   180029b92:	imul   $0x45514040,0x67(%rsi),%ebp
    180029b99:	rex.B
    180029b9a:	pop    %r8
    180029b9c:	pop    %rdi
    180029b9d:	rex.WX
    180029b9e:	rex pop %rdx
    180029ba0:	add    %al,(%rax)
-   180029ba2:	(bad)
-   180029ba3:	or     %edi,(%rdi)
+   180029ba2:	cmp    %cl,(%rcx)
+   180029ba4:	(bad)
    180029ba5:	movsxd 0x70(%rcx),%esp
    180029ba8:	(bad)
    180029ba9:	movsxd 0x74(%rcx),%ebp
    180029bac:	jns    0x180029bee
    180029bae:	push   %rcx
    180029baf:	push   %rbx
    180029bb0:	je     0x180029c24
    180029bb2:	imul   $0x45514040,0x67(%rsi),%ebp
    180029bb9:	rex.X
    180029bba:	pop    %r15
    180029bbc:	rex.WX pop %rax
    180029bbe:	pop    %rdx
-   180029bbf:	add    %al,0x65723f16(%rdx)
+   180029bbf:	add    %al,0x65723f16(%rbx)
    180029bc5:	jae    0x180029c2c
    180029bc7:	jb     0x180029c3f
    180029bc9:	gs rex push %rcx
    180029bcc:	push   %rbx
    180029bcd:	je     0x180029c41
    180029bcf:	imul   $0x45514040,0x67(%rsi),%ebp
    180029bd6:	rex.B
    180029bd7:	pop    %r8
    180029bd9:	pop    %rdi
    180029bda:	rex.WX
    180029bdb:	rex pop %rdx
-   180029bdd:	add    %ah,0x7461643f(%rbx,%rcx,1)
-   180029be4:	(bad)
+   180029bdd:	add    %ah,0x61643f0b(%rbp)
+   180029be3:	je     0x180029c46
    180029be5:	rex push %rcx
    180029be7:	push   %rbx
    180029be8:	je     0x180029c5c
    180029bea:	imul   $0x45514040,0x67(%rsi),%ebp
    180029bf1:	rex.B
    180029bf2:	push   %r8
    180029bf4:	rex.RB
    180029bf5:	push   %r14
    180029bf7:	push   %rcx
    180029bf8:	rex.XB push $0x40407261
    180029bfe:	pop    %rax
    180029bff:	pop    %rdx
    180029c00:	add    %al,(%rax)
-   180029c02:	rex.WB or (%r15),%dil
+   180029c02:	rex.WX or (%rdi),%dil
    180029c05:	movsxd 0x6e(%rdi),%ebp
    180029c08:	jae    0x180029c7e
    180029c0a:	rex.R (bad)
    180029c0c:	je     0x180029c6f
    180029c0e:	rex push %rcx
    180029c10:	push   %rbx
    180029c11:	je     0x180029c85
@@ -61991,40 +61981,40 @@
    180029c1b:	push   %r8
    180029c1d:	rex.RB
    180029c1e:	rex.X push %rsi
    180029c20:	push   %rcx
    180029c21:	rex.XB push $0x40407261
    180029c27:	pop    %rax
    180029c28:	pop    %rdx
-   180029c29:	add    %dl,(%rax)
+   180029c29:	add    %dl,(%rcx)
    180029c2b:	or     $0x3f,%al
    180029c2d:	fs gs je 0x180029c92
    180029c31:	movsxd 0x40(%rax),%ebp
    180029c34:	push   %rcx
    180029c35:	push   %rbx
    180029c36:	je     0x180029caa
    180029c38:	imul   $0x45514040,0x67(%rsi),%ebp
    180029c3f:	rex.B
    180029c40:	pop    %r8
    180029c42:	pop    %rax
    180029c43:	pop    %rdx
    180029c44:	add    %al,(%rax)
-   180029c46:	popf
+   180029c46:	sahf
    180029c47:	or     %edi,(%rdi)
    180029c49:	movsxd 0x61(%rbp,%riz,2),%ebp
    180029c4d:	jb     0x180029c8f
    180029c4f:	push   %rcx
    180029c50:	push   %rbx
    180029c51:	je     0x180029cc5
    180029c53:	imul   $0x45514040,0x67(%rsi),%ebp
    180029c5a:	rex.B
    180029c5b:	pop    %r8
    180029c5d:	pop    %rax
    180029c5e:	pop    %rdx
-   180029c5f:	add    %dh,0x74733f19(%rdx)
+   180029c5f:	add    %dh,0x74733f19(%rbx)
    180029c65:	(bad)
    180029c66:	jb     0x180029cdc
    180029c68:	jae    0x180029cc1
    180029c6a:	imul   $0x72745351,0x40(%rax,%rbp,2),%esi
    180029c72:	imul   $0x45514040,0x67(%rsi),%ebp
    180029c79:	rex.X
    180029c7a:	pop    %r15
@@ -62042,15 +62032,15 @@
    180029c8e:	je     0x180029cf9
    180029c90:	jbe    0x180029cfb
    180029c92:	je     0x180029d0d
    180029c94:	rex push %rcx
    180029c96:	je     0x180029cd8
    180029c98:	rex
    180029c99:	rex pop %rdx
-   180029c9b:	add    %ah,(%rcx)
+   180029c9b:	add    %ah,(%rdx)
    180029c9d:	or     %bh,(%rdi)
    180029c9f:	(bad)
    180029ca0:	jo     0x180029d12
    180029ca2:	outsb  %gs:(%rsi),(%dx)
    180029ca4:	fs rex push %rcx
    180029ca7:	push   %rbx
    180029ca8:	je     0x180029d1c
@@ -62090,29 +62080,30 @@
    180029ced:	rex.X jns 0x180029d64
    180029cf0:	gs rex.B jb 0x180029d66
    180029cf4:	(bad)
    180029cf5:	jns    0x180029d37
    180029cf7:	rex pop %rax
    180029cf9:	pop    %rdx
    180029cfa:	add    %al,(%rax)
-   180029cfc:	cmp    $0x756e3f13,%eax
-   180029d01:	insl   (%dx),%es:(%rdi)
+   180029cfc:	ds adc (%rdi),%edi
+   180029cff:	outsb  %ds:(%rsi),(%dx)
+   180029d00:	jne    0x180029d6f
    180029d02:	(bad)
    180029d04:	jb     0x180029d46
    180029d06:	push   %rcx
    180029d07:	push   %rbx
    180029d08:	je     0x180029d7c
    180029d0a:	imul   $0x41534040,0x67(%rsi),%ebp
    180029d11:	(bad)
    180029d12:	push   %r14
    180029d14:	xor    %eax,0x5f(%rax)
    180029d17:	rex.WX
    180029d18:	rex.W
    180029d19:	rex pop %rdx
-   180029d1b:	add    %ah,(%rdi)
+   180029d1b:	add    %ch,(%rax)
    180029d1d:	or     %bh,(%rdi)
    180029d1f:	(bad)
    180029d20:	jo     0x180029d92
    180029d22:	outsb  %gs:(%rsi),(%dx)
    180029d24:	fs rex.WR (bad)
    180029d27:	je     0x180029d92
    180029d29:	outsb  %ds:(%rsi),(%dx)
@@ -62141,15 +62132,15 @@
    180029d55:	addr32 rex
    180029d57:	rex push %rax
    180029d59:	rex.RB
    180029d5a:	push   %r14
    180029d5c:	push   %rcx
    180029d5d:	rex.XB push $0x40407261
    180029d63:	rex pop %rdx
-   180029d65:	add    %ah,%al
+   180029d65:	add    %ah,%cl
    180029d67:	(bad)
    180029d69:	imul   $0x7974706d,0x45(%rbx),%esi
    180029d70:	rex push %rcx
    180029d72:	push   %rbp
    180029d73:	jb     0x180029de1
    180029d75:	rex
    180029d76:	rex push %rcx
@@ -62186,20 +62177,17 @@
    180029db1:	push   %rbx
    180029db2:	je     0x180029e26
    180029db4:	imul   $0x45414040,0x67(%rsi),%ebp
    180029dbb:	rex.X push %rsi
    180029dbd:	xor    0x31(%rax),%al
    180029dc0:	rex pop %rdx
    180029dc2:	add    %al,(%rax)
-   180029dc4:	sub    $0x69643f0c,%eax
-   180029dc9:	jae    0x180029e2e
-   180029dcb:	outsl  %ds:(%rsi),(%dx)
-   180029dcc:	outsb  %ds:(%rsi),(%dx)
-   180029dcd:	outsb  %ds:(%rsi),(%dx)
-   180029dce:	movsxd %gs:0x51(%rax,%rax,2),%esi
+   180029dc4:	cs or  $0x3f,%al
+   180029dc7:	imul   $0x656e6e6f,%fs:0x63(%rbx),%esi
+   180029dcf:	movsxd 0x51(%rax,%rax,2),%esi
    180029dd3:	rex.WRXB (bad)
    180029dd5:	push   $0x65
    180029dd7:	movsxd 0x40(%rax,%rax,2),%esi
    180029ddb:	push   %rbx
    180029ddc:	pop    %r15
    180029dde:	rex.WRX
    180029ddf:	rex.B
@@ -62213,15 +62201,15 @@
    180029ded:	rex push %rcx
    180029def:	rex.WRB
    180029df0:	gs je  0x180029e54
    180029df3:	rex.WRXB (bad)
    180029df5:	push   $0x65
    180029df7:	movsxd 0x40(%rax,%rax,2),%esi
    180029dfb:	rex pop %rdx
-   180029dfd:	add    %dh,%dh
+   180029dfd:	add    %dh,%bh
    180029dff:	or     (%rdi),%edi
    180029e01:	fs gs insb (%dx),%es:(%rdi)
    180029e04:	gs je  0x180029e6c
    180029e07:	rex.WR (bad)
    180029e09:	je     0x180029e70
    180029e0b:	jb     0x180029e4d
    180029e0d:	push   %rcx
@@ -62350,16 +62338,16 @@
    180029ee5:	je     0x180029f4c
    180029ee7:	push   %rsp
    180029ee8:	imul   $0x45514040,0x65(%rbp),%ebp
    180029eef:	rex.X
    180029ef0:	pop    %r15
    180029ef2:	rex.WX pop %rax
    180029ef4:	pop    %rdx
-   180029ef5:	add    %cl,(%rbx)
-   180029ef7:	or     (%rdi),%edi
+   180029ef5:	add    %cl,(%rbx,%rcx,1)
+   180029ef8:	(bad)
    180029ef9:	movsxd 0x72(%rbp),%esi
    180029efc:	jb     0x180029f63
    180029efe:	outsb  %ds:(%rsi),(%dx)
    180029eff:	je     0x180029f45
    180029f01:	(bad)
    180029f02:	je     0x180029f69
    180029f04:	push   %rsp
@@ -62370,15 +62358,15 @@
    180029f11:	push   %rsp
    180029f12:	imul   $0x41534040,0x65(%rbp),%ebp
    180029f19:	(bad)
    180029f1a:	push   %r14
    180029f1c:	xor    %eax,0x58(%rax)
    180029f1f:	pop    %rdx
    180029f20:	add    %al,(%rax)
-   180029f22:	cmp    %cl,(%rsi)
+   180029f22:	cmp    %ecx,(%rsi)
    180029f24:	(bad)
    180029f25:	addr32 gs je 0x180029f69
    180029f29:	push   %rcx
    180029f2a:	rex.WRXB (bad)
    180029f2c:	push   $0x65
    180029f2e:	movsxd 0x72(%rax,%rdx,2),%esi
    180029f32:	imul   $0x40406574,0x61(%rsi),%esi
@@ -62391,15 +62379,15 @@
    180029f43:	push   %r14
    180029f45:	push   %rcx
    180029f46:	rex.WRXB (bad)
    180029f48:	push   $0x65
    180029f4a:	movsxd 0x40(%rax,%rax,2),%esi
    180029f4e:	rex pop %rdx
    180029f50:	add    %al,(%rax)
-   180029f52:	jno    0x180029f69
+   180029f52:	jb     0x180029f69
    180029f54:	(bad)
    180029f55:	jno    0x180029fcc
    180029f57:	gs jb  0x180029fd3
    180029f5a:	rex.WB je 0x180029fc2
    180029f5d:	insl   (%dx),%es:(%rdi)
    180029f5e:	jae    0x180029fa0
    180029f60:	push   %rcx
@@ -62453,15 +62441,15 @@
    180029fbe:	push   %rbp
    180029fbf:	jb     0x18002a02d
    180029fc1:	rex
    180029fc2:	rex
    180029fc3:	rex
    180029fc4:	rex
    180029fc5:	rex pop %rdx
-   180029fc7:	add    %bh,%ch
+   180029fc7:	add    %bh,%dh
    180029fc9:	or     (%rdi),%bh
    180029fcb:	movsxd 0x69(%rdx),%esi
    180029fce:	je     0x18002a039
    180029fd0:	movsxd 0x6c(%rcx),%esp
    180029fd3:	rex push %rcx
    180029fd5:	rex.WRB
    180029fd6:	gs jae 0x18002a04c
@@ -62514,44 +62502,44 @@
    18002a036:	rex.RB
    18002a037:	push   %r14
    18002a039:	xor    %al,0x41(%rax)
    18002a03c:	rex.RB
    18002a03d:	rex.X push %rsi
    18002a03f:	xor    %al,0x40(%rax)
    18002a042:	pop    %rdx
-   18002a043:	add    %cl,%bh
+   18002a043:	add    %dl,%al
    18002a045:	(bad)
    18002a047:	imul   $0x7974706d,0x45(%rbx),%esi
    18002a04e:	rex push %rcx
    18002a050:	rex.X jns 0x18002a0c7
    18002a053:	gs rex.B jb 0x18002a0c9
    18002a057:	(bad)
    18002a058:	jns    0x18002a09a
    18002a05a:	rex push %rcx
    18002a05c:	rex.RB
    18002a05d:	rex.X
    18002a05e:	pop    %r15
    18002a060:	rex.WRX pop %rax
    18002a062:	pop    %rdx
-   18002a063:	add    %dl,0x65723f16(%rdi)
+   18002a063:	add    %bl,0x65723f16(%rax)
    18002a069:	jae    0x18002a0d4
    18002a06b:	jp     0x18002a0d2
    18002a06d:	rex push %rcx
    18002a06f:	rex.X jns 0x18002a0e6
    18002a072:	gs rex.B jb 0x18002a0e8
    18002a076:	(bad)
    18002a077:	jns    0x18002a0b9
    18002a079:	rex push %rcx
    18002a07b:	rex.RB
    18002a07c:	rex.B
    18002a07d:	pop    %r8
    18002a07f:	pop    %rdi
    18002a080:	rex.WX
    18002a081:	rex pop %rdx
-   18002a083:	add    %dh,(%rsi)
+   18002a083:	add    %dh,(%rdi)
    18002a085:	or     %edi,(%rdi)
    18002a087:	movsxd 0x70(%rcx),%esp
    18002a08a:	(bad)
    18002a08b:	movsxd 0x74(%rcx),%ebp
    18002a08e:	jns    0x18002a0d0
    18002a090:	push   %rcx
    18002a091:	rex.X jns 0x18002a108
@@ -62561,15 +62549,15 @@
    18002a09b:	rex push %rcx
    18002a09d:	rex.RB
    18002a09e:	rex.X
    18002a09f:	pop    %r15
    18002a0a1:	rex.WX pop %rax
    18002a0a3:	pop    %rdx
    18002a0a4:	add    %al,(%rax)
-   18002a0a6:	cltd
+   18002a0a6:	(bad)
    18002a0a7:	or     (%rdi),%edi
    18002a0a9:	fs (bad)
    18002a0ab:	je     0x18002a10e
    18002a0ad:	rex push %rcx
    18002a0af:	rex.X jns 0x18002a126
    18002a0b2:	gs rex.B jb 0x18002a128
    18002a0b6:	(bad)
@@ -62579,30 +62567,29 @@
    18002a0bc:	rex.B
    18002a0bd:	push   %r8
    18002a0bf:	rex.RB
    18002a0c0:	rex.B
    18002a0c1:	rex.R pop %rax
    18002a0c3:	pop    %rdx
    18002a0c4:	add    %al,(%rax)
-   18002a0c6:	(bad)
-   18002a0c7:	or     $0x3f,%al
+   18002a0c6:	or     %cl,(%rdi,%rdi,1)
    18002a0c9:	fs gs je 0x18002a12e
    18002a0cd:	movsxd 0x40(%rax),%ebp
    18002a0d0:	push   %rcx
    18002a0d1:	rex.X jns 0x18002a148
    18002a0d4:	gs rex.B jb 0x18002a14a
    18002a0d8:	(bad)
    18002a0d9:	jns    0x18002a11b
    18002a0db:	rex push %rcx
    18002a0dd:	rex.RB
    18002a0de:	rex.B
    18002a0df:	pop    %r8
    18002a0e1:	pop    %rax
    18002a0e2:	pop    %rdx
-   18002a0e3:	add    %bh,%dh
+   18002a0e3:	add    %bh,%bh
    18002a0e5:	(bad)
    18002a0e6:	(bad)
    18002a0e7:	(bad)
    18002a0e8:	jo     0x18002a15a
    18002a0ea:	outsb  %gs:(%rsi),(%dx)
    18002a0ec:	fs rex push %rcx
    18002a0ef:	rex.X jns 0x18002a166
@@ -62618,15 +62605,15 @@
    18002a100:	push   %r14
    18002a102:	xor    %eax,0x41(%rax)
    18002a105:	rex.RB
    18002a106:	rex.X push %rsi
    18002a108:	xor    %eax,0x40(%rax)
    18002a10b:	pop    %rdx
    18002a10c:	add    %al,(%rax)
-   18002a10e:	jl     0x18002a11c
+   18002a10e:	jge    0x18002a11c
    18002a110:	(bad)
    18002a111:	outsb  %gs:(%rsi),(%dx)
    18002a113:	fs rex push %rcx
    18002a116:	rex.X jns 0x18002a18d
    18002a119:	gs rex.B jb 0x18002a18f
    18002a11d:	(bad)
    18002a11e:	jns    0x18002a160
@@ -62634,15 +62621,15 @@
    18002a122:	rex.RB
    18002a123:	rex.X
    18002a124:	push   %r8
    18002a126:	rex.RB
    18002a127:	rex.X
    18002a128:	rex.R pop %rax
    18002a12a:	pop    %rdx
-   18002a12b:	add    %ch,0x16(%rsi)
+   18002a12b:	add    %ch,0x16(%rdi)
    18002a12e:	(bad)
    18002a12f:	jb     0x18002a196
    18002a131:	jo     0x18002a19f
    18002a133:	(bad)
    18002a134:	movsxd 0x40(%rbp),%esp
    18002a137:	push   %rcx
    18002a138:	push   %rbx
@@ -62665,15 +62652,15 @@
    18002a15e:	je     0x18002a1c9
    18002a160:	jbe    0x18002a1cb
    18002a162:	je     0x18002a1dd
    18002a164:	rex push %rcx
    18002a166:	je     0x18002a1a8
    18002a168:	rex
    18002a169:	rex pop %rdx
-   18002a16b:	add    %ah,%ah
+   18002a16b:	add    %ah,%ch
    18002a16d:	or     $0x6f72663f,%eax
    18002a172:	insl   (%dx),%es:(%rdi)
    18002a173:	rex.WR (bad)
    18002a175:	je     0x18002a1e0
    18002a177:	outsb  %ds:(%rsi),(%dx)
    18002a178:	xor    %eax,0x51(%rax)
    18002a17b:	push   %rbx
@@ -62740,17 +62727,17 @@
    18002a1fe:	imul   $0x6974704f,0x67(%rsi),%ebp
    18002a205:	outsl  %ds:(%rsi),(%dx)
    18002a206:	outsb  %ds:(%rsi),(%dx)
    18002a207:	rex xor 0x40(%rax),%al
    18002a20b:	rex
    18002a20c:	rex pop %rdx
    18002a20e:	add    %al,(%rax)
-   18002a210:	test   $0x73693f0f,%eax
-   18002a215:	rex.XB jb 0x18002a281
-   18002a218:	je     0x18002a283
+   18002a210:	stos   %al,%es:(%rdi)
+   18002a211:	(bad)
+   18002a213:	imul   $0x69746972,0x43(%rbx),%esi
    18002a21a:	movsxd 0x6c(%rcx),%esp
    18002a21d:	rex.RB outsb %ds:(%rsi),(%dx)
    18002a21f:	(bad)
    18002a220:	(bad)
    18002a221:	insb   (%dx),%es:(%rdi)
    18002a222:	gs fs rex push %rcx
    18002a226:	rex.WR outsl %ds:(%rsi),(%dx)
@@ -62760,15 +62747,15 @@
    18002a235:	rex
    18002a236:	rex push %rcx
    18002a238:	rex.RB
    18002a239:	rex.X
    18002a23a:	pop    %r15
    18002a23c:	rex.WRX pop %rax
    18002a23e:	pop    %rdx
-   18002a23f:	add    %ah,0x61683f0e(%rcx)
+   18002a23f:	add    %ah,0x61683f0e(%rdx)
    18002a245:	jae    0x18002a2af
    18002a247:	rex push %rcx
    18002a249:	rex.WRB
    18002a24a:	gs jae 0x18002a2c0
    18002a24d:	(bad)
    18002a24e:	addr32 gs rex.B jne 0x18002a2c7
    18002a253:	push   $0x69746e65
@@ -62801,15 +62788,15 @@
    18002a28e:	outsl  %ds:(%rsi),(%dx)
    18002a28f:	addr32 jb 0x18002a2f3
    18002a292:	jo     0x18002a2fc
    18002a294:	imul   $0x40687361,0x48(%rbx),%esp
    18002a29b:	rex
    18002a29c:	rex pop %rdx
    18002a29e:	add    %al,(%rax)
-   18002a2a0:	fisttpll (%rbx)
+   18002a2a0:	fimuls (%rbx)
    18002a2a2:	(bad)
    18002a2a3:	(bad)
    18002a2aa:	rex.WRB
    18002a2ab:	gs jae 0x18002a321
    18002a2ae:	(bad)
    18002a2af:	rex.WR outsl %gs:(%esi),(%dx)
    18002a2b3:	addr32 addr32 gs jb 0x18002a2f8
@@ -62842,15 +62829,15 @@
    18002a2e7:	rex.X jns 0x18002a35e
    18002a2ea:	gs rex.B jb 0x18002a360
    18002a2ee:	(bad)
    18002a2ef:	jns    0x18002a331
    18002a2f1:	rex pop %rax
    18002a2f3:	pop    %rdx
    18002a2f4:	add    %al,(%rax)
-   18002a2f6:	sbb    %dl,(%rcx)
+   18002a2f6:	sbb    %edx,(%rcx)
    18002a2f8:	(bad)
    18002a2f9:	imul   $0x64696c61,0x56(%rbx),%esi
    18002a300:	rex push %rcx
    18002a302:	push   %rsi
    18002a303:	(bad)
    18002a304:	jb     0x18002a36f
    18002a306:	(bad)
@@ -62879,15 +62866,15 @@
    18002a329:	rex.X
    18002a32a:	rex.B
    18002a32b:	rex.W push %rax
    18002a32d:	rex.RB
    18002a32e:	pop    %r15
    18002a330:	rex.WRX
    18002a331:	rex pop %rdx
-   18002a333:	add    %cl,%dl
+   18002a333:	add    %cl,%bl
    18002a335:	(bad)
    18002a336:	(bad)
    18002a337:	(bad)
    18002a338:	fs fs push %rbx
    18002a33b:	movsxd %gs:0x40(%rbx),%esi
    18002a33f:	push   %rcx
    18002a340:	rex.R (bad)
@@ -62896,15 +62883,15 @@
    18002a345:	imul   $0x45514040,0x65(%rbp),%ebp
    18002a34c:	rex.X
    18002a34d:	rex.B (bad)
    18002a34f:	push   %r14
    18002a351:	xor    %eax,0x5f(%rax)
    18002a354:	rex.WX
    18002a355:	rex pop %rdx
-   18002a357:	add    %cl,(%rsi)
+   18002a357:	add    %cl,(%rdi)
    18002a359:	(bad)
    18002a35a:	(bad)
    18002a35b:	jae    0x18002a3c2
    18002a35d:	movsxd 0x54(%rbx),%esi
    18002a360:	outsl  %ds:(%rsi),(%dx)
    18002a361:	rex push %rcx
    18002a363:	rex.R (bad)
@@ -62939,15 +62926,15 @@
    18002a394:	imul   $0x34574040,0x67(%rsi),%ebp
    18002a39b:	push   %rax
    18002a39c:	(bad)
    18002a39d:	jb     0x18002a412
    18002a39f:	imul   $0x65646f4d,0x67(%rsi),%ebp
    18002a3a6:	rex xor %al,0x40(%rax)
    18002a3aa:	pop    %rdx
-   18002a3ab:	add    %dh,0x73693f0f(%rdx)
+   18002a3ab:	add    %dh,0x73693f0f(%rbx)
    18002a3b1:	rex.R
    18002a3b2:	(bad)
    18002a3b8:	(bad)
    18002a3b9:	(bad)
    18002a3ba:	insb   (%dx),%es:(%rdi)
    18002a3bb:	gs fs rex push %rcx
    18002a3bf:	rex.WR outsl %ds:(%rsi),(%dx)
@@ -62982,15 +62969,15 @@
    18002a3f2:	xor    %al,0x24(%rax)
    18002a3f5:	and    $0x51,%al
    18002a3f7:	rex.RB
    18002a3f8:	push   %r14
    18002a3fa:	xor    %al,0x40(%rax)
    18002a3fd:	pop    %rdx
    18002a3fe:	add    %al,(%rax)
-   18002a400:	xchg   %eax,%edx
+   18002a400:	xchg   %eax,%ebx
    18002a401:	or     %edi,(%rdi)
    18002a403:	movsxd 0x61(%rbp,%riz,2),%ebp
    18002a407:	jb     0x18002a449
    18002a409:	push   %rcx
    18002a40a:	rex.X jns 0x18002a481
    18002a40d:	gs rex.B jb 0x18002a483
    18002a411:	(bad)
@@ -62998,15 +62985,15 @@
    18002a414:	rex push %rcx
    18002a416:	rex.RB
    18002a417:	rex.B
    18002a418:	pop    %r8
    18002a41a:	pop    %rax
    18002a41b:	pop    %rdx
    18002a41c:	add    %al,(%rax)
-   18002a41e:	push   %rax
+   18002a41e:	push   %rcx
    18002a41f:	or     %bh,(%rdi)
    18002a421:	(bad)
    18002a422:	je     0x18002a464
    18002a424:	push   %rcx
    18002a425:	rex.X jns 0x18002a49c
    18002a428:	gs rex.B jb 0x18002a49e
    18002a42c:	(bad)
@@ -63014,15 +63001,15 @@
    18002a42f:	rex push %rcx
    18002a431:	rex.RB
    18002a432:	rex.X
    18002a433:	rex.B
    18002a434:	rex.R pop %rdi
    18002a436:	rex.WX
    18002a437:	rex pop %rdx
-   18002a439:	add    %bl,%dl
+   18002a439:	add    %bl,%bl
    18002a43b:	(bad)
    18002a43c:	(bad)
    18002a43d:	imul   $0x664f7865,0x64(%rsi),%ebp
    18002a444:	rex push %rcx
    18002a446:	rex.X jns 0x18002a4bd
    18002a449:	gs rex.B jb 0x18002a4bf
    18002a44d:	(bad)
@@ -63032,28 +63019,28 @@
    18002a453:	rex.X
    18002a454:	pop    %r15
    18002a456:	rex.WX
    18002a457:	rex.R pop %rdi
    18002a459:	rex.WX
    18002a45a:	rex pop %rdx
    18002a45c:	add    %al,(%rax)
-   18002a45e:	adc    %gs:(%rdi),%bh
+   18002a45e:	data16 adc (%rdi),%bh
    18002a461:	insl   (%dx),%es:(%rdi)
    18002a462:	imul   $0x65747942,0x51(%rax,%rax,2),%esp
    18002a46a:	rex.B jb 0x18002a4df
    18002a46d:	(bad)
    18002a46e:	jns    0x18002a4b0
    18002a470:	rex push %rcx
    18002a472:	rex.RB
    18002a473:	rex.X
    18002a474:	rex.B (bad)
    18002a476:	push   %r14
    18002a478:	xor    %eax,0x5f(%rax)
    18002a47b:	rex.WX xor %al,0x5a(%rax)
-   18002a47f:	add    %ch,0x74733f19(%rdi)
+   18002a47f:	add    %dh,0x74733f19(%rax)
    18002a485:	(bad)
    18002a486:	jb     0x18002a4fc
    18002a488:	jae    0x18002a4e1
    18002a48a:	imul   $0x74794251,0x40(%rax,%rbp,2),%esi
    18002a492:	gs rex.B jb 0x18002a508
    18002a496:	(bad)
    18002a497:	jns    0x18002a4d9
@@ -63064,15 +63051,15 @@
    18002a49f:	rex.WRX push %rsi
    18002a4a1:	push   %rcx
    18002a4a2:	rex.X jns 0x18002a519
    18002a4a5:	gs rex.B jb 0x18002a51b
    18002a4a9:	(bad)
    18002a4aa:	jns    0x18002a502
    18002a4ac:	imul   $0x5a404040,0x77(%rbp),%esp
-   18002a4b3:	add    %ah,0x6e653f0c(%rax)
+   18002a4b3:	add    %ah,0x6e653f0c(%rcx)
    18002a4b9:	fs jae 0x18002a513
    18002a4bc:	imul   $0x74794251,0x40(%rax,%rbp,2),%esi
    18002a4c4:	gs rex.B jb 0x18002a53a
    18002a4c8:	(bad)
    18002a4c9:	jns    0x18002a50b
    18002a4cb:	rex push %rcx
    18002a4cd:	rex.RB
@@ -63081,15 +63068,15 @@
    18002a4d1:	rex.WRX push %rsi
    18002a4d3:	push   %rcx
    18002a4d4:	rex.X jns 0x18002a54b
    18002a4d7:	gs rex.B jb 0x18002a54d
    18002a4db:	(bad)
    18002a4dc:	jns    0x18002a534
    18002a4de:	imul   $0x5a404040,0x77(%rbp),%esp
-   18002a4e5:	add    %bh,0x9(%rbp)
+   18002a4e5:	add    %bh,0x9(%rsi)
    18002a4e8:	(bad)
    18002a4e9:	movsxd 0x6f(%rax),%ebp
    18002a4ec:	jo     0x18002a52e
    18002a4ee:	push   %rcx
    18002a4ef:	rex.X jns 0x18002a566
    18002a4f2:	gs rex.B jb 0x18002a568
    18002a4f6:	(bad)
@@ -63113,15 +63100,15 @@
    18002a51c:	rex.RB
    18002a51d:	rex.W
    18002a51e:	rex.B
    18002a51f:	rex.B (bad)
    18002a521:	push   %r14
    18002a523:	xor    %eax,0x58(%rax)
    18002a526:	pop    %rdx
-   18002a527:	add    %dh,(%rsi)
+   18002a527:	add    %dh,(%rdi)
    18002a529:	adc    (%rdi),%edi
    18002a52b:	outsb  %ds:(%rsi),(%dx)
    18002a52c:	jne    0x18002a59b
    18002a52e:	(bad)
    18002a530:	jb     0x18002a572
    18002a532:	push   %rcx
    18002a533:	rex.X jns 0x18002a5aa
@@ -63161,15 +63148,15 @@
    18002a572:	je     0x18002a5d5
    18002a574:	push   %rax
    18002a575:	outsl  %ds:(%rsi),(%dx)
    18002a576:	imul   $0x44407265,0x74(%rsi),%ebp
    18002a57d:	rex
    18002a57e:	rex
    18002a57f:	rex pop %rdx
-   18002a581:	add    %bh,(%rax)
+   18002a581:	add    %bh,(%rcx)
    18002a583:	or     %bh,(%rdi)
    18002a585:	(bad)
    18002a586:	jb     0x18002a5ef
    18002a588:	rex push %rcx
    18002a58a:	push   %rbx
    18002a58b:	je     0x18002a5ff
    18002a58d:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -63179,26 +63166,26 @@
    18002a599:	xor    %eax,0x47(%rax)
    18002a59c:	rex.W
    18002a59d:	rex.W push %rsi
    18002a59f:	push   %rcx
    18002a5a0:	rex.XB push $0x40407261
    18002a5a6:	rex pop %rdx
    18002a5a8:	add    %al,(%rax)
-   18002a5aa:	push   $0x696d3f12
-   18002a5af:	fs rex push %rcx
+   18002a5aa:	imul   $0x64696d3f,(%rdx),%edx
+   18002a5b0:	rex push %rcx
    18002a5b2:	push   %rbx
    18002a5b3:	je     0x18002a627
    18002a5b5:	imul   $0x45514040,0x67(%rsi),%ebp
    18002a5bc:	rex.X
    18002a5bd:	rex.B (bad)
    18002a5bf:	push   %r14
    18002a5c1:	xor    %eax,0x5f(%rax)
    18002a5c4:	rex.WX xor %al,0x5a(%rax)
    18002a5c8:	add    %al,(%rax)
-   18002a5ca:	mov    $0x19,%bl
+   18002a5ca:	mov    $0x19,%ah
    18002a5cc:	(bad)
    18002a5cd:	jae    0x18002a643
    18002a5cf:	(bad)
    18002a5d0:	jb     0x18002a646
    18002a5d2:	jae    0x18002a62b
    18002a5d4:	imul   $0x72745351,0x40(%rax,%rbp,2),%esi
    18002a5dc:	imul   $0x45514040,0x67(%rsi),%ebp
@@ -63217,15 +63204,15 @@
    18002a5fa:	je     0x18002a665
    18002a5fc:	jbe    0x18002a667
    18002a5fe:	je     0x18002a679
    18002a600:	rex push %rcx
    18002a602:	je     0x18002a644
    18002a604:	rex
    18002a605:	rex pop %rdx
-   18002a607:	add    %bh,(%rax)
+   18002a607:	add    %bh,(%rcx)
    18002a609:	adc    (%rdi),%edi
    18002a60b:	outsb  %ds:(%rsi),(%dx)
    18002a60c:	jne    0x18002a67b
    18002a60e:	(bad)
    18002a610:	jb     0x18002a652
    18002a612:	push   %rcx
    18002a613:	push   %rbx
@@ -63254,16 +63241,16 @@
    18002a64b:	outsl  %ds:(%rsi),(%dx)
    18002a64c:	outsb  %ds:(%rsi),(%dx)
    18002a64d:	rex push %rcx
    18002a64f:	je     0x18002a691
    18002a651:	rex
    18002a652:	rex pop %rdx
    18002a654:	add    %al,(%rax)
-   18002a656:	xlat   %ds:(%rbx)
-   18002a657:	sbb    %bh,(%rdi)
+   18002a656:	fcomps (%rax)
+   18002a658:	(bad)
    18002a659:	jae    0x18002a6c0
    18002a65b:	je     0x18002a6b2
    18002a65d:	jb     0x18002a6cb
    18002a65f:	rex push %rcx
    18002a661:	push   %rbp
    18002a662:	jb     0x18002a6d0
    18002a664:	rex
@@ -63281,30 +63268,32 @@
    18002a67a:	push   %rax
    18002a67b:	(bad)
    18002a67c:	jb     0x18002a6f1
    18002a67e:	imul   $0x65646f4d,0x67(%rsi),%ebp
    18002a685:	rex xor %eax,0x40(%rax)
    18002a689:	pop    %rdx
    18002a68a:	add    %al,(%rax)
-   18002a68c:	(bad)
-   18002a68d:	adc    %edi,(%rdi)
+   18002a68c:	sbb    %dl,(%rcx)
+   18002a68e:	(bad)
    18002a68f:	imul   $0x64696c61,0x56(%rbx),%esi
    18002a696:	rex push %rcx
    18002a698:	push   %rbp
    18002a699:	jb     0x18002a707
    18002a69b:	rex
    18002a69c:	rex push %rcx
    18002a69e:	rex.RB
    18002a69f:	rex.X
    18002a6a0:	pop    %r15
    18002a6a2:	rex.WRX pop %rax
    18002a6a4:	pop    %rdx
-   18002a6a5:	add    %dl,0x7461703f(%rbx,%rdx,1)
-   18002a6ac:	push   $0x72555140
-   18002a6b1:	insb   (%dx),%es:(%rdi)
+   18002a6a5:	add    %dl,0x61703f13(%rbp)
+   18002a6ab:	je     0x18002a715
+   18002a6ad:	rex push %rcx
+   18002a6af:	push   %rbp
+   18002a6b0:	jb     0x18002a71e
    18002a6b2:	rex
    18002a6b3:	rex push %rcx
    18002a6b5:	rex.RB
    18002a6b6:	rex.X
    18002a6b7:	rex.B (bad)
    18002a6b9:	push   %r14
    18002a6bb:	push   %rcx
@@ -63374,16 +63363,15 @@
    18002a73b:	rex.X jns 0x18002a7b2
    18002a73e:	gs rex.B jb 0x18002a7b4
    18002a742:	(bad)
    18002a743:	jns    0x18002a785
    18002a745:	rex
    18002a746:	rex pop %rdx
    18002a748:	add    %al,(%rax)
-   18002a74a:	(bad)
-   18002a74b:	(bad)
+   18002a74a:	rex (bad)
    18002a74c:	(bad)
    18002a74d:	addr32 gs je 0x18002a794
    18002a751:	push   $0x51407261
    18002a756:	rex.WB
    18002a757:	rex.WRXB
    18002a758:	rex.R
    18002a759:	gs jbe 0x18002a7c5
@@ -63394,15 +63382,15 @@
    18002a763:	pop    %r15
    18002a765:	rex.WRX push %rax
    18002a767:	rex.RB
    18002a768:	rex.B
    18002a769:	rex.R
    18002a76a:	rex pop %rdx
    18002a76c:	add    %al,(%rax)
-   18002a76e:	mov    $0x65723f15,%ecx
+   18002a76e:	mov    $0x65723f15,%edx
    18002a773:	(bad)
    18002a774:	fs jns 0x18002a7c9
    18002a777:	gs (bad)
    18002a779:	fs rex push %rcx
    18002a77c:	rex.WB
    18002a77d:	rex.WRXB
    18002a77e:	rex.R
@@ -63410,15 +63398,15 @@
    18002a782:	movsxd 0x40(%rbp),%esp
    18002a785:	rex push %rcx
    18002a787:	rex.RB
    18002a788:	rex.B
    18002a789:	pop    %r8
    18002a78b:	pop    %rax
    18002a78c:	pop    %rdx
-   18002a78d:	add    %ch,(%rsi)
+   18002a78d:	add    %ch,(%rdi)
    18002a78f:	or     %bh,(%rdi)
    18002a791:	(bad)
    18002a792:	jo     0x18002a804
    18002a794:	insb   (%dx),%es:(%rdi)
    18002a795:	imul   $0x6e6f6974,0x61(%rbx),%esp
    18002a79c:	rex.WRX (bad)
    18002a79e:	insl   (%dx),%es:(%rdi)
@@ -63432,15 +63420,15 @@
    18002a7b2:	rex push %rbx
    18002a7b4:	rex.B (bad)
    18002a7b6:	push   %r14
    18002a7b8:	push   %rcx
    18002a7b9:	push   %rbx
    18002a7ba:	je     0x18002a82e
    18002a7bc:	imul   $0x5a584040,0x67(%rsi),%ebp
-   18002a7c3:	add    %al,0xf(%rsi)
+   18002a7c3:	add    %al,0xf(%rdi)
    18002a7c6:	(bad)
    18002a7c7:	imul   $0x636e6174,0x73(%rsi),%ebp
    18002a7ce:	gs rex push %rcx
    18002a7d1:	rex.XB outsl %ds:(%rsi),(%dx)
    18002a7d3:	jb     0x18002a83a
    18002a7d5:	rex.B jo 0x18002a848
    18002a7d8:	insb   (%dx),%es:(%rdi)
@@ -63470,15 +63458,15 @@
    18002a809:	movsxd 0x40(%rbp),%esp
    18002a80c:	rex xor 0x51(%rbp),%dl
    18002a810:	rex.WRB
    18002a811:	gs je  0x18002a875
    18002a814:	rex.WRXB (bad)
    18002a816:	push   $0x65
    18002a818:	movsxd 0x40(%rax,%rax,2),%esi
-   18002a81c:	rex.X add %dl,0x10(%rsi)
+   18002a81c:	rex.X add %dl,0x10(%rdi)
    18002a820:	(bad)
    18002a821:	imul   $0x406c6c75,0x4e(%rbx),%esi
    18002a828:	push   %rcx
    18002a829:	push   %rsi
    18002a82a:	(bad)
    18002a82b:	jb     0x18002a896
    18002a82d:	(bad)
@@ -63542,31 +63530,31 @@
    18002a892:	outsb  %ds:(%rsi),(%dx)
    18002a893:	je     0x18002a8d5
    18002a895:	rex
    18002a896:	rex
    18002a897:	rex pop %rax
    18002a899:	pop    %rdx
    18002a89a:	add    %al,(%rax)
-   18002a89c:	xlat   %ds:(%rbx)
-   18002a89d:	(bad)
+   18002a89c:	fmuls  (%rdi)
+   18002a89e:	(bad)
    18002a89f:	imul   $0x7974706d,0x45(%rbx),%esi
    18002a8a6:	rex push %rcx
    18002a8a8:	rex.WX jae 0x18002a91a
    18002a8ab:	outsb  %ds:(%rsi),(%dx)
    18002a8ac:	rex.WRXB (bad)
    18002a8ae:	push   $0x65
    18002a8b0:	movsxd 0x40(%rax,%rax,2),%esi
    18002a8b4:	push   %rcx
    18002a8b5:	rex.RB
    18002a8b6:	rex.X
    18002a8b7:	pop    %r15
    18002a8b9:	rex.WRX pop %rax
    18002a8bb:	pop    %rdx
    18002a8bc:	add    %al,(%rax)
-   18002a8be:	fisttpl 0x6f72663f(%rip)        # 0x1ef750f03
+   18002a8be:	fmull  0x6f72663f(%rip)        # 0x1ef750f03
    18002a8c4:	insl   (%dx),%es:(%rdi)
    18002a8c5:	rex.WX jae 0x18002a937
    18002a8c8:	outsb  %ds:(%rsi),(%dx)
    18002a8c9:	rex push %rcx
    18002a8cb:	rex.WX jae 0x18002a93d
    18002a8ce:	outsb  %ds:(%rsi),(%dx)
    18002a8cf:	rex.R outsl %ds:(%rsi),(%dx)
@@ -63594,15 +63582,15 @@
    18002a8fa:	(bad)
    18002a8fb:	jb     0x18002a970
    18002a8fd:	gs rex.RB jb 0x18002a973
    18002a901:	outsl  %ds:(%rsi),(%dx)
    18002a902:	jb     0x18002a944
    18002a904:	rex
    18002a905:	rex pop %rdx
-   18002a907:	add    %bl,0x10(%rdx)
+   18002a907:	add    %bl,0x10(%rbx)
    18002a90a:	(bad)
    18002a90b:	imul   $0x63656a62,0x4f(%rbx),%esi
    18002a912:	je     0x18002a954
    18002a914:	push   %rcx
    18002a915:	rex.WX jae 0x18002a987
    18002a918:	outsb  %ds:(%rsi),(%dx)
    18002a919:	rex.R outsl %ds:(%rsi),(%dx)
@@ -63611,15 +63599,15 @@
    18002a920:	je     0x18002a962
    18002a922:	rex push %rcx
    18002a924:	rex.RB
    18002a925:	rex.X
    18002a926:	pop    %r15
    18002a928:	rex.WRX pop %rax
    18002a92a:	pop    %rdx
-   18002a92b:	add    %al,0x13(%rdx)
+   18002a92b:	add    %al,0x13(%rbx)
    18002a92e:	(bad)
    18002a92f:	outsl  %ds:(%rsi),(%dx)
    18002a930:	(bad)
    18002a931:	push   $0x65
    18002a933:	movsxd 0x51(%rax,%rax,2),%esi
    18002a937:	rex.WX jae 0x18002a9a9
    18002a93a:	outsb  %ds:(%rsi),(%dx)
@@ -63636,15 +63624,15 @@
    18002a94d:	rex.WX jae 0x18002a9bf
    18002a950:	outsb  %ds:(%rsi),(%dx)
    18002a951:	rex.WRXB (bad)
    18002a953:	push   $0x65
    18002a955:	movsxd 0x40(%rax,%rax,2),%esi
    18002a959:	pop    %rax
    18002a95a:	pop    %rdx
-   18002a95b:	add    %dl,0x65723f15(%rbp)
+   18002a95b:	add    %dl,0x65723f15(%rsi)
    18002a961:	(bad)
    18002a962:	fs rex.B insb (%dx),%es:(%rdi)
    18002a965:	insb   (%dx),%es:(%rdi)
    18002a966:	rex push %rcx
    18002a968:	rex.WB
    18002a969:	rex.WRXB
    18002a96a:	rex.R
@@ -63658,15 +63646,15 @@
    18002a979:	push   %rcx
    18002a97a:	rex.X jns 0x18002a9f1
    18002a97d:	gs rex.B jb 0x18002a9f3
    18002a981:	(bad)
    18002a982:	jns    0x18002a9c4
    18002a984:	rex pop %rax
    18002a986:	pop    %rdx
-   18002a987:	add    %ch,%cl
+   18002a987:	add    %ch,%dl
    18002a989:	or     $0x3f,%al
    18002a98b:	gs jb  0x18002aa00
    18002a98e:	outsl  %ds:(%rsi),(%dx)
    18002a98f:	jb     0x18002a9e4
    18002a991:	je     0x18002aa05
    18002a993:	imul   $0x4f495140,0x67(%rsi),%ebp
    18002a99a:	rex.R
@@ -64519,31 +64507,31 @@
    18002b548:	or     $0x8,%al
    18002b54a:	add    %al,(%rax)
    18002b54c:	add    %al,(%rax)
    18002b54e:	add    %al,(%rax)
    18002b550:	add    %bl,0x0(%rbx)
    18002b553:	addb   $0x0,(%rcx)
    18002b556:	add    %al,(%rax)
-   18002b558:	jo     0x18002b532
-   18002b55a:	add    %eax,0x1(%rax)
+   18002b558:	push   $0x18001df
 	...
-   18002b5a8:	adc    %bl,0x0(%rbx)
-   18002b5ab:	addb   $0x0,(%rcx)
-   18002b5ae:	add    %al,(%rax)
+   18002b5a5:	add    %al,(%rax)
+   18002b5a7:	add    %dl,(%rax)
+   18002b5a9:	pop    %rbx
+   18002b5aa:	add    %al,0x1(%rax)
    18002b5b0:	add    %eax,(%rax)
    18002b5b2:	or     %al,(%rax)
    18002b5b4:	or     %al,(%rax)
    18002b5b6:	add    %al,(%rax)
    18002b5b8:	(bad)
    18002b5b9:	rolb   $0x0,(%rax)
    18002b5bc:	adc    %al,(%rax)
 	...
    18002b5c6:	add    %al,(%rax)
-   18002b5c8:	cwtl
-   18002b5c9:	fadds  (%rcx)
+   18002b5c8:	nop
+   18002b5c9:	filds  (%rcx)
    18002b5cb:	addb   $0x0,(%rcx)
    18002b5ce:	add    %al,(%rax)
    18002b5d0:	nop
    18002b5d1:	pop    %rbx
    18002b5d2:	add    %al,0x1(%rax)
    18002b5d8:	movabs 0xb00000000180005b,%al
    18002b5e1:	pop    %rbx
@@ -64572,45 +64560,46 @@
    18002b628:	add    %eax,%eax
    18002b62a:	add    %al,(%rax)
    18002b62c:	add    %al,(%rax)
    18002b62e:	add    %al,(%rax)
    18002b630:	rcrb   0x0(%rbx)
    18002b633:	addb   $0x0,(%rcx)
    18002b636:	add    %al,(%rax)
-   18002b638:	test   $0xd8,%al
-   18002b63a:	add    %eax,0x1(%rax)
+   18002b638:	movabs 0x18001df,%al
 	...
-   18002b658:	xor    %ah,(%rdx)
-   18002b65a:	add    %al,0x1(%rax)
+   18002b655:	add    %al,(%rax)
+   18002b657:	add    %dh,(%rax)
+   18002b659:	and    (%rax),%al
+   18002b65b:	addb   $0x0,(%rcx)
 	...
+   18002b68e:	add    %al,(%rax)
    18002b690:	add    %eax,(%rax)
    18002b692:	or     %al,(%rax)
    18002b694:	or     %al,(%rax)
    18002b696:	add    %al,(%rax)
    18002b698:	or     $0x8,%al
    18002b69a:	add    %al,(%rax)
    18002b69c:	add    %al,(%rax)
    18002b69e:	add    %al,(%rax)
    18002b6a0:	loopne 0x18002b6fd
    18002b6a2:	add    %al,0x1(%rax)
-   18002b6a8:	mov    $0x18001d8,%eax
+   18002b6a8:	mov    $0xdf,%al
+   18002b6aa:	add    %eax,0x1(%rax)
 	...
-   18002b6f5:	add    %al,(%rax)
-   18002b6f7:	add    %dh,%al
-   18002b6f9:	pop    %rbx
+   18002b6f8:	lock pop %rbx
    18002b6fa:	add    %al,0x1(%rax)
    18002b700:	add    %eax,(%rax)
    18002b702:	or     %al,(%rax)
    18002b704:	or     %al,(%rax)
    18002b706:	add    %al,(%rax)
    18002b708:	(bad)
    18002b709:	rolb   $0x0,(%rax)
 	...
-   18002b718:	enter  $0x1d8,$0x80
-   18002b71c:	add    %eax,(%rax)
+   18002b718:	rcr    $0x1,%bh
+   18002b71b:	addb   $0x0,(%rcx)
    18002b71e:	add    %al,(%rax)
    18002b720:	adc    %bl,-0x80(%rax,%rax,1)
    18002b724:	add    %eax,(%rax)
    18002b726:	add    %al,(%rax)
    18002b728:	and    %bl,-0x80(%rax,%rax,1)
    18002b72c:	add    %eax,(%rax)
    18002b72e:	add    %al,(%rax)
@@ -64635,19 +64624,19 @@
    18002b7d2:	or     %al,(%rax)
    18002b7d4:	adc    %al,(%rax)
    18002b7d6:	add    %al,(%rax)
    18002b7d8:	add    %eax,%eax
    18002b7da:	add    %al,(%rax)
    18002b7dc:	add    %al,(%rax)
    18002b7de:	add    %al,(%rax)
-   18002b7e0:	adc    %cl,(%rdi)
-   18002b7e2:	add    %eax,0x1(%rax)
-   18002b7e8:	adc    %ch,%dh
+   18002b7e0:	push   %rax
+   18002b7e1:	sgdt   0x1(%rax)
+   18002b7e8:	and    %ch,%dh
    18002b7ea:	add    %eax,0x1(%rax)
-   18002b7f0:	adc    %dl,(%rax)
+   18002b7f0:	adc    %cl,(%rdi)
    18002b7f2:	add    %eax,0x1(%rax)
 	...
    18002b808:	xor    %ah,(%rdx)
    18002b80a:	add    %al,0x1(%rax)
 	...
    18002b840:	add    %eax,(%rax)
    18002b842:	or     %al,(%rax)
@@ -64655,17 +64644,17 @@
    18002b846:	add    %al,(%rax)
    18002b848:	add    %eax,%eax
    18002b84a:	add    %al,(%rax)
    18002b84c:	add    %al,(%rax)
    18002b84e:	add    %al,(%rax)
    18002b850:	push   %rax
    18002b851:	rex.WX add %rax,0x1(%rax)
-   18002b858:	xor    $0x1,%cl
-   18002b85b:	addb   $0x0,(%rcx)
-   18002b85e:	add    %al,(%rax)
+   18002b858:	nop
+   18002b859:	int1
+   18002b85a:	add    %eax,0x1(%rax)
    18002b860:	(bad)
    18002b861:	rex.WX add %rax,0x1(%rax)
 	...
    18002b878:	xor    %ah,(%rdx)
    18002b87a:	add    %al,0x1(%rax)
 	...
    18002b8b0:	add    %eax,(%rax)
@@ -64674,17 +64663,16 @@
    18002b8b6:	add    %al,(%rax)
    18002b8b8:	add    %eax,%eax
    18002b8ba:	add    %al,(%rax)
    18002b8bc:	add    %al,(%rax)
    18002b8be:	add    %al,(%rax)
    18002b8c0:	mov    $0x4a,%al
    18002b8c2:	add    %eax,0x1(%rax)
-   18002b8c8:	enter  $0x1f4,$0x80
-   18002b8cc:	add    %eax,(%rax)
-   18002b8ce:	add    %al,(%rax)
+   18002b8c8:	fdiv   %st(4),%st
+   18002b8ca:	add    %eax,0x1(%rax)
    18002b8d0:	rolb   0x18001(%rcx)
 	...
    18002b8e6:	add    %al,(%rax)
    18002b8e8:	xor    %ah,(%rdx)
    18002b8ea:	add    %al,0x1(%rax)
 	...
    18002b920:	int    $0x5d
@@ -64708,15 +64696,16 @@
    18002b952:	add    %al,(%rax)
    18002b954:	add    %al,(%rax)
    18002b956:	add    %al,(%rax)
    18002b958:	add    %eax,(%rax)
    18002b95a:	add    %al,(%rax)
    18002b95c:	add    %al,(%rax)
    18002b95e:	add    %al,(%rax)
-   18002b960:	rex testb $0x80,(%rcx)
+   18002b960:	push   %rax
+   18002b961:	testb  $0x80,(%rcx)
    18002b964:	add    %eax,(%rax)
 	...
    18002b96e:	add    %al,(%rax)
    18002b970:	cs (bad)
    18002b972:	push   %r14
    18002b974:	(bad)
    18002b979:	jb     0x18002b9ed
@@ -64726,51 +64715,53 @@
    18002b97f:	gs ja  0x18002b9e1
    18002b982:	insb   (%dx),%es:(%rdi)
    18002b983:	outsb  %gs:(%rsi),(%dx)
    18002b985:	addr32 je 0x18002b9f0
    18002b988:	rex jae 0x18002b9ff
    18002b98b:	fs rex
    18002b98d:	rex add %al,(%rax)
-   18002b990:	rex testb $0x80,(%rcx)
+   18002b990:	push   %rax
+   18002b991:	testb  $0x80,(%rcx)
    18002b994:	add    %eax,(%rax)
 	...
    18002b99e:	add    %al,(%rax)
    18002b9a0:	cs (bad)
    18002b9a2:	push   %r14
    18002b9a4:	(bad)
    18002b9a9:	insb   (%dx),%es:(%rdi)
    18002b9aa:	insb   (%dx),%es:(%rdi)
    18002b9ab:	outsl  %ds:(%rsi),(%dx)
    18002b9ac:	movsxd 0x73(%rax),%eax
    18002b9af:	je     0x18002ba15
    18002b9b1:	rex
    18002b9b2:	rex add %al,(%rax)
    18002b9b5:	add    %al,(%rax)
-   18002b9b7:	add    %al,-0xa(%rax)
+   18002b9b7:	add    %dl,-0xa(%rax)
    18002b9ba:	add    %eax,0x1(%rax)
 	...
    18002b9c8:	cs (bad)
    18002b9ca:	push   %r14
    18002b9cc:	gs js  0x18002ba32
    18002b9cf:	gs jo  0x18002ba46
    18002b9d2:	imul   $0x64747340,0x6e(%rdi),%ebp
    18002b9d9:	rex
    18002b9da:	rex add %al,(%rax)
    18002b9dd:	add    %al,(%rax)
-   18002b9df:	add    %al,-0xa(%rax)
+   18002b9df:	add    %dl,-0xa(%rax)
    18002b9e2:	add    %eax,0x1(%rax)
 	...
    18002b9f0:	cs (bad)
    18002b9f2:	push   %r14
    18002b9f4:	push   %rcx
    18002b9f5:	rex.WRXB
    18002b9f6:	rex.B jne 0x18002ba6d
    18002b9f9:	push   $0x404031
    18002b9fe:	add    %al,(%rax)
-   18002ba00:	rex testb $0x80,(%rcx)
+   18002ba00:	push   %rax
+   18002ba01:	testb  $0x80,(%rcx)
    18002ba04:	add    %eax,(%rax)
 	...
    18002ba0e:	add    %al,(%rax)
    18002ba10:	cs (bad)
    18002ba12:	push   %r14
    18002ba14:	push   %rcx
    18002ba15:	rex.WRXB
@@ -64784,15 +64775,16 @@
    18002ba28:	rex.XB outsl %ds:(%rsi),(%dx)
    18002ba2a:	fs gs rex.RX insb (%dx),%es:(%rdi)
    18002ba2e:	outsl  %ds:(%rsi),(%dx)
    18002ba2f:	ja     0x18002ba71
    18002ba31:	rex add %al,(%rax)
    18002ba34:	add    %al,(%rax)
    18002ba36:	add    %al,(%rax)
-   18002ba38:	rex testb $0x80,(%rcx)
+   18002ba38:	push   %rax
+   18002ba39:	testb  $0x80,(%rcx)
    18002ba3c:	add    %eax,(%rax)
 	...
    18002ba46:	add    %al,(%rax)
    18002ba48:	cs (bad)
    18002ba4a:	push   %r14
    18002ba4c:	push   %rcx
    18002ba4d:	rex.WRX
@@ -64803,78 +64795,80 @@
    18002ba58:	jae    0x18002bacd
    18002ba5a:	rex.WRB (bad)
    18002ba5c:	outsb  %ds:(%rsi),(%dx)
    18002ba5d:	(bad)
    18002ba5e:	addr32 gs jb 0x18002baa2
    18002ba62:	rex add %al,(%rax)
    18002ba65:	add    %al,(%rax)
-   18002ba67:	add    %al,-0xa(%rax)
+   18002ba67:	add    %dl,-0xa(%rax)
    18002ba6a:	add    %eax,0x1(%rax)
 	...
    18002ba78:	cs (bad)
    18002ba7a:	push   %r14
    18002ba7c:	push   %rcx
    18002ba7d:	rex.WRXB (bad)
    18002ba7f:	push   $0x65
    18002ba81:	movsxd 0x40(%rax,%rax,2),%esi
    18002ba85:	add    %al,(%rax)
-   18002ba87:	add    %al,-0xa(%rax)
+   18002ba87:	add    %dl,-0xa(%rax)
    18002ba8a:	add    %eax,0x1(%rax)
 	...
    18002ba98:	cs (bad)
    18002ba9a:	push   %r14
    18002ba9c:	push   %rcx
    18002ba9d:	(bad)
    18002baa3:	movsxd 0x41(%rdi,%rcx,2),%esi
    18002baa7:	jne    0x18002bb1d
    18002baa9:	push   $0x76697250
    18002baae:	(bad)
    18002baaf:	je     0x18002bb16
    18002bab1:	rex
    18002bab2:	rex add %al,(%rax)
    18002bab5:	add    %al,(%rax)
-   18002bab7:	add    %al,-0xa(%rax)
+   18002bab7:	add    %dl,-0xa(%rax)
    18002baba:	add    %eax,0x1(%rax)
 	...
    18002bac8:	cs (bad)
    18002baca:	push   %r14
    18002bacc:	push   %rcx
    18002bacd:	rex.WRXB (bad)
    18002bacf:	push   $0x65
    18002bad1:	movsxd 0x72(%rax,%rdx,2),%esi
    18002bad5:	imul   $0x40406574,0x61(%rsi),%esi
    18002badc:	add    %al,(%rax)
    18002bade:	add    %al,(%rax)
-   18002bae0:	rex testb $0x80,(%rcx)
+   18002bae0:	push   %rax
+   18002bae1:	testb  $0x80,(%rcx)
    18002bae4:	add    %eax,(%rax)
 	...
    18002baee:	add    %al,(%rax)
    18002baf0:	cs (bad)
    18002baf2:	push   %r14
    18002baf4:	push   %rcx
    18002baf5:	rex.WRXB (bad)
    18002baf7:	push   $0x65
    18002baf9:	movsxd 0x61(%rsp,%rax,2),%esi
    18002bafd:	je     0x18002bb60
    18002baff:	rex
    18002bb00:	rex add %al,(%rax)
    18002bb03:	add    %al,(%rax)
    18002bb05:	add    %al,(%rax)
-   18002bb07:	add    %al,-0xa(%rax)
+   18002bb07:	add    %dl,-0xa(%rax)
    18002bb0a:	add    %eax,0x1(%rax)
 	...
    18002bb18:	cs (bad)
    18002bb1a:	push   %r14
    18002bb1c:	push   %rcx
    18002bb1d:	(bad)
    18002bb23:	movsxd 0x41(%rdi,%rcx,2),%esi
    18002bb27:	jne    0x18002bb9d
    18002bb29:	push   $0x4040
    18002bb2e:	add    %al,(%rax)
-   18002bb30:	rex testb $0x80,(%rcx)
+   18002bb30:	push   %rax
+   18002bb31:	testb  $0x80,(%rcx)
    18002bb34:	add    %eax,(%rax)
 	...
    18002bb3e:	add    %al,(%rax)
    18002bb40:	cs (bad)
    18002bb42:	push   %r14
    18002bb44:	push   %rcx
    18002bb45:	(bad)
@@ -64882,27 +64876,29 @@
    18002bb4f:	jne    0x18002bbc5
    18002bb51:	push   $0x69725032
    18002bb56:	jbe    0x18002bbb9
    18002bb58:	je     0x18002bbbf
    18002bb5a:	rex
    18002bb5b:	rex add %al,(%rax)
    18002bb5e:	add    %al,(%rax)
-   18002bb60:	rex testb $0x80,(%rcx)
+   18002bb60:	push   %rax
+   18002bb61:	testb  $0x80,(%rcx)
    18002bb64:	add    %eax,(%rax)
 	...
    18002bb6e:	add    %al,(%rax)
    18002bb70:	cs (bad)
    18002bb72:	push   %r14
    18002bb74:	push   %rcx
    18002bb75:	(bad)
    18002bb7b:	movsxd 0x41(%rdi,%rcx,2),%esi
    18002bb7f:	jne    0x18002bbf5
    18002bb81:	push   $0x404032
    18002bb86:	add    %al,(%rax)
-   18002bb88:	rex testb $0x80,(%rcx)
+   18002bb88:	push   %rax
+   18002bb89:	testb  $0x80,(%rcx)
    18002bb8c:	add    %eax,(%rax)
 	...
    18002bb96:	add    %al,(%rax)
    18002bb98:	cs (bad)
    18002bb9a:	push   %r14
    18002bb9c:	push   %rcx
    18002bb9d:	(bad)
@@ -64914,30 +64910,32 @@
    18002bbb1:	outsb  %ds:(%rsi),(%dx)
    18002bbb2:	fs insb (%dx),%es:(%rdi)
    18002bbb4:	gs jb  0x18002bbf7
    18002bbb7:	rex add %al,(%rax)
    18002bbba:	add    %al,(%rax)
    18002bbbc:	add    %al,(%rax)
    18002bbbe:	add    %al,(%rax)
-   18002bbc0:	rex testb $0x80,(%rcx)
+   18002bbc0:	push   %rax
+   18002bbc1:	testb  $0x80,(%rcx)
    18002bbc4:	add    %eax,(%rax)
 	...
    18002bbce:	add    %al,(%rax)
    18002bbd0:	cs (bad)
    18002bbd2:	push   %r14
    18002bbd4:	push   %rcx
    18002bbd5:	rex.WRXB
    18002bbd6:	rex.B jne 0x18002bc4d
    18002bbd9:	push   $0x69725031
    18002bbde:	jbe    0x18002bc41
    18002bbe0:	je     0x18002bc47
    18002bbe2:	rex
    18002bbe3:	rex add %al,(%rax)
    18002bbe6:	add    %al,(%rax)
-   18002bbe8:	rex testb $0x80,(%rcx)
+   18002bbe8:	push   %rax
+   18002bbe9:	testb  $0x80,(%rcx)
    18002bbec:	add    %eax,(%rax)
 	...
    18002bbf6:	add    %al,(%rax)
    18002bbf8:	cs (bad)
    18002bbfa:	push   %r14
    18002bbfc:	push   %rcx
    18002bbfd:	rex.WRXB
@@ -64955,15 +64953,15 @@
    18002bc19:	jb     0x18002bc84
    18002bc1b:	jbe    0x18002bc7e
    18002bc1d:	je     0x18002bc84
    18002bc1f:	rex
    18002bc20:	rex add %al,(%rax)
    18002bc23:	add    %al,(%rax)
    18002bc25:	add    %al,(%rax)
-   18002bc27:	add    %al,-0xa(%rax)
+   18002bc27:	add    %dl,-0xa(%rax)
    18002bc2a:	add    %eax,0x1(%rax)
 	...
    18002bc38:	cs (bad)
    18002bc3a:	push   %r14
    18002bc3c:	push   %rcx
    18002bc3d:	rex.WRXB
    18002bc3e:	rex.B jne 0x18002bcb5
@@ -64976,15 +64974,16 @@
    18002bc52:	(bad)
    18002bc53:	outsb  %ds:(%rsi),(%dx)
    18002bc54:	fs insb (%dx),%es:(%rdi)
    18002bc56:	gs jb  0x18002bc99
    18002bc59:	rex add %al,(%rax)
    18002bc5c:	add    %al,(%rax)
    18002bc5e:	add    %al,(%rax)
-   18002bc60:	rex testb $0x80,(%rcx)
+   18002bc60:	push   %rax
+   18002bc61:	testb  $0x80,(%rcx)
    18002bc64:	add    %eax,(%rax)
 	...
    18002bc6e:	add    %al,(%rax)
    18002bc70:	cs (bad)
    18002bc72:	push   %r14
    18002bc74:	push   %rcx
    18002bc75:	rex.WRXB
@@ -64994,15 +64993,15 @@
    18002bc81:	jns    0x18002bccb
    18002bc83:	(bad)
    18002bc84:	outsb  %ds:(%rsi),(%dx)
    18002bc85:	fs insb (%dx),%es:(%rdi)
    18002bc87:	gs jb  0x18002bcca
    18002bc8a:	rex add %al,(%rax)
    18002bc8d:	add    %al,(%rax)
-   18002bc8f:	add    %al,-0xa(%rax)
+   18002bc8f:	add    %dl,-0xa(%rax)
    18002bc92:	add    %eax,0x1(%rax)
 	...
    18002bca0:	cs (bad)
    18002bca2:	push   %r14
    18002bca4:	je     0x18002bd1f
    18002bca6:	jo     0x18002bd0d
    18002bca8:	pop    %rdi
@@ -66944,37 +66943,37 @@
    18002f27e:	add    %eax,(%rax)
    18002f280:	adc    $0x1b,%al
    18002f282:	add    (%rax),%al
    18002f284:	mov    $0x900010e,%esi
    18002f289:	sgdt   (%rax)
    18002f28c:	sub    %bl,(%rbx)
    18002f28e:	add    (%rax),%al
-   18002f290:	and    %cl,(%rdi)
+   18002f290:	adc    %cl,(%rdi)
    18002f292:	add    %eax,(%rax)
-   18002f294:	scas   %es:(%rdi),%eax
+   18002f294:	push   %rax
    18002f295:	sgdt   (%rax)
-   18002f298:	sbb    %cl,0xfaf0002(%rip)        # 0x18fb1f2a0
-   18002f29e:	add    %eax,(%rax)
-   18002f2a0:	lock sgdt (%rax)
-   18002f2a4:	pushf
-   18002f2a5:	(bad)
-   18002f2a6:	add    (%rax),%al
-   18002f2a8:	lock sgdt (%rax)
-   18002f2ac:	or     (%rax),%edx
+   18002f298:	mov    $0x6000021f,%esp
+   18002f29d:	sgdt   (%rax)
+   18002f2a0:	out    %eax,(%dx)
+   18002f2a1:	sgdt   (%rax)
+   18002f2a4:	sbb    %cl,0xfef0002(%rip)        # 0x18ff1f2ac
+   18002f2aa:	add    %eax,(%rax)
+   18002f2ac:	xor    %dl,(%rax)
    18002f2ae:	add    %eax,(%rax)
-   18002f2b0:	mov    $0x1e,%al
+   18002f2b0:	pushf
+   18002f2b1:	(bad)
    18002f2b2:	add    (%rax),%al
-   18002f2b4:	adc    %dl,(%rax)
+   18002f2b4:	xor    %dl,(%rax)
    18002f2b6:	add    %eax,(%rax)
-   18002f2b8:	push   %rax
-   18002f2b9:	adc    %al,(%rcx)
-   18002f2bb:	add    %bh,0x10500002(%rdi,%rbx,1)
-   18002f2c2:	add    %eax,(%rax)
-   18002f2c4:	rex.W adc (%rcx),%al
-   18002f2c7:	add    %dl,%ah
+   18002f2b8:	rex.WXB adc %al,(%r9)
+   18002f2bb:	add    %dh,0x5000021e(%rax)
+   18002f2c1:	adc    %al,(%rcx)
+   18002f2c3:	add    %cl,0x12(%rax)
+   18002f2c6:	add    %eax,(%rax)
+   18002f2c8:	(bad)
    18002f2c9:	and    %al,(%rdx)
    18002f2cb:	add    %dl,0x12(%rax)
    18002f2ce:	add    %eax,(%rax)
    18002f2d0:	mov    (%rdx),%edx
    18002f2d2:	add    %eax,(%rax)
    18002f2d4:	adc    %cl,(%rbx)
    18002f2d6:	add    (%rax),%al
@@ -68021,17 +68020,17 @@
    1800300bc:	rex.WB add %cl,0x0(%r14)
    1800300c0:	rex.RX add %r9b,0x0(%rdi)
    1800300c4:	add    %al,(%rax)
    1800300c6:	add    %al,(%rax)
    1800300c8:	mov    $0xfeef04,%ebp
    1800300cd:	add    %al,(%rcx)
    1800300cf:	add    %al,0x600(%rip)        # 0x1800306d5
-   1800300d5:	add    %al,(%rcx)
+   1800300d5:	add    %al,(%rdx)
    1800300d7:	add    %al,0x600(%rip)        # 0x1800306dd
-   1800300dd:	add    %al,(%rcx)
+   1800300dd:	add    %al,(%rdx)
    1800300df:	add    %bh,(%rdi)
    1800300e1:	add    %al,(%rax)
    1800300e3:	add    %al,(%rax)
    1800300e5:	add    %al,(%rax)
    1800300e7:	add    %al,(%rax,%rax,1)
    1800300ea:	add    $0x0,%al
    1800300ec:	add    (%rax),%al
@@ -68143,15 +68142,15 @@
    180030203:	add    %ah,0x0(%rbp)
    180030206:	jb     0x180030208
    180030208:	jae    0x18003020a
    18003020a:	imul   $0x6e006f,(%rax),%eax
    180030210:	add    %al,(%rax)
    180030212:	add    %al,(%rax)
    180030214:	ss add %ch,(%rsi)
-   180030217:	add    %dh,0x31002e00(%rip)        # 0x1b103301d
+   180030217:	add    %dh,0x32002e00(%rip)        # 0x1b203301d
    18003021d:	add    %ch,(%rsi)
    18003021f:	add    %dh,(%rax)
    180030221:	add    %al,(%rax)
    180030223:	add    %ah,0x1003e00(%rax)
    180030229:	add    %cl,0x65(%rax,%rax,1)
    18003022d:	add    %ah,0x0(%rdi)
    180030230:	(bad)
@@ -68268,15 +68267,15 @@
    180030350:	push   %rsi
    180030351:	add    %ah,0x0(%rbp)
    180030354:	jb     0x180030356
    180030356:	jae    0x180030358
    180030358:	imul   $0x6e006f,(%rax),%eax
    18003035e:	add    %al,(%rax)
    180030360:	ss add %ch,(%rsi)
-   180030363:	add    %dh,0x31002e00(%rip)        # 0x1b1033169
+   180030363:	add    %dh,0x32002e00(%rip)        # 0x1b2033169
    180030369:	add    %ch,(%rsi)
    18003036b:	add    %dh,(%rax)
    18003036d:	add    %al,(%rax)
    18003036f:	add    %bl,(%rax)
    180030371:	add    %al,(%rax)
    180030373:	add    %al,(%rcx)
    180030375:	add    %al,0x0(%rbx)
@@ -68517,20 +68516,20 @@
    180031069:	cmpsb  %es:(%rdi),%ds:(%rsi)
    18003106a:	andb   $0x98,-0x596f5978(%rsi)
    180031071:	cmpsb  %es:(%rdi),%ds:(%rsi)
    180031072:	clc
    180031073:	cmpsb  %es:(%rdi),%ds:(%rsi)
    180031074:	add    %ah,-0x58ef58f8(%rdi)
    18003107a:	and    %ah,0x1d000(%rdi)
-   180031080:	in     (%dx),%al
-   180031081:	add    %al,(%rax)
-   180031083:	add    %ah,(%rax)
-   180031085:	movabs 0xa040a038a030a028,%al
-   18003108e:	rex.W movabs 0xa068a060a058a050,%al
-   180031098:	jo     0x18003103a
+   180031080:	jo     0x180031083
+   180031082:	add    %al,(%rax)
+   180031084:	and    %ah,-0x5fcf5fd8(%rax)
+   18003108a:	cmp    %ah,-0x5fb75fc0(%rax)
+   180031090:	push   %rax
+   180031091:	movabs 0xa070a068a060a058,%al
    18003109a:	js     0x18003103c
    18003109c:	andb   $0x98,-0x5f6f5f78(%rax)
    1800310a3:	movabs 0xa0b8a0b0a0a8a0a0,%al
    1800310ac:	shlb   $0xd8,-0x5f2f5f38(%rax)
    1800310b3:	movabs 0xa100a0f8a0f0a0e0,%al
    1800310bc:	adc    %ah,-0x5ed75ee8(%rcx)
    1800310c2:	cmp    %ah,-0x5eaf5ec0(%rcx)
@@ -68572,159 +68571,184 @@
    180031143:	cmpsl  %es:(%rdi),%ds:(%rsi)
    180031144:	(bad)
    180031145:	cmpsl  %es:(%rdi),%ds:(%rsi)
    180031146:	push   $0x78a770a7
    18003114b:	cmpsl  %es:(%rdi),%ds:(%rsi)
    18003114c:	andb   $0x98,-0x586f5878(%rdi)
    180031153:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   180031154:	movabs 0x78a7b8a7b0a7a8a7,%al
-   18003115d:	stos   %al,%es:(%rdi)
-   18003115e:	subb   $0xa0,-0x556f5578(%rdx)
-   180031165:	stos   %al,%es:(%rdi)
-   180031166:	add    %al,(%rax)
-   180031168:	add    %ah,%al
-   18003116a:	add    %eax,(%rax)
-   18003116c:	push   $0x60000001
-   180031171:	movabs %al,0xa280a278a270a268
-   18003117a:	mov    %ah,-0x5d675d70(%rdx)
-   180031180:	movabs 0xc0a2b8a2b0a2a8a2,%al
-   180031189:	movabs %al,0xa2e0a2d8a2d0a2c8
-   180031192:	call   0x178a60239
-   180031197:	movabs %al,0xa318a310a308a300
-   1800311a0:	and    %ah,-0x5ccf5cd8(%rbx)
-   1800311a6:	cmp    %ah,-0x5cb75cc0(%rbx)
-   1800311ac:	push   %rax
-   1800311ad:	movabs %eax,0xa370a368a360a358
-   1800311b6:	js     0x18003115b
-   1800311b8:	andb   $0x98,-0x5c6f5c78(%rbx)
-   1800311bf:	movabs %eax,0xa3b8a3b0a3a8a3a0
-   1800311c8:	shlb   $0xd8,-0x5c2f5c38(%rbx)
-   1800311cf:	movabs %eax,0xa3f8a3f0a3e8a3e0
-   1800311d8:	add    %ah,0x18a410a4(%rax,%rcx,1)
-   1800311df:	movsb  %ds:(%rsi),%es:(%rdi)
-   1800311e0:	and    %ah,0x38a430a4(%rax,%rbp,1)
-   1800311e7:	movsb  %ds:(%rsi),%es:(%rdi)
-   1800311e8:	rex movsb %ds:(%rsi),%es:(%rdi)
-   1800311ea:	rex.W movsb %ds:(%rsi),%es:(%rdi)
-   1800311ec:	push   %rax
-   1800311ed:	movsb  %ds:(%rsi),%es:(%rdi)
-   1800311ee:	pop    %rax
-   1800311ef:	movsb  %ds:(%rsi),%es:(%rdi)
-   1800311f0:	(bad)
-   1800311f1:	movsb  %ds:(%rsi),%es:(%rdi)
-   1800311f2:	push   $0x78a470a4
-   1800311f7:	movsb  %ds:(%rsi),%es:(%rdi)
-   1800311f8:	andb   $0xa4,-0x675b6f5c(%rax,%rcx,4)
-   180031200:	movabs 0xc0a4b8a4b0a4a8a4,%al
-   180031209:	movsb  %ds:(%rsi),%es:(%rdi)
-   18003120a:	enter  $0xd0a4,$0xa4
-   18003120e:	fsubs  -0xf5b175c(%rax,%riz,8)
+   180031154:	movabs 0x30a7b8a7b0a7a8a7,%al
+   18003115d:	lods   %ds:(%rsi),%eax
+   18003115e:	cmp    %ch,-0x52b752c0(%rbp)
+   180031164:	push   %rax
+   180031165:	lods   %ds:(%rsi),%eax
+   180031166:	pop    %rax
+   180031167:	lods   %ds:(%rsi),%eax
+   180031168:	(bad)
+   180031169:	lods   %ds:(%rsi),%eax
+   18003116a:	push   $0x78ad70ad
+   18003116f:	lods   %ds:(%rsi),%eax
+   180031170:	subb   $0x98,-0x526f5278(%rbp)
+   180031177:	lods   %ds:(%rsi),%eax
+   180031178:	movabs 0xc0adb8adb0ada8ad,%al
+   180031181:	lods   %ds:(%rsi),%eax
+   180031182:	enter  $0xd0ad,$0xad
+   180031186:	fsubrs -0x52175220(%rbp)
+   18003118c:	lock lods %ds:(%rsi),%eax
+   18003118e:	clc
+   18003118f:	lods   %ds:(%rsi),%eax
+   180031190:	add    %ch,-0x51ef51f8(%rsi)
+   180031196:	sbb    %ch,-0x51d751e0(%rsi)
+   18003119c:	xor    %ch,-0x51bf51c8(%rsi)
+   1800311a2:	rex.W scas %es:(%rdi),%al
+   1800311a4:	push   %rax
+   1800311a5:	scas   %es:(%rdi),%al
+   1800311a6:	pop    %rax
+   1800311a7:	scas   %es:(%rdi),%al
+   1800311a8:	(bad)
+   1800311a9:	scas   %es:(%rdi),%al
+   1800311aa:	push   $0x78ae70ae
+   1800311af:	scas   %es:(%rdi),%al
+   1800311b0:	subb   $0x98,-0x516f5178(%rsi)
+   1800311b7:	scas   %es:(%rdi),%al
+   1800311b8:	movabs 0xc0aeb8aeb0aea8ae,%al
+   1800311c1:	scas   %es:(%rdi),%al
+   1800311c2:	enter  $0xd0ae,$0xae
+   1800311c6:	fsubrs -0x51175120(%rsi)
+   1800311cc:	lock scas %es:(%rdi),%al
+   1800311ce:	clc
+   1800311cf:	scas   %es:(%rdi),%al
+   1800311d0:	add    %ch,-0x50ef50f8(%rdi)
+   1800311d6:	sbb    %ch,-0x50d750e0(%rdi)
+   1800311dc:	xor    %ch,-0x50bf50c8(%rdi)
+   1800311e2:	scas   %es:(%rdi),%rax
+   1800311e4:	push   %rax
+   1800311e5:	scas   %es:(%rdi),%eax
+   1800311e6:	pop    %rax
+   1800311e7:	scas   %es:(%rdi),%eax
+   1800311e8:	(bad)
+   1800311e9:	scas   %es:(%rdi),%eax
+   1800311ea:	add    %al,(%rax)
+   1800311ec:	add    %ah,%al
+   1800311ee:	add    %eax,(%rax)
+   1800311f0:	in     $0x0,%al
+   1800311f2:	add    %al,(%rax)
+   1800311f4:	js     0x180031197
+   1800311f6:	andb   $0xa0,-0x5e6f5e78(%rcx)
+   1800311fd:	movabs 0xa4b8a4b0a4a8a4a0,%eax
+   180031206:	shlb   $0xa4,-0x275b2f5c(%rax,%rcx,8)
+   18003120e:	loopne 0x1800311b4
+   180031210:	call   0x178a802b9
    180031215:	movsb  %ds:(%rsi),%es:(%rdi)
-   180031216:	clc
-   180031217:	movsb  %ds:(%rsi),%es:(%rdi)
-   180031218:	add    %ah,-0x5aef5af8(%rbp)
-   18003121e:	sbb    %ah,-0x5ad75ae0(%rbp)
-   180031224:	xor    %ah,-0x5abf5ac8(%rbp)
-   18003122a:	movsq  %ds:(%rsi),%es:(%rdi)
-   18003122c:	push   %rax
+   180031216:	add    %ah,-0x5aef5af8(%rbp)
+   18003121c:	sbb    %ah,-0x5ad75ae0(%rbp)
+   180031222:	xor    %ah,-0x5abf5ac8(%rbp)
+   180031228:	movsq  %ds:(%rsi),%es:(%rdi)
+   18003122a:	push   %rax
+   18003122b:	movsl  %ds:(%rsi),%es:(%rdi)
+   18003122c:	pop    %rax
    18003122d:	movsl  %ds:(%rsi),%es:(%rdi)
-   18003122e:	pop    %rax
+   18003122e:	(bad)
    18003122f:	movsl  %ds:(%rsi),%es:(%rdi)
-   180031230:	(bad)
-   180031231:	movsl  %ds:(%rsi),%es:(%rdi)
-   180031232:	push   $0x30a570a5
-   180031237:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180031238:	cmp    %ah,-0x59b759c0(%rsi)
-   18003123e:	push   %rax
+   180031230:	push   $0x78a570a5
+   180031235:	movsl  %ds:(%rsi),%es:(%rdi)
+   180031236:	rex cmpsb %es:(%rdi),%ds:(%rsi)
+   180031238:	rex.W cmpsb %es:(%rdi),%ds:(%rsi)
+   18003123a:	push   %rax
+   18003123b:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   18003123c:	pop    %rax
+   18003123d:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   18003123e:	(bad)
    18003123f:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180031240:	pop    %rax
-   180031241:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180031242:	(bad)
-   180031243:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180031244:	push   $0x78a670a6
-   180031249:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   18003124a:	andb   $0x98,-0x596f5978(%rsi)
-   180031251:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180031252:	rex.W test $0x50,%al
-   180031255:	test   $0x58,%al
-   180031257:	test   $0x60,%al
-   180031259:	test   $0x68,%al
-   18003125b:	test   $0x70,%al
-   18003125d:	test   $0x78,%al
-   18003125f:	test   $0x80,%al
-   180031261:	test   $0x88,%al
-   180031263:	test   $0x90,%al
-   180031265:	test   $0x98,%al
-   180031267:	test   $0xa0,%al
-   180031269:	test   $0xa8,%al
-   18003126b:	test   $0xb0,%al
-   18003126d:	test   $0xb8,%al
-   18003126f:	test   $0xc0,%al
-   180031271:	test   $0xc8,%al
-   180031273:	test   $0xd0,%al
-   180031275:	test   $0xd8,%al
-   180031277:	test   $0xe0,%al
-   180031279:	test   $0x8,%al
-   18003127b:	test   $0xa918a910,%eax
-   180031280:	loopne 0x18003122f
-   180031282:	call   0x178b10334
-   180031287:	lods   %ds:(%rsi),%eax
-   180031288:	add    %ch,-0x51c751f8(%rsi)
-   18003128e:	rex scas %es:(%rdi),%al
-   180031290:	rex.W scas %es:(%rdi),%al
-   180031292:	push   %rax
+   180031240:	push   $0x78a670a6
+   180031245:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   180031246:	andb   $0x98,-0x596f5978(%rsi)
+   18003124d:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   18003124e:	movabs 0x68a860a858a6a8a6,%al
+   180031257:	test   $0x70,%al
+   180031259:	test   $0x78,%al
+   18003125b:	test   $0x80,%al
+   18003125d:	test   $0x88,%al
+   18003125f:	test   $0x90,%al
+   180031261:	test   $0x98,%al
+   180031263:	test   $0xa0,%al
+   180031265:	test   $0xa8,%al
+   180031267:	test   $0xb0,%al
+   180031269:	test   $0xb8,%al
+   18003126b:	test   $0xc0,%al
+   18003126d:	test   $0xc8,%al
+   18003126f:	test   $0xd0,%al
+   180031271:	test   $0xd8,%al
+   180031273:	test   $0xe0,%al
+   180031275:	test   $0xe8,%al
+   180031277:	test   $0xf0,%al
+   180031279:	test   $0x18,%al
+   18003127b:	test   $0xa928a920,%eax
+   180031280:	lock lods %ds:(%rsi),%eax
+   180031282:	clc
+   180031283:	lods   %ds:(%rsi),%eax
+   180031284:	add    %ch,-0x51ef51f8(%rsi)
+   18003128a:	sbb    %ch,-0x51af51b8(%rsi)
+   180031290:	pop    %rax
+   180031291:	scas   %es:(%rdi),%al
+   180031292:	(bad)
    180031293:	scas   %es:(%rdi),%al
-   180031294:	(bad)
-   180031295:	scas   %es:(%rdi),%al
-   180031296:	jo     0x180031246
-   180031298:	js     0x180031248
-   18003129a:	subb   $0x98,-0x516f5178(%rsi)
-   1800312a1:	scas   %es:(%rdi),%al
-   1800312a2:	movabs 0xc0aeb8aeb0aea8ae,%al
-   1800312ab:	scas   %es:(%rdi),%al
-   1800312ac:	enter  $0xd0ae,$0xae
-   1800312b0:	fsubrs -0x51175120(%rsi)
-   1800312b6:	lock scas %es:(%rdi),%al
-   1800312b8:	clc
-   1800312b9:	scas   %es:(%rdi),%al
-   1800312ba:	add    %ch,-0x50ef50f8(%rdi)
-   1800312c0:	sbb    %ch,-0x50d750e0(%rdi)
-   1800312c6:	xor    %ch,-0x50bf50c8(%rdi)
-   1800312cc:	scas   %es:(%rdi),%rax
+   180031294:	jo     0x180031244
+   180031296:	subb   $0x98,-0x516f5178(%rsi)
+   18003129d:	scas   %es:(%rdi),%al
+   18003129e:	movabs 0xc0aeb8aeb0aea8ae,%al
+   1800312a7:	scas   %es:(%rdi),%al
+   1800312a8:	enter  $0xd0ae,$0xae
+   1800312ac:	fsubrs -0x51175120(%rsi)
+   1800312b2:	lock scas %es:(%rdi),%al
+   1800312b4:	clc
+   1800312b5:	scas   %es:(%rdi),%al
+   1800312b6:	add    %ch,-0x50ef50f8(%rdi)
+   1800312bc:	sbb    %ch,-0x50d750e0(%rdi)
+   1800312c2:	xor    %ch,-0x50bf50c8(%rdi)
+   1800312c8:	scas   %es:(%rdi),%rax
+   1800312ca:	push   %rax
+   1800312cb:	scas   %es:(%rdi),%eax
+   1800312cc:	pop    %rax
+   1800312cd:	scas   %es:(%rdi),%eax
    1800312ce:	add    %al,(%rax)
    1800312d0:	add    %dh,%al
    1800312d2:	add    %eax,(%rax)
    1800312d4:	jl     0x1800312d6
    1800312d6:	add    %al,(%rax)
-   1800312d8:	js     0x18003127b
-   1800312da:	test   $0xa1,%al
-   1800312dc:	mov    $0xa1,%al
-   1800312de:	mov    $0xd0a1c0a1,%eax
-   1800312e3:	movabs 0xa1f8a1f0a1e8a1e0,%eax
-   1800312ec:	add    %ah,-0x5def5df8(%rdx)
-   1800312f2:	sbb    %ah,-0x5dd75de0(%rdx)
-   1800312f8:	xor    %ah,-0x5dbf5dc8(%rdx)
-   1800312fe:	rex.W movabs %al,0xa440a438a430a428
-   180031308:	push   %rax
+   1800312d8:	mov    %ah,-0x5e3f5e48(%rcx)
+   1800312de:	enter  $0xd0a1,$0xa1
+   1800312e2:	loopne 0x180031285
+   1800312e4:	lock movabs 0xa210a208a200a1f8,%eax
+   1800312ee:	sbb    %ah,-0x5dd75de0(%rdx)
+   1800312f4:	xor    %ah,-0x5dbf5dc8(%rdx)
+   1800312fa:	rex.W movabs %al,0xa440a438a258a250
+   180031304:	rex.W movsb %ds:(%rsi),%es:(%rdi)
+   180031306:	push   %rax
+   180031307:	movsb  %ds:(%rsi),%es:(%rdi)
+   180031308:	(bad)
    180031309:	movsb  %ds:(%rsi),%es:(%rdi)
-   18003130a:	shlb   $0xa4,-0xf5b175c(%rax,%riz,8)
-   180031312:	clc
-   180031313:	movsb  %ds:(%rsi),%es:(%rdi)
-   180031314:	add    %ah,-0x5aef5af8(%rbp)
-   18003131a:	sbb    %ah,-0x5ad75ae0(%rbp)
-   180031320:	xor    %ah,-0x5abf5ac8(%rbp)
-   180031326:	movsq  %ds:(%rsi),%es:(%rdi)
-   180031328:	cmp    %ah,-0x58d759c0(%rsi)
-   18003132e:	xor    %ah,-0x57ff5818(%rdi)
-   180031334:	or     %ch,-0x57cf57f0(%rax)
-   18003133a:	nop
-   18003133b:	test   $0xa8,%al
-   18003133d:	test   $0xb0,%al
-   18003133f:	test   $0xb8,%al
-   180031341:	test   $0xc0,%al
+   18003130a:	shlb   0xa4f8a4(%rax,%rsi,8)
+   180031311:	movsl  %ds:(%rsi),%es:(%rdi)
+   180031312:	or     %ah,-0x5ae75af0(%rbp)
+   180031318:	and    %ah,-0x5acf5ad8(%rbp)
+   18003131e:	cmp    %ah,-0x5ab75ac0(%rbp)
+   180031324:	push   %rax
+   180031325:	movsl  %ds:(%rsi),%es:(%rdi)
+   180031326:	pop    %rax
+   180031327:	movsl  %ds:(%rsi),%es:(%rdi)
+   180031328:	rex.W cmpsb %es:(%rdi),%ds:(%rsi)
+   18003132a:	push   %rax
+   18003132b:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   18003132c:	cmp    %ah,-0x580758c0(%rdi)
+   180031332:	adc    %ch,-0x57df57e8(%rax)
+   180031338:	rex test $0xa0,%al
+   18003133b:	test   $0xb8,%al
+   18003133d:	test   $0xc0,%al
+   18003133f:	test   $0xc8,%al
+   180031341:	test   $0xd0,%al
    180031343:	test   $0x0,%al
    180031345:	test   $0xa910a908,%eax
    18003134a:	sbb    %ch,0x2b000(%rcx)
    180031350:	or     $0x1,%al
    180031352:	add    %al,(%rax)
    180031354:	sbb    %ah,-0x5fd75fe0(%rax)
    18003135a:	xor    %ah,-0x5fbf5fc8(%rax)
```

## Comparing `PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/LICENSE` & `PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PyQt6_NetworkAuth_Qt6-6.5.1.dist-info/METADATA` & `PyQt6_NetworkAuth_Qt6-6.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-NetworkAuth-Qt6
-Version: 6.5.1
+Version: 6.5.2
 Summary: The subset of a Qt installation needed by PyQt6-NetworkAuth.
 Home-page: https://www.riverbankcomputing.com/software/pyqt/
 Author: Riverbank Computing Limited
 Author-email: info@riverbankcomputing.com
 License: GPL v3
 Platform: Linux
 Platform: macOS
```

