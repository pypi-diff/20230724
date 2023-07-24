# Comparing `tmp/peakrdl-euvm-1.0.tar.gz` & `tmp/peakrdl-euvm-1.1.tar.gz`

## Comparing `peakrdl-euvm-1.0.tar` & `peakrdl-euvm-1.1.tar`

### file list

```diff
@@ -1,121 +1,44 @@
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:47:51.000000 peakrdl-euvm-1.0/
--rw-rw-r--   0 kun       (1000) kun       (1000)     1858 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.gitignore
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:41:59.000000 peakrdl-euvm-1.0/test/
--rwxrwxr-x   0 kun       (1000) kun       (1000)      888 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/run.sh
--rw-rw-r--   0 kun       (1000) kun       (1000)    18135 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/pylint.rc
--rw-rw-r--   0 kun       (1000) kun       (1000)       21 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/.gitignore
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/testcases/
--rw-rw-r--   0 kun       (1000) kun       (1000)     1320 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/testcases/basic.rdl
--rw-rw-r--   0 kun       (1000) kun       (1000)       11 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/testcases/.gitignore
--rwxrwxr-x   0 kun       (1000) kun       (1000)      366 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/vsim_test.sh
--rwxrwxr-x   0 kun       (1000) kun       (1000)      374 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/rdl_to_uvm.py
--rw-rw-r--   0 kun       (1000) kun       (1000)     4060 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/test/generate_testcase_data.py
--rw-rw-r--   0 kun       (1000) kun       (1000)     2508 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/README.md
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:48:12.000000 peakrdl-euvm-1.0/.git/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/info/
--rw-rw-r--   0 kun       (1000) kun       (1000)      240 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/info/exclude
--rw-rw-r--   0 kun       (1000) kun       (1000)      112 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/packed-refs
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/logs/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/logs/refs/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/logs/refs/remotes/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:35:48.000000 peakrdl-euvm-1.0/.git/logs/refs/remotes/origin/
--rw-rw-r--   0 kun       (1000) kun       (1000)      320 2023-07-24 09:42:33.000000 peakrdl-euvm-1.0/.git/logs/refs/remotes/origin/main
--rw-rw-r--   0 kun       (1000) kun       (1000)      208 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/logs/refs/remotes/origin/HEAD
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/logs/refs/heads/
--rw-rw-r--   0 kun       (1000) kun       (1000)      767 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/logs/refs/heads/main
--rw-rw-r--   0 kun       (1000) kun       (1000)      767 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/logs/HEAD
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/branches/
--rw-rw-r--   0 kun       (1000) kun       (1000)       30 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/COMMIT_EDITMSG
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/refs/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/refs/remotes/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:42:33.000000 peakrdl-euvm-1.0/.git/refs/remotes/origin/
--rw-rw-r--   0 kun       (1000) kun       (1000)       41 2023-07-24 09:42:33.000000 peakrdl-euvm-1.0/.git/refs/remotes/origin/main
--rw-rw-r--   0 kun       (1000) kun       (1000)       30 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/refs/remotes/origin/HEAD
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/refs/tags/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/refs/heads/
--rw-rw-r--   0 kun       (1000) kun       (1000)       41 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/refs/heads/main
--rw-rw-r--   0 kun       (1000) kun       (1000)     2614 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/index
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/
--rwxrwxr-x   0 kun       (1000) kun       (1000)     4655 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/fsmonitor-watchman.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)     4898 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/pre-rebase.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)      189 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/post-update.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)     1374 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/pre-push.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)      424 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/pre-applypatch.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)     1643 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/pre-commit.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)      544 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/pre-receive.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)     3650 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/update.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)      478 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/applypatch-msg.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)      416 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/pre-merge-commit.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)     2783 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/push-to-checkout.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)     1492 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/prepare-commit-msg.sample
--rwxrwxr-x   0 kun       (1000) kun       (1000)      896 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/hooks/commit-msg.sample
--rw-rw-r--   0 kun       (1000) kun       (1000)       21 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/HEAD
--rw-rw-r--   0 kun       (1000) kun       (1000)      267 2023-07-24 08:29:21.000000 peakrdl-euvm-1.0/.git/config
--rw-rw-r--   0 kun       (1000) kun       (1000)       73 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/description
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:35.000000 peakrdl-euvm-1.0/.git/objects/info/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:27:25.000000 peakrdl-euvm-1.0/.git/objects/a1/
--r--r--r--   0 kun       (1000) kun       (1000)      801 2023-07-24 08:27:25.000000 peakrdl-euvm-1.0/.git/objects/a1/846b11964d3bdb73f0222b0a8f21d0c61db953
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/87/
--r--r--r--   0 kun       (1000) kun       (1000)       55 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/87/baefbeffb8cfdf3f89b7b2b2f63e93aa44f66c
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/19/
--r--r--r--   0 kun       (1000) kun       (1000)      177 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/19/bfe48f59c6325d8e770e8dc55c11cac079f85f
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:28:07.000000 peakrdl-euvm-1.0/.git/objects/2b/
--r--r--r--   0 kun       (1000) kun       (1000)     1274 2023-07-24 08:28:07.000000 peakrdl-euvm-1.0/.git/objects/2b/30bade6fdb14520203cba2f02cd43fc6ee9281
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:27:51.000000 peakrdl-euvm-1.0/.git/objects/3a/
--r--r--r--   0 kun       (1000) kun       (1000)      244 2023-07-24 08:27:51.000000 peakrdl-euvm-1.0/.git/objects/3a/ed79321caf4e910a6eb351b505d13c68288d8e
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:27:51.000000 peakrdl-euvm-1.0/.git/objects/3c/
--r--r--r--   0 kun       (1000) kun       (1000)      184 2023-07-24 08:27:51.000000 peakrdl-euvm-1.0/.git/objects/3c/2ff676b48215ec3c4995e893d1c08c5444e68d
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/objects/pack/
--r--r--r--   0 kun       (1000) kun       (1000)     1996 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/objects/pack/pack-89e9e1c9af1acd0477ce795848e0d35603706e0f.idx
--r--r--r--   0 kun       (1000) kun       (1000)    33121 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/.git/objects/pack/pack-89e9e1c9af1acd0477ce795848e0d35603706e0f.pack
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/eb/
--r--r--r--   0 kun       (1000) kun       (1000)      177 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/eb/f02c61965ef9812e0313131a4fbca8836a4a94
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/c5/
--r--r--r--   0 kun       (1000) kun       (1000)       54 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/c5/362e16396508a4a9ec96435d59f07c59b5d2f3
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/64/
--r--r--r--   0 kun       (1000) kun       (1000)      225 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/64/23863cc8837f1d6789487343b19b3fb4d24cb8
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/7b/
--r--r--r--   0 kun       (1000) kun       (1000)      225 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/7b/b9cba7d6d06b742b9ef156fe92dbdac58504ac
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/a5/
--r--r--r--   0 kun       (1000) kun       (1000)      244 2023-07-24 09:42:25.000000 peakrdl-euvm-1.0/.git/objects/a5/ecdf7ed2fe18d363fde6cfda3fada892832e2e
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/80/
--r--r--r--   0 kun       (1000) kun       (1000)      264 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/80/d42ef48a865417d56eb47c21bba206206b9d3e
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:28:09.000000 peakrdl-euvm-1.0/.git/objects/f5/
--r--r--r--   0 kun       (1000) kun       (1000)      923 2023-07-24 08:28:09.000000 peakrdl-euvm-1.0/.git/objects/f5/1facb8c07958fe98cc125191f06d00d7aa5e86
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:41:33.000000 peakrdl-euvm-1.0/.git/objects/48/
--r--r--r--   0 kun       (1000) kun       (1000)       36 2023-07-24 09:41:33.000000 peakrdl-euvm-1.0/.git/objects/48/02e90f8edc38346215a3277cf96f0fa7474c32
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/4f/
--r--r--r--   0 kun       (1000) kun       (1000)      245 2023-07-24 08:28:32.000000 peakrdl-euvm-1.0/.git/objects/4f/7c9da3560981d6f1c226cf43f8fda875a9d16f
--rw-rw-r--   0 kun       (1000) kun       (1000)     1893 2023-07-24 07:47:53.000000 peakrdl-euvm-1.0/setup.py
--rw-rw-r--   0 kun       (1000) kun       (1000)       72 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/MANIFEST.in
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:15:10.000000 peakrdl-euvm-1.0/src/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:28:44.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/
--rw-rw-r--   0 kun       (1000) kun       (1000)     1816 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__peakrdl__.py
--rw-rw-r--   0 kun       (1000) kun       (1000)       20 2023-07-24 09:28:44.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__about__.py
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:25:52.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/
--rw-rw-r--   0 kun       (1000) kun       (1000)     3708 2023-07-24 08:25:48.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_reg_block-mem.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     2508 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_vreg.d
--rw-rw-r--   0 kun       (1000) kun       (1000)      893 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/main.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     5766 2023-07-24 08:25:52.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_reg.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     1371 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/utils.d
--rw-rw-r--   0 kun       (1000) kun       (1000)      119 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/top_include.d
--rw-rw-r--   0 kun       (1000) kun       (1000)      187 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/top_pkg.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     4414 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_reg_block.d
--rw-rw-r--   0 kun       (1000) kun       (1000)       71 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__init__.py
--rw-rw-r--   0 kun       (1000) kun       (1000)     1255 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/pre_export_listener.py
--rw-rw-r--   0 kun       (1000) kun       (1000)    15683 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/exporter.py
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 08:15:35.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/
--rw-rw-r--   0 kun       (1000) kun       (1000)      191 2023-07-24 08:15:35.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/__about__.cpython-310.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)      259 2023-07-24 08:15:35.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)    10858 2023-07-24 08:15:35.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/exporter.cpython-310.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)     1866 2023-07-24 08:15:35.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/pre_export_listener.cpython-310.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)     1956 2023-07-24 08:15:35.000000 peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/__peakrdl__.cpython-310.pyc
-drwxr-xr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 09:33:13.000000 peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/
--rw-r--r--   0 kun       (1000) kun       (1000)      752 2023-07-24 09:33:13.000000 peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/SOURCES.txt
--rw-r--r--   0 kun       (1000) kun       (1000)       13 2023-07-24 09:33:13.000000 peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/top_level.txt
--rw-r--r--   0 kun       (1000) kun       (1000)        1 2023-07-24 09:33:13.000000 peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/dependency_links.txt
--rw-r--r--   0 kun       (1000) kun       (1000)     3751 2023-07-24 09:33:13.000000 peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/PKG-INFO
--rw-r--r--   0 kun       (1000) kun       (1000)       62 2023-07-24 09:33:13.000000 peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/entry_points.txt
--rw-r--r--   0 kun       (1000) kun       (1000)       34 2023-07-24 09:33:13.000000 peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/requires.txt
--rw-rw-r--   0 kun       (1000) kun       (1000)    35149 2023-07-24 06:49:36.000000 peakrdl-euvm-1.0/LICENSE
+drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:10:12.000000 peakrdl-euvm-1.1/
+drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/
+-rwxrwxr-x   0 kun       (1000) kun       (1000)      888 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/run.sh
+-rw-rw-r--   0 kun       (1000) kun       (1000)    18135 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/pylint.rc
+-rw-rw-r--   0 kun       (1000) kun       (1000)       21 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/.gitignore
+drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/testcases/
+-rw-rw-r--   0 kun       (1000) kun       (1000)     1320 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/testcases/basic.rdl
+-rw-rw-r--   0 kun       (1000) kun       (1000)       11 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/testcases/.gitignore
+-rwxrwxr-x   0 kun       (1000) kun       (1000)      366 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/vsim_test.sh
+-rwxrwxr-x   0 kun       (1000) kun       (1000)      374 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/rdl_to_uvm.py
+-rw-rw-r--   0 kun       (1000) kun       (1000)     4060 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/generate_testcase_data.py
+-rw-rw-r--   0 kun       (1000) kun       (1000)     2508 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/README.md
+-rw-rw-r--   0 kun       (1000) kun       (1000)     1893 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/setup.py
+-rw-rw-r--   0 kun       (1000) kun       (1000)       72 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/MANIFEST.in
+drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/
+drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:03:55.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/
+-rw-rw-r--   0 kun       (1000) kun       (1000)     1816 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__peakrdl__.py
+-rw-rw-r--   0 kun       (1000) kun       (1000)       20 2023-07-24 11:03:32.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__about__.py
+drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:49:09.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/
+-rw-rw-r--   0 kun       (1000) kun       (1000)     3411 2023-07-24 10:48:59.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg_block-mem.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)     2509 2023-07-24 10:28:39.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_vreg.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)      893 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/main.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)     5472 2023-07-24 10:49:09.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)     1369 2023-07-24 10:10:13.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/utils.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)      119 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/top_include.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)      212 2023-07-24 10:29:29.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/top_pkg.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)     3996 2023-07-24 10:48:38.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg_block.d
+-rw-rw-r--   0 kun       (1000) kun       (1000)       71 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__init__.py
+-rw-rw-r--   0 kun       (1000) kun       (1000)     1255 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/pre_export_listener.py
+-rw-rw-r--   0 kun       (1000) kun       (1000)    15683 2023-07-24 10:45:31.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/exporter.py
+drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:49:45.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/
+-rw-rw-r--   0 kun       (1000) kun       (1000)     1908 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/pre_export_listener.cpython-38.pyc
+-rw-rw-r--   0 kun       (1000) kun       (1000)      227 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 kun       (1000) kun       (1000)    10802 2023-07-24 10:49:45.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/exporter.cpython-38.pyc
+-rw-rw-r--   0 kun       (1000) kun       (1000)     1899 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/__peakrdl__.cpython-38.pyc
+-rw-rw-r--   0 kun       (1000) kun       (1000)      157 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/__about__.cpython-38.pyc
+drwxr-xr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/
+-rw-r--r--   0 kun       (1000) kun       (1000)      752 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/SOURCES.txt
+-rw-r--r--   0 kun       (1000) kun       (1000)       13 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/top_level.txt
+-rw-r--r--   0 kun       (1000) kun       (1000)        1 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/dependency_links.txt
+-rw-r--r--   0 kun       (1000) kun       (1000)     3751 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/PKG-INFO
+-rw-r--r--   0 kun       (1000) kun       (1000)       62 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/entry_points.txt
+-rw-r--r--   0 kun       (1000) kun       (1000)       34 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/requires.txt
+-rw-rw-r--   0 kun       (1000) kun       (1000)    35149 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/LICENSE
```

### Comparing `peakrdl-euvm-1.0/test/run.sh` & `peakrdl-euvm-1.1/test/run.sh`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/test/pylint.rc` & `peakrdl-euvm-1.1/test/pylint.rc`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/test/testcases/basic.rdl` & `peakrdl-euvm-1.1/test/testcases/basic.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/test/generate_testcase_data.py` & `peakrdl-euvm-1.1/test/generate_testcase_data.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/README.md` & `peakrdl-euvm-1.1/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/setup.py` & `peakrdl-euvm-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/__peakrdl__.py` & `peakrdl-euvm-1.1/src/peakrdl_euvm/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_reg_block-mem.d` & `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg_block-mem.d`

 * *Files 11% similar despite different names*

```diff
@@ -57,24 +57,24 @@
 
 
 //------------------------------------------------------------------------------
 // build() actions for uvm_reg_block instance (called by parent)
 //------------------------------------------------------------------------------
 {% macro build_instance(node) -%}
 {%- if node.is_array %}
-foreach(this.{{get_inst_name(node)}}[{{utils.array_iterator_list(node)}}]) begin
+foreach (uint {{utils.array_iterator_list(node)}}, ref inst; this.{{get_inst_name(node)}}) {
     {%- if use_uvm_factory %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}} = {{get_class_name(node)}}.type_id.create($sformatf("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
+    inst = {{get_class_name(node)}}.type_id.create(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
     {%- else %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}} = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
+    inst = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
     {%- endif %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.configure(this);
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.build();
-    this.default_map.add_submap(this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.default_map, {{get_array_address_offset_expr(node)}});
-end
+    inst.configure(this);
+    inst.build();
+    this.default_map.add_submap(inst.default_map, {{get_array_address_offset_expr(node)}});
+ }
 {%- else %}
 {%- if use_uvm_factory %}
 this.{{get_inst_name(node)}} = {{get_class_name(node)}}.type_id.create("{{get_inst_name(node)}}");
 {%- else %}
 this.{{get_inst_name(node)}} = new {{get_class_name(node)}}("{{get_inst_name(node)}}");
 {%- endif %}
 this.{{get_inst_name(node)}}.configure(this);
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_vreg.d` & `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_vreg.d`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 
 //------------------------------------------------------------------------------
 // build() function
 //------------------------------------------------------------------------------
 {% macro function_build(node) -%}
