# Comparing `tmp/fastbloom_rs-0.5.4-cp37-abi3-win_amd64.whl.zip` & `tmp/fastbloom_rs-0.5.5-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 182683 bytes, number of entries: 7
--rw-r--r--  4.6 unx    22045 b- defN 23-Jul-11 14:58 fastbloom_rs-0.5.4.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Jul-11 14:58 fastbloom_rs-0.5.4.dist-info/WHEEL
--rw-r--r--  4.6 unx     5232 b- defN 23-Jul-11 14:58 fastbloom_rs/fastbloom_rs.pyi
--rw-r--r--  4.6 unx    24510 b- defN 23-Jul-11 14:58 fastbloom_rs/filter.py
--rw-r--r--  4.6 unx      315 b- defN 23-Jul-11 14:58 fastbloom_rs/__init__.py
--rwxr-xr-x  4.6 unx   458240 b- defN 23-Jul-11 14:58 fastbloom_rs/fastbloom_rs.pyd
--rw-r--r--  4.6 unx      556 b- defN 23-Jul-11 14:58 fastbloom_rs-0.5.4.dist-info/RECORD
-7 files, 510993 bytes uncompressed, 181709 bytes compressed:  64.4%
+Zip file size: 180683 bytes, number of entries: 7
+-rw-r--r--  4.6 unx    22388 b- defN 23-Jul-24 14:27 fastbloom_rs-0.5.5.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Jul-24 14:27 fastbloom_rs-0.5.5.dist-info/WHEEL
+-rw-r--r--  4.6 unx     5232 b- defN 23-Jul-24 14:27 fastbloom_rs/fastbloom_rs.pyi
+-rw-r--r--  4.6 unx    24510 b- defN 23-Jul-24 14:27 fastbloom_rs/filter.py
+-rw-r--r--  4.6 unx      315 b- defN 23-Jul-24 14:27 fastbloom_rs/__init__.py
+-rwxr-xr-x  4.6 unx   446976 b- defN 23-Jul-24 14:27 fastbloom_rs/fastbloom_rs.pyd
+-rw-r--r--  4.6 unx      556 b- defN 23-Jul-24 14:27 fastbloom_rs-0.5.5.dist-info/RECORD
+7 files, 500072 bytes uncompressed, 179709 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: fastbloom_rs-0.5.4.dist-info/METADATA
+Filename: fastbloom_rs-0.5.5.dist-info/METADATA
 Comment: 
 
-Filename: fastbloom_rs-0.5.4.dist-info/WHEEL
+Filename: fastbloom_rs-0.5.5.dist-info/WHEEL
 Comment: 
 
 Filename: fastbloom_rs/fastbloom_rs.pyi
 Comment: 
 
 Filename: fastbloom_rs/filter.py
 Comment: 
 
 Filename: fastbloom_rs/__init__.py
 Comment: 
 
 Filename: fastbloom_rs/fastbloom_rs.pyd
 Comment: 
 
-Filename: fastbloom_rs-0.5.4.dist-info/RECORD
+Filename: fastbloom_rs-0.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fastbloom_rs-0.5.4.dist-info/METADATA` & `fastbloom_rs-0.5.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastbloom_rs
-Version: 0.5.4
+Version: 0.5.5
 Classifier: Programming Language :: Python
 Requires-Dist: pytest <= 7.1.1; extra == 'test'
 Requires-Dist: pybloom_live; extra == 'test'
 Provides-Extra: test
 Summary: Some fast bloom filter implemented by Rust for Python and Rust! 10x faster than pybloom!
 Keywords: bloom-filter,bloom,filter,bloomfilter,probabilistic data structure,counting-bloom-filter
 Home-Page: https://github.com/yankun1992/fastbloom
@@ -211,38 +211,40 @@
 	   distributed under the License is distributed on an "AS IS" BASIS,
 	   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 	   See the License for the specific language governing permissions and
 	   limitations under the License.
 	
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/yankun1992/fastbloom
 Project-URL: documentation, https://github.com/yankun1992/fastbloom/blob/main/README.md
 Project-URL: repository, https://github.com/yankun1992/fastbloom
-Project-URL: homepage, https://github.com/yankun1992/fastbloom
 
 <h1>fastbloom</h1>
 
 [![OSCS Status](https://www.oscs1024.com/platform/badge/yankun1992/fastbloom.svg?size=small)](https://www.oscs1024.com/project/yankun1992/fastbloom?ref=badge_small)
 [![docs.rs](https://img.shields.io/docsrs/fastbloom-rs/latest)](https://docs.rs/fastbloom-rs)
 [![Test Rust](https://github.com/yankun1992/fastbloom/actions/workflows/test_rust.yml/badge.svg)](https://github.com/yankun1992/fastbloom/actions/workflows/test_rust.yml)
 [![Test Python](https://github.com/yankun1992/fastbloom/actions/workflows/test_python.yml/badge.svg)](https://github.com/yankun1992/fastbloom/actions/workflows/test_python.yml)
 [![Benchmark](https://github.com/yankun1992/fastbloom/actions/workflows/benchmark.yml/badge.svg)](https://github.com/yankun1992/fastbloom/actions/workflows/benchmark.yml)
 [![Crates Latest Release](https://img.shields.io/crates/v/fastbloom-rs)](https://crates.io/crates/fastbloom-rs)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/fastbloom-rs)](https://pypi.org/project/fastbloom-rs/)
+![Sonatype Nexus (Snapshots)](https://img.shields.io/nexus/s/io.github.yankun1992/fastbloom?server=https%3A%2F%2Fs01.oss.sonatype.org)
 
 A fast [bloom filter](#BloomFilter) | [counting bloom filter](#countingbloomfilter) implemented by Rust for Rust and
 Python!
 
 Language: [简体中文](./docs/README.zh_cn.md)
 
 - [setup](#setup)
     - [Python](#python)
         - [requirements](#requirements)
         - [install](#install)
     - [Rust](#rust)
+    - [Java](#java)
 - [Examples](#examples)
     - [BloomFilter](#bloomfilter)
         - [Python](#python-1)
         - [Rust](#rust-1)
     - [CountingBloomFilter](#countingbloomfilter)
         - [Python](#python-2)
         - [Rust](#rust-2)
@@ -275,14 +277,24 @@
 
 ## Rust
 
 ```toml
 fastbloom-rs = "{latest}"
 ```
 
+## Java
+maven
+```xml
+<dependency>
+    <groupId>io.github.yankun1992</groupId>
+    <artifactId>fastbloom</artifactId>
+    <version>{latest-version}</version>
+</dependency>
+```
+
 # Examples
 
 ## BloomFilter
 
 A Bloom filter is a space-efficient probabilistic data structure, conceived by Burton Howard
 Bloom in 1970, that is used to test whether an element is a member of a set. False positive
 matches are possible, but false negatives are not.
```

