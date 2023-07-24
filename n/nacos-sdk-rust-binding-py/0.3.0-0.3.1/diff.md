# Comparing `tmp/nacos_sdk_rust_binding_py-0.3.0.tar.gz` & `tmp/nacos_sdk_rust_binding_py-0.3.1.tar.gz`

## Comparing `nacos_sdk_rust_binding_py-0.3.0.tar` & `nacos_sdk_rust_binding_py-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      519 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/.gitignore
--rw-r--r--   0     1001      123    11357 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/LICENSE
--rw-r--r--   0     1001      123     6358 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/README.md
--rw-r--r--   0     1001      123       10 2023-06-16 15:27:32.000000 nacos_sdk_rust_binding_py-0.3.0/dist/nacos_sdk_rust_binding_py-0.3.0.tar.gz
--rw-r--r--   0     1001      123     1852 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/examples/config.py
--rw-r--r--   0     1001      123     1498 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/examples/naming.py
--rw-r--r--   0     1001      123      856 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123     6025 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/src/config.rs
--rw-r--r--   0     1001      123     2647 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123    11291 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/src/naming.rs
--rw-r--r--   0     1001      123      230 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/test.sh
--rw-r--r--   0     1001      123    38636 2023-06-16 15:27:29.000000 nacos_sdk_rust_binding_py-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     7286 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      519 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/LICENSE
+-rw-r--r--   0     1001      123     6358 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/README.md
+-rw-r--r--   0     1001      123       10 2023-07-24 07:06:48.000000 nacos_sdk_rust_binding_py-0.3.1/dist/nacos_sdk_rust_binding_py-0.3.1.tar.gz
+-rw-r--r--   0     1001      123     1852 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/examples/config.py
+-rw-r--r--   0     1001      123     1498 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/examples/naming.py
+-rw-r--r--   0     1001      123      856 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/pyproject.toml
+-rw-r--r--   0     1001      123     6025 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/src/config.rs
+-rw-r--r--   0     1001      123     2647 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      123    11291 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/src/naming.rs
+-rw-r--r--   0     1001      123      230 2023-07-24 07:06:41.000000 nacos_sdk_rust_binding_py-0.3.1/test.sh
+-rw-r--r--   0     1001      123    40568 2023-07-24 07:06:46.000000 nacos_sdk_rust_binding_py-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0     7286 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.3.1/PKG-INFO
```

### Comparing `nacos_sdk_rust_binding_py-0.3.0/Cargo.toml` & `nacos_sdk_rust_binding_py-0.3.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nacos-sdk-rust-binding-py"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 license = "Apache-2.0"
 publish = false
 authors = ["CheirshCai <785427346@qq.com>"]
 readme = "README.md"
 repository = "https://github.com/opc-source/nacos-sdk-rust-binding-py.git"
 description = "nacos-sdk-rust binding for Python with PyO3."
@@ -16,14 +16,14 @@
 name = "nacos_sdk_rust_binding_py"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3 = "0.18"
 
-nacos-sdk = { version = "0.3.0", features = ["default"] }
+nacos-sdk = { version = "0.3.1", features = ["default"] }
 #nacos-sdk = { git = "https://github.com/nacos-group/nacos-sdk-rust.git", features = ["default"] }
 
 tracing-subscriber = { version = "0.3", features = ["default"] }
 #tracing-subscriber = { version = "0.3", features = ["env-filter", "local-time"] } # occur `<unknown time>`
 tracing-appender = "0.2"
 lazy_static = "1.4.0"
```

### Comparing `nacos_sdk_rust_binding_py-0.3.0/.github/workflows/CI.yml` & `nacos_sdk_rust_binding_py-0.3.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/.gitignore` & `nacos_sdk_rust_binding_py-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/LICENSE` & `nacos_sdk_rust_binding_py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/README.md` & `nacos_sdk_rust_binding_py-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/examples/config.py` & `nacos_sdk_rust_binding_py-0.3.1/examples/config.py`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/examples/naming.py` & `nacos_sdk_rust_binding_py-0.3.1/examples/naming.py`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/pyproject.toml` & `nacos_sdk_rust_binding_py-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/src/config.rs` & `nacos_sdk_rust_binding_py-0.3.1/src/config.rs`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/src/lib.rs` & `nacos_sdk_rust_binding_py-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/src/naming.rs` & `nacos_sdk_rust_binding_py-0.3.1/src/naming.rs`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.3.0/Cargo.lock` & `nacos_sdk_rust_binding_py-0.3.1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 
 [[package]]
 name = "async-stream"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