-void build(){
+void build() {
     {%- for field in node.fields() %}
     {%- if use_uvm_factory %}
     this.{{get_inst_name(field)}} = uvm_vreg_field.type_id.create("{{get_inst_name(field)}}");
     {%- else %}
     this.{{get_inst_name(field)}} = new uvm_vreg_field("{{get_inst_name(field)}}");
     {%- endif %}
     this.{{get_inst_name(field)}}.configure(this, {{field.width}}, {{field.lsb}});
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/templates/main.d` & `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/main.d`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_reg.d` & `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg.d`

 * *Files 4% similar despite different names*

```diff
@@ -39,43 +39,43 @@
 {%- endmacro %}
 
 
 //------------------------------------------------------------------------------
 // build() function
 //------------------------------------------------------------------------------
 {% macro function_build(node) -%}
-void build(){
+void build() {
     {%- for field in node.fields() %}
     {%- if use_uvm_factory %}
     this.{{get_inst_name(field)}} = uvm_reg_field.type_id.create("{{get_inst_name(field)}}");
     {%- else %}
     this.{{get_inst_name(field)}} = new uvm_reg_field("{{get_inst_name(field)}}");
     {%- endif %}
-    this.{{get_inst_name(field)}}.configure(this, {{field.width}}, {{field.lsb}}, "{{get_field_access(field)}}", {{field.is_volatile|lower}},cast(uvm_reg_data_t) {{"0b%x" % field.get_property('reset', default=0)}}, {{field.get_property('reset') is not none|int}}, 1, 0);
+    this.{{get_inst_name(field)}}.configure(this, {{field.width}}, {{field.lsb}}, "{{get_field_access(field)}}", {{field.is_volatile|lower}},cast(uvm_reg_data_t) {{"0x%x" % field.get_property('reset', default=0)}}, {{field.get_property('reset') is not none|int}}, 1, 0);
     {%- endfor %}
 }
 {%- endmacro %}
 
 
 //------------------------------------------------------------------------------
 // build() actions for uvm_reg instance (called by parent)
 //------------------------------------------------------------------------------
 {% macro build_instance(node) -%}
 {%- if node.is_array %}
-foreach(this.{{get_inst_name(node)}}[{{utils.array_iterator_list(node)}}]) begin
+foreach (uint {{utils.array_iterator_list(node)}}, ref inst; this.{{get_inst_name(node)}}) {
     {%- if use_uvm_factory %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}} = {{get_class_name(node)}}.type_id.create(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
+    inst = {{get_class_name(node)}}.type_id.create(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
     {%- else %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}} = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
+    inst = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
     {%- endif %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.configure(this);
+    inst.configure(this);
     {{add_hdl_path_slices(node, get_inst_name(node) + utils.array_iterator_suffix(node))|trim|indent}}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.build();
-    this.default_map.add_reg(this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}, {{get_array_address_offset_expr(node)}});
-end
+    inst.build();
+    this.default_map.add_reg(inst, {{get_array_address_offset_expr(node)}});
+}
 {%- else %}
 {%- if use_uvm_factory %}
 this.{{get_inst_name(node)}} = {{get_class_name(node)}}.type_id.create("{{get_inst_name(node)}}");
 {%- else %}
 this.{{get_inst_name(node)}} = new {{get_class_name(node)}}("{{get_inst_name(node)}}");
 {%- endif %}
 this.{{get_inst_name(node)}}.configure(this);
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/templates/utils.d` & `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/utils.d`

 * *Files 4% similar despite different names*

```diff
@@ -49,8 +49,7 @@
 {% macro array_suffix_format(node) -%}
     {%- if node.is_array -%}
         {%- for _ in node.array_dimensions -%}
             {{- "[%0d]" -}}
         {%- endfor -%}
     {%- endif -%}
 {%- endmacro %}
-`
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/templates/uvm_reg_block.d` & `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg_block.d`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,33 @@
 
 //------------------------------------------------------------------------------
 // uvm_reg_block definition
 //------------------------------------------------------------------------------
 {% macro class_definition(node) -%}
 {%- if class_needs_definition(node) %}
 // {{get_class_friendly_name(node)}}
-class {{get_class_name(node)}}: uvm_reg_block{
+class {{get_class_name(node)}}: uvm_reg_block {
 {%- if use_uvm_factory %}
  mixin uvm_object_utils;
 {%- endif %}
     {{child_insts(node)|indent}}
     {{function_new(node)|indent}}
 
     {{function_build(node)|indent}}
-    
 }
 {% endif -%}
 {%- endmacro %}
 
 
 //------------------------------------------------------------------------------
 // Child instances
 //------------------------------------------------------------------------------
 {% macro child_insts(node) -%}
 {%- for child in node.children() if isinstance(child, AddressableNode) -%}
-@rand {{get_class_name(child)}} {{get_inst_name(child)}}{{utils.array_inst_suffix(child)}};
+@rand {{get_class_name(child)}}{{utils.array_inst_suffix(child)}} {{get_inst_name(child)}};
 {% endfor -%}
 {%- endmacro %}
 
 
 //------------------------------------------------------------------------------
 // new() function
 //------------------------------------------------------------------------------
@@ -40,15 +39,15 @@
 {%- endmacro %}
 
 
 //------------------------------------------------------------------------------
 // build() function
 //------------------------------------------------------------------------------
 {% macro function_build(node) -%}
-void build(){
+void build() {
     this.default_map = create_map("reg_map", 0, {{get_bus_width(node)}}, {{get_endianness(node)}});
     {%- for child in node.children() -%}
         {%- if isinstance(child, RegNode) -%}
             {{uvm_reg.build_instance(child)|indent}}
         {%- elif isinstance(child, (RegfileNode, AddrmapNode)) -%}
             {{build_instance(child)|indent}}
         {%- elif isinstance(child, MemNode) -%}
@@ -60,31 +59,31 @@
 
 
 //------------------------------------------------------------------------------
 // build() actions for uvm_reg_block instance (called by parent)
 //------------------------------------------------------------------------------
 {% macro build_instance(node) -%}
 {%- if node.is_array %}
-foreach(this.{{get_inst_name(node)}}[{{utils.array_iterator_list(node)}}]) begin
+foreach (uint {{utils.array_iterator_list(node)}}, ref inst; this.{{get_inst_name(node)}}) {
     {%- if use_uvm_factory %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}} = {{get_class_name(node)}}.type_id.create(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}",{{utils.array_iterator_list(node)}}));
+    inst = {{get_class_name(node)}}.type_id.create(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
     {%- else %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}} = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
+    inst = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
     {%- endif %}
     {%- if node.get_property('hdl_path') %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.configure(this, "{{node.get_property('hdl_path')}}");
+    inst.configure(this, "{{node.get_property('hdl_path')}}");
     {%- else %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.configure(this);
+    inst.configure(this);
     {%- endif %}
     {%- if node.get_property('hdl_path_gate') %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.add_hdl_path("{{node.get_property('hdl_path_gate')}}", "GATE");
+    inst.add_hdl_path("{{node.get_property('hdl_path_gate')}}", "GATE");
     {%- endif %}
-    this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.build();
-    this.default_map.add_submap(this.{{get_inst_name(node)}}{{utils.array_iterator_suffix(node)}}.default_map, {{get_array_address_offset_expr(node)}});
-end
+    inst.build();
+    this.default_map.add_submap(inst.default_map, {{get_array_address_offset_expr(node)}});
+ }
 {%- else %}
 {%- if use_uvm_factory %}
 this.{{get_inst_name(node)}} = {{get_class_name(node)}}.type_id.create("{{get_inst_name(node)}}");
 {%- else %}
 this.{{get_inst_name(node)}} = new {{get_class_name(node)}}("{{get_inst_name(node)}}");
 {%- endif %}
 {%- if node.get_property('hdl_path') %}
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/pre_export_listener.py` & `peakrdl-euvm-1.1/src/peakrdl_euvm/pre_export_listener.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/exporter.py` & `peakrdl-euvm-1.1/src/peakrdl_euvm/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,21 +391,21 @@
         """
         Returns an expression to calculate the address offset
         for example, a 4-dimensional array allocated as:
             [A][B][C][D] @ X += Y
         results in:
             X + i0*B*C*D*Y + i1*C*D*Y + i2*D*Y + i3*Y
         """
-        s = "'h%x" % node.raw_address_offset
+        s = "0x%x" % node.raw_address_offset
         if node.is_array:
             for i in range(len(node.array_dimensions)):
                 m = node.array_stride
                 for j in range(i+1, len(node.array_dimensions)):
                     m *= node.array_dimensions[j]
-                s += " + i%d*'h%x" % (i, m)
+                s += " + i%d*0x%x" % (i, m)
         return s
 
 
     def _get_endianness(self, node: Node) -> str:
         amap = node.owning_addrmap
         if amap.get_property("bigendian"):
             return "UVM_BIG_ENDIAN"
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/exporter.cpython-310.pyc` & `peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/exporter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 06:49:36 2023 UTC, .py size: 15683 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 001f be64 433d 0000  o..........dC=..
+00000000: 550d 0d0a 0000 0000 4b56 be64 433d 0000  U.......KV.dC=..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c06 6d07 5a07 6d08 5a08  Z.d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6404 6c06 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
@@ -20,660 +20,657 @@
 00000130: 7265 7373 6162 6c65 4e6f 6465 2903 da0a  ressableNode)...
 00000140: 4163 6365 7373 5479 7065 da0a 4f6e 5265  AccessType..OnRe
 00000150: 6164 5479 7065 da0b 4f6e 5772 6974 6554  adType..OnWriteT
 00000160: 7970 6529 01da 0452 6f6f 7429 01da 0952  ype)...Root)...R
 00000170: 444c 5761 6c6b 6572 e901 0000 0029 01da  DLWalker.....)..
 00000180: 1150 7265 4578 706f 7274 4c69 7374 656e  .PreExportListen
 00000190: 6572 6300 0000 0000 0000 0000 0000 0000  erc.............
-000001a0: 0000 0008 0000 0040 0000 0073 3801 0000  .......@...s8...
+000001a0: 0000 0005 0000 0040 0000 0073 1601 0000  .......@...s....
 000001b0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
-000001c0: 6403 6504 6404 6505 6604 6405 6406 8404  d.e.d.e.f.d.d...
-000001d0: 5a06 6404 6505 6407 6505 6604 6408 6409  Z.d.e.d.e.f.d.d.
-000001e0: 8404 5a07 6404 6505 6407 6505 6604 640a  ..Z.d.e.d.e.f.d.
-000001f0: 640b 8404 5a08 6403 6504 6407 6505 6604  d...Z.d.e.d.e.f.
-00000200: 640c 640d 8404 5a09 642d 6403 6504 640f  d.d...Z.d-d.e.d.
-00000210: 6505 6407 650a 6505 1900 6606 6410 6411  e.d.e.e...f.d.d.
-00000220: 8405 5a0b 6403 6504 6407 6505 6604 6412  ..Z.d.e.d.e.f.d.
-00000230: 6413 8404 5a0c 6403 6504 6407 6505 6604  d...Z.d.e.d.e.f.
-00000240: 6414 6415 8404 5a0d 6403 6504 6407 6505  d.d...Z.d.e.d.e.
-00000250: 6604 6416 6417 8404 5a0e 6403 6504 6407  f.d.d...Z.d.e.d.
-00000260: 650f 6604 6418 6419 8404 5a10 641a 6511  e.f.d.d...Z.d.e.
-00000270: 6407 6505 6604 641b 641c 8404 5a12 641d  d.e.f.d.d...Z.d.
-00000280: 6513 6407 6505 6604 641e 641f 8404 5a14  e.d.e.f.d.d...Z.
-00000290: 6403 6515 6407 6505 6604 6420 6421 8404  d.e.d.e.f.d d!..
-000002a0: 5a16 6403 6504 6407 6505 6604 6422 6423  Z.d.e.d.e.f.d"d#
-000002b0: 8404 5a17 6403 6504 6407 6518 6604 6424  ..Z.d.e.d.e.f.d$
-000002c0: 6425 8404 5a19 6426 6518 6427 6518 6407  d%..Z.d&e.d'e.d.
-000002d0: 6518 6606 6428 6429 8404 5a1a 642a 642b  e.f.d(d)..Z.d*d+
-000002e0: 8400 5a1b 642c 5300 292e da0c 6555 564d  ..Z.d,S.)...eUVM
-000002f0: 4578 706f 7274 6572 6301 0000 0000 0000  Exporterc.......
-00000300: 0000 0000 0004 0000 000d 0000 004b 0000  .............K..
-00000310: 0073 1201 0000 7c01 a000 6401 6402 a102  .s....|...d.d...
-00000320: 7d02 7c01 a000 6403 6900 a102 7c00 5f01  }.|...d.i...|._.
-00000330: 7c01 721b 7402 6404 7403 7c01 a004 a100  |.r.t.d.t.|.....
-00000340: 8301 6405 1900 1600 8301 8201 7c02 724c  ..d.........|.rL
-00000350: 7405 a006 7405 a007 7c02 a101 7405 a007  t...t...|...t...
-00000360: 7408 6a09 a00a 7408 6a09 a00b 740c a101  t.j...t.j...t...
-00000370: 6406 a102 a101 7405 6a0d 7405 a007 7c02  d.....t.j.t...|.
-00000380: a101 7405 a007 7408 6a09 a00a 7408 6a09  ..t...t.j...t.j.
-00000390: a00b 740c a101 6406 a102 a101 6407 9c02  ..t...d.....d...
-000003a0: 6408 6409 8d02 6703 a101 7d03 6e26 7405  d.d...g...}.n&t.
-000003b0: a006 7405 a007 7408 6a09 a00a 7408 6a09  ..t...t.j...t.j.
-000003c0: a00b 740c a101 6406 a102 a101 7405 6a0d  ..t...d.....t.j.
-000003d0: 640a 7405 a007 7408 6a09 a00a 7408 6a09  d.t...t.j...t.j.
-000003e0: a00b 740c a101 6406 a102 a101 6901 6408  ..t...d.....i.d.
-000003f0: 6409 8d02 6702 a101 7d03 7405 6a0e 7c03  d...g...}.t.j.|.
-00000400: 7405 6a0f 640b 8d02 7c00 5f10 6402 7c00  t.j.d...|._.d.|.
-00000410: 5f11 6900 7c00 5f12 6900 7c00 5f13 640c  _.i.|._.i.|._.d.
-00000420: 7c00 5f14 6402 5300 290d 6143 0100 000a  |._.d.S.).aC....
-00000430: 2020 2020 2020 2020 436f 6e73 7472 7563          Construc
-00000440: 746f 7220 666f 7220 7468 6520 6555 564d  tor for the eUVM
-00000450: 2045 7870 6f72 7465 7220 636c 6173 730a   Exporter class.
-00000460: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00000470: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00000480: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2075  ------.        u
-00000490: 7365 725f 7465 6d70 6c61 7465 5f64 6972  ser_template_dir
-000004a0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000004b0: 2020 5061 7468 2074 6f20 6120 6469 7265    Path to a dire
-000004c0: 6374 6f72 7920 7768 6572 6520 7573 6572  ctory where user
-000004d0: 2d64 6566 696e 6564 2074 656d 706c 6174  -defined templat
-000004e0: 6520 6f76 6572 7269 6465 7320 6172 6520  e overrides are 
-000004f0: 7374 6f72 6564 2e0a 2020 2020 2020 2020  stored..        
-00000500: 7573 6572 5f74 656d 706c 6174 655f 636f  user_template_co
-00000510: 6e74 6578 743a 2064 6963 740a 2020 2020  ntext: dict.    
-00000520: 2020 2020 2020 2020 4164 6469 7469 6f6e          Addition
-00000530: 616c 2063 6f6e 7465 7874 2076 6172 6961  al context varia
-00000540: 626c 6573 2074 6f20 6c6f 6164 2069 6e74  bles to load int
-00000550: 6f20 7468 6520 7465 6d70 6c61 7465 206e  o the template n
-00000560: 616d 6573 7061 6365 2e0a 2020 2020 2020  amespace..      
-00000570: 2020 da11 7573 6572 5f74 656d 706c 6174    ..user_templat
-00000580: 655f 6469 724e da15 7573 6572 5f74 656d  e_dirN..user_tem
-00000590: 706c 6174 655f 636f 6e74 6578 74fa 2767  plate_context.'g
-000005a0: 6f74 2061 6e20 756e 6578 7065 6374 6564  ot an unexpected
-000005b0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-000005c0: 7420 2725 7327 7201 0000 00da 0974 656d  t '%s'r......tem
-000005d0: 706c 6174 6573 2902 da04 7573 6572 da04  plates)...user..
-000005e0: 6261 7365 fa01 3a29 01da 0964 656c 696d  base..:)...delim
-000005f0: 6974 6572 7218 0000 0029 02da 066c 6f61  iterr....)...loa
-00000600: 6465 72da 0975 6e64 6566 696e 6564 5429  der..undefinedT)
-00000610: 15da 0370 6f70 7214 0000 00da 0954 7970  ...popr......Typ
-00000620: 6545 7272 6f72 da04 6c69 7374 da04 6b65  eError..list..ke
-00000630: 7973 da02 6a6a da0c 4368 6f69 6365 4c6f  ys..jj..ChoiceLo
-00000640: 6164 6572 da10 4669 6c65 5379 7374 656d  ader..FileSystem
-00000650: 4c6f 6164 6572 da02 6f73 da04 7061 7468  Loader..os..path
-00000660: da04 6a6f 696e da07 6469 726e 616d 65da  ..join..dirname.
-00000670: 085f 5f66 696c 655f 5fda 0c50 7265 6669  .__file__..Prefi
-00000680: 784c 6f61 6465 72da 0b45 6e76 6972 6f6e  xLoader..Environ
-00000690: 6d65 6e74 da0f 5374 7269 6374 556e 6465  ment..StrictUnde
-000006a0: 6669 6e65 64da 066a 6a5f 656e 76da 0374  fined..jj_env..t
-000006b0: 6f70 da0c 6275 735f 7769 6474 685f 6462  op..bus_width_db
-000006c0: da0c 6e61 6d65 7370 6163 655f 6462 da17  ..namespace_db..
-000006d0: 7265 7573 655f 636c 6173 735f 6465 6669  reuse_class_defi
-000006e0: 6e69 7469 6f6e 7329 04da 0473 656c 66da  nitions)...self.
-000006f0: 066b 7761 7267 7372 1300 0000 721b 0000  .kwargsr....r...
-00000700: 00a9 0072 3300 0000 fa4c 2f68 6f6d 652f  ...r3....L/home/
-00000710: 6b75 6e2f 6575 766d 5f70 726f 6a65 6374  kun/euvm_project
-00000720: 732f 7379 7374 656d 5f72 646c 2f50 6561  s/system_rdl/Pea
-00000730: 6b52 444c 2d65 7576 6d2f 7372 632f 7065  kRDL-euvm/src/pe
-00000740: 616b 7264 6c5f 6575 766d 2f65 7870 6f72  akrdl_euvm/expor
-00000750: 7465 722e 7079 da08 5f5f 696e 6974 5f5f  ter.py..__init__
-00000760: 1000 0000 733e 0000 000c 0b0e 0104 0318  ....s>..........
-00000770: 0104 0204 0108 011a 0104 0108 011a 0104  ................
-00000780: fe02 0304 fd08 fd04 091a 0104 011c 0102  ................
-00000790: ff02 0204 fe06 fe04 0702 0104 0108 fe06  ................
-000007a0: 0806 0606 060a 027a 1565 5556 4d45 7870  .......z.eUVMExp
-000007b0: 6f72 7465 722e 5f5f 696e 6974 5f5f da04  orter.__init__..
-000007c0: 6e6f 6465 7225 0000 0063 0300 0000 0000  noder%...c......
-000007d0: 0000 0000 0000 0900 0000 0700 0000 4b00  ..............K.
-000007e0: 0000 738e 0100 007c 03a0 0064 0164 02a1  ..s....|...d.d..
-000007f0: 027d 047c 03a0 0064 0364 04a1 027d 057c  .}.|...d.d...}.|
-00000800: 03a0 0064 0564 02a1 027c 005f 017c 0372  ...d.d...|._.|.r
-00000810: 2174 0264 0674 037c 03a0 04a1 0083 0164  !t.d.t.|.......d
-00000820: 0719 0016 0083 0182 0174 057c 0174 0683  .........t.|.t..
-00000830: 0272 297c 016a 077d 017c 017c 005f 0774  .r)|.j.}.|.|._.t
-00000840: 057c 0174 0883 0272 467c 01a0 0964 08a1  .|.t...rF|...d..
-00000850: 0172 467c 016a 0a6a 0ba0 0c64 097c 016a  .rF|.j.j...d.|.j
-00000860: 0d6a 0ea0 0f64 087c 016a 0d6a 10a1 02a1  .j...d.|.j.j....
-00000870: 0201 0069 007c 005f 1174 1283 00a0 137c  ...i.|._.t.....|
-00000880: 006a 0774 147c 0083 01a1 0201 0069 0064  .j.t.|.......i.d
-00000890: 0a7c 0193 0164 0b74 1593 0164 0c74 1693  .|...d.t...d.t..
-000008a0: 0164 0d74 0893 0164 0e74 1793 0164 0f74  .d.t...d.t...d.t
-000008b0: 1893 0164 1074 0593 0164 117c 006a 1993  ...d.t...d.|.j..
-000008c0: 0164 127c 006a 1a93 0164 137c 006a 1b93  .d.|.j...d.|.j..
-000008d0: 0164 147c 006a 1c93 0164 157c 006a 1d93  .d.|.j...d.|.j..
-000008e0: 0164 167c 006a 1e93 0164 177c 006a 1f93  .d.|.j...d.|.j..
-000008f0: 0164 187c 006a 2093 0164 197c 006a 2193  .d.|.j ..d.|.j!.
-00000900: 0164 1a7c 006a 2293 017c 006a 237c 0564  .d.|.j"..|.j#|.d
-00000910: 1b9c 02a5 017d 067c 06a0 247c 006a 25a1  .....}.|..$|.j%.
-00000920: 0101 007c 0472 ae7c 00a0 267c 02a1 017c  ...|.r.|..&|...|
-00000930: 0664 1c3c 007c 006a 27a0 2864 1da1 017d  .d.<.|.j'.(d...}
-00000940: 076e 0d7c 00a0 297c 02a1 017c 0664 1e3c  .n.|..)|...|.d.<
-00000950: 007c 006a 27a0 2864 1fa1 017d 077c 07a0  .|.j'.(d...}.|..
-00000960: 2a7c 06a1 017d 087c 08a0 2b7c 02a1 0101  *|...}.|..+|....
-00000970: 0064 2053 0029 2161 7604 0000 0a20 2020  .d S.)!av....   
-00000980: 2020 2020 2050 6572 666f 726d 2074 6865       Perform the
-00000990: 2065 7870 6f72 7421 0a0a 2020 2020 2020   export!..      
-000009a0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000009b0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-000009c0: 2020 2020 2020 2020 6e6f 6465 3a20 7379          node: sy
-000009d0: 7374 656d 7264 6c2e 4e6f 6465 0a20 2020  stemrdl.Node.   
-000009e0: 2020 2020 2020 2020 2054 6f70 2d6c 6576           Top-lev
-000009f0: 656c 206e 6f64 6520 746f 2065 7870 6f72  el node to expor
-00000a00: 742e 2043 616e 2062 6520 7468 6520 746f  t. Can be the to
-00000a10: 702d 6c65 7665 6c20 6052 6f6f 744e 6f64  p-level `RootNod
-00000a20: 6560 206f 7220 616e 790a 2020 2020 2020  e` or any.      
-00000a30: 2020 2020 2020 696e 7465 726e 616c 2060        internal `
-00000a40: 4164 6472 6d61 704e 6f64 6560 2e0a 2020  AddrmapNode`..  
-00000a50: 2020 2020 2020 7061 7468 3a20 7374 720a        path: str.
-00000a60: 2020 2020 2020 2020 2020 2020 4f75 7470              Outp
-00000a70: 7574 2066 696c 652e 0a20 2020 2020 2020  ut file..       
-00000a80: 2065 7870 6f72 745f 6173 5f70 6163 6b61   export_as_packa
-00000a90: 6765 3a20 626f 6f6c 0a20 2020 2020 2020  ge: bool.       
-00000aa0: 2020 2020 2049 6620 5472 7565 2028 4465       If True (De
-00000ab0: 6661 756c 7429 2c20 6555 564d 2072 6567  fault), eUVM reg
-00000ac0: 6973 7465 7220 6d6f 6465 6c20 6973 2065  ister model is e
-00000ad0: 7870 6f72 7465 6420 6173 2061 2053 7973  xported as a Sys
-00000ae0: 7465 6d56 6572 696c 6f67 0a20 2020 2020  temVerilog.     
-00000af0: 2020 2020 2020 2070 6163 6b61 6765 2e20         package. 
-00000b00: 5061 636b 6167 6520 6e61 6d65 2069 7320  Package name is 
-00000b10: 6261 7365 6420 6f6e 2074 6865 206f 7574  based on the out
-00000b20: 7075 7420 6669 6c65 206e 616d 652e 0a0a  put file name...
-00000b30: 2020 2020 2020 2020 2020 2020 4966 2046              If F
-00000b40: 616c 7365 2c20 7265 6769 7374 6572 206d  alse, register m
-00000b50: 6f64 656c 2069 7320 6578 706f 7274 6564  odel is exported
-00000b60: 2061 7320 616e 2069 6e63 6c75 6461 626c   as an includabl
-00000b70: 6520 6865 6164 6572 2e0a 2020 2020 2020  e header..      
-00000b80: 2020 7265 7573 655f 636c 6173 735f 6465    reuse_class_de
-00000b90: 6669 6e69 7469 6f6e 733a 2062 6f6f 6c0a  finitions: bool.
-00000ba0: 2020 2020 2020 2020 2020 2020 4966 2054              If T
-00000bb0: 7275 6520 2844 6566 6175 6c74 292c 2065  rue (Default), e
-00000bc0: 7870 6f72 7465 7220 6174 7465 6d70 7473  xporter attempts
-00000bd0: 2074 6f20 7265 2d75 7365 2063 6c61 7373   to re-use class
-00000be0: 2064 6566 696e 6974 696f 6e73 0a20 2020   definitions.   
-00000bf0: 2020 2020 2020 2020 2077 6865 7265 2070           where p
-00000c00: 6f73 7369 626c 652e 2043 6c61 7373 206e  ossible. Class n
-00000c10: 616d 6573 2061 7265 2062 6173 6564 206f  ames are based o
-00000c20: 6e20 7468 6520 6c65 7869 6361 6c20 7363  n the lexical sc
-00000c30: 6f70 6520 6f66 2074 6865 0a20 2020 2020  ope of the.     
-00000c40: 2020 2020 2020 206f 7269 6769 6e61 6c20         original 
-00000c50: 5379 7374 656d 5244 4c20 6465 6669 6e69  SystemRDL defini
-00000c60: 7469 6f6e 732e 0a0a 2020 2020 2020 2020  tions...        
-00000c70: 2020 2020 4966 2046 616c 7365 2c20 636c      If False, cl
-00000c80: 6173 7320 6465 6669 6e69 7469 6f6e 7320  ass definitions 
-00000c90: 6172 6520 6e6f 7420 7265 7573 6564 2e20  are not reused. 
-00000ca0: 436c 6173 7320 6e61 6d65 7320 6172 6520  Class names are 
-00000cb0: 6261 7365 6420 6f6e 0a20 2020 2020 2020  based on.       
-00000cc0: 2020 2020 2074 6865 2069 6e73 7461 6e63       the instanc
-00000cd0: 6527 7320 6869 6572 6172 6368 6963 616c  e's hierarchical
-00000ce0: 2070 6174 682e 0a20 2020 2020 2020 2075   path..        u
-00000cf0: 7365 5f75 766d 5f66 6163 746f 7279 3a20  se_uvm_factory: 
-00000d00: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-00000d10: 2049 6620 5472 7565 2c20 636c 6173 7320   If True, class 
-00000d20: 6465 6669 6e69 7469 6f6e 7320 616e 6420  definitions and 
-00000d30: 636c 6173 7320 696e 7374 616e 6365 7320  class instances 
-00000d40: 6172 6520 6372 6561 7465 6420 7573 696e  are created usin
-00000d50: 6720 7468 650a 2020 2020 2020 2020 2020  g the.          
-00000d60: 2020 5556 4d20 6661 6374 6f72 792e 0a0a    UVM factory...
-00000d70: 2020 2020 2020 2020 2020 2020 4966 2046              If F
-00000d80: 616c 7365 2028 4465 6661 756c 7429 2c20  alse (Default), 
-00000d90: 5556 4d20 6661 6374 6f72 7920 6973 2064  UVM factory is d
-00000da0: 6973 6162 6c65 642e 2043 6c61 7373 6573  isabled. Classes
-00000db0: 2061 7265 2063 7265 6174 6564 0a20 2020   are created.   
-00000dc0: 2020 2020 2020 2020 2064 6972 6563 746c           directl
-00000dd0: 7920 7669 6120 6e65 7728 2920 636f 6e73  y via new() cons
-00000de0: 7472 7563 746f 7273 2e0a 2020 2020 2020  tructors..      
-00000df0: 2020 da11 6578 706f 7274 5f61 735f 7061    ..export_as_pa
-00000e00: 636b 6167 6554 da0f 7573 655f 7576 6d5f  ckageT..use_uvm_
-00000e10: 6661 6374 6f72 7946 7230 0000 0072 1500  factoryFr0...r..
-00000e20: 0000 7201 0000 00da 0662 7269 6467 657a  ..r......bridgez
-00000e30: 6e65 5556 4d20 5241 4c20 6765 6e65 7261  neUVM RAL genera
-00000e40: 746f 7220 646f 6573 206e 6f74 2068 6176  tor does not hav
-00000e50: 6520 7072 6f70 6572 2073 7570 706f 7274  e proper support
-00000e60: 2066 6f72 2062 7269 6467 6520 6164 646d   for bridge addm
-00000e70: 6170 7320 7965 742e 2054 6865 2027 6272  aps yet. The 'br
-00000e80: 6964 6765 2720 7072 6f70 6572 7479 2077  idge' property w
-00000e90: 696c 6c20 6265 2069 676e 6f72 6564 2eda  ill be ignored..
-00000ea0: 0874 6f70 5f6e 6f64 6572 0500 0000 7207  .top_noder....r.
-00000eb0: 0000 0072 0600 0000 7209 0000 0072 0a00  ...r....r....r..
-00000ec0: 0000 da0a 6973 696e 7374 616e 6365 da16  ....isinstance..
-00000ed0: 636c 6173 735f 6e65 6564 735f 6465 6669  class_needs_defi
-00000ee0: 6e69 7469 6f6e da0e 6765 745f 636c 6173  nition..get_clas
-00000ef0: 735f 6e61 6d65 da17 6765 745f 636c 6173  s_name..get_clas
-00000f00: 735f 6672 6965 6e64 6c79 5f6e 616d 65da  s_friendly_name.
-00000f10: 0d67 6574 5f69 6e73 745f 6e61 6d65 da10  .get_inst_name..
-00000f20: 6765 745f 6669 656c 645f 6163 6365 7373  get_field_access
-00000f30: da1d 6765 745f 6172 7261 795f 6164 6472  ..get_array_addr
-00000f40: 6573 735f 6f66 6673 6574 5f65 7870 72da  ess_offset_expr.
-00000f50: 0e67 6574 5f65 6e64 6961 6e6e 6573 73da  .get_endianness.
-00000f60: 0d67 6574 5f62 7573 5f77 6964 7468 da0e  .get_bus_width..
-00000f70: 6765 745f 6d65 6d5f 6163 6365 7373 da0a  get_mem_access..
-00000f80: 726f 756e 6475 705f 746f 2902 da0c 726f  roundup_to)...ro
-00000f90: 756e 6475 705f 706f 7732 7238 0000 00da  undup_pow2r8....
-00000fa0: 0c70 6163 6b61 6765 5f6e 616d 657a 0974  .package_namez.t
-00000fb0: 6f70 5f70 6b67 2e64 da0d 696e 636c 7564  op_pkg.d..includ
-00000fc0: 655f 6775 6172 647a 0d74 6f70 5f69 6e63  e_guardz.top_inc
-00000fd0: 6c75 6465 2e64 4e29 2c72 1d00 0000 7230  lude.dN),r....r0
-00000fe0: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
-00000ff0: 0000 723b 0000 0072 0300 0000 722d 0000  ..r;...r....r-..
-00001000: 0072 0600 0000 da0c 6765 745f 7072 6f70  .r......get_prop
-00001010: 6572 7479 da03 656e 76da 036d 7367 da07  erty..env..msg..
-00001020: 7761 726e 696e 67da 0469 6e73 74da 1070  warning..inst..p
-00001030: 726f 7065 7274 795f 7372 635f 7265 66da  roperty_src_ref.
-00001040: 0367 6574 da0c 696e 7374 5f73 7263 5f72  .get..inst_src_r
-00001050: 6566 722e 0000 0072 0f00 0000 da04 7761  efr....r......wa
-00001060: 6c6b 7211 0000 0072 0500 0000 7207 0000  lkr....r....r...
-00001070: 0072 0900 0000 720a 0000 00da 175f 636c  .r....r......_cl
-00001080: 6173 735f 6e65 6564 735f 6465 6669 6e69  ass_needs_defini
-00001090: 7469 6f6e da0f 5f67 6574 5f63 6c61 7373  tion.._get_class
-000010a0: 5f6e 616d 65da 185f 6765 745f 636c 6173  _name.._get_clas
-000010b0: 735f 6672 6965 6e64 6c79 5f6e 616d 65da  s_friendly_name.
-000010c0: 0e5f 6765 745f 696e 7374 5f6e 616d 65da  ._get_inst_name.
-000010d0: 115f 6765 745f 6669 656c 645f 6163 6365  ._get_field_acce
-000010e0: 7373 da1e 5f67 6574 5f61 7272 6179 5f61  ss.._get_array_a
-000010f0: 6464 7265 7373 5f6f 6666 7365 745f 6578  ddress_offset_ex
-00001100: 7072 da0f 5f67 6574 5f65 6e64 6961 6e6e  pr.._get_endiann
-00001110: 6573 73da 0e5f 6765 745f 6275 735f 7769  ess.._get_bus_wi
-00001120: 6474 68da 0f5f 6765 745f 6d65 6d5f 6163  dth.._get_mem_ac
-00001130: 6365 7373 da0b 5f72 6f75 6e64 7570 5f74  cess.._roundup_t
-00001140: 6fda 0d5f 726f 756e 6475 705f 706f 7732  o.._roundup_pow2
-00001150: da06 7570 6461 7465 7214 0000 00da 115f  ..updater......_
-00001160: 6765 745f 7061 636b 6167 655f 6e61 6d65  get_package_name
-00001170: 722c 0000 00da 0c67 6574 5f74 656d 706c  r,.....get_templ
-00001180: 6174 65da 125f 6765 745f 696e 636c 7564  ate.._get_includ
-00001190: 655f 6775 6172 64da 0673 7472 6561 6dda  e_guard..stream.
-000011a0: 0464 756d 7029 0972 3100 0000 7236 0000  .dump).r1...r6..
-000011b0: 0072 2500 0000 7232 0000 0072 3700 0000  .r%...r2...r7...
-000011c0: 7238 0000 00da 0763 6f6e 7465 7874 da08  r8.....context..
-000011d0: 7465 6d70 6c61 7465 7261 0000 0072 3300  templatera...r3.
-000011e0: 0000 7233 0000 0072 3400 0000 da06 6578  ..r3...r4.....ex
-000011f0: 706f 7274 4c00 0000 737a 0000 000c 1e0c  portL...sz......
-00001200: 010e 0104 0318 010a 0306 0106 0114 0208  ................
-00001210: 0102 0112 0104 fe06 0614 0102 0204 0102  ................
-00001220: ff04 0202 fe04 0302 fd04 0402 fc04 0502  ................
-00001230: fb04 0602 fa04 0702 f906 0802 f806 0902  ................
-00001240: f706 0a02 f606 0b02 f506 0c02 f406 0d02  ................
-00001250: f306 0e02 f206 0f02 f106 1002 f006 1102  ................
-00001260: ef04 1202 0108 ed0c 1604 020e 010e 010e  ................
-00001270: 020c 010a 010e 017a 1365 5556 4d45 7870  .......z.eUVMExp
-00001280: 6f72 7465 722e 6578 706f 7274 da06 7265  orter.export..re
-00001290: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
-000012a0: 0003 0000 0005 0000 0043 0000 0073 2a00  .........C...s*.
-000012b0: 0000 7400 6a01 a002 7400 6a01 a003 7c01  ..t.j...t.j...|.
-000012c0: a101 a101 6401 1900 7d02 7404 a005 6402  ....d...}.t...d.
-000012d0: 6403 7c02 a103 7d02 7c02 5300 2904 4e72  d.|...}.|.S.).Nr
-000012e0: 0100 0000 fa05 5b5e 5c77 5dda 015f 2906  ......[^\w].._).
-000012f0: 7224 0000 0072 2500 0000 da08 7370 6c69  r$...r%.....spli
-00001300: 7465 7874 da08 6261 7365 6e61 6d65 da02  text..basename..
-00001310: 7265 da03 7375 62a9 0372 3100 0000 7225  re..sub..r1...r%
-00001320: 0000 00da 0173 7233 0000 0072 3300 0000  .....sr3...r3...
-00001330: 7234 0000 0072 5e00 0000 a300 0000 7306  r4...r^.......s.
-00001340: 0000 0018 010e 0104 017a 1e65 5556 4d45  .........z.eUVME
-00001350: 7870 6f72 7465 722e 5f67 6574 5f70 6163  xporter._get_pac
-00001360: 6b61 6765 5f6e 616d 6563 0200 0000 0000  kage_namec......
-00001370: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00001380: 0000 7322 0000 0074 006a 01a0 027c 01a1  ..s"...t.j...|..
-00001390: 017d 0274 03a0 0464 0164 027c 02a1 03a0  .}.t...d.d.|....
-000013a0: 05a1 007d 027c 0253 0029 034e 7267 0000  ...}.|.S.).Nrg..
-000013b0: 0072 6800 0000 2906 7224 0000 0072 2500  .rh...).r$...r%.
-000013c0: 0000 726a 0000 0072 6b00 0000 726c 0000  ..rj...rk...rl..
-000013d0: 00da 0575 7070 6572 726d 0000 0072 3300  ...upperrm...r3.
-000013e0: 0000 7233 0000 0072 3400 0000 7260 0000  ..r3...r4...r`..
-000013f0: 00a9 0000 0073 0600 0000 0c01 1201 0401  .....s..........
-00001400: 7a1f 6555 564d 4578 706f 7274 6572 2e5f  z.eUVMExporter._
-00001410: 6765 745f 696e 636c 7564 655f 6775 6172  get_include_guar
-00001420: 6463 0200 0000 0000 0000 0000 0000 0300  dc..............
-00001430: 0000 0600 0000 4300 0000 7326 0000 007c  ......C...s&...|
-00001440: 006a 0072 0609 007c 0253 007c 016a 017c  .j.r...|.S.|.j.|
-00001450: 006a 026a 0364 0164 0264 0264 038d 047d  .j.j.d.d.d.d...}
-00001460: 027c 0253 0029 04fa 6d0a 2020 2020 2020  .|.S.)..m.      
-00001470: 2020 5265 7475 726e 7320 7468 6520 636c    Returns the cl
-00001480: 6173 7320 7479 7065 206e 616d 652e 0a20  ass type name.. 
-00001490: 2020 2020 2020 2053 6861 6c6c 2062 6520         Shall be 
-000014a0: 756e 6971 7565 2065 6e6f 7567 6820 746f  unique enough to
-000014b0: 2070 7265 7665 6e74 2074 7970 6520 6e61   prevent type na
-000014c0: 6d65 2063 6f6c 6c69 7369 6f6e 730a 2020  me collisions.  
-000014d0: 2020 2020 2020 da02 5f5f da00 a903 da0e        ..__......
-000014e0: 6869 6572 5f73 6570 6172 6174 6f72 da0c  hier_separator..
-000014f0: 6172 7261 795f 7375 6666 6978 da12 656d  array_suffix..em
-00001500: 7074 795f 6172 7261 795f 7375 6666 6978  pty_array_suffix
-00001510: 2904 7230 0000 00da 0c67 6574 5f72 656c  ).r0.....get_rel
-00001520: 5f70 6174 6872 2d00 0000 da06 7061 7265  _pathr-.....pare
-00001530: 6e74 2903 7231 0000 0072 3600 0000 da0a  nt).r1...r6.....
-00001540: 636c 6173 735f 6e61 6d65 7233 0000 0072  class_namer3...r
-00001550: 3300 0000 7234 0000 00da 135f 6765 745f  3...r4....._get_
-00001560: 636c 6173 735f 6e61 6d65 5f6e 6577 af00  class_name_new..
-00001570: 0000 7310 0000 0006 0502 0104 0704 fb06  ..s.............
-00001580: 0106 0106 fe04 057a 2065 5556 4d45 7870  .......z eUVMExp
-00001590: 6f72 7465 722e 5f67 6574 5f63 6c61 7373  orter._get_class
-000015a0: 5f6e 616d 655f 6e65 77fa 023a 3ada 0973  _name_new..::..s
-000015b0: 6570 6172 6174 6f72 6303 0000 0000 0000  eparatorc.......
-000015c0: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-000015d0: 0073 8c00 0000 7c01 6a00 6a01 6401 7500  .s....|.j.j.d.u.
-000015e0: 7208 6401 5300 7402 7c01 6a00 6a01 7403  r.d.S.t.|.j.j.t.
-000015f0: 8302 7212 7c01 6a04 5300 7c01 6a05 7d03  ..r.|.j.S.|.j.}.
-00001600: 7c03 7244 7c03 6a00 6a06 6401 7500 721f  |.rD|.j.j.d.u.r.
-00001610: 6401 5300 7c03 6a00 6a06 7c01 6a00 6a01  d.S.|.j.j.|.j.j.
-00001620: 7500 723f 7c00 a007 7c03 7c02 a102 7d04  u.r?|...|.|...}.
-00001630: 7c04 6401 7500 7336 7c01 6a04 6401 7500  |.d.u.s6|.j.d.u.
-00001640: 7238 6401 5300 7c04 7c02 1700 7c01 6a04  r8d.S.|.|...|.j.
-00001650: 1700 5300 7c03 6a05 7d03 7c03 7317 6401  ..S.|.j.}.|.s.d.
-00001660: 5300 2902 7a81 0a20 2020 2020 2020 2052  S.).z..        R
-00001670: 6574 7572 6e73 2074 6865 2073 636f 7065  eturns the scope
-00001680: 2070 6174 682c 2062 7574 2077 6974 6820   path, but with 
-00001690: 7265 736f 6c76 6564 2074 7970 6520 6e61  resolved type na
-000016a0: 6d65 730a 2020 2020 2020 2020 5265 7475  mes.        Retu
-000016b0: 726e 7320 4e6f 6e65 2069 6620 616e 7920  rns None if any 
-000016c0: 7365 676d 656e 7420 696e 2074 6865 2070  segment in the p
-000016d0: 6174 6820 6973 2075 6e6b 6e6f 776e 0a20  ath is unknown. 
-000016e0: 2020 2020 2020 204e 2908 724d 0000 00da         N).rM....
-000016f0: 0c70 6172 656e 745f 7363 6f70 6572 3b00  .parent_scoper;.
-00001700: 0000 720e 0000 00da 0974 7970 655f 6e61  ..r......type_na
-00001710: 6d65 7278 0000 00da 0c6f 7269 6769 6e61  merx.....origina
-00001720: 6c5f 6465 66da 185f 6765 745f 7265 736f  l_def.._get_reso
-00001730: 6c76 6564 5f73 636f 7065 5f70 6174 6829  lved_scope_path)
-00001740: 0572 3100 0000 7236 0000 0072 7c00 0000  .r1...r6...r|...
-00001750: da13 6375 7272 656e 745f 7061 7265 6e74  ..current_parent
-00001760: 5f6e 6f64 65da 1170 6172 656e 745f 7363  _node..parent_sc
-00001770: 6f70 655f 7061 7468 7233 0000 0072 3300  ope_pathr3...r3.
-00001780: 0000 7234 0000 0072 8000 0000 be00 0000  ..r4...r........
-00001790: 7320 0000 000c 0604 020e 0206 0206 0504  s ..............
-000017a0: 020c 0104 0210 010c 0212 0104 010e 0106  ................
-000017b0: 0204 f504 0e7a 2565 5556 4d45 7870 6f72  .....z%eUVMExpor
-000017c0: 7465 722e 5f67 6574 5f72 6573 6f6c 7665  ter._get_resolve
-000017d0: 645f 7363 6f70 655f 7061 7468 6302 0000  d_scope_pathc...
-000017e0: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-000017f0: 0043 0000 0073 5e00 0000 7c00 6a00 7222  .C...s^...|.j.r"
-00001800: 7c00 a001 7c01 6401 a102 7d02 7c02 6402  |...|.d...}.|.d.
-00001810: 7501 7211 7c02 7d03 7c03 5300 7c01 6a02  u.r.|.}.|.S.|.j.
-00001820: 7c00 6a03 6a04 6401 6403 6403 6404 8d04  |.j.j.d.d.d.d...
-00001830: 7d03 6405 7c03 1700 7d03 7c03 5300 7c01  }.d.|...}.|.S.|.
-00001840: 6a02 7c00 6a03 6a04 6401 6403 6403 6404  j.|.j.j.d.d.d.d.
-00001850: 8d04 7d03 7c03 5300 2906 7270 0000 0072  ..}.|.S.).rp...r
-00001860: 7100 0000 4e72 7200 0000 7273 0000 00da  q...Nrr...rs....
-00001870: 0778 7465 726e 5f5f 2905 7230 0000 0072  .xtern__).r0...r
-00001880: 8000 0000 7277 0000 0072 2d00 0000 7278  ....rw...r-...rx
-00001890: 0000 0029 0472 3100 0000 7236 0000 00da  ...).r1...r6....
-000018a0: 0a73 636f 7065 5f70 6174 6872 7900 0000  .scope_pathry...
-000018b0: 7233 0000 0072 3300 0000 7234 0000 0072  r3...r3...r4...r
-000018c0: 5300 0000 e100 0000 7320 0000 0006 050c  S.......s ......
-000018d0: 0108 0204 0104 0f04 f406 0106 0106 fe08  ................
-000018e0: 0504 0704 fb06 0106 0106 fe04 057a 1c65  .............z.e
-000018f0: 5556 4d45 7870 6f72 7465 722e 5f67 6574  UVMExporter._get
-00001900: 5f63 6c61 7373 5f6e 616d 6563 0200 0000  _class_namec....
-00001910: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00001920: 4300 0000 7350 0000 007c 006a 0072 177c  C...sP...|.j.r.|
-00001930: 00a0 017c 01a1 017d 027c 0264 0175 0172  ...|...}.|.d.u.r
-00001940: 0f7c 027d 036e 0f7c 01a0 027c 006a 036a  .|.}.n.|...|.j.j
-00001950: 04a1 017d 036e 077c 01a0 027c 006a 036a  ...}.n.|...|.j.j
-00001960: 04a1 017d 0374 057c 016a 0683 016a 0764  ...}.t.|.j...j.d
-00001970: 0217 007c 0317 0053 0029 037a 670a 2020  ...|...S.).zg.  
-00001980: 2020 2020 2020 5265 7475 726e 7320 6120        Returns a 
-00001990: 7573 6566 756c 2073 7472 696e 6720 7468  useful string th
-000019a0: 6174 2068 656c 7073 2069 6465 6e74 6966  at helps identif
-000019b0: 7920 7468 6520 636c 6173 7320 6465 6669  y the class defi
-000019c0: 6e69 7469 6f6e 2069 6e0a 2020 2020 2020  nition in.      
-000019d0: 2020 6120 636f 6d6d 656e 740a 2020 2020    a comment.    
-000019e0: 2020 2020 4e7a 0320 2d20 2908 7230 0000      Nz. - ).r0..
-000019f0: 0072 8000 0000 7277 0000 0072 2d00 0000  .r....rw...r-...
-00001a00: 7278 0000 00da 0474 7970 6572 4d00 0000  rx.....typerM...
-00001a10: da08 5f5f 6e61 6d65 5f5f 2904 7231 0000  ..__name__).r1..
-00001a20: 0072 3600 0000 7284 0000 00da 0d66 7269  .r6...r......fri
-00001a30: 656e 646c 795f 6e61 6d65 7233 0000 0072  endly_namer3...r
-00001a40: 3300 0000 7234 0000 0072 5400 0000 fc00  3...r4...rT.....
-00001a50: 0000 730e 0000 0006 050a 0108 0206 0110  ..s.............
-00001a60: 030e 0214 027a 2565 5556 4d45 7870 6f72  .....z%eUVMExpor
-00001a70: 7465 722e 5f67 6574 5f63 6c61 7373 5f66  ter._get_class_f
-00001a80: 7269 656e 646c 795f 6e61 6d65 6302 0000  riendly_namec...
-00001a90: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-00001aa0: 0043 0000 0073 0600 0000 7c01 6a00 5300  .C...s....|.j.S.
-00001ab0: 2901 7a31 0a20 2020 2020 2020 2052 6574  ).z1.        Ret
-00001ac0: 7572 6e73 2074 6865 2063 6c61 7373 2069  urns the class i
-00001ad0: 6e73 7461 6e63 6520 6e61 6d65 0a20 2020  nstance name.   
-00001ae0: 2020 2020 2029 01da 0969 6e73 745f 6e61       )...inst_na
-00001af0: 6d65 2902 7231 0000 0072 3600 0000 7233  me).r1...r6...r3
-00001b00: 0000 0072 3300 0000 7234 0000 0072 5500  ...r3...r4...rU.
-00001b10: 0000 0f01 0000 7302 0000 0006 047a 1b65  ......s......z.e
-00001b20: 5556 4d45 7870 6f72 7465 722e 5f67 6574  UVMExporter._get
-00001b30: 5f69 6e73 745f 6e61 6d65 6302 0000 0000  _inst_namec.....
-00001b40: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
-00001b50: 0000 0073 5000 0000 7c00 a000 7c01 a101  ...sP...|...|...
-00001b60: 7d02 7c02 7c00 6a01 7600 721f 7c00 6a01  }.|.|.j.v.r.|.j.
-00001b70: 7c02 1900 7d03 7c03 6401 7500 7319 7c03  |...}.|.d.u.s.|.
-00001b80: 7c01 6a02 6a03 7501 721d 7404 6402 8301  |.j.j.u.r.t.d...
-00001b90: 8201 6403 5300 7c01 6a02 6a03 7c00 6a01  ..d.S.|.j.j.|.j.
-00001ba0: 7c02 3c00 6404 5300 2905 616c 0100 000a  |.<.d.S.).al....
-00001bb0: 2020 2020 2020 2020 4368 6563 6b73 2069          Checks i
-00001bc0: 6620 7468 6520 636c 6173 7320 7468 6174  f the class that
-00001bd0: 2064 6566 696e 6573 2074 6869 7320 6e6f   defines this no
-00001be0: 6465 2061 6c72 6561 6479 2065 7869 7374  de already exist
-00001bf0: 732e 0a20 2020 2020 2020 2049 6620 6e6f  s..        If no
-00001c00: 742c 2072 6574 7572 6e73 2054 7275 652c  t, returns True,
-00001c10: 2069 6e64 6963 6174 696e 6720 7468 6174   indicating that
-00001c20: 2061 2064 6566 696e 6974 696f 6e20 7368   a definition sh
-00001c30: 616c 6c20 6265 2065 6d69 7474 6564 2e0a  all be emitted..
-00001c40: 0a20 2020 2020 2020 2049 6620 7265 7475  .        If retu
-00001c50: 726e 696e 6720 5472 7565 2c20 7468 656e  rning True, then
-00001c60: 2074 6865 2061 6374 206f 6620 6361 6c6c   the act of call
-00001c70: 696e 6720 7468 6973 2066 756e 6374 696f  ing this functio
-00001c80: 6e20 616c 736f 2072 6567 6973 7465 7273  n also registers
-00001c90: 0a20 2020 2020 2020 2074 6865 2063 6c61  .        the cla
-00001ca0: 7373 2064 6566 696e 6974 696f 6e20 696e  ss definition in
-00001cb0: 746f 2074 6865 206e 616d 6573 7061 6365  to the namespace
-00001cc0: 2064 6174 6162 6173 6520 736f 2074 6861   database so tha
-00001cd0: 7420 6675 7475 7265 2063 616c 6c73 0a20  t future calls. 
-00001ce0: 2020 2020 2020 2066 6f72 2065 7175 6976         for equiv
-00001cf0: 616c 656e 7420 6e6f 6465 2074 7970 6573  alent node types
-00001d00: 2077 696c 6c20 7265 7475 726e 2046 616c   will return Fal
-00001d10: 7365 0a20 2020 2020 2020 204e 7a56 4e61  se.        NzVNa
-00001d20: 6d65 7370 6163 6520 636f 6c6c 6973 696f  mespace collisio
-00001d30: 6e21 2054 7970 652d 6e61 6d65 2067 656e  n! Type-name gen
-00001d40: 6572 6174 696f 6e20 6973 206e 6f74 2072  eration is not r
-00001d50: 6f62 7573 7420 656e 6f75 6768 2074 6f20  obust enough to 
-00001d60: 6372 6561 7465 2075 6e69 7175 6520 6e61  create unique na
-00001d70: 6d65 7321 4654 2905 7253 0000 0072 2f00  mes!FT).rS...r/.
-00001d80: 0000 724d 0000 0072 7f00 0000 da0c 5275  ..rM...r......Ru
-00001d90: 6e74 696d 6545 7272 6f72 2904 7231 0000  ntimeError).r1..
-00001da0: 0072 3600 0000 727e 0000 00da 036f 626a  .r6...r~.....obj
-00001db0: 7233 0000 0072 3300 0000 7234 0000 0072  r3...r3...r4...r
-00001dc0: 5200 0000 1601 0000 7310 0000 000a 090a  R.......s.......
-00001dd0: 020a 0114 0308 0104 040e 0404 017a 2465  .............z$e
-00001de0: 5556 4d45 7870 6f72 7465 722e 5f63 6c61  UVMExporter._cla
-00001df0: 7373 5f6e 6565 6473 5f64 6566 696e 6974  ss_needs_definit
-00001e00: 696f 6eda 0566 6965 6c64 6302 0000 0000  ion..fieldc.....
-00001e10: 0000 0000 0000 0005 0000 0003 0000 0043  ...............C
-00001e20: 0000 0073 e801 0000 7c01 a000 6401 a101  ...s....|...d...
-00001e30: 7d02 7c01 a000 6402 a101 7d03 7c01 a000  }.|...d...}.|...
-00001e40: 6403 a101 7d04 7c02 7401 6a02 6b02 72ae  d...}.|.t.j.k.r.
-00001e50: 7c04 6404 7500 721e 7c03 6404 7500 721e  |.d.u.r.|.d.u.r.
-00001e60: 6405 5300 7c03 7403 6a04 6b02 722a 7c04  d.S.|.t.j.k.r*|.
-00001e70: 7405 6a06 6b02 722a 6406 5300 7c03 7403  t.j.k.r*d.S.|.t.
-00001e80: 6a04 6b02 7236 7c04 7405 6a07 6b02 7236  j.k.r6|.t.j.k.r6
-00001e90: 6407 5300 7c03 7403 6a04 6b02 7242 7c04  d.S.|.t.j.k.rB|.
-00001ea0: 7405 6a08 6b02 7242 6408 5300 7c03 7403  t.j.k.rBd.S.|.t.
-00001eb0: 6a09 6b02 724e 7c04 7405 6a0a 6b02 724e  j.k.rN|.t.j.k.rN
-00001ec0: 6409 5300 7c03 7403 6a09 6b02 725a 7c04  d.S.|.t.j.k.rZ|.
-00001ed0: 7405 6a0b 6b02 725a 640a 5300 7c03 7403  t.j.k.rZd.S.|.t.
-00001ee0: 6a09 6b02 7266 7c04 7405 6a0c 6b02 7266  j.k.rf|.t.j.k.rf
-00001ef0: 640b 5300 7c04 7405 6a0a 6b02 726d 640c  d.S.|.t.j.k.rmd.
-00001f00: 5300 7c04 7405 6a06 6b02 7274 640d 5300  S.|.t.j.k.rtd.S.
-00001f10: 7c04 7405 6a0d 6b02 727b 640e 5300 7c04  |.t.j.k.r{d.S.|.
-00001f20: 7405 6a0b 6b02 7282 640f 5300 7c04 7405  t.j.k.r.d.S.|.t.
-00001f30: 6a07 6b02 7289 6410 5300 7c04 7405 6a0e  j.k.r.d.S.|.t.j.
-00001f40: 6b02 7290 6411 5300 7c04 7405 6a0c 6b02  k.r.d.S.|.t.j.k.
-00001f50: 7297 6412 5300 7c04 7405 6a08 6b02 729e  r.d.S.|.t.j.k.r.
-00001f60: 6413 5300 7c03 7403 6a04 6b02 72a5 6414  d.S.|.t.j.k.r.d.
-00001f70: 5300 7c03 7403 6a09 6b02 72ac 6415 5300  S.|.t.j.k.r.d.S.
-00001f80: 6405 5300 7c02 7401 6a0f 6b02 72c9 7c03  d.S.|.t.j.k.r.|.
-00001f90: 6404 7500 72b9 6416 5300 7c03 7403 6a04  d.u.r.d.S.|.t.j.
-00001fa0: 6b02 72c0 6417 5300 7c03 7403 6a09 6b02  k.r.d.S.|.t.j.k.
-00001fb0: 72c7 6418 5300 6416 5300 7c02 7401 6a10  r.d.S.d.S.|.t.j.
-00001fc0: 6b02 72e4 7c04 6404 7500 72d4 6419 5300  k.r.|.d.u.r.d.S.
-00001fd0: 7c04 7405 6a0c 6b02 72db 641a 5300 7c04  |.t.j.k.r.d.S.|.
-00001fe0: 7405 6a08 6b02 72e2 641b 5300 6419 5300  t.j.k.r.d.S.d.S.
-00001ff0: 7c02 7401 6a11 6b02 72eb 641c 5300 7c02  |.t.j.k.r.d.S.|.
-00002000: 7401 6a12 6b02 72f2 641d 5300 641e 5300  t.j.k.r.d.S.d.S.
-00002010: 291f 7a2f 0a20 2020 2020 2020 2047 6574  ).z/.        Get
-00002020: 2066 6965 6c64 2773 2055 564d 2061 6363   field's UVM acc
-00002030: 6573 7320 7374 7269 6e67 0a20 2020 2020  ess string.     
-00002040: 2020 20da 0273 77da 066f 6e72 6561 64da     ..sw..onread.
-00002050: 076f 6e77 7269 7465 4eda 0252 57da 0557  .onwriteN..RW..W
-00002060: 3153 5243 da05 5730 5352 43da 0457 5352  1SRC..W0SRC..WSR
-00002070: 43da 0557 3143 5253 da05 5730 4352 53da  C..W1CRS..W0CRS.
-00002080: 0457 4352 53da 0357 3143 da03 5731 53da  .WCRS..W1C..W1S.
-00002090: 0357 3154 da03 5730 43da 0357 3053 da03  .W1T..W0C..W0S..
-000020a0: 5730 54da 0257 43da 0257 53da 0357 5243  W0T..WC..WS..WRC
-000020b0: da03 5752 53da 0252 4fda 0252 43da 0252  ..WRS..RO..RC..R
-000020c0: 53da 0257 4fda 0357 4f43 da03 574f 53da  S..WO..WOC..WOS.
-000020d0: 0257 31da 0357 4f31 da08 4e4f 4143 4345  .W1..WO1..NOACCE
-000020e0: 5353 2913 7249 0000 0072 0b00 0000 da02  SS).rI...r......
-000020f0: 7277 720c 0000 00da 0472 636c 7272 0d00  rwr......rclrr..
-00002100: 0000 da05 776f 7365 74da 0377 7a73 da04  ....woset..wzs..
-00002110: 7773 6574 da04 7273 6574 da05 776f 636c  wset..rset..wocl
-00002120: 72da 0377 7a63 da04 7763 6c72 da03 776f  r..wzc..wclr..wo
-00002130: 74da 0377 7a74 da01 72da 0177 da03 7277  t..wzt..r..w..rw
-00002140: 31da 0277 3129 0572 3100 0000 728b 0000  1..w1).r1...r...
-00002150: 0072 8c00 0000 728d 0000 0072 8e00 0000  .r....r....r....
-00002160: 7233 0000 0072 3300 0000 7234 0000 0072  r3...r3...r4...r
-00002170: 5600 0000 3201 0000 7378 0000 000a 040a  V...2...sx......
-00002180: 010a 010a 0210 0104 0114 0104 0114 0104  ................
-00002190: 0114 0104 0114 0104 0114 0104 0114 0104  ................
-000021a0: 010a 0104 010a 0104 010a 0104 010a 0104  ................
-000021b0: 010a 0104 010a 0104 010a 0104 010a 0104  ................
-000021c0: 010a 0104 010a 0104 0104 020a 0208 0104  ................
-000021d0: 010a 0104 010a 0104 0104 020a 0208 0104  ................
-000021e0: 010a 0104 010a 0104 0104 020a 0204 010a  ................
-000021f0: 0204 0104 037a 1e65 5556 4d45 7870 6f72  .....z.eUVMExpor
-00002200: 7465 722e 5f67 6574 5f66 6965 6c64 5f61  ter._get_field_a
-00002210: 6363 6573 73da 036d 656d 6302 0000 0000  ccess..memc.....
-00002220: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-00002230: 0000 0073 1c00 0000 7c01 a000 6401 a101  ...s....|...d...
-00002240: 7d02 7c02 7401 6a02 6b02 720c 6402 5300  }.|.t.j.k.r.d.S.
-00002250: 6403 5300 2904 4e72 8c00 0000 72a0 0000  d.S.).Nr....r...
-00002260: 0072 8f00 0000 2903 7249 0000 0072 0b00  .r....).rI...r..
-00002270: 0000 72b4 0000 0029 0372 3100 0000 72b8  ..r....).r1...r.
-00002280: 0000 0072 8c00 0000 7233 0000 0072 3300  ...r....r3...r3.
-00002290: 0000 7234 0000 0072 5a00 0000 7e01 0000  ..r4...rZ...~...
-000022a0: 7308 0000 000a 010a 0104 0104 027a 1c65  s............z.e
-000022b0: 5556 4d45 7870 6f72 7465 722e 5f67 6574  UVMExporter._get
-000022c0: 5f6d 656d 5f61 6363 6573 7363 0200 0000  _mem_accessc....
-000022d0: 0000 0000 0000 0000 0600 0000 0500 0000  ................
-000022e0: 4300 0000 7366 0000 0064 017c 016a 0016  C...sf...d.|.j..
-000022f0: 007d 027c 016a 0172 3174 0274 037c 016a  .}.|.j.r1t.t.|.j
-00002300: 0483 0183 0144 005d 217d 037c 016a 057d  .....D.]!}.|.j.}
-00002310: 0474 027c 0364 0217 0074 037c 016a 0483  .t.|.d...t.|.j..
-00002320: 0183 0244 005d 097d 057c 047c 016a 047c  ...D.].}.|.|.j.|
-00002330: 0519 0039 007d 0471 1e7c 0264 037c 037c  ...9.}.q.|.d.|.|
-00002340: 0466 0216 0037 007d 0271 0f7c 0253 0029  .f...7.}.q.|.S.)
-00002350: 047a ec0a 2020 2020 2020 2020 5265 7475  .z..        Retu
-00002360: 726e 7320 616e 2065 7870 7265 7373 696f  rns an expressio
-00002370: 6e20 746f 2063 616c 6375 6c61 7465 2074  n to calculate t
-00002380: 6865 2061 6464 7265 7373 206f 6666 7365  he address offse
-00002390: 740a 2020 2020 2020 2020 666f 7220 6578  t.        for ex
-000023a0: 616d 706c 652c 2061 2034 2d64 696d 656e  ample, a 4-dimen
-000023b0: 7369 6f6e 616c 2061 7272 6179 2061 6c6c  sional array all
-000023c0: 6f63 6174 6564 2061 733a 0a20 2020 2020  ocated as:.     
-000023d0: 2020 2020 2020 205b 415d 5b42 5d5b 435d         [A][B][C]
-000023e0: 5b44 5d20 4020 5820 2b3d 2059 0a20 2020  [D] @ X += Y.   
-000023f0: 2020 2020 2072 6573 756c 7473 2069 6e3a       results in:
-00002400: 0a20 2020 2020 2020 2020 2020 2058 202b  .            X +
-00002410: 2069 302a 422a 432a 442a 5920 2b20 6931   i0*B*C*D*Y + i1
-00002420: 2a43 2a44 2a59 202b 2069 322a 442a 5920  *C*D*Y + i2*D*Y 
-00002430: 2b20 6933 2a59 0a20 2020 2020 2020 207a  + i3*Y.        z
-00002440: 0427 6825 7872 1000 0000 7a0b 202b 2069  .'h%xr....z. + i
-00002450: 2564 2a27 6825 7829 06da 1272 6177 5f61  %d*'h%x)...raw_a
-00002460: 6464 7265 7373 5f6f 6666 7365 74da 0869  ddress_offset..i
-00002470: 735f 6172 7261 79da 0572 616e 6765 da03  s_array..range..
-00002480: 6c65 6eda 1061 7272 6179 5f64 696d 656e  len..array_dimen
-00002490: 7369 6f6e 73da 0c61 7272 6179 5f73 7472  sions..array_str
-000024a0: 6964 6529 0672 3100 0000 7236 0000 0072  ide).r1...r6...r
-000024b0: 6e00 0000 da01 69da 016d da01 6a72 3300  n.....i..m..jr3.
-000024c0: 0000 7233 0000 0072 3400 0000 7257 0000  ..r3...r4...rW..
-000024d0: 0086 0100 0073 1000 0000 0a08 0601 1201  .....s..........
-000024e0: 0601 1801 1001 1201 0401 7a2b 6555 564d  ..........z+eUVM
-000024f0: 4578 706f 7274 6572 2e5f 6765 745f 6172  Exporter._get_ar
-00002500: 7261 795f 6164 6472 6573 735f 6f66 6673  ray_address_offs
-00002510: 6574 5f65 7870 7263 0200 0000 0000 0000  et_exprc........
-00002520: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-00002530: 7326 0000 007c 016a 007d 027c 02a0 0164  s&...|.j.}.|...d
-00002540: 01a1 0172 0a64 0253 007c 02a0 0164 03a1  ...r.d.S.|...d..
-00002550: 0172 1164 0453 0064 0553 0029 064e da09  .r.d.S.d.S.).N..
-00002560: 6269 6765 6e64 6961 6eda 0e55 564d 5f42  bigendian..UVM_B
-00002570: 4947 5f45 4e44 4941 4eda 0c6c 6974 746c  IG_ENDIAN..littl
-00002580: 6565 6e64 6961 6eda 1155 564d 5f4c 4954  eendian..UVM_LIT
-00002590: 544c 455f 454e 4449 414e da0d 5556 4d5f  TLE_ENDIAN..UVM_
-000025a0: 4e4f 5f45 4e44 4941 4e29 02da 0e6f 776e  NO_ENDIAN)...own
-000025b0: 696e 675f 6164 6472 6d61 7072 4900 0000  ing_addrmaprI...
-000025c0: 2903 7231 0000 0072 3600 0000 da04 616d  ).r1...r6.....am
-000025d0: 6170 7233 0000 0072 3300 0000 7234 0000  apr3...r3...r4..
-000025e0: 0072 5800 0000 9801 0000 730c 0000 0006  .rX.......s.....
-000025f0: 010a 0104 010a 0104 0104 027a 1c65 5556  ...........z.eUV
-00002600: 4d45 7870 6f72 7465 722e 5f67 6574 5f65  MExporter._get_e
-00002610: 6e64 6961 6e6e 6573 7363 0200 0000 0000  ndiannessc......
-00002620: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00002630: 0000 732a 0000 007c 006a 007c 01a0 01a1  ..s*...|.j.|....
-00002640: 0019 007d 027c 0264 0116 0072 117c 0264  ...}.|.d...r.|.d
-00002650: 011a 0064 0217 0053 007c 0264 011a 0053  ...d...S.|.d...S
-00002660: 0029 037a 400a 2020 2020 2020 2020 5265  .).z@.        Re
-00002670: 7475 726e 7320 6772 6f75 702d 6c69 6b65  turns group-like
-00002680: 206e 6f64 6527 7320 6275 7320 7769 6474   node's bus widt
-00002690: 6820 2869 6e20 6279 7465 7329 0a20 2020  h (in bytes).   
-000026a0: 2020 2020 20e9 0800 0000 7210 0000 0029       .....r....)
-000026b0: 0272 2e00 0000 da08 6765 745f 7061 7468  .r......get_path
-000026c0: 2903 7231 0000 0072 3600 0000 da05 7769  ).r1...r6.....wi
-000026d0: 6474 6872 3300 0000 7233 0000 0072 3400  dthr3...r3...r4.
-000026e0: 0000 7259 0000 00a2 0100 0073 0800 0000  ..rY.......s....
-000026f0: 0e04 0803 0c01 0802 7a1b 6555 564d 4578  ........z.eUVMEx
-00002700: 706f 7274 6572 2e5f 6765 745f 6275 735f  porter._get_bus_
-00002710: 7769 6474 68da 0178 da01 6e63 0300 0000  width..x..nc....
-00002720: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00002730: 4300 0000 7324 0000 007c 017c 0216 0072  C...s$...|.|...r
-00002740: 0c7c 017c 021a 0064 0117 007c 0214 0053  .|.|...d...|...S
-00002750: 007c 017c 021a 007c 0214 0053 0029 027a  .|.|...|...S.).z
-00002760: 2d0a 2020 2020 2020 2020 526f 756e 6420  -.        Round 
-00002770: 7820 7570 2074 6f20 7468 6520 6e65 6172  x up to the near
-00002780: 6573 7420 6e0a 2020 2020 2020 2020 7210  est n.        r.
-00002790: 0000 0072 3300 0000 2903 7231 0000 0072  ...r3...).r1...r
-000027a0: cc00 0000 72cd 0000 0072 3300 0000 7233  ....r....r3...r3
-000027b0: 0000 0072 3400 0000 725b 0000 00af 0100  ...r4...r[......
-000027c0: 0073 0600 0000 0804 1001 0c02 7a18 6555  .s..........z.eU
-000027d0: 564d 4578 706f 7274 6572 2e5f 726f 756e  VMExporter._roun
-000027e0: 6475 705f 746f 6302 0000 0000 0000 0000  dup_toc.........
-000027f0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00002800: 1000 0000 6401 7c01 6401 1800 a000 a100  ....d.|.d.......
-00002810: 3e00 5300 2902 4e72 1000 0000 2901 da0a  >.S.).Nr....)...
-00002820: 6269 745f 6c65 6e67 7468 2902 7231 0000  bit_length).r1..
-00002830: 0072 cc00 0000 7233 0000 0072 3300 0000  .r....r3...r3...
-00002840: 7234 0000 0072 5c00 0000 b901 0000 7302  r4...r\.......s.
-00002850: 0000 0010 017a 1a65 5556 4d45 7870 6f72  .....z.eUVMExpor
-00002860: 7465 722e 5f72 6f75 6e64 7570 5f70 6f77  ter._roundup_pow
-00002870: 324e 2901 727b 0000 0029 1c72 8600 0000  2N).r{...).r....
-00002880: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00002890: 7175 616c 6e61 6d65 5f5f 7235 0000 0072  qualname__r5...r
-000028a0: 0400 0000 da03 7374 7272 6500 0000 725e  ......strre...r^
-000028b0: 0000 0072 6000 0000 727a 0000 0072 0200  ...r`...rz...r..
-000028c0: 0000 7280 0000 0072 5300 0000 7254 0000  ..r....rS...rT..
-000028d0: 0072 5500 0000 da04 626f 6f6c 7252 0000  .rU.....boolrR..
-000028e0: 0072 0800 0000 7256 0000 0072 0900 0000  .r....rV...r....
-000028f0: 725a 0000 0072 0a00 0000 7257 0000 0072  rZ...r....rW...r
-00002900: 5800 0000 da03 696e 7472 5900 0000 725b  X.....intrY...r[
-00002910: 0000 0072 5c00 0000 7233 0000 0072 3300  ...r\...r3...r3.
-00002920: 0000 7233 0000 0072 3400 0000 7212 0000  ..r3...r4...r...
-00002930: 000e 0000 0073 2400 0000 0800 0802 123c  .....s$........<
-00002940: 1257 1206 1206 1c0f 1223 121b 1213 1207  .W.......#......
-00002950: 121c 124c 1208 1212 120a 160d 0c0a 7212  ...L..........r.
-00002960: 0000 0029 1a72 2400 0000 726b 0000 00da  ...).r$...rk....
-00002970: 0674 7970 696e 6772 0200 0000 da06 6a69  .typingr......ji
-00002980: 6e6a 6132 7221 0000 00da 0e73 7973 7465  nja2r!.....syste
-00002990: 6d72 646c 2e6e 6f64 6572 0300 0000 7204  mrdl.noder....r.
-000029a0: 0000 0072 0500 0000 7206 0000 0072 0700  ...r....r....r..
-000029b0: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-000029c0: 00da 1273 7973 7465 6d72 646c 2e72 646c  ...systemrdl.rdl
-000029d0: 7479 7065 7372 0b00 0000 720c 0000 0072  typesr....r....r
-000029e0: 0d00 0000 da13 7379 7374 656d 7264 6c2e  ......systemrdl.
-000029f0: 636f 6d70 6f6e 656e 7472 0e00 0000 da09  componentr......
-00002a00: 7379 7374 656d 7264 6c72 0f00 0000 da13  systemrdlr......
-00002a10: 7072 655f 6578 706f 7274 5f6c 6973 7465  pre_export_liste
-00002a20: 6e65 7272 1100 0000 7212 0000 0072 3300  nerr....r....r3.
-00002a30: 0000 7233 0000 0072 3300 0000 7234 0000  ..r3...r3...r4..
-00002a40: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00002a50: 1600 0000 0800 0801 0c01 0802 1c01 1401  ................
-00002a60: 1401 0c01 0c01 0c02 1202                 ..........
+000001c0: 6504 6505 6403 9c02 6404 6405 8404 5a06  e.e.d...d.d...Z.
+000001d0: 6505 6505 6406 9c02 6407 6408 8404 5a07  e.e.d...d.d...Z.
+000001e0: 6505 6505 6406 9c02 6409 640a 8404 5a08  e.e.d...d.d...Z.
+000001f0: 6504 6505 640b 9c02 640c 640d 8404 5a09  e.e.d...d.d...Z.
+00000200: 642c 6504 6505 650a 6505 1900 640f 9c03  d,e.e.e.e...d...
+00000210: 6410 6411 8405 5a0b 6504 6505 640b 9c02  d.d...Z.e.e.d...
+00000220: 6412 6413 8404 5a0c 6504 6505 640b 9c02  d.d...Z.e.e.d...
+00000230: 6414 6415 8404 5a0d 6504 6505 640b 9c02  d.d...Z.e.e.d...
+00000240: 6416 6417 8404 5a0e 6504 650f 640b 9c02  d.d...Z.e.e.d...
+00000250: 6418 6419 8404 5a10 6511 6505 641a 9c02  d.d...Z.e.e.d...
+00000260: 641b 641c 8404 5a12 6513 6505 641d 9c02  d.d...Z.e.e.d...
+00000270: 641e 641f 8404 5a14 6515 6505 640b 9c02  d.d...Z.e.e.d...
+00000280: 6420 6421 8404 5a16 6504 6505 640b 9c02  d d!..Z.e.e.d...
+00000290: 6422 6423 8404 5a17 6504 6518 640b 9c02  d"d#..Z.e.e.d...
+000002a0: 6424 6425 8404 5a19 6518 6518 6518 6426  d$d%..Z.e.e.e.d&
+000002b0: 9c03 6427 6428 8404 5a1a 6429 642a 8400  ..d'd(..Z.d)d*..
+000002c0: 5a1b 642b 5300 292d da0c 6555 564d 4578  Z.d+S.)-..eUVMEx
+000002d0: 706f 7274 6572 6301 0000 0000 0000 0000  porterc.........
+000002e0: 0000 0004 0000 000d 0000 004b 0000 0073  ...........K...s
+000002f0: 1201 0000 7c01 a000 6401 6402 a102 7d02  ....|...d.d...}.
+00000300: 7c01 a000 6403 6900 a102 7c00 5f01 7c01  |...d.i...|._.|.
+00000310: 7236 7402 6404 7403 7c01 a004 a100 8301  r6t.d.t.|.......
+00000320: 6405 1900 1600 8301 8201 7c02 7298 7405  d.........|.r.t.
+00000330: a006 7405 a007 7c02 a101 7405 a007 7408  ..t...|...t...t.
+00000340: 6a09 a00a 7408 6a09 a00b 740c a101 6406  j...t.j...t...d.
+00000350: a102 a101 7405 6a0d 7405 a007 7c02 a101  ....t.j.t...|...
+00000360: 7405 a007 7408 6a09 a00a 7408 6a09 a00b  t...t.j...t.j...
+00000370: 740c a101 6406 a102 a101 6407 9c02 6408  t...d.....d...d.
+00000380: 6409 8d02 6703 a101 7d03 6e4c 7405 a006  d...g...}.nLt...
+00000390: 7405 a007 7408 6a09 a00a 7408 6a09 a00b  t...t.j...t.j...
+000003a0: 740c a101 6406 a102 a101 7405 6a0d 640a  t...d.....t.j.d.
+000003b0: 7405 a007 7408 6a09 a00a 7408 6a09 a00b  t...t.j...t.j...
+000003c0: 740c a101 6406 a102 a101 6901 6408 6409  t...d.....i.d.d.
+000003d0: 8d02 6702 a101 7d03 7405 6a0e 7c03 7405  ..g...}.t.j.|.t.
+000003e0: 6a0f 640b 8d02 7c00 5f10 6402 7c00 5f11  j.d...|._.d.|._.
+000003f0: 6900 7c00 5f12 6900 7c00 5f13 640c 7c00  i.|._.i.|._.d.|.
+00000400: 5f14 6402 5300 290d 6143 0100 000a 2020  _.d.S.).aC....  
+00000410: 2020 2020 2020 436f 6e73 7472 7563 746f        Constructo
+00000420: 7220 666f 7220 7468 6520 6555 564d 2045  r for the eUVM E
+00000430: 7870 6f72 7465 7220 636c 6173 730a 0a20  xporter class.. 
+00000440: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00000450: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00000460: 2d2d 2d2d 0a20 2020 2020 2020 2075 7365  ----.        use
+00000470: 725f 7465 6d70 6c61 7465 5f64 6972 3a20  r_template_dir: 
+00000480: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00000490: 5061 7468 2074 6f20 6120 6469 7265 6374  Path to a direct
+000004a0: 6f72 7920 7768 6572 6520 7573 6572 2d64  ory where user-d
+000004b0: 6566 696e 6564 2074 656d 706c 6174 6520  efined template 
+000004c0: 6f76 6572 7269 6465 7320 6172 6520 7374  overrides are st
+000004d0: 6f72 6564 2e0a 2020 2020 2020 2020 7573  ored..        us
+000004e0: 6572 5f74 656d 706c 6174 655f 636f 6e74  er_template_cont
+000004f0: 6578 743a 2064 6963 740a 2020 2020 2020  ext: dict.      
+00000500: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+00000510: 2063 6f6e 7465 7874 2076 6172 6961 626c   context variabl
+00000520: 6573 2074 6f20 6c6f 6164 2069 6e74 6f20  es to load into 
+00000530: 7468 6520 7465 6d70 6c61 7465 206e 616d  the template nam
+00000540: 6573 7061 6365 2e0a 2020 2020 2020 2020  espace..        
+00000550: da11 7573 6572 5f74 656d 706c 6174 655f  ..user_template_
+00000560: 6469 724e da15 7573 6572 5f74 656d 706c  dirN..user_templ
+00000570: 6174 655f 636f 6e74 6578 74fa 2767 6f74  ate_context.'got
+00000580: 2061 6e20 756e 6578 7065 6374 6564 206b   an unexpected k
+00000590: 6579 776f 7264 2061 7267 756d 656e 7420  eyword argument 
+000005a0: 2725 7327 7201 0000 00da 0974 656d 706c  '%s'r......templ
+000005b0: 6174 6573 2902 da04 7573 6572 da04 6261  ates)...user..ba
+000005c0: 7365 fa01 3a29 01da 0964 656c 696d 6974  se..:)...delimit
+000005d0: 6572 7218 0000 0029 02da 066c 6f61 6465  err....)...loade
+000005e0: 72da 0975 6e64 6566 696e 6564 5429 15da  r..undefinedT)..
+000005f0: 0370 6f70 7214 0000 00da 0954 7970 6545  .popr......TypeE
+00000600: 7272 6f72 da04 6c69 7374 da04 6b65 7973  rror..list..keys
+00000610: da02 6a6a da0c 4368 6f69 6365 4c6f 6164  ..jj..ChoiceLoad
+00000620: 6572 da10 4669 6c65 5379 7374 656d 4c6f  er..FileSystemLo
+00000630: 6164 6572 da02 6f73 da04 7061 7468 da04  ader..os..path..
+00000640: 6a6f 696e da07 6469 726e 616d 65da 085f  join..dirname.._
+00000650: 5f66 696c 655f 5fda 0c50 7265 6669 784c  _file__..PrefixL
+00000660: 6f61 6465 72da 0b45 6e76 6972 6f6e 6d65  oader..Environme
+00000670: 6e74 da0f 5374 7269 6374 556e 6465 6669  nt..StrictUndefi
+00000680: 6e65 64da 066a 6a5f 656e 76da 0374 6f70  ned..jj_env..top
+00000690: da0c 6275 735f 7769 6474 685f 6462 da0c  ..bus_width_db..
+000006a0: 6e61 6d65 7370 6163 655f 6462 da17 7265  namespace_db..re
+000006b0: 7573 655f 636c 6173 735f 6465 6669 6e69  use_class_defini
+000006c0: 7469 6f6e 7329 04da 0473 656c 66da 066b  tions)...self..k
+000006d0: 7761 7267 7372 1300 0000 721b 0000 00a9  wargsr....r.....
+000006e0: 0072 3300 0000 fa2e 2f74 6d70 2f50 6561  .r3...../tmp/Pea
+000006f0: 6b52 444c 2d65 7576 6d2f 7372 632f 7065  kRDL-euvm/src/pe
+00000700: 616b 7264 6c5f 6575 766d 2f65 7870 6f72  akrdl_euvm/expor
+00000710: 7465 722e 7079 da08 5f5f 696e 6974 5f5f  ter.py..__init__
+00000720: 1000 0000 7340 0000 0000 0b0c 010e 0304  ....s@..........
+00000730: 0118 0204 0104 0108 011a 0104 0108 011a  ................
+00000740: fe04 0302 fd04 fd08 0904 011a 0104 0102  ................
+00000750: 001a ff02 0202 fe04 fe06 0704 0102 0104  ................
+00000760: fe08 0806 0606 0606 027a 1565 5556 4d45  .........z.eUVME
+00000770: 7870 6f72 7465 722e 5f5f 696e 6974 5f5f  xporter.__init__
+00000780: 2902 da04 6e6f 6465 7225 0000 0063 0300  )...noder%...c..
+00000790: 0000 0000 0000 0000 0000 0900 0000 1400  ................
+000007a0: 0000 4b00 0000 7348 0100 007c 03a0 0064  ..K...sH...|...d
+000007b0: 0164 02a1 027d 047c 03a0 0064 0364 04a1  .d...}.|...d.d..
+000007c0: 027d 057c 03a0 0064 0564 02a1 027c 005f  .}.|...d.d...|._
+000007d0: 017c 0372 4274 0264 0674 037c 03a0 04a1  .|.rBt.d.t.|....
+000007e0: 0083 0164 0719 0016 0083 0182 0174 057c  ...d.........t.|
+000007f0: 0174 0683 0272 527c 016a 077d 017c 017c  .t...rR|.j.}.|.|
+00000800: 005f 0774 057c 0174 0883 0272 8c7c 01a0  ._.t.|.t...r.|..
+00000810: 0964 08a1 0172 8c7c 016a 0a6a 0ba0 0c64  .d...r.|.j.j...d
+00000820: 097c 016a 0d6a 0ea0 0f64 087c 016a 0d6a  .|.j.j...d.|.j.j
+00000830: 10a1 02a1 0201 0069 007c 005f 1174 1283  .......i.|._.t..
+00000840: 00a0 137c 006a 0774 147c 0083 01a1 0201  ...|.j.t.|......
+00000850: 007c 0174 1574 1674 0874 1774 1874 057c  .|.t.t.t.t.t.t.|
+00000860: 006a 197c 006a 1a7c 006a 1b7c 006a 1c7c  .j.|.j.|.j.|.j.|
+00000870: 006a 1d7c 006a 1e7c 006a 1f7c 006a 207c  .j.|.j.|.j.|.j |
+00000880: 006a 217c 006a 227c 006a 237c 0564 0a9c  .j!|.j"|.j#|.d..
+00000890: 137d 067c 06a0 247c 006a 25a1 0101 007c  .}.|..$|.j%....|
+000008a0: 0490 0172 167c 00a0 267c 02a1 017c 0664  ...r.|..&|...|.d
+000008b0: 0b3c 007c 006a 27a0 2864 0ca1 017d 076e  .<.|.j'.(d...}.n
+000008c0: 1a7c 00a0 297c 02a1 017c 0664 0d3c 007c  .|..)|...|.d.<.|
+000008d0: 006a 27a0 2864 0ea1 017d 077c 07a0 2a7c  .j'.(d...}.|..*|
+000008e0: 06a1 017d 087c 08a0 2b7c 02a1 0101 0064  ...}.|..+|.....d
+000008f0: 0f53 0029 1061 7604 0000 0a20 2020 2020  .S.).av....     
+00000900: 2020 2050 6572 666f 726d 2074 6865 2065     Perform the e
+00000910: 7870 6f72 7421 0a0a 2020 2020 2020 2020  xport!..        
+00000920: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00000930: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000940: 2020 2020 2020 6e6f 6465 3a20 7379 7374        node: syst
+00000950: 656d 7264 6c2e 4e6f 6465 0a20 2020 2020  emrdl.Node.     
+00000960: 2020 2020 2020 2054 6f70 2d6c 6576 656c         Top-level
+00000970: 206e 6f64 6520 746f 2065 7870 6f72 742e   node to export.
+00000980: 2043 616e 2062 6520 7468 6520 746f 702d   Can be the top-
+00000990: 6c65 7665 6c20 6052 6f6f 744e 6f64 6560  level `RootNode`
+000009a0: 206f 7220 616e 790a 2020 2020 2020 2020   or any.        
+000009b0: 2020 2020 696e 7465 726e 616c 2060 4164      internal `Ad
+000009c0: 6472 6d61 704e 6f64 6560 2e0a 2020 2020  drmapNode`..    
+000009d0: 2020 2020 7061 7468 3a20 7374 720a 2020      path: str.  
+000009e0: 2020 2020 2020 2020 2020 4f75 7470 7574            Output
+000009f0: 2066 696c 652e 0a20 2020 2020 2020 2065   file..        e
+00000a00: 7870 6f72 745f 6173 5f70 6163 6b61 6765  xport_as_package
+00000a10: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+00000a20: 2020 2049 6620 5472 7565 2028 4465 6661     If True (Defa
+00000a30: 756c 7429 2c20 6555 564d 2072 6567 6973  ult), eUVM regis
+00000a40: 7465 7220 6d6f 6465 6c20 6973 2065 7870  ter model is exp
+00000a50: 6f72 7465 6420 6173 2061 2053 7973 7465  orted as a Syste
+00000a60: 6d56 6572 696c 6f67 0a20 2020 2020 2020  mVerilog.       
+00000a70: 2020 2020 2070 6163 6b61 6765 2e20 5061       package. Pa
+00000a80: 636b 6167 6520 6e61 6d65 2069 7320 6261  ckage name is ba
+00000a90: 7365 6420 6f6e 2074 6865 206f 7574 7075  sed on the outpu
+00000aa0: 7420 6669 6c65 206e 616d 652e 0a0a 2020  t file name...  
+00000ab0: 2020 2020 2020 2020 2020 4966 2046 616c            If Fal
+00000ac0: 7365 2c20 7265 6769 7374 6572 206d 6f64  se, register mod
+00000ad0: 656c 2069 7320 6578 706f 7274 6564 2061  el is exported a
+00000ae0: 7320 616e 2069 6e63 6c75 6461 626c 6520  s an includable 
+00000af0: 6865 6164 6572 2e0a 2020 2020 2020 2020  header..        
+00000b00: 7265 7573 655f 636c 6173 735f 6465 6669  reuse_class_defi
+00000b10: 6e69 7469 6f6e 733a 2062 6f6f 6c0a 2020  nitions: bool.  
+00000b20: 2020 2020 2020 2020 2020 4966 2054 7275            If Tru
+00000b30: 6520 2844 6566 6175 6c74 292c 2065 7870  e (Default), exp
+00000b40: 6f72 7465 7220 6174 7465 6d70 7473 2074  orter attempts t
+00000b50: 6f20 7265 2d75 7365 2063 6c61 7373 2064  o re-use class d
+00000b60: 6566 696e 6974 696f 6e73 0a20 2020 2020  efinitions.     
+00000b70: 2020 2020 2020 2077 6865 7265 2070 6f73         where pos
+00000b80: 7369 626c 652e 2043 6c61 7373 206e 616d  sible. Class nam
+00000b90: 6573 2061 7265 2062 6173 6564 206f 6e20  es are based on 
+00000ba0: 7468 6520 6c65 7869 6361 6c20 7363 6f70  the lexical scop
+00000bb0: 6520 6f66 2074 6865 0a20 2020 2020 2020  e of the.       
+00000bc0: 2020 2020 206f 7269 6769 6e61 6c20 5379       original Sy
+00000bd0: 7374 656d 5244 4c20 6465 6669 6e69 7469  stemRDL definiti
+00000be0: 6f6e 732e 0a0a 2020 2020 2020 2020 2020  ons...          
+00000bf0: 2020 4966 2046 616c 7365 2c20 636c 6173    If False, clas
+00000c00: 7320 6465 6669 6e69 7469 6f6e 7320 6172  s definitions ar
+00000c10: 6520 6e6f 7420 7265 7573 6564 2e20 436c  e not reused. Cl
+00000c20: 6173 7320 6e61 6d65 7320 6172 6520 6261  ass names are ba
+00000c30: 7365 6420 6f6e 0a20 2020 2020 2020 2020  sed on.         
+00000c40: 2020 2074 6865 2069 6e73 7461 6e63 6527     the instance'
+00000c50: 7320 6869 6572 6172 6368 6963 616c 2070  s hierarchical p
+00000c60: 6174 682e 0a20 2020 2020 2020 2075 7365  ath..        use
+00000c70: 5f75 766d 5f66 6163 746f 7279 3a20 626f  _uvm_factory: bo
+00000c80: 6f6c 0a20 2020 2020 2020 2020 2020 2049  ol.            I
+00000c90: 6620 5472 7565 2c20 636c 6173 7320 6465  f True, class de
+00000ca0: 6669 6e69 7469 6f6e 7320 616e 6420 636c  finitions and cl
+00000cb0: 6173 7320 696e 7374 616e 6365 7320 6172  ass instances ar
+00000cc0: 6520 6372 6561 7465 6420 7573 696e 6720  e created using 
+00000cd0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00000ce0: 5556 4d20 6661 6374 6f72 792e 0a0a 2020  UVM factory...  
+00000cf0: 2020 2020 2020 2020 2020 4966 2046 616c            If Fal
+00000d00: 7365 2028 4465 6661 756c 7429 2c20 5556  se (Default), UV
+00000d10: 4d20 6661 6374 6f72 7920 6973 2064 6973  M factory is dis
+00000d20: 6162 6c65 642e 2043 6c61 7373 6573 2061  abled. Classes a
+00000d30: 7265 2063 7265 6174 6564 0a20 2020 2020  re created.     
+00000d40: 2020 2020 2020 2064 6972 6563 746c 7920         directly 
+00000d50: 7669 6120 6e65 7728 2920 636f 6e73 7472  via new() constr
+00000d60: 7563 746f 7273 2e0a 2020 2020 2020 2020  uctors..        
+00000d70: da11 6578 706f 7274 5f61 735f 7061 636b  ..export_as_pack
+00000d80: 6167 6554 da0f 7573 655f 7576 6d5f 6661  ageT..use_uvm_fa
+00000d90: 6374 6f72 7946 7230 0000 0072 1500 0000  ctoryFr0...r....
+00000da0: 7201 0000 00da 0662 7269 6467 657a 6e65  r......bridgezne
+00000db0: 5556 4d20 5241 4c20 6765 6e65 7261 746f  UVM RAL generato
+00000dc0: 7220 646f 6573 206e 6f74 2068 6176 6520  r does not have 
+00000dd0: 7072 6f70 6572 2073 7570 706f 7274 2066  proper support f
+00000de0: 6f72 2062 7269 6467 6520 6164 646d 6170  or bridge addmap
+00000df0: 7320 7965 742e 2054 6865 2027 6272 6964  s yet. The 'brid
+00000e00: 6765 2720 7072 6f70 6572 7479 2077 696c  ge' property wil
+00000e10: 6c20 6265 2069 676e 6f72 6564 2e29 13da  l be ignored.)..
+00000e20: 0874 6f70 5f6e 6f64 6572 0500 0000 7207  .top_noder....r.
+00000e30: 0000 0072 0600 0000 7209 0000 0072 0a00  ...r....r....r..
+00000e40: 0000 da0a 6973 696e 7374 616e 6365 5a16  ....isinstanceZ.
+00000e50: 636c 6173 735f 6e65 6564 735f 6465 6669  class_needs_defi
+00000e60: 6e69 7469 6f6e 5a0e 6765 745f 636c 6173  nitionZ.get_clas
+00000e70: 735f 6e61 6d65 5a17 6765 745f 636c 6173  s_nameZ.get_clas
+00000e80: 735f 6672 6965 6e64 6c79 5f6e 616d 655a  s_friendly_nameZ
+00000e90: 0d67 6574 5f69 6e73 745f 6e61 6d65 5a10  .get_inst_nameZ.
+00000ea0: 6765 745f 6669 656c 645f 6163 6365 7373  get_field_access
+00000eb0: 5a1d 6765 745f 6172 7261 795f 6164 6472  Z.get_array_addr
+00000ec0: 6573 735f 6f66 6673 6574 5f65 7870 725a  ess_offset_exprZ
+00000ed0: 0e67 6574 5f65 6e64 6961 6e6e 6573 735a  .get_endiannessZ
+00000ee0: 0d67 6574 5f62 7573 5f77 6964 7468 5a0e  .get_bus_widthZ.
+00000ef0: 6765 745f 6d65 6d5f 6163 6365 7373 da0a  get_mem_access..
+00000f00: 726f 756e 6475 705f 746f da0c 726f 756e  roundup_to..roun
+00000f10: 6475 705f 706f 7732 7238 0000 00da 0c70  dup_pow2r8.....p
+00000f20: 6163 6b61 6765 5f6e 616d 657a 0974 6f70  ackage_namez.top
+00000f30: 5f70 6b67 2e64 5a0d 696e 636c 7564 655f  _pkg.dZ.include_
+00000f40: 6775 6172 647a 0d74 6f70 5f69 6e63 6c75  guardz.top_inclu
+00000f50: 6465 2e64 4e29 2c72 1d00 0000 7230 0000  de.dN),r....r0..
+00000f60: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000f70: 723b 0000 0072 0300 0000 722d 0000 0072  r;...r....r-...r
+00000f80: 0600 0000 da0c 6765 745f 7072 6f70 6572  ......get_proper
+00000f90: 7479 da03 656e 76da 036d 7367 da07 7761  ty..env..msg..wa
+00000fa0: 726e 696e 67da 0469 6e73 74da 1070 726f  rning..inst..pro
+00000fb0: 7065 7274 795f 7372 635f 7265 66da 0367  perty_src_ref..g
+00000fc0: 6574 da0c 696e 7374 5f73 7263 5f72 6566  et..inst_src_ref
+00000fd0: 722e 0000 0072 0f00 0000 da04 7761 6c6b  r....r......walk
+00000fe0: 7211 0000 0072 0500 0000 7207 0000 0072  r....r....r....r
+00000ff0: 0900 0000 720a 0000 00da 175f 636c 6173  ....r......_clas
+00001000: 735f 6e65 6564 735f 6465 6669 6e69 7469  s_needs_definiti
+00001010: 6f6e da0f 5f67 6574 5f63 6c61 7373 5f6e  on.._get_class_n
+00001020: 616d 65da 185f 6765 745f 636c 6173 735f  ame.._get_class_
+00001030: 6672 6965 6e64 6c79 5f6e 616d 65da 0e5f  friendly_name.._
+00001040: 6765 745f 696e 7374 5f6e 616d 65da 115f  get_inst_name.._
+00001050: 6765 745f 6669 656c 645f 6163 6365 7373  get_field_access
+00001060: da1e 5f67 6574 5f61 7272 6179 5f61 6464  .._get_array_add
+00001070: 7265 7373 5f6f 6666 7365 745f 6578 7072  ress_offset_expr
+00001080: da0f 5f67 6574 5f65 6e64 6961 6e6e 6573  .._get_endiannes
+00001090: 73da 0e5f 6765 745f 6275 735f 7769 6474  s.._get_bus_widt
+000010a0: 68da 0f5f 6765 745f 6d65 6d5f 6163 6365  h.._get_mem_acce
+000010b0: 7373 da0b 5f72 6f75 6e64 7570 5f74 6fda  ss.._roundup_to.
+000010c0: 0d5f 726f 756e 6475 705f 706f 7732 da06  ._roundup_pow2..
+000010d0: 7570 6461 7465 7214 0000 00da 115f 6765  updater......_ge
+000010e0: 745f 7061 636b 6167 655f 6e61 6d65 722c  t_package_namer,
+000010f0: 0000 00da 0c67 6574 5f74 656d 706c 6174  .....get_templat
+00001100: 65da 125f 6765 745f 696e 636c 7564 655f  e.._get_include_
+00001110: 6775 6172 64da 0673 7472 6561 6dda 0464  guard..stream..d
+00001120: 756d 7029 0972 3100 0000 7236 0000 0072  ump).r1...r6...r
+00001130: 2500 0000 7232 0000 0072 3700 0000 7238  %...r2...r7...r8
+00001140: 0000 00da 0763 6f6e 7465 7874 da08 7465  .....context..te
+00001150: 6d70 6c61 7465 7257 0000 0072 3300 0000  mplaterW...r3...
+00001160: 7233 0000 0072 3400 0000 da06 6578 706f  r3...r4.....expo
+00001170: 7274 4c00 0000 7356 0000 0000 1e0c 010c  rtL...sV........
+00001180: 010e 0304 0118 030a 0106 0106 0214 0108  ................
+00001190: 0102 0112 fe04 0606 0114 0302 0102 0102  ................
+000011a0: 0102 0102 0102 0102 0104 0104 0104 0104  ................
+000011b0: 0104 0104 0104 0104 0104 0104 0104 0102  ................
+000011c0: ed06 160c 0206 010e 010e 020e 010c 010a  ................
+000011d0: 017a 1365 5556 4d45 7870 6f72 7465 722e  .z.eUVMExporter.
+000011e0: 6578 706f 7274 2902 7225 0000 00da 0672  export).r%.....r
+000011f0: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
+00001200: 0000 0300 0000 0500 0000 4300 0000 732a  ..........C...s*
+00001210: 0000 0074 006a 01a0 0274 006a 01a0 037c  ...t.j...t.j...|
+00001220: 01a1 01a1 0164 0119 007d 0274 04a0 0564  .....d...}.t...d
+00001230: 0264 037c 02a1 037d 027c 0253 0029 044e  .d.|...}.|.S.).N
+00001240: 7201 0000 00fa 055b 5e5c 775d da01 5f29  r......[^\w].._)
+00001250: 0672 2400 0000 7225 0000 00da 0873 706c  .r$...r%.....spl
+00001260: 6974 6578 74da 0862 6173 656e 616d 65da  itext..basename.
+00001270: 0272 65da 0373 7562 a903 7231 0000 0072  .re..sub..r1...r
+00001280: 2500 0000 da01 7372 3300 0000 7233 0000  %.....sr3...r3..
+00001290: 0072 3400 0000 7254 0000 00a3 0000 0073  .r4...rT.......s
+000012a0: 0600 0000 0001 1801 0e01 7a1e 6555 564d  ..........z.eUVM
+000012b0: 4578 706f 7274 6572 2e5f 6765 745f 7061  Exporter._get_pa
+000012c0: 636b 6167 655f 6e61 6d65 6302 0000 0000  ckage_namec.....
+000012d0: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+000012e0: 0000 0073 2200 0000 7400 6a01 a002 7c01  ...s"...t.j...|.
+000012f0: a101 7d02 7403 a004 6401 6402 7c02 a103  ..}.t...d.d.|...
+00001300: a005 a100 7d02 7c02 5300 2903 4e72 5d00  ....}.|.S.).Nr].
+00001310: 0000 725e 0000 0029 0672 2400 0000 7225  ..r^...).r$...r%
+00001320: 0000 0072 6000 0000 7261 0000 0072 6200  ...r`...ra...rb.
+00001330: 0000 da05 7570 7065 7272 6300 0000 7233  ....upperrc...r3
+00001340: 0000 0072 3300 0000 7234 0000 0072 5600  ...r3...r4...rV.
+00001350: 0000 a900 0000 7306 0000 0000 010c 0112  ......s.........
+00001360: 017a 1f65 5556 4d45 7870 6f72 7465 722e  .z.eUVMExporter.
+00001370: 5f67 6574 5f69 6e63 6c75 6465 5f67 7561  _get_include_gua
+00001380: 7264 2902 7236 0000 0072 5c00 0000 6302  rd).r6...r\...c.
+00001390: 0000 0000 0000 0000 0000 0003 0000 0006  ................
+000013a0: 0000 0043 0000 0073 2200 0000 7c00 6a00  ...C...s"...|.j.
+000013b0: 7208 6e16 7c01 6a01 7c00 6a02 6a03 6401  r.n.|.j.|.j.j.d.
+000013c0: 6402 6402 6403 8d04 7d02 7c02 5300 2904  d.d.d...}.|.S.).
+000013d0: fa6d 0a20 2020 2020 2020 2052 6574 7572  .m.        Retur
+000013e0: 6e73 2074 6865 2063 6c61 7373 2074 7970  ns the class typ
+000013f0: 6520 6e61 6d65 2e0a 2020 2020 2020 2020  e name..        
+00001400: 5368 616c 6c20 6265 2075 6e69 7175 6520  Shall be unique 
+00001410: 656e 6f75 6768 2074 6f20 7072 6576 656e  enough to preven
+00001420: 7420 7479 7065 206e 616d 6520 636f 6c6c  t type name coll
+00001430: 6973 696f 6e73 0a20 2020 2020 2020 20da  isions.        .
+00001440: 025f 5fda 00a9 03da 0e68 6965 725f 7365  .__......hier_se
+00001450: 7061 7261 746f 72da 0c61 7272 6179 5f73  parator..array_s
+00001460: 7566 6669 78da 1265 6d70 7479 5f61 7272  uffix..empty_arr
+00001470: 6179 5f73 7566 6669 7829 0472 3000 0000  ay_suffix).r0...
+00001480: da0c 6765 745f 7265 6c5f 7061 7468 722d  ..get_rel_pathr-
+00001490: 0000 00da 0670 6172 656e 7429 0372 3100  .....parent).r1.
+000014a0: 0000 7236 0000 00da 0a63 6c61 7373 5f6e  ..r6.....class_n
+000014b0: 616d 6572 3300 0000 7233 0000 0072 3400  amer3...r3...r4.
+000014c0: 0000 da13 5f67 6574 5f63 6c61 7373 5f6e  ...._get_class_n
+000014d0: 616d 655f 6e65 77af 0000 0073 1200 0000  ame_new....s....
+000014e0: 0005 0601 0202 0401 0601 0200 0200 02fe  ................
+000014f0: 0605 7a20 6555 564d 4578 706f 7274 6572  ..z eUVMExporter
+00001500: 2e5f 6765 745f 636c 6173 735f 6e61 6d65  ._get_class_name
+00001510: 5f6e 6577 fa02 3a3a 2903 7236 0000 00da  _new..::).r6....
+00001520: 0973 6570 6172 6174 6f72 725c 0000 0063  .separatorr\...c
+00001530: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00001540: 0400 0000 4300 0000 738a 0000 007c 016a  ....C...s....|.j
+00001550: 006a 0164 016b 0872 1064 0153 0074 027c  .j.d.k.r.d.S.t.|
+00001560: 016a 006a 0174 0383 0272 247c 016a 0453  .j.j.t...r$|.j.S
+00001570: 007c 016a 057d 037c 0372 867c 036a 006a  .|.j.}.|.r.|.j.j
+00001580: 0664 016b 0872 3e64 0153 007c 036a 006a  .d.k.r>d.S.|.j.j
+00001590: 067c 016a 006a 016b 0872 7e7c 00a0 077c  .|.j.j.k.r~|...|
+000015a0: 037c 02a1 027d 047c 0464 016b 0873 6c7c  .|...}.|.d.k.sl|
+000015b0: 016a 0464 016b 0872 7064 0153 007c 047c  .j.d.k.rpd.S.|.|
+000015c0: 0217 007c 016a 0417 0053 007c 036a 057d  ...|.j...S.|.j.}
+000015d0: 0371 2a64 0153 0029 027a 810a 2020 2020  .q*d.S.).z..    
+000015e0: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
+000015f0: 7363 6f70 6520 7061 7468 2c20 6275 7420  scope path, but 
+00001600: 7769 7468 2072 6573 6f6c 7665 6420 7479  with resolved ty
+00001610: 7065 206e 616d 6573 0a20 2020 2020 2020  pe names.       
+00001620: 2052 6574 7572 6e73 204e 6f6e 6520 6966   Returns None if
+00001630: 2061 6e79 2073 6567 6d65 6e74 2069 6e20   any segment in 
+00001640: 7468 6520 7061 7468 2069 7320 756e 6b6e  the path is unkn
+00001650: 6f77 6e0a 2020 2020 2020 2020 4e29 0872  own.        N).r
+00001660: 4300 0000 da0c 7061 7265 6e74 5f73 636f  C.....parent_sco
+00001670: 7065 723b 0000 0072 0e00 0000 da09 7479  per;...r......ty
+00001680: 7065 5f6e 616d 6572 6e00 0000 da0c 6f72  pe_namern.....or
+00001690: 6967 696e 616c 5f64 6566 da18 5f67 6574  iginal_def.._get
+000016a0: 5f72 6573 6f6c 7665 645f 7363 6f70 655f  _resolved_scope_
+000016b0: 7061 7468 2905 7231 0000 0072 3600 0000  path).r1...r6...
+000016c0: 7272 0000 005a 1363 7572 7265 6e74 5f70  rr...Z.current_p
+000016d0: 6172 656e 745f 6e6f 6465 5a11 7061 7265  arent_nodeZ.pare
+000016e0: 6e74 5f73 636f 7065 5f70 6174 6872 3300  nt_scope_pathr3.
+000016f0: 0000 7233 0000 0072 3400 0000 7276 0000  ..r3...r4...rv..
+00001700: 00be 0000 0073 1e00 0000 0006 0c02 0402  .....s..........
+00001710: 0e02 0605 0602 0401 0c02 0401 1002 0c01  ................
+00001720: 1201 0401 0e02 0803 7a25 6555 564d 4578  ........z%eUVMEx
+00001730: 706f 7274 6572 2e5f 6765 745f 7265 736f  porter._get_reso
+00001740: 6c76 6564 5f73 636f 7065 5f70 6174 6863  lved_scope_pathc
+00001750: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00001760: 0600 0000 4300 0000 735a 0000 007c 006a  ....C...sZ...|.j
+00001770: 0072 407c 00a0 017c 0164 01a1 027d 027c  .r@|...|.d...}.|
+00001780: 0264 026b 0972 207c 027d 0371 567c 016a  .d.k.r |.}.qV|.j
+00001790: 027c 006a 036a 0464 0164 0364 0364 048d  .|.j.j.d.d.d.d..
+000017a0: 047d 0364 057c 0317 007d 036e 167c 016a  .}.d.|...}.n.|.j
+000017b0: 027c 006a 036a 0464 0164 0364 0364 048d  .|.j.j.d.d.d.d..
+000017c0: 047d 037c 0353 0029 0672 6600 0000 7267  .}.|.S.).rf...rg
+000017d0: 0000 004e 7268 0000 0072 6900 0000 5a07  ...Nrh...ri...Z.
+000017e0: 7874 6572 6e5f 5f29 0572 3000 0000 7276  xtern__).r0...rv
+000017f0: 0000 0072 6d00 0000 722d 0000 0072 6e00  ...rm...r-...rn.
+00001800: 0000 2904 7231 0000 0072 3600 0000 da0a  ..).r1...r6.....
+00001810: 7363 6f70 655f 7061 7468 726f 0000 0072  scope_pathro...r
+00001820: 3300 0000 7233 0000 0072 3400 0000 7249  3...r3...r4...rI
+00001830: 0000 00e1 0000 0073 2400 0000 0005 0601  .......s$.......
+00001840: 0c02 0801 0603 0401 0601 0200 0200 02fe  ................
+00001850: 0605 0a02 0401 0601 0200 0200 02fe 0605  ................
+00001860: 7a1c 6555 564d 4578 706f 7274 6572 2e5f  z.eUVMExporter._
+00001870: 6765 745f 636c 6173 735f 6e61 6d65 6302  get_class_namec.
+00001880: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00001890: 0000 0043 0000 0073 5000 0000 7c00 6a00  ...C...sP...|.j.
+000018a0: 722e 7c00 a001 7c01 a101 7d02 7c02 6401  r.|...|...}.|.d.
+000018b0: 6b09 721e 7c02 7d03 713c 7c01 a002 7c00  k.r.|.}.q<|...|.
+000018c0: 6a03 6a04 a101 7d03 6e0e 7c01 a002 7c00  j.j...}.n.|...|.
+000018d0: 6a03 6a04 a101 7d03 7405 7c01 6a06 8301  j.j...}.t.|.j...
+000018e0: 6a07 6402 1700 7c03 1700 5300 2903 7a67  j.d...|...S.).zg
+000018f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001900: 2061 2075 7365 6675 6c20 7374 7269 6e67   a useful string
+00001910: 2074 6861 7420 6865 6c70 7320 6964 656e   that helps iden
+00001920: 7469 6679 2074 6865 2063 6c61 7373 2064  tify the class d
+00001930: 6566 696e 6974 696f 6e20 696e 0a20 2020  efinition in.   
+00001940: 2020 2020 2061 2063 6f6d 6d65 6e74 0a20       a comment. 
+00001950: 2020 2020 2020 204e 7a03 202d 2029 0872         Nz. - ).r
+00001960: 3000 0000 7276 0000 0072 6d00 0000 722d  0...rv...rm...r-
+00001970: 0000 0072 6e00 0000 da04 7479 7065 7243  ...rn.....typerC
+00001980: 0000 00da 085f 5f6e 616d 655f 5f29 0472  .....__name__).r
+00001990: 3100 0000 7236 0000 0072 7700 0000 5a0d  1...r6...rw...Z.
+000019a0: 6672 6965 6e64 6c79 5f6e 616d 6572 3300  friendly_namer3.
+000019b0: 0000 7233 0000 0072 3400 0000 724a 0000  ..r3...r4...rJ..
+000019c0: 00fc 0000 0073 0e00 0000 0005 0601 0a02  .....s..........
+000019d0: 0801 0603 1002 0e02 7a25 6555 564d 4578  ........z%eUVMEx
+000019e0: 706f 7274 6572 2e5f 6765 745f 636c 6173  porter._get_clas
+000019f0: 735f 6672 6965 6e64 6c79 5f6e 616d 6563  s_friendly_namec
+00001a00: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001a10: 0100 0000 4300 0000 7306 0000 007c 016a  ....C...s....|.j
+00001a20: 0053 0029 017a 310a 2020 2020 2020 2020  .S.).z1.        
+00001a30: 5265 7475 726e 7320 7468 6520 636c 6173  Returns the clas
+00001a40: 7320 696e 7374 616e 6365 206e 616d 650a  s instance name.
+00001a50: 2020 2020 2020 2020 2901 da09 696e 7374          )...inst
+00001a60: 5f6e 616d 6529 0272 3100 0000 7236 0000  _name).r1...r6..
+00001a70: 0072 3300 0000 7233 0000 0072 3400 0000  .r3...r3...r4...
+00001a80: 724b 0000 000f 0100 0073 0200 0000 0004  rK.......s......
+00001a90: 7a1b 6555 564d 4578 706f 7274 6572 2e5f  z.eUVMExporter._
+00001aa0: 6765 745f 696e 7374 5f6e 616d 6563 0200  get_inst_namec..
+00001ab0: 0000 0000 0000 0000 0000 0400 0000 0300  ................
+00001ac0: 0000 4300 0000 7350 0000 007c 00a0 007c  ..C...sP...|...|
+00001ad0: 01a1 017d 027c 027c 006a 016b 0672 3e7c  ...}.|.|.j.k.r>|
+00001ae0: 006a 017c 0219 007d 037c 0364 016b 0873  .j.|...}.|.d.k.s
+00001af0: 327c 037c 016a 026a 036b 0972 3a74 0464  2|.|.j.j.k.r:t.d
+00001b00: 0283 0182 0164 0353 007c 016a 026a 037c  .....d.S.|.j.j.|
+00001b10: 006a 017c 023c 0064 0453 0029 0561 6c01  .j.|.<.d.S.).al.
+00001b20: 0000 0a20 2020 2020 2020 2043 6865 636b  ...        Check
+00001b30: 7320 6966 2074 6865 2063 6c61 7373 2074  s if the class t
+00001b40: 6861 7420 6465 6669 6e65 7320 7468 6973  hat defines this
+00001b50: 206e 6f64 6520 616c 7265 6164 7920 6578   node already ex
+00001b60: 6973 7473 2e0a 2020 2020 2020 2020 4966  ists..        If
+00001b70: 206e 6f74 2c20 7265 7475 726e 7320 5472   not, returns Tr
+00001b80: 7565 2c20 696e 6469 6361 7469 6e67 2074  ue, indicating t
+00001b90: 6861 7420 6120 6465 6669 6e69 7469 6f6e  hat a definition
+00001ba0: 2073 6861 6c6c 2062 6520 656d 6974 7465   shall be emitte
+00001bb0: 642e 0a0a 2020 2020 2020 2020 4966 2072  d...        If r
+00001bc0: 6574 7572 6e69 6e67 2054 7275 652c 2074  eturning True, t
+00001bd0: 6865 6e20 7468 6520 6163 7420 6f66 2063  hen the act of c
+00001be0: 616c 6c69 6e67 2074 6869 7320 6675 6e63  alling this func
+00001bf0: 7469 6f6e 2061 6c73 6f20 7265 6769 7374  tion also regist
+00001c00: 6572 730a 2020 2020 2020 2020 7468 6520  ers.        the 
+00001c10: 636c 6173 7320 6465 6669 6e69 7469 6f6e  class definition
+00001c20: 2069 6e74 6f20 7468 6520 6e61 6d65 7370   into the namesp
+00001c30: 6163 6520 6461 7461 6261 7365 2073 6f20  ace database so 
+00001c40: 7468 6174 2066 7574 7572 6520 6361 6c6c  that future call
+00001c50: 730a 2020 2020 2020 2020 666f 7220 6571  s.        for eq
+00001c60: 7569 7661 6c65 6e74 206e 6f64 6520 7479  uivalent node ty
+00001c70: 7065 7320 7769 6c6c 2072 6574 7572 6e20  pes will return 
+00001c80: 4661 6c73 650a 2020 2020 2020 2020 4e7a  False.        Nz
+00001c90: 564e 616d 6573 7061 6365 2063 6f6c 6c69  VNamespace colli
+00001ca0: 7369 6f6e 2120 5479 7065 2d6e 616d 6520  sion! Type-name 
+00001cb0: 6765 6e65 7261 7469 6f6e 2069 7320 6e6f  generation is no
+00001cc0: 7420 726f 6275 7374 2065 6e6f 7567 6820  t robust enough 
+00001cd0: 746f 2063 7265 6174 6520 756e 6971 7565  to create unique
+00001ce0: 206e 616d 6573 2146 5429 0572 4900 0000   names!FT).rI...
+00001cf0: 722f 0000 0072 4300 0000 7275 0000 00da  r/...rC...ru....
+00001d00: 0c52 756e 7469 6d65 4572 726f 7229 0472  .RuntimeError).r
+00001d10: 3100 0000 7236 0000 0072 7400 0000 da03  1...r6...rt.....
+00001d20: 6f62 6a72 3300 0000 7233 0000 0072 3400  objr3...r3...r4.
+00001d30: 0000 7248 0000 0016 0100 0073 1000 0000  ..rH.......s....
+00001d40: 0009 0a02 0a01 0a03 1401 0804 0404 0e01  ................
+00001d50: 7a24 6555 564d 4578 706f 7274 6572 2e5f  z$eUVMExporter._
+00001d60: 636c 6173 735f 6e65 6564 735f 6465 6669  class_needs_defi
+00001d70: 6e69 7469 6f6e 2902 da05 6669 656c 6472  nition)...fieldr
+00001d80: 5c00 0000 6302 0000 0000 0000 0000 0000  \...c...........
+00001d90: 0005 0000 0003 0000 0043 0000 0073 1a02  .........C...s..
+00001da0: 0000 7c01 a000 6401 a101 7d02 7c01 a000  ..|...d...}.|...
+00001db0: 6402 a101 7d03 7c01 a000 6403 a101 7d04  d...}.|...d...}.
+00001dc0: 7c02 7401 6a02 6b02 9001 7272 7c04 6404  |.t.j.k...rr|.d.
+00001dd0: 6b08 723e 7c03 6404 6b08 723e 6405 5300  k.r>|.d.k.r>d.S.
+00001de0: 7c03 7403 6a04 6b02 7256 7c04 7405 6a06  |.t.j.k.rV|.t.j.
+00001df0: 6b02 7256 6406 5300 7c03 7403 6a04 6b02  k.rVd.S.|.t.j.k.
+00001e00: 726e 7c04 7405 6a07 6b02 726e 6407 5300  rn|.t.j.k.rnd.S.
+00001e10: 7c03 7403 6a04 6b02 7286 7c04 7405 6a08  |.t.j.k.r.|.t.j.
+00001e20: 6b02 7286 6408 5300 7c03 7403 6a09 6b02  k.r.d.S.|.t.j.k.
+00001e30: 729e 7c04 7405 6a0a 6b02 729e 6409 5300  r.|.t.j.k.r.d.S.
+00001e40: 7c03 7403 6a09 6b02 72b6 7c04 7405 6a0b  |.t.j.k.r.|.t.j.
+00001e50: 6b02 72b6 640a 5300 7c03 7403 6a09 6b02  k.r.d.S.|.t.j.k.
+00001e60: 72ce 7c04 7405 6a0c 6b02 72ce 640b 5300  r.|.t.j.k.r.d.S.
+00001e70: 7c04 7405 6a0a 6b02 72dc 640c 5300 7c04  |.t.j.k.r.d.S.|.
+00001e80: 7405 6a06 6b02 9000 72ec 640d 5300 7c04  t.j.k...r.d.S.|.
+00001e90: 7405 6a0d 6b02 9000 72fc 640e 5300 7c04  t.j.k...r.d.S.|.
+00001ea0: 7405 6a0b 6b02 9001 720c 640f 5300 7c04  t.j.k...r.d.S.|.
+00001eb0: 7405 6a07 6b02 9001 721c 6410 5300 7c04  t.j.k...r.d.S.|.
+00001ec0: 7405 6a0e 6b02 9001 722c 6411 5300 7c04  t.j.k...r,d.S.|.
+00001ed0: 7405 6a0c 6b02 9001 723c 6412 5300 7c04  t.j.k...r<d.S.|.
+00001ee0: 7405 6a08 6b02 9001 724c 6413 5300 7c03  t.j.k...rLd.S.|.
+00001ef0: 7403 6a04 6b02 9001 725c 6414 5300 7c03  t.j.k...r\d.S.|.
+00001f00: 7403 6a09 6b02 9001 726c 6415 5300 6405  t.j.k...rld.S.d.
+00001f10: 5300 6ea4 7c02 7401 6a0f 6b02 9001 72b2  S.n.|.t.j.k...r.
+00001f20: 7c03 6404 6b08 9001 728c 6416 5300 7c03  |.d.k...r.d.S.|.
+00001f30: 7403 6a04 6b02 9001 729c 6417 5300 7c03  t.j.k...r.d.S.|.
+00001f40: 7403 6a09 6b02 9001 72ac 6418 5300 6416  t.j.k...r.d.S.d.
+00001f50: 5300 6e64 7c02 7401 6a10 6b02 9001 72f2  S.nd|.t.j.k...r.
+00001f60: 7c04 6404 6b08 9001 72cc 6419 5300 7c04  |.d.k...r.d.S.|.
+00001f70: 7405 6a0c 6b02 9001 72dc 641a 5300 7c04  t.j.k...r.d.S.|.
+00001f80: 7405 6a08 6b02 9001 72ec 641b 5300 6419  t.j.k...r.d.S.d.
+00001f90: 5300 6e24 7c02 7401 6a11 6b02 9002 7202  S.n$|.t.j.k...r.
+00001fa0: 641c 5300 7c02 7401 6a12 6b02 9002 7212  d.S.|.t.j.k...r.
+00001fb0: 641d 5300 641e 5300 6404 5300 291f 7a2f  d.S.d.S.d.S.).z/
+00001fc0: 0a20 2020 2020 2020 2047 6574 2066 6965  .        Get fie
+00001fd0: 6c64 2773 2055 564d 2061 6363 6573 7320  ld's UVM access 
+00001fe0: 7374 7269 6e67 0a20 2020 2020 2020 20da  string.        .
+00001ff0: 0273 77da 066f 6e72 6561 64da 076f 6e77  .sw..onread..onw
+00002000: 7269 7465 4eda 0252 575a 0557 3153 5243  riteN..RWZ.W1SRC
+00002010: 5a05 5730 5352 435a 0457 5352 435a 0557  Z.W0SRCZ.WSRCZ.W
+00002020: 3143 5253 5a05 5730 4352 535a 0457 4352  1CRSZ.W0CRSZ.WCR
+00002030: 535a 0357 3143 5a03 5731 535a 0357 3154  SZ.W1CZ.W1SZ.W1T
+00002040: 5a03 5730 435a 0357 3053 5a03 5730 545a  Z.W0CZ.W0SZ.W0TZ
+00002050: 0257 43da 0257 535a 0357 5243 5a03 5752  .WC..WSZ.WRCZ.WR
+00002060: 53da 0252 4fda 0252 435a 0252 535a 0257  S..RO..RCZ.RSZ.W
+00002070: 4f5a 0357 4f43 5a03 574f 535a 0257 315a  OZ.WOCZ.WOSZ.W1Z
+00002080: 0357 4f31 5a08 4e4f 4143 4345 5353 2913  .WO1Z.NOACCESS).
+00002090: 723f 0000 0072 0b00 0000 da02 7277 720c  r?...r......rwr.
+000020a0: 0000 00da 0472 636c 7272 0d00 0000 da05  .....rclrr......
+000020b0: 776f 7365 74da 0377 7a73 da04 7773 6574  woset..wzs..wset
+000020c0: da04 7273 6574 da05 776f 636c 72da 0377  ..rset..woclr..w
+000020d0: 7a63 da04 7763 6c72 da03 776f 74da 0377  zc..wclr..wot..w
+000020e0: 7a74 da01 72da 0177 da03 7277 31da 0277  zt..r..w..rw1..w
+000020f0: 3129 0572 3100 0000 727d 0000 0072 7e00  1).r1...r}...r~.
+00002100: 0000 727f 0000 0072 8000 0000 7233 0000  ..r....r....r3..
+00002110: 0072 3300 0000 7234 0000 0072 4c00 0000  .r3...r4...rL...
+00002120: 3201 0000 7378 0000 0000 040a 010a 010a  2...sx..........
+00002130: 020c 0110 0104 0114 0104 0114 0104 0114  ................
+00002140: 0104 0114 0104 0114 0104 0114 0104 010a  ................
+00002150: 0104 010c 0104 010c 0104 010c 0104 010c  ................
+00002160: 0104 010c 0104 010c 0104 010c 0104 010c  ................
+00002170: 0104 010c 0104 0206 020c 010a 0104 010c  ................
+00002180: 0104 010c 0104 0206 020c 010a 0104 010c  ................
+00002190: 0104 010c 0104 0206 020c 0104 020c 0104  ................
+000021a0: 037a 1e65 5556 4d45 7870 6f72 7465 722e  .z.eUVMExporter.
+000021b0: 5f67 6574 5f66 6965 6c64 5f61 6363 6573  _get_field_acces
+000021c0: 7329 02da 036d 656d 725c 0000 0063 0200  s)...memr\...c..
+000021d0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000021e0: 0000 4300 0000 7320 0000 007c 01a0 0064  ..C...s ...|...d
+000021f0: 01a1 017d 027c 0274 016a 026b 0272 1864  ...}.|.t.j.k.r.d
+00002200: 0253 0064 0353 0064 0053 0029 044e 727e  .S.d.S.d.S.).Nr~
+00002210: 0000 0072 8300 0000 7281 0000 0029 0372  ...r....r....).r
+00002220: 3f00 0000 720b 0000 0072 9000 0000 2903  ?...r....r....).
+00002230: 7231 0000 0072 9400 0000 727e 0000 0072  r1...r....r~...r
+00002240: 3300 0000 7233 0000 0072 3400 0000 7250  3...r3...r4...rP
+00002250: 0000 007e 0100 0073 0800 0000 0001 0a01  ...~...s........
+00002260: 0a01 0402 7a1c 6555 564d 4578 706f 7274  ....z.eUVMExport
+00002270: 6572 2e5f 6765 745f 6d65 6d5f 6163 6365  er._get_mem_acce
+00002280: 7373 6302 0000 0000 0000 0000 0000 0006  ssc.............
+00002290: 0000 0005 0000 0043 0000 0073 6600 0000  .......C...sf...
+000022a0: 6401 7c01 6a00 1600 7d02 7c01 6a01 7262  d.|.j...}.|.j.rb
+000022b0: 7402 7403 7c01 6a04 8301 8301 4400 5d42  t.t.|.j.....D.]B
+000022c0: 7d03 7c01 6a05 7d04 7402 7c03 6402 1700  }.|.j.}.t.|.d...
+000022d0: 7403 7c01 6a04 8301 8302 4400 5d12 7d05  t.|.j.....D.].}.
+000022e0: 7c04 7c01 6a04 7c05 1900 3900 7d04 713c  |.|.j.|...9.}.q<
+000022f0: 7c02 6403 7c03 7c04 6602 1600 3700 7d02  |.d.|.|.f...7.}.
+00002300: 711e 7c02 5300 2904 7aec 0a20 2020 2020  q.|.S.).z..     
+00002310: 2020 2052 6574 7572 6e73 2061 6e20 6578     Returns an ex
+00002320: 7072 6573 7369 6f6e 2074 6f20 6361 6c63  pression to calc
+00002330: 756c 6174 6520 7468 6520 6164 6472 6573  ulate the addres
+00002340: 7320 6f66 6673 6574 0a20 2020 2020 2020  s offset.       
+00002350: 2066 6f72 2065 7861 6d70 6c65 2c20 6120   for example, a 
+00002360: 342d 6469 6d65 6e73 696f 6e61 6c20 6172  4-dimensional ar
+00002370: 7261 7920 616c 6c6f 6361 7465 6420 6173  ray allocated as
+00002380: 3a0a 2020 2020 2020 2020 2020 2020 5b41  :.            [A
+00002390: 5d5b 425d 5b43 5d5b 445d 2040 2058 202b  ][B][C][D] @ X +
+000023a0: 3d20 590a 2020 2020 2020 2020 7265 7375  = Y.        resu
+000023b0: 6c74 7320 696e 3a0a 2020 2020 2020 2020  lts in:.        
+000023c0: 2020 2020 5820 2b20 6930 2a42 2a43 2a44      X + i0*B*C*D
+000023d0: 2a59 202b 2069 312a 432a 442a 5920 2b20  *Y + i1*C*D*Y + 
+000023e0: 6932 2a44 2a59 202b 2069 332a 590a 2020  i2*D*Y + i3*Y.  
+000023f0: 2020 2020 2020 7a04 3078 2578 7210 0000        z.0x%xr...
+00002400: 007a 0b20 2b20 6925 642a 3078 2578 2906  .z. + i%d*0x%x).
+00002410: da12 7261 775f 6164 6472 6573 735f 6f66  ..raw_address_of
+00002420: 6673 6574 da08 6973 5f61 7272 6179 da05  fset..is_array..
+00002430: 7261 6e67 65da 036c 656e da10 6172 7261  range..len..arra
+00002440: 795f 6469 6d65 6e73 696f 6e73 da0c 6172  y_dimensions..ar
+00002450: 7261 795f 7374 7269 6465 2906 7231 0000  ray_stride).r1..
+00002460: 0072 3600 0000 7264 0000 00da 0169 da01  .r6...rd.....i..
+00002470: 6dda 016a 7233 0000 0072 3300 0000 7234  m..jr3...r3...r4
+00002480: 0000 0072 4d00 0000 8601 0000 7310 0000  ...rM.......s...
+00002490: 0000 080a 0106 0112 0106 0118 0110 0112  ................
+000024a0: 017a 2b65 5556 4d45 7870 6f72 7465 722e  .z+eUVMExporter.
+000024b0: 5f67 6574 5f61 7272 6179 5f61 6464 7265  _get_array_addre
+000024c0: 7373 5f6f 6666 7365 745f 6578 7072 6302  ss_offset_exprc.
+000024d0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000024e0: 0000 0043 0000 0073 2a00 0000 7c01 6a00  ...C...s*...|.j.
+000024f0: 7d02 7c02 a001 6401 a101 7214 6402 5300  }.|...d...r.d.S.
+00002500: 7c02 a001 6403 a101 7222 6404 5300 6405  |...d...r"d.S.d.
+00002510: 5300 6400 5300 2906 4eda 0962 6967 656e  S.d.S.).N..bigen
+00002520: 6469 616e 5a0e 5556 4d5f 4249 475f 454e  dianZ.UVM_BIG_EN
+00002530: 4449 414e da0c 6c69 7474 6c65 656e 6469  DIAN..littleendi
+00002540: 616e 5a11 5556 4d5f 4c49 5454 4c45 5f45  anZ.UVM_LITTLE_E
+00002550: 4e44 4941 4e5a 0d55 564d 5f4e 4f5f 454e  NDIANZ.UVM_NO_EN
+00002560: 4449 414e 2902 da0e 6f77 6e69 6e67 5f61  DIAN)...owning_a
+00002570: 6464 726d 6170 723f 0000 0029 0372 3100  ddrmapr?...).r1.
+00002580: 0000 7236 0000 005a 0461 6d61 7072 3300  ..r6...Z.amapr3.
+00002590: 0000 7233 0000 0072 3400 0000 724e 0000  ..r3...r4...rN..
+000025a0: 0098 0100 0073 0c00 0000 0001 0601 0a01  .....s..........
+000025b0: 0401 0a01 0402 7a1c 6555 564d 4578 706f  ......z.eUVMExpo
+000025c0: 7274 6572 2e5f 6765 745f 656e 6469 616e  rter._get_endian
+000025d0: 6e65 7373 6302 0000 0000 0000 0000 0000  nessc...........
+000025e0: 0003 0000 0003 0000 0043 0000 0073 2e00  .........C...s..
+000025f0: 0000 7c00 6a00 7c01 a001 a100 1900 7d02  ..|.j.|.......}.
+00002600: 7c02 6401 1600 7222 7c02 6401 1a00 6402  |.d...r"|.d...d.
+00002610: 1700 5300 7c02 6401 1a00 5300 6403 5300  ..S.|.d...S.d.S.
+00002620: 2904 7a40 0a20 2020 2020 2020 2052 6574  ).z@.        Ret
+00002630: 7572 6e73 2067 726f 7570 2d6c 696b 6520  urns group-like 
+00002640: 6e6f 6465 2773 2062 7573 2077 6964 7468  node's bus width
+00002650: 2028 696e 2062 7974 6573 290a 2020 2020   (in bytes).    
+00002660: 2020 2020 e908 0000 0072 1000 0000 4e29      .....r....N)
+00002670: 0272 2e00 0000 da08 6765 745f 7061 7468  .r......get_path
+00002680: 2903 7231 0000 0072 3600 0000 da05 7769  ).r1...r6.....wi
+00002690: 6474 6872 3300 0000 7233 0000 0072 3400  dthr3...r3...r4.
+000026a0: 0000 724f 0000 00a2 0100 0073 0800 0000  ..rO.......s....
+000026b0: 0004 0e03 0801 0c02 7a1b 6555 564d 4578  ........z.eUVMEx
+000026c0: 706f 7274 6572 2e5f 6765 745f 6275 735f  porter._get_bus_
+000026d0: 7769 6474 6829 03da 0178 da01 6e72 5c00  width)...x..nr\.
+000026e0: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+000026f0: 0000 0002 0000 0043 0000 0073 2800 0000  .......C...s(...
+00002700: 7c01 7c02 1600 7218 7c01 7c02 1a00 6401  |.|...r.|.|...d.
+00002710: 1700 7c02 1400 5300 7c01 7c02 1a00 7c02  ..|...S.|.|...|.
+00002720: 1400 5300 6402 5300 2903 7a2d 0a20 2020  ..S.d.S.).z-.   
+00002730: 2020 2020 2052 6f75 6e64 2078 2075 7020       Round x up 
+00002740: 746f 2074 6865 206e 6561 7265 7374 206e  to the nearest n
+00002750: 0a20 2020 2020 2020 2072 1000 0000 4e72  .        r....Nr
+00002760: 3300 0000 2903 7231 0000 0072 a400 0000  3...).r1...r....
+00002770: 72a5 0000 0072 3300 0000 7233 0000 0072  r....r3...r3...r
+00002780: 3400 0000 7251 0000 00af 0100 0073 0600  4...rQ.......s..
+00002790: 0000 0004 0801 1002 7a18 6555 564d 4578  ........z.eUVMEx
+000027a0: 706f 7274 6572 2e5f 726f 756e 6475 705f  porter._roundup_
+000027b0: 746f 6302 0000 0000 0000 0000 0000 0002  toc.............
+000027c0: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
+000027d0: 6401 7c01 6401 1800 a000 a100 3e00 5300  d.|.d.......>.S.
+000027e0: 2902 4e72 1000 0000 2901 da0a 6269 745f  ).Nr....)...bit_
+000027f0: 6c65 6e67 7468 2902 7231 0000 0072 a400  length).r1...r..
+00002800: 0000 7233 0000 0072 3300 0000 7234 0000  ..r3...r3...r4..
+00002810: 0072 5200 0000 b901 0000 7302 0000 0000  .rR.......s.....
+00002820: 017a 1a65 5556 4d45 7870 6f72 7465 722e  .z.eUVMExporter.
+00002830: 5f72 6f75 6e64 7570 5f70 6f77 324e 2901  _roundup_pow2N).
+00002840: 7271 0000 0029 1c72 7900 0000 da0a 5f5f  rq...).ry.....__
+00002850: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00002860: 6e61 6d65 5f5f 7235 0000 0072 0400 0000  name__r5...r....
+00002870: da03 7374 7272 5b00 0000 7254 0000 0072  ..strr[...rT...r
+00002880: 5600 0000 7270 0000 0072 0200 0000 7276  V...rp...r....rv
+00002890: 0000 0072 4900 0000 724a 0000 0072 4b00  ...rI...rJ...rK.
+000028a0: 0000 da04 626f 6f6c 7248 0000 0072 0800  ....boolrH...r..
+000028b0: 0000 724c 0000 0072 0900 0000 7250 0000  ..rL...r....rP..
+000028c0: 0072 0a00 0000 724d 0000 0072 4e00 0000  .r....rM...rN...
+000028d0: da03 696e 7472 4f00 0000 7251 0000 0072  ..intrO...rQ...r
+000028e0: 5200 0000 7233 0000 0072 3300 0000 7233  R...r3...r3...r3
+000028f0: 0000 0072 3400 0000 7212 0000 000e 0000  ...r4...r.......
+00002900: 0073 2200 0000 0802 083c 1057 1006 1006  .s"......<.W....
+00002910: 100f 1823 101b 1013 1007 101c 104c 1008  ...#.........L..
+00002920: 1012 100a 100d 120a 7212 0000 0029 1a72  ........r....).r
+00002930: 2400 0000 7261 0000 00da 0674 7970 696e  $...ra.....typin
+00002940: 6772 0200 0000 da06 6a69 6e6a 6132 7221  gr......jinja2r!
+00002950: 0000 005a 0e73 7973 7465 6d72 646c 2e6e  ...Z.systemrdl.n
+00002960: 6f64 6572 0300 0000 7204 0000 0072 0500  oder....r....r..
+00002970: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00002980: 0072 0900 0000 720a 0000 005a 1273 7973  .r....r....Z.sys
+00002990: 7465 6d72 646c 2e72 646c 7479 7065 7372  temrdl.rdltypesr
+000029a0: 0b00 0000 720c 0000 0072 0d00 0000 5a13  ....r....r....Z.
+000029b0: 7379 7374 656d 7264 6c2e 636f 6d70 6f6e  systemrdl.compon
+000029c0: 656e 7472 0e00 0000 da09 7379 7374 656d  entr......system
+000029d0: 7264 6c72 0f00 0000 5a13 7072 655f 6578  rdlr....Z.pre_ex
+000029e0: 706f 7274 5f6c 6973 7465 6e65 7272 1100  port_listenerr..
+000029f0: 0000 7212 0000 0072 3300 0000 7233 0000  ..r....r3...r3..
+00002a00: 0072 3300 0000 7234 0000 00da 083c 6d6f  .r3...r4.....<mo
+00002a10: 6475 6c65 3e01 0000 0073 1400 0000 0801  dule>....s......
+00002a20: 0801 0c02 0801 1c01 1401 1401 0c01 0c02  ................
+00002a30: 0c02                                     ..
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/pre_export_listener.cpython-310.pyc` & `peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/pre_export_listener.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 06:49:36 2023 UTC, .py size: 1255 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 001f be64 e704 0000  o..........d....
+00000000: 550d 0d0a 0000 0000 4b4d be64 e704 0000  U.......KM.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0b52 444c 4c69 7374  .....)...RDLList
 00000060: 656e 6572 6300 0000 0000 0000 0000 0000  enerc...........
 00000070: 0000 0000 0002 0000 0040 0000 0073 5400  .........@...sT.
