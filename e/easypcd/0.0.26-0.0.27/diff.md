# Comparing `tmp/easypcd-0.0.26-py3-none-any.whl.zip` & `tmp/easypcd-0.0.27-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3826 bytes, number of entries: 6
+Zip file size: 8283 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Jul-24 02:49 easypcd/__init__.py
--rw-rw-rw-  2.0 fat     3868 b- defN 23-Jul-24 02:36 easypcd/easypcd.py
--rw-rw-rw-  2.0 fat     2392 b- defN 23-Jul-24 06:47 easypcd-0.0.26.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 06:47 easypcd-0.0.26.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-24 06:47 easypcd-0.0.26.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      450 b- defN 23-Jul-24 06:47 easypcd-0.0.26.dist-info/RECORD
-6 files, 6856 bytes uncompressed, 3010 bytes compressed:  56.1%
+-rw-rw-rw-  2.0 fat     4681 b- defN 23-Jul-24 07:41 easypcd/easypcd.py
+-rw-rw-rw-  2.0 fat     9719 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2400 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      539 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/RECORD
+7 files, 17485 bytes uncompressed, 7327 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: easypcd/__init__.py
 Comment: 
 
 Filename: easypcd/easypcd.py
 Comment: 
 
-Filename: easypcd-0.0.26.dist-info/METADATA
+Filename: easypcd-0.0.27.dist-info/LICENSE
 Comment: 
 
-Filename: easypcd-0.0.26.dist-info/WHEEL
+Filename: easypcd-0.0.27.dist-info/METADATA
 Comment: 
 
-Filename: easypcd-0.0.26.dist-info/top_level.txt
+Filename: easypcd-0.0.27.dist-info/WHEEL
 Comment: 
 
-Filename: easypcd-0.0.26.dist-info/RECORD
+Filename: easypcd-0.0.27.dist-info/top_level.txt
+Comment: 
+
+Filename: easypcd-0.0.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## easypcd/easypcd.py

```diff
@@ -20,20 +20,24 @@
 class ep():
     def __init__(self):
         self.format_dic = {0: 'pcd', 1: "txt"}
         self.pcd_head = '# .PCD v0.7 - Point Cloud Data file format'
         self.VERSION = 'VERSION 0.7'
 
     def processing_str(self, input, s, length):
+        """功能：输入一个字符、将其增加到length长度"""
         for i in range(length):
             input += " "
             input += str(s)
         return input
 
     def read_pcd(self, pcd_file):
+        """功能：读取pcd文件
+        pcd_file：输入读取pcd文件的路径
+        """
         format_type = {"I": np.int32, "U": np.uint, "F": np.float32}
         pcd_data = []
         pcd_information = {}
         with open(pcd_file, 'r') as f:
             lines = f.readlines()
             for i in lines[1:11]:
                 info = list(i.strip('\n').split(' '))
@@ -54,14 +58,26 @@
                     pcd_data.append(tmp)
             points = np.array(pcd_data)
             pcd_information.update({"points": points})
         return DotDict(pcd_information)
 
     def write_pcd(self, save_name, points, color=False, normal=False, _SIZE=4,
                   _TYPE="F", _COUNT=1, _HEIGHT=1, _VIEWPOINT='0 0 0 1 0 0 0', _DATA='ascii'):
+        """功能：写入pcd文件
+            必要参数：
+                save_name:保存的文件名
+                points：需要保存的点云数据
+
+            可选参数
+                color：是否有颜色信息（True/False），默认False
+                normal：是否有向量信息（True/False），默认False
+                _SIZE：字节数量，默认为4
+                _TYPE：字符类型，默认为F
+                _DATA：编码格式
+        """
         if color == True and normal == False:
             length = 6
             FIELDS = "FIELDS x y z r g b"
         if color == False and normal == False:
             length = 3
             FIELDS = "FIELDS x y z"
         if color == False and normal == True:
@@ -87,21 +103,25 @@
             with open(save_name, mode='w') as f:
                 for i in pcd_init:
                     f.write(pcd_init[i] + '\n')
                 np.savetxt(f, points, delimiter=' ', fmt='%d')
         except:
             assert "一个未知的错误！"
 
-    def write_txt(self, points, save_name):
+    def write_txt(self, save_name, points):
+        """功能：写入txt文件
+            save_name:保存的文件名
+            points：需要保存的点云数据
+        """
         with open(save_name, mode='w') as f:
             for line in points:
                 for p in line:
                     p = str(int(p))
                     f.write(p)
                     f.write(" ")
                 f.write("\n")
 
 
 if __name__ == '__main__':
-    easypcd1 = easypcd()
+    easypcd1 = ep()
     pcd = easypcd1.read_pcd("point.pcd")
     easypcd1.write_pcd("1.pcd", pcd.points, True, True)
```

## Comparing `easypcd-0.0.26.dist-info/METADATA` & `easypcd-0.0.27.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: easypcd
-Version: 0.0.26
+Version: 0.0.27
 Summary: a package for pcd
-Home-page: https://blog.csdn.net/qq_18566467?spm=1010.2135.3001.5343
+Home-page: https://gitee.com/wang2wan/easypcd_project
 Author: GentleWang
 Author-email: 189030005@stu.just.edu.cn
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 
 #### Easypcd使你更专注与代码本身，而不需要因为pcd格式所带来的烦恼。  
 
 **1、 调用easypcd**  
 `from easypcd import ep`  
 `import open3d as o3d`
```