@@ -23,39 +38,39 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "cc6dde6e4ed435a4c1ee4e73592f5ba9da2151af10076cc04858746af9352d09"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "axum"
-version = "0.6.18"
+version = "0.6.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8175979259124331c1d7bf6586ee7e0da434155e4b2d48ec2c8386281d8df39"
+checksum = "a6a1de45611fdb535bfde7b7de4fd54f4fd2b17b1737c0a59b69bf9b92074b8c"
 dependencies = [
  "async-trait",
  "axum-core",
  "bitflags",
  "bytes",
  "futures-util",
  "http",
@@ -89,14 +104,29 @@
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bitflags"
@@ -113,14 +143,20 @@
 [[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "crossbeam-channel"
@@ -174,30 +210,30 @@
  "darling_core",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dashmap"
-version = "5.4.0"
+version = "5.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+checksum = "6943ae99c34386c84a470c499d3414f66502a41340aa895406e0d2e4a207b91d"
 dependencies = [
  "cfg-if",
- "hashbrown",
+ "hashbrown 0.14.0",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
@@ -271,15 +307,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -316,18 +352,24 @@
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "h2"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -341,21 +383,24 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+
+[[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "home"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
 dependencies = [
@@ -394,17 +439,17 @@
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
 [[package]]
 name = "hyper"
-version = "0.14.26"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -451,43 +496,43 @@
 [[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "ipnet"
-version = "2.7.2"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
@@ -498,17 +543,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "local_ipaddress"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6a104730949fbc4c78e4fa98ed769ca0faa02e9818936b61032d2d77526afa9"
 
@@ -552,14 +597,23 @@
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "mio"
 version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "wasi",
@@ -576,17 +630,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "nacos-sdk"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c804bed6b1feec49f2113f8a273552ab37b0a13527ff9f155b56d889bfeacac0"
+checksum = "1d19dd3631dc7a59542c17c361a66a03977aeb41de930274f192f5bea3ac5b00"
 dependencies = [
  "async-stream",
  "async-trait",
  "dashmap",
  "futures",
  "futures-util",
  "home",
@@ -605,15 +659,15 @@
  "tower",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "nacos-sdk-rust-binding-py"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "lazy_static",
  "nacos-sdk",
  "pyo3",
  "tracing-appender",
  "tracing-subscriber",
 ]
@@ -626,23 +680,32 @@
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "overload"
@@ -677,37 +740,37 @@
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -715,17 +778,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
 version = "0.11.9"
@@ -816,17 +879,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -897,56 +960,62 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "5d25439cd7397d044e2748a6fe2432b5e85db703d6d097bd014b3c0ad1ebff0b"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "b23f7ade6f110613c0d63858ddb8b94c1041f550eab58a16b371bdf2c9c80ab4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.97"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -986,17 +1055,17 @@
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "socket2"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
@@ -1019,70 +1088,70 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.22"
+version = "0.3.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+checksum = "59e399c068f43a5d116fedaf73b203fa4f9c519f17e2b34f63221d3792f81446"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
@@ -1090,17 +1159,17 @@
 name = "time-core"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+checksum = "96ba15a897f3c86766b757e5ac7221554c6750054d74d5b28844fce5fb36a6c4"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
@@ -1114,19 +1183,20 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
@@ -1149,15 +1219,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
@@ -1263,21 +1333,21 @@
  "crossbeam-channel",
  "time",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.24"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -1321,17 +1391,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -1393,15 +1463,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1427,15 +1497,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -1481,17 +1551,17 @@
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
```

### Comparing `nacos_sdk_rust_binding_py-0.3.0/PKG-INFO` & `nacos_sdk_rust_binding_py-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacos-sdk-rust-binding-py
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pdoc ; extra == 'docs'
 Requires-Dist: behave ; extra == 'test'
 Provides-Extra: docs
 Provides-Extra: test
```