@@ -14,104 +14,107 @@
 000000d0: 5a0b 6413 5300 2914 da11 5072 6545 7870  Z.d.S.)...PreExp
 000000e0: 6f72 744c 6973 7465 6e65 7263 0200 0000  ortListenerc....
 000000f0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
 00000100: 4300 0000 7310 0000 007c 017c 005f 0067  C...s....|.|._.g
 00000110: 007c 005f 0164 0053 00a9 014e 2902 da08  .|._.d.S...N)...
 00000120: 6578 706f 7274 6572 da0f 6d61 785f 7769  exporter..max_wi
 00000130: 6474 685f 7374 6163 6b29 02da 0473 656c  dth_stack)...sel
-00000140: 6672 0500 0000 a900 7208 0000 00fa 572f  fr......r.....W/
-00000150: 686f 6d65 2f6b 756e 2f65 7576 6d5f 7072  home/kun/euvm_pr
-00000160: 6f6a 6563 7473 2f73 7973 7465 6d5f 7264  ojects/system_rd
-00000170: 6c2f 5065 616b 5244 4c2d 6575 766d 2f73  l/PeakRDL-euvm/s
-00000180: 7263 2f70 6561 6b72 646c 5f65 7576 6d2f  rc/peakrdl_euvm/
-00000190: 7072 655f 6578 706f 7274 5f6c 6973 7465  pre_export_liste
-000001a0: 6e65 722e 7079 da08 5f5f 696e 6974 5f5f  ner.py..__init__
-000001b0: 0500 0000 7304 0000 0006 010a 037a 1a50  ....s........z.P
-000001c0: 7265 4578 706f 7274 4c69 7374 656e 6572  reExportListener
-000001d0: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-000001e0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000001f0: 0000 f30e 0000 007c 00a0 007c 01a1 0101  .......|...|....
-00000200: 0064 0053 0072 0400 0000 a901 da0b 656e  .d.S.r........en
-00000210: 7465 725f 6772 6f75 70a9 0272 0700 0000  ter_group..r....
-00000220: da04 6e6f 6465 7208 0000 0072 0800 0000  ..noder....r....
-00000230: 7209 0000 00da 0d65 6e74 6572 5f41 6464  r......enter_Add
-00000240: 726d 6170 0b00 0000 f302 0000 000e 017a  rmap...........z
-00000250: 1f50 7265 4578 706f 7274 4c69 7374 656e  .PreExportListen
-00000260: 6572 2e65 6e74 6572 5f41 6464 726d 6170  er.enter_Addrmap
-00000270: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000280: 0003 0000 0043 0000 0072 0b00 0000 7204  .....C...r....r.
-00000290: 0000 00a9 01da 0a65 7869 745f 6772 6f75  .......exit_grou
-000002a0: 7072 0e00 0000 7208 0000 0072 0800 0000  pr....r....r....
-000002b0: 7209 0000 00da 0c65 7869 745f 4164 6472  r......exit_Addr
-000002c0: 6d61 700e 0000 0072 1100 0000 7a1e 5072  map....r....z.Pr
-000002d0: 6545 7870 6f72 744c 6973 7465 6e65 722e  eExportListener.
-000002e0: 6578 6974 5f41 6464 726d 6170 6302 0000  exit_Addrmapc...
-000002f0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000300: 0043 0000 0072 0b00 0000 7204 0000 0072  .C...r....r....r
-00000310: 0c00 0000 720e 0000 0072 0800 0000 7208  ....r....r....r.
+00000140: 6672 0500 0000 a900 7208 0000 00fa 392f  fr......r.....9/
+00000150: 746d 702f 5065 616b 5244 4c2d 6575 766d  tmp/PeakRDL-euvm
+00000160: 2f73 7263 2f70 6561 6b72 646c 5f65 7576  /src/peakrdl_euv
+00000170: 6d2f 7072 655f 6578 706f 7274 5f6c 6973  m/pre_export_lis
+00000180: 7465 6e65 722e 7079 da08 5f5f 696e 6974  tener.py..__init
+00000190: 5f5f 0500 0000 7304 0000 0000 0106 037a  __....s........z
+000001a0: 1a50 7265 4578 706f 7274 4c69 7374 656e  .PreExportListen
+000001b0: 6572 2e5f 5f69 6e69 745f 5f63 0200 0000  er.__init__c....
+000001c0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000001d0: 4300 0000 730e 0000 007c 00a0 007c 01a1  C...s....|...|..
+000001e0: 0101 0064 0053 0072 0400 0000 a901 da0b  ...d.S.r........
+000001f0: 656e 7465 725f 6772 6f75 70a9 0272 0700  enter_group..r..
+00000200: 0000 da04 6e6f 6465 7208 0000 0072 0800  ....noder....r..
+00000210: 0000 7209 0000 00da 0d65 6e74 6572 5f41  ..r......enter_A
+00000220: 6464 726d 6170 0b00 0000 7302 0000 0000  ddrmap....s.....
+00000230: 017a 1f50 7265 4578 706f 7274 4c69 7374  .z.PreExportList
+00000240: 656e 6572 2e65 6e74 6572 5f41 6464 726d  ener.enter_Addrm
+00000250: 6170 6302 0000 0000 0000 0000 0000 0002  apc.............
+00000260: 0000 0003 0000 0043 0000 0073 0e00 0000  .......C...s....
+00000270: 7c00 a000 7c01 a101 0100 6400 5300 7204  |...|.....d.S.r.
+00000280: 0000 00a9 01da 0a65 7869 745f 6772 6f75  .......exit_grou
+00000290: 7072 0d00 0000 7208 0000 0072 0800 0000  pr....r....r....
+000002a0: 7209 0000 00da 0c65 7869 745f 4164 6472  r......exit_Addr
+000002b0: 6d61 700e 0000 0073 0200 0000 0001 7a1e  map....s......z.
+000002c0: 5072 6545 7870 6f72 744c 6973 7465 6e65  PreExportListene
+000002d0: 722e 6578 6974 5f41 6464 726d 6170 6302  r.exit_Addrmapc.
+000002e0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000002f0: 0000 0043 0000 0073 0e00 0000 7c00 a000  ...C...s....|...
+00000300: 7c01 a101 0100 6400 5300 7204 0000 0072  |.....d.S.r....r
+00000310: 0b00 0000 720d 0000 0072 0800 0000 7208  ....r....r....r.
 00000320: 0000 0072 0900 0000 da0d 656e 7465 725f  ...r......enter_
