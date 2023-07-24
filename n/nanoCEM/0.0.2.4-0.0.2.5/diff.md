# Comparing `tmp/nanoCEM-0.0.2.4.tar.gz` & `tmp/nanoCEM-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.2.4.tar", last modified: Fri Jul 21 02:53:22 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.2.5.tar", last modified: Mon Jul 24 04:49:01 2023, max compression
```

## Comparing `nanoCEM-0.0.2.4.tar` & `nanoCEM-0.0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.4/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10208 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9625 2023-07-20 11:04:47.000000 nanoCEM-0.0.2.4/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10148 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.4/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.4/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.4/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8385 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.4/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.4/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.4/nanoCEM/extract_sub_fastq_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.4/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.4/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.4/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.4/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10208 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      458 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1192 2023-07-21 02:53:01.000000 nanoCEM-0.0.2.4/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.5/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10233 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9650 2023-07-24 02:19:07.000000 nanoCEM-0.0.2.5/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10148 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.5/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.5/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.5/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8385 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.5/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.5/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.2.5/nanoCEM/extract_sub_fastq_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.5/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.5/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.5/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.5/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10233 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      458 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1192 2023-07-24 04:48:56.000000 nanoCEM-0.0.2.5/setup.py
```

### Comparing `nanoCEM-0.0.2.4/LICENSE` & `nanoCEM-0.0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/PKG-INFO` & `nanoCEM-0.0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
 The electric current signal level data produced from a nanopore read is referred to as a **squiggle**.
 Base calling this squiggle information generally contains some errors compared to a reference sequence. 
 The re-squiggle algorithm defines a new assignment from squiggle to reference sequence, hence a **re-squiggle**.
-Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but resquiggle is a more fine alignment than the move table in most cases.
+Although new basecall program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but re-squiggle is a more fine alignment than the move table in most cases.
 
 <center>
 
 ![alt text](example/resquiggle.png)
 
 </center>
 
@@ -69,15 +69,15 @@
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.2.0
+pip install nanoCEM==0.0.2.4
 ```
 
 Other tools if you needed
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
@@ -132,24 +132,24 @@
                         base shift if required (default:2)
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
-# q 30 is recommended but you can try other filter in your data
+# q 30 is recommended for DNA and q 5 for RNA ,but you can try other filter in your data
 # guppy is just an example, and other basecalling software such as Bonito and Dorado can also be used.
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 5 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
-In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
+In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1, and I am interested in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
```

### Comparing `nanoCEM-0.0.2.4/README.md` & `nanoCEM-0.0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
 The electric current signal level data produced from a nanopore read is referred to as a **squiggle**.
 Base calling this squiggle information generally contains some errors compared to a reference sequence. 
 The re-squiggle algorithm defines a new assignment from squiggle to reference sequence, hence a **re-squiggle**.
-Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but resquiggle is a more fine alignment than the move table in most cases.
+Although new basecall program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but re-squiggle is a more fine alignment than the move table in most cases.
 
 <center>
 
 ![alt text](example/resquiggle.png)
 
 </center>
 
@@ -55,15 +55,15 @@
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.2.0
+pip install nanoCEM==0.0.2.4
 ```
 
 Other tools if you needed
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
@@ -118,24 +118,24 @@
                         base shift if required (default:2)
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
-# q 30 is recommended but you can try other filter in your data
+# q 30 is recommended for DNA and q 5 for RNA ,but you can try other filter in your data
 # guppy is just an example, and other basecalling software such as Bonito and Dorado can also be used.
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 5 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
-In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
+In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1, and I am interested in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
```

### Comparing `nanoCEM-0.0.2.4/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.2.5/nanoCEM/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM/cem_utils.py` & `nanoCEM-0.0.2.5/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.2.5/nanoCEM/current_events_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.2.5/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM/extract_sub_fastq_from_bam` & `nanoCEM-0.0.2.5/nanoCEM/extract_sub_fastq_from_bam`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 from Bio import SeqIO
 import pysam
 import argparse
 
 def main(args):
     result_dict= {}
     # read bam
```

### Comparing `nanoCEM-0.0.2.4/nanoCEM/normalization.py` & `nanoCEM-0.0.2.5/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM/plot.py` & `nanoCEM-0.0.2.5/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.2.5/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.2.5/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.4/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.2.5/nanoCEM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
 The electric current signal level data produced from a nanopore read is referred to as a **squiggle**.
 Base calling this squiggle information generally contains some errors compared to a reference sequence. 
 The re-squiggle algorithm defines a new assignment from squiggle to reference sequence, hence a **re-squiggle**.
-Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but resquiggle is a more fine alignment than the move table in most cases.
+Although new basecall program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but re-squiggle is a more fine alignment than the move table in most cases.
 
 <center>
 
 ![alt text](example/resquiggle.png)
 
 </center>
 
@@ -69,15 +69,15 @@
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.2.0
+pip install nanoCEM==0.0.2.4
 ```
 
 Other tools if you needed
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
@@ -132,24 +132,24 @@
                         base shift if required (default:2)
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
-# q 30 is recommended but you can try other filter in your data
+# q 30 is recommended for DNA and q 5 for RNA ,but you can try other filter in your data
 # guppy is just an example, and other basecalling software such as Bonito and Dorado can also be used.
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 5 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
-In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
+In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1, and I am interested in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
```

### Comparing `nanoCEM-0.0.2.4/setup.py` & `nanoCEM-0.0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.2.4",
+    version="0.0.2.5",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