-00000330: 5265 6766 696c 6511 0000 0072 1100 0000  Regfile....r....
-00000340: 7a1f 5072 6545 7870 6f72 744c 6973 7465  z.PreExportListe
-00000350: 6e65 722e 656e 7465 725f 5265 6766 696c  ner.enter_Regfil
-00000360: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00000370: 0000 0300 0000 4300 0000 720b 0000 0072  ......C...r....r
-00000380: 0400 0000 7212 0000 0072 0e00 0000 7208  ....r....r....r.
-00000390: 0000 0072 0800 0000 7209 0000 00da 0c65  ...r....r......e
-000003a0: 7869 745f 5265 6766 696c 6514 0000 0072  xit_Regfile....r
-000003b0: 1100 0000 7a1e 5072 6545 7870 6f72 744c  ....z.PreExportL
-000003c0: 6973 7465 6e65 722e 6578 6974 5f52 6567  istener.exit_Reg
-000003d0: 6669 6c65 6302 0000 0000 0000 0000 0000  filec...........
-000003e0: 0002 0000 0004 0000 0043 0000 00f3 2000  .........C.... .
-000003f0: 0000 7400 7c01 a001 6401 a101 7c00 6a02  ..t.|...d...|.j.
-00000400: 6402 1900 8302 7c00 6a02 6402 3c00 6400  d.....|.j.d.<.d.
-00000410: 5300 2903 4eda 0b61 6363 6573 7377 6964  S.).N..accesswid
-00000420: 7468 e9ff ffff ffa9 03da 036d 6178 da0c  th.........max..
-00000430: 6765 745f 7072 6f70 6572 7479 7206 0000  get_propertyr...
-00000440: 0072 0e00 0000 7208 0000 0072 0800 0000  .r....r....r....
-00000450: 7209 0000 00da 0965 6e74 6572 5f52 6567  r......enter_Reg
-00000460: 1700 0000 f302 0000 0020 027a 1b50 7265  ......... .z.Pre
-00000470: 4578 706f 7274 4c69 7374 656e 6572 2e65  ExportListener.e
-00000480: 6e74 6572 5f52 6567 6302 0000 0000 0000  nter_Regc.......
-00000490: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000004a0: 0072 1700 0000 2903 4eda 086d 656d 7769  .r....).N..memwi
-000004b0: 6474 6872 1900 0000 721a 0000 0072 0e00  dthr....r....r..
-000004c0: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
-000004d0: 00da 0965 6e74 6572 5f4d 656d 1b00 0000  ...enter_Mem....
-000004e0: 721e 0000 007a 1b50 7265 4578 706f 7274  r....z.PreExport
-000004f0: 4c69 7374 656e 6572 2e65 6e74 6572 5f4d  Listener.enter_M
-00000500: 656d 6302 0000 0000 0000 0000 0000 0002  emc.............
-00000510: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
-00000520: 7c00 6a00 a001 6401 a101 0100 6400 5300  |.j...d.....d.S.
-00000530: 2902 4e72 0100 0000 2902 7206 0000 00da  ).Nr....).r.....
-00000540: 0661 7070 656e 6472 0e00 0000 7208 0000  .appendr....r...
-00000550: 0072 0800 0000 7209 0000 0072 0d00 0000  .r....r....r....
-00000560: 2000 0000 7302 0000 0010 017a 1d50 7265   ...s......z.Pre
-00000570: 4578 706f 7274 4c69 7374 656e 6572 2e65  ExportListener.e
-00000580: 6e74 6572 5f67 726f 7570 6302 0000 0000  nter_groupc.....
-00000590: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-000005a0: 0000 0073 3e00 0000 7c00 6a00 a001 a100  ...s>...|.j.....
-000005b0: 7d02 7c02 7c00 6a02 6a03 7c01 a004 a100  }.|.|.j.j.|.....
-000005c0: 3c00 7c00 6a00 721d 7405 7c02 7c00 6a00  <.|.j.r.t.|.|.j.
-000005d0: 6401 1900 8302 7c00 6a00 6401 3c00 6400  d.....|.j.d.<.d.
-000005e0: 5300 6400 5300 2902 4e72 1900 0000 2906  S.d.S.).Nr....).
-000005f0: 7206 0000 00da 0370 6f70 7205 0000 00da  r......popr.....
-00000600: 0c62 7573 5f77 6964 7468 5f64 62da 0867  .bus_width_db..g
-00000610: 6574 5f70 6174 6872 1b00 0000 2903 7207  et_pathr....).r.
-00000620: 0000 0072 0f00 0000 da09 6d61 785f 7769  ...r......max_wi
-00000630: 6474 6872 0800 0000 7208 0000 0072 0900  dthr....r....r..
-00000640: 0000 7213 0000 0023 0000 0073 0a00 0000  ..r....#...s....
-00000650: 0a01 1003 0603 1a01 04ff 7a1c 5072 6545  ..........z.PreE
-00000660: 7870 6f72 744c 6973 7465 6e65 722e 6578  xportListener.ex
-00000670: 6974 5f67 726f 7570 4e29 0cda 085f 5f6e  it_groupN)...__n
-00000680: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000690: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-000006a0: 0a00 0000 7210 0000 0072 1400 0000 7215  ....r....r....r.
-000006b0: 0000 0072 1600 0000 721d 0000 0072 2000  ...r....r....r .
-000006c0: 0000 720d 0000 0072 1300 0000 7208 0000  ..r....r....r...
-000006d0: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-000006e0: 7203 0000 0004 0000 0073 1400 0000 0800  r........s......
-000006f0: 0801 0806 0803 0803 0803 0803 0804 0805  ................
-00000700: 0c03 7203 0000 004e 2903 da09 7379 7374  ..r....N)...syst
-00000710: 656d 7264 6c72 0200 0000 7203 0000 0072  emrdlr....r....r
-00000720: 0800 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
-00000730: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000740: 0073 0400 0000 0c01 1402                 .s........
+00000330: 5265 6766 696c 6511 0000 0073 0200 0000  Regfile....s....
+00000340: 0001 7a1f 5072 6545 7870 6f72 744c 6973  ..z.PreExportLis
+00000350: 7465 6e65 722e 656e 7465 725f 5265 6766  tener.enter_Regf
+00000360: 696c 6563 0200 0000 0000 0000 0000 0000  ilec............
+00000370: 0200 0000 0300 0000 4300 0000 730e 0000  ........C...s...
+00000380: 007c 00a0 007c 01a1 0101 0064 0053 0072  .|...|.....d.S.r
+00000390: 0400 0000 7210 0000 0072 0d00 0000 7208  ....r....r....r.
+000003a0: 0000 0072 0800 0000 7209 0000 00da 0c65  ...r....r......e
+000003b0: 7869 745f 5265 6766 696c 6514 0000 0073  xit_Regfile....s
+000003c0: 0200 0000 0001 7a1e 5072 6545 7870 6f72  ......z.PreExpor
+000003d0: 744c 6973 7465 6e65 722e 6578 6974 5f52  tListener.exit_R
+000003e0: 6567 6669 6c65 6302 0000 0000 0000 0000  egfilec.........
+000003f0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000400: 2000 0000 7400 7c01 a001 6401 a101 7c00   ...t.|...d...|.
+00000410: 6a02 6402 1900 8302 7c00 6a02 6402 3c00  j.d.....|.j.d.<.
+00000420: 6400 5300 2903 4eda 0b61 6363 6573 7377  d.S.).N..accessw
+00000430: 6964 7468 e9ff ffff ffa9 03da 036d 6178  idth.........max
+00000440: da0c 6765 745f 7072 6f70 6572 7479 7206  ..get_propertyr.
+00000450: 0000 0072 0d00 0000 7208 0000 0072 0800  ...r....r....r..
+00000460: 0000 7209 0000 00da 0965 6e74 6572 5f52  ..r......enter_R
+00000470: 6567 1700 0000 7302 0000 0000 027a 1b50  eg....s......z.P
+00000480: 7265 4578 706f 7274 4c69 7374 656e 6572  reExportListener
+00000490: 2e65 6e74 6572 5f52 6567 6302 0000 0000  .enter_Regc.....
+000004a0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000004b0: 0000 0073 2000 0000 7400 7c01 a001 6401  ...s ...t.|...d.
+000004c0: a101 7c00 6a02 6402 1900 8302 7c00 6a02  ..|.j.d.....|.j.
+000004d0: 6402 3c00 6400 5300 2903 4eda 086d 656d  d.<.d.S.).N..mem
+000004e0: 7769 6474 6872 1600 0000 7217 0000 0072  widthr....r....r
+000004f0: 0d00 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
+00000500: 0000 00da 0965 6e74 6572 5f4d 656d 1b00  .....enter_Mem..
+00000510: 0000 7302 0000 0000 027a 1b50 7265 4578  ..s......z.PreEx
+00000520: 706f 7274 4c69 7374 656e 6572 2e65 6e74  portListener.ent
+00000530: 6572 5f4d 656d 6302 0000 0000 0000 0000  er_Memc.........
+00000540: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00000550: 1000 0000 7c00 6a00 a001 6401 a101 0100  ....|.j...d.....
+00000560: 6400 5300 2902 4e72 0100 0000 2902 7206  d.S.).Nr....).r.
+00000570: 0000 00da 0661 7070 656e 6472 0d00 0000  .....appendr....
+00000580: 7208 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00000590: 0c00 0000 2000 0000 7302 0000 0000 017a  .... ...s......z
+000005a0: 1d50 7265 4578 706f 7274 4c69 7374 656e  .PreExportListen
+000005b0: 6572 2e65 6e74 6572 5f67 726f 7570 6302  er.enter_groupc.
+000005c0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+000005d0: 0000 0043 0000 0073 3a00 0000 7c00 6a00  ...C...s:...|.j.
+000005e0: a001 a100 7d02 7c02 7c00 6a02 6a03 7c01  ....}.|.|.j.j.|.
+000005f0: a004 a100 3c00 7c00 6a00 7236 7405 7c02  ....<.|.j.r6t.|.
+00000600: 7c00 6a00 6401 1900 8302 7c00 6a00 6401  |.j.d.....|.j.d.
+00000610: 3c00 6400 5300 2902 4e72 1600 0000 2906  <.d.S.).Nr....).
+00000620: 7206 0000 00da 0370 6f70 7205 0000 00da  r......popr.....
+00000630: 0c62 7573 5f77 6964 7468 5f64 62da 0867  .bus_width_db..g
+00000640: 6574 5f70 6174 6872 1800 0000 2903 7207  et_pathr....).r.
+00000650: 0000 0072 0e00 0000 da09 6d61 785f 7769  ...r......max_wi
+00000660: 6474 6872 0800 0000 7208 0000 0072 0900  dthr....r....r..
+00000670: 0000 7211 0000 0023 0000 0073 0800 0000  ..r....#...s....
+00000680: 0001 0a03 1003 0601 7a1c 5072 6545 7870  ........z.PreExp
+00000690: 6f72 744c 6973 7465 6e65 722e 6578 6974  ortListener.exit
+000006a0: 5f67 726f 7570 4e29 0cda 085f 5f6e 616d  _groupN)...__nam
+000006b0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000006c0: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0a00  .__qualname__r..
+000006d0: 0000 720f 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000006e0: 0072 1400 0000 721a 0000 0072 1c00 0000  .r....r....r....
+000006f0: 720c 0000 0072 1100 0000 7208 0000 0072  r....r....r....r
+00000700: 0800 0000 7208 0000 0072 0900 0000 7203  ....r....r....r.
+00000710: 0000 0004 0000 0073 1200 0000 0801 0806  .......s........
+00000720: 0803 0803 0803 0803 0804 0805 0803 7203  ..............r.
+00000730: 0000 004e 2903 da09 7379 7374 656d 7264  ...N)...systemrd
+00000740: 6c72 0200 0000 7203 0000 0072 0800 0000  lr....r....r....
+00000750: 7208 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
+00000760: 083c 6d6f 6475 6c65 3e02 0000 0073 0200  .<module>....s..
+00000770: 0000 0c02                                ....
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm/__pycache__/__peakrdl__.cpython-310.pyc` & `peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/__peakrdl__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 06:49:36 2023 UTC, .py size: 1816 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,119 @@
-00000000: 6f0d 0d0a 0000 0000 001f be64 1807 0000  o..........d....
+00000000: 550d 0d0a 0000 0000 4b4d be64 1807 0000  U.......KM.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6501 721e 6400 6405 6c06 5a06 6400  ..e.r.d.d.l.Z.d.
+00000050: 0100 6501 723c 6400 6405 6c06 5a06 6400  ..e.r<d.d.l.Z.d.
 00000060: 6406 6c07 6d08 5a08 0100 4700 6407 6408  d.l.m.Z...G.d.d.
 00000070: 8400 6408 6503 8303 5a09 6405 5300 2909  ..d.e...Z.d.S.).
 00000080: e900 0000 0029 01da 0d54 5950 455f 4348  .....)...TYPE_CH
 00000090: 4543 4b49 4e47 2901 da18 4578 706f 7274  ECKING)...Export
 000000a0: 6572 5375 6263 6f6d 6d61 6e64 506c 7567  erSubcommandPlug
 000000b0: 696e e901 0000 0029 01da 0c65 5556 4d45  in.....)...eUVME
 000000c0: 7870 6f72 7465 724e 2901 da0b 4164 6472  xporterN)...Addr
 000000d0: 6d61 704e 6f64 6563 0000 0000 0000 0000  mapNodec........
-000000e0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000000f0: 7324 0000 0065 005a 0164 005a 0264 015a  s$...e.Z.d.Z.d.Z
-00000100: 0364 0e64 0664 0784 045a 0464 0f64 0c64  .d.d.d...Z.d.d.d
-00000110: 0d84 045a 0564 0553 0029 10da 0845 7870  ...Z.d.S.)...Exp
-00000120: 6f72 7465 727a 1e47 656e 6572 6174 6520  orterz.Generate 
-00000130: 6120 6555 564d 2072 6567 6973 7465 7220  a eUVM register 
-00000140: 6d6f 6465 6cda 0961 7267 5f67 726f 7570  model..arg_group
-00000150: fa17 6172 6770 6172 7365 2e41 7267 756d  ..argparse.Argum
-00000160: 656e 7450 6172 7365 72da 0672 6574 7572  entParser..retur
-00000170: 6e4e 6302 0000 0000 0000 0000 0000 0002  nNc.............
-00000180: 0000 0007 0000 0043 0000 0073 4800 0000  .......C...sH...
-00000190: 7c01 6a00 6401 6402 6403 6404 6702 6403  |.j.d.d.d.d.g.d.
-000001a0: 6405 6406 8d05 0100 7c01 6a00 6407 6408  d.d.....|.j.d.d.
-000001b0: 6409 640a 6702 6409 640b 6406 8d05 0100  d.d.g.d.d.d.....
-000001c0: 7c01 6a00 640c 640d 640e 640f 6410 6411  |.j.d.d.d.d.d.d.
-000001d0: 8d05 0100 6400 5300 2912 4e7a 0b2d 2d66  ....d.S.).Nz.--f
-000001e0: 696c 652d 7479 7065 da09 6669 6c65 5f74  ile-type..file_t
-000001f0: 7970 65da 0770 6163 6b61 6765 da06 6865  ype..package..he
-00000200: 6164 6572 7a40 4368 6f6f 7365 2074 6865  aderz@Choose the
-00000210: 2066 696c 6520 636f 6e74 6169 6e65 7220   file container 
-00000220: 7374 796c 6520 6f66 2074 6865 2072 6567  style of the reg
-00000230: 6973 7465 7220 6d6f 6465 6c2e 205b 7061  ister model. [pa
-00000240: 636b 6167 655d 2904 da04 6465 7374 da07  ckage])...dest..
-00000250: 6368 6f69 6365 73da 0764 6566 6175 6c74  choices..default
-00000260: da04 6865 6c70 7a0c 2d2d 7479 7065 2d73  ..helpz.--type-s
-00000270: 7479 6c65 da0a 7479 7065 5f73 7479 6c65  tyle..type_style
-00000280: da07 6c65 7869 6361 6cda 0468 6965 7261  ..lexical..hiera
-00000290: 2801 0000 4368 6f6f 7365 2068 6f77 2063  (...Choose how c
-000002a0: 6c61 7373 2074 7970 6520 6e61 6d65 7320  lass type names 
-000002b0: 6172 6520 6765 6e65 7261 7465 642e 0a20  are generated.. 
-000002c0: 2020 2020 2020 2020 2020 2054 6865 2027             The '
-000002d0: 6c65 7869 6361 6c27 2073 7479 6c65 2077  lexical' style w
-000002e0: 696c 6c20 7573 6520 5244 4c20 6c65 7869  ill use RDL lexi
-000002f0: 6361 6c20 7363 6f70 6520 2620 7479 7065  cal scope & type
-00000300: 206e 616d 6573 2077 6865 7265 0a20 2020   names where.   
-00000310: 2020 2020 2020 2020 2070 6f73 7369 626c           possibl
-00000320: 6520 616e 6420 6174 7465 6d70 7420 746f  e and attempt to
-00000330: 2072 652d 7573 6520 6571 7569 7661 6c65   re-use equivale
-00000340: 6e74 2063 6c61 7373 2064 6566 696e 6974  nt class definit
-00000350: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
-00000360: 2020 5468 6520 2768 6965 7227 2073 7479    The 'hier' sty
-00000370: 6c65 2075 7365 7320 636f 6d70 6f6e 656e  le uses componen
-00000380: 7427 7320 6869 6572 6172 6368 7920 6173  t's hierarchy as
-00000390: 2074 6865 2063 6c61 7373 2074 7970 6520   the class type 
-000003a0: 6e61 6d65 2e20 5b6c 6578 6963 616c 5d0a  name. [lexical].
-000003b0: 2020 2020 2020 2020 2020 2020 7a0d 2d2d              z.--
-000003c0: 7573 652d 6661 6374 6f72 79da 0b75 7365  use-factory..use
-000003d0: 5f66 6163 746f 7279 46da 0a73 746f 7265  _factoryF..store
-000003e0: 5f74 7275 657a 4f49 6620 7365 742c 2063  _truezOIf set, c
-000003f0: 6c61 7373 2064 6566 696e 6974 696f 6e73  lass definitions
-00000400: 2061 6e64 2063 6c61 7373 2069 6e73 7461   and class insta
-00000410: 6e63 6573 2061 7265 2063 7265 6174 6564  nces are created
-00000420: 2075 7369 6e67 2074 6865 2055 564d 2066   using the UVM f
-00000430: 6163 746f 7279 2904 720e 0000 0072 1000  actory).r....r..
-00000440: 0000 da06 6163 7469 6f6e 7211 0000 0029  ....actionr....)
-00000450: 01da 0c61 6464 5f61 7267 756d 656e 7429  ...add_argument)
-00000460: 02da 0473 656c 6672 0800 0000 a900 721a  ...selfr......r.
-00000470: 0000 00fa 4f2f 686f 6d65 2f6b 756e 2f65  ....O/home/kun/e
-00000480: 7576 6d5f 7072 6f6a 6563 7473 2f73 7973  uvm_projects/sys
-00000490: 7465 6d5f 7264 6c2f 5065 616b 5244 4c2d  tem_rdl/PeakRDL-
-000004a0: 6575 766d 2f73 7263 2f70 6561 6b72 646c  euvm/src/peakrdl
-000004b0: 5f65 7576 6d2f 5f5f 7065 616b 7264 6c5f  _euvm/__peakrdl_
-000004c0: 5f2e 7079 da16 6164 645f 6578 706f 7274  _.py..add_export
-000004d0: 6572 5f61 7267 756d 656e 7473 0f00 0000  er_arguments....
-000004e0: 732a 0000 0004 0102 0102 0106 0102 0102  s*..............
-000004f0: 0106 fb04 0802 0102 0106 0102 0102 0106  ................
-00000500: fb04 0c02 0102 0102 0102 0102 010a fb7a  ...............z
-00000510: 1f45 7870 6f72 7465 722e 6164 645f 6578  .Exporter.add_ex
-00000520: 706f 7274 6572 5f61 7267 756d 656e 7473  porter_arguments
-00000530: da08 746f 705f 6e6f 6465 7206 0000 00da  ..top_noder.....
-00000540: 076f 7074 696f 6e73 fa12 6172 6770 6172  .options..argpar
-00000550: 7365 2e4e 616d 6573 7061 6365 6303 0000  se.Namespacec...
-00000560: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00000570: 0043 0000 0073 2e00 0000 7400 8300 7d03  .C...s....t...}.
-00000580: 7c03 6a01 7c01 7c02 6a02 7c02 6a03 6401  |.j.|.|.j.|.j.d.
-00000590: 6b02 7c02 6a04 6402 6b02 7c02 6a05 6403  k.|.j.d.k.|.j.d.
-000005a0: 8d05 0100 6400 5300 2904 4e72 0c00 0000  ....d.S.).Nr....
-000005b0: 7213 0000 0029 03da 1165 7870 6f72 745f  r....)...export_
-000005c0: 6173 5f70 6163 6b61 6765 da17 7265 7573  as_package..reus
-000005d0: 655f 636c 6173 735f 6465 6669 6e69 7469  e_class_definiti
-000005e0: 6f6e 73da 0f75 7365 5f75 766d 5f66 6163  ons..use_uvm_fac
-000005f0: 746f 7279 2906 7205 0000 00da 0665 7870  tory).r......exp
-00000600: 6f72 74da 066f 7574 7075 7472 0b00 0000  ort..outputr....
-00000610: 7212 0000 0072 1500 0000 2904 7219 0000  r....r....).r...
-00000620: 0072 1d00 0000 721e 0000 00da 0178 721a  .r....r......xr.
-00000630: 0000 0072 1a00 0000 721b 0000 00da 0964  ...r....r......d
-00000640: 6f5f 6578 706f 7274 2d00 0000 7310 0000  o_export-...s...
-00000650: 0006 0104 0102 0104 0108 0108 0104 010a  ................
-00000660: fb7a 1245 7870 6f72 7465 722e 646f 5f65  .z.Exporter.do_e
-00000670: 7870 6f72 7429 0472 0800 0000 7209 0000  xport).r....r...
-00000680: 0072 0a00 0000 4e29 0672 1d00 0000 7206  .r....N).r....r.
-00000690: 0000 0072 1e00 0000 721f 0000 0072 0a00  ...r....r....r..
-000006a0: 0000 4e29 06da 085f 5f6e 616d 655f 5fda  ..N)...__name__.
-000006b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000006c0: 7561 6c6e 616d 655f 5fda 0a73 686f 7274  ualname__..short
-000006d0: 5f64 6573 6372 1c00 0000 7226 0000 0072  _descr....r&...r
-000006e0: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
-000006f0: 0000 0072 0700 0000 0c00 0000 7308 0000  ...r........s...
-00000700: 0008 0004 010a 020e 1e72 0700 0000 290a  .........r....).
-00000710: da06 7479 7069 6e67 7202 0000 00da 1870  ..typingr......p
-00000720: 6561 6b72 646c 2e70 6c75 6769 6e73 2e65  eakrdl.plugins.e
-00000730: 7870 6f72 7465 7272 0300 0000 da08 6578  xporterr......ex
-00000740: 706f 7274 6572 7205 0000 00da 0861 7267  porterr......arg
-00000750: 7061 7273 65da 0e73 7973 7465 6d72 646c  parse..systemrdl
-00000760: 2e6e 6f64 6572 0600 0000 7207 0000 0072  .noder....r....r
-00000770: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
-00000780: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000790: 0073 0e00 0000 0c00 0c02 0c02 0402 0801  .s..............
-000007a0: 0c01 1403                                ....
+000000e0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
+000000f0: 7332 0000 0065 005a 0164 005a 0264 015a  s2...e.Z.d.Z.d.Z
+00000100: 0364 0264 0364 049c 0264 0564 0684 045a  .d.d.d...d.d...Z
+00000110: 0464 0764 0864 0364 099c 0364 0a64 0b84  .d.d.d.d...d.d..
+00000120: 045a 0564 0353 0029 0cda 0845 7870 6f72  .Z.d.S.)...Expor
+00000130: 7465 727a 1e47 656e 6572 6174 6520 6120  terz.Generate a 
+00000140: 6555 564d 2072 6567 6973 7465 7220 6d6f  eUVM register mo
+00000150: 6465 6c7a 1761 7267 7061 7273 652e 4172  delz.argparse.Ar
+00000160: 6775 6d65 6e74 5061 7273 6572 4e29 02da  gumentParserN)..
+00000170: 0961 7267 5f67 726f 7570 da06 7265 7475  .arg_group..retu
+00000180: 726e 6302 0000 0000 0000 0000 0000 0002  rnc.............
+00000190: 0000 0007 0000 0043 0000 0073 4800 0000  .......C...sH...
+000001a0: 7c01 6a00 6401 6402 6403 6404 6702 6403  |.j.d.d.d.d.g.d.
+000001b0: 6405 6406 8d05 0100 7c01 6a00 6407 6408  d.d.....|.j.d.d.
+000001c0: 6409 640a 6702 6409 640b 6406 8d05 0100  d.d.g.d.d.d.....
+000001d0: 7c01 6a00 640c 640d 640e 640f 6410 6411  |.j.d.d.d.d.d.d.
+000001e0: 8d05 0100 6400 5300 2912 4e7a 0b2d 2d66  ....d.S.).Nz.--f
+000001f0: 696c 652d 7479 7065 da09 6669 6c65 5f74  ile-type..file_t
+00000200: 7970 65da 0770 6163 6b61 6765 da06 6865  ype..package..he
+00000210: 6164 6572 7a40 4368 6f6f 7365 2074 6865  aderz@Choose the
+00000220: 2066 696c 6520 636f 6e74 6169 6e65 7220   file container 
+00000230: 7374 796c 6520 6f66 2074 6865 2072 6567  style of the reg
+00000240: 6973 7465 7220 6d6f 6465 6c2e 205b 7061  ister model. [pa
+00000250: 636b 6167 655d 2904 da04 6465 7374 da07  ckage])...dest..
+00000260: 6368 6f69 6365 73da 0764 6566 6175 6c74  choices..default
+00000270: da04 6865 6c70 7a0c 2d2d 7479 7065 2d73  ..helpz.--type-s
+00000280: 7479 6c65 da0a 7479 7065 5f73 7479 6c65  tyle..type_style
+00000290: da07 6c65 7869 6361 6c5a 0468 6965 7261  ..lexicalZ.hiera
+000002a0: 2801 0000 4368 6f6f 7365 2068 6f77 2063  (...Choose how c
+000002b0: 6c61 7373 2074 7970 6520 6e61 6d65 7320  lass type names 
+000002c0: 6172 6520 6765 6e65 7261 7465 642e 0a20  are generated.. 
+000002d0: 2020 2020 2020 2020 2020 2054 6865 2027             The '
+000002e0: 6c65 7869 6361 6c27 2073 7479 6c65 2077  lexical' style w
+000002f0: 696c 6c20 7573 6520 5244 4c20 6c65 7869  ill use RDL lexi
+00000300: 6361 6c20 7363 6f70 6520 2620 7479 7065  cal scope & type
+00000310: 206e 616d 6573 2077 6865 7265 0a20 2020   names where.   
+00000320: 2020 2020 2020 2020 2070 6f73 7369 626c           possibl
+00000330: 6520 616e 6420 6174 7465 6d70 7420 746f  e and attempt to
+00000340: 2072 652d 7573 6520 6571 7569 7661 6c65   re-use equivale
+00000350: 6e74 2063 6c61 7373 2064 6566 696e 6974  nt class definit
+00000360: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+00000370: 2020 5468 6520 2768 6965 7227 2073 7479    The 'hier' sty
+00000380: 6c65 2075 7365 7320 636f 6d70 6f6e 656e  le uses componen
+00000390: 7427 7320 6869 6572 6172 6368 7920 6173  t's hierarchy as
+000003a0: 2074 6865 2063 6c61 7373 2074 7970 6520   the class type 
+000003b0: 6e61 6d65 2e20 5b6c 6578 6963 616c 5d0a  name. [lexical].
+000003c0: 2020 2020 2020 2020 2020 2020 7a0d 2d2d              z.--
+000003d0: 7573 652d 6661 6374 6f72 79da 0b75 7365  use-factory..use
+000003e0: 5f66 6163 746f 7279 46da 0a73 746f 7265  _factoryF..store
+000003f0: 5f74 7275 657a 4f49 6620 7365 742c 2063  _truezOIf set, c
+00000400: 6c61 7373 2064 6566 696e 6974 696f 6e73  lass definitions
+00000410: 2061 6e64 2063 6c61 7373 2069 6e73 7461   and class insta
+00000420: 6e63 6573 2061 7265 2063 7265 6174 6564  nces are created
+00000430: 2075 7369 6e67 2074 6865 2055 564d 2066   using the UVM f
+00000440: 6163 746f 7279 2904 720d 0000 0072 0f00  actory).r....r..
+00000450: 0000 da06 6163 7469 6f6e 7210 0000 0029  ....actionr....)
+00000460: 01da 0c61 6464 5f61 7267 756d 656e 7429  ...add_argument)
+00000470: 02da 0473 656c 6672 0800 0000 a900 7218  ...selfr......r.
+00000480: 0000 00fa 312f 746d 702f 5065 616b 5244  ....1/tmp/PeakRD
+00000490: 4c2d 6575 766d 2f73 7263 2f70 6561 6b72  L-euvm/src/peakr
+000004a0: 646c 5f65 7576 6d2f 5f5f 7065 616b 7264  dl_euvm/__peakrd
+000004b0: 6c5f 5f2e 7079 da16 6164 645f 6578 706f  l__.py..add_expo
+000004c0: 7274 6572 5f61 7267 756d 656e 7473 0f00  rter_arguments..
+000004d0: 0000 732a 0000 0000 0104 0102 0102 0106  ..s*............
+000004e0: 0102 0102 fb06 0804 0102 0102 0106 0102  ................
+000004f0: 0102 fb06 0c04 0102 0102 0102 0102 0102  ................
+00000500: fb7a 1f45 7870 6f72 7465 722e 6164 645f  .z.Exporter.add_
+00000510: 6578 706f 7274 6572 5f61 7267 756d 656e  exporter_argumen
+00000520: 7473 7206 0000 007a 1261 7267 7061 7273  tsr....z.argpars
+00000530: 652e 4e61 6d65 7370 6163 6529 03da 0874  e.Namespace)...t
+00000540: 6f70 5f6e 6f64 65da 076f 7074 696f 6e73  op_node..options
+00000550: 7209 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00000560: 0000 0400 0000 0700 0000 4300 0000 732e  ..........C...s.
+00000570: 0000 0074 0083 007d 037c 036a 017c 017c  ...t...}.|.j.|.|
+00000580: 026a 027c 026a 0364 016b 027c 026a 0464  .j.|.j.d.k.|.j.d
+00000590: 026b 027c 026a 0564 038d 0501 0064 0053  .k.|.j.d.....d.S
+000005a0: 0029 044e 720b 0000 0072 1200 0000 2903  .).Nr....r....).
+000005b0: da11 6578 706f 7274 5f61 735f 7061 636b  ..export_as_pack
+000005c0: 6167 65da 1772 6575 7365 5f63 6c61 7373  age..reuse_class
+000005d0: 5f64 6566 696e 6974 696f 6e73 da0f 7573  _definitions..us
+000005e0: 655f 7576 6d5f 6661 6374 6f72 7929 0672  e_uvm_factory).r
+000005f0: 0500 0000 da06 6578 706f 7274 da06 6f75  ......export..ou
+00000600: 7470 7574 720a 0000 0072 1100 0000 7213  tputr....r....r.
+00000610: 0000 0029 0472 1700 0000 721b 0000 0072  ...).r....r....r
+00000620: 1c00 0000 da01 7872 1800 0000 7218 0000  ......xr....r...
+00000630: 0072 1900 0000 da09 646f 5f65 7870 6f72  .r......do_expor
+00000640: 742d 0000 0073 1000 0000 0001 0601 0401  t-...s..........
+00000650: 0201 0401 0801 0801 04fb 7a12 4578 706f  ..........z.Expo
+00000660: 7274 6572 2e64 6f5f 6578 706f 7274 2906  rter.do_export).
+00000670: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000680: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000690: 6d65 5f5f da0a 7368 6f72 745f 6465 7363  me__..short_desc
+000006a0: 721a 0000 0072 2300 0000 7218 0000 0072  r....r#...r....r
+000006b0: 1800 0000 7218 0000 0072 1900 0000 7207  ....r....r....r.
+000006c0: 0000 000c 0000 0073 0600 0000 0801 0402  .......s........
+000006d0: 101e 7207 0000 0029 0ada 0674 7970 696e  ..r....)...typin
+000006e0: 6772 0200 0000 5a18 7065 616b 7264 6c2e  gr....Z.peakrdl.
+000006f0: 706c 7567 696e 732e 6578 706f 7274 6572  plugins.exporter
+00000700: 7203 0000 00da 0865 7870 6f72 7465 7272  r......exporterr
+00000710: 0500 0000 da08 6172 6770 6172 7365 5a0e  ......argparseZ.
+00000720: 7379 7374 656d 7264 6c2e 6e6f 6465 7206  systemrdl.noder.
+00000730: 0000 0072 0700 0000 7218 0000 0072 1800  ...r....r....r..
+00000740: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
+00000750: 6f64 756c 653e 0100 0000 730c 0000 000c  odule>....s.....
+00000760: 020c 020c 0204 0108 010c 03              ...........
```

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/SOURCES.txt` & `peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.0/src/peakrdl_euvm.egg-info/PKG-INFO` & `peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-euvm
-Version: 1.0
+Version: 1.1
 Summary: Generate eUVM register model from compiled SystemRDL input
 Home-page: https://github.com/coverify/PeakRDL-euvm
 Author: Alex Mykyta, Jude Zhang
 License: UNKNOWN
 Project-URL: Source, https://github.com/coverify/PeakRDL-euvm
 Project-URL: Tracker, https://github.com/coverify/PeakRDL-euvm/issues
 Platform: UNKNOWN
```

### Comparing `peakrdl-euvm-1.0/LICENSE` & `peakrdl-euvm-1.1/LICENSE`

 * *Files identical despite different names*

