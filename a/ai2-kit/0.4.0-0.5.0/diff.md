# Comparing `tmp/ai2_kit-0.4.0.tar.gz` & `tmp/ai2_kit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.4.0.tar", max compression
+gzip compressed data, was "ai2_kit-0.5.0.tar", max compression
```

## Comparing `ai2_kit-0.4.0.tar` & `ai2_kit-0.5.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.4.0/LICENSE
--rw-r--r--   0        0        0     1962 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.4.0/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.4.0/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.4.0/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
--rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.4.0/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
--rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
--rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.4.0/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     7307 2023-02-14 03:43:41.330120 ai2_kit-0.4.0/ai2_kit/core/__pycache__/connector.cpython-39.pyc
--rw-r--r--   0        0        0     9582 2023-07-20 03:31:48.646223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/executor.cpython-39.pyc
--rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.4.0/ai2_kit/core/__pycache__/future.cpython-39.pyc
--rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/job.cpython-39.pyc
--rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.4.0/ai2_kit/core/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0    10069 2023-07-20 07:05:10.973356 ai2_kit-0.4.0/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
--rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
--rw-r--r--   0        0        0     2611 2023-07-20 03:31:49.026223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/script.cpython-39.pyc
--rw-r--r--   0        0        0     6829 2023-07-19 08:28:35.806120 ai2_kit-0.4.0/ai2_kit/core/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5745 2023-07-10 01:27:05.779682 ai2_kit-0.4.0/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.4.0/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7939 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.4.0/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.4.0/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/core/script.py
--rw-r--r--   0        0        0     5050 2023-07-18 07:59:30.544857 ai2_kit-0.4.0/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.4.0/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.4.0/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4374 2023-07-19 08:29:57.336102 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
--rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
--rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/common.cpython-39.pyc
--rw-r--r--   0        0        0     1430 2023-07-19 08:30:00.906101 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0     5609 2023-07-21 01:23:26.304847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
--rw-r--r--   0        0        0     5983 2023-07-21 01:23:26.104847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/data.cpython-39.pyc
--rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
--rw-r--r--   0        0        0     6358 2023-07-21 01:23:26.094847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
--rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
--rw-r--r--   0        0        0    12264 2023-07-21 01:23:26.164847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
--rw-r--r--   0        0        0     9313 2023-07-21 01:23:26.174847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
--rw-r--r--   0        0        0     3599 2023-07-21 01:23:26.174847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
--rw-r--r--   0        0        0      538 2023-07-21 01:23:26.544847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
--rw-r--r--   0        0        0     3360 2023-07-20 03:31:49.356223 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     6463 2023-07-21 01:23:26.304847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
--rw-r--r--   0        0        0     5276 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/asap.py
--rw-r--r--   0        0        0     1650 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     6679 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/data.py
--rw-r--r--   0        0        0     7895 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.4.0/ai2_kit/domain/iface.py
--rw-r--r--   0        0        0    17292 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     9028 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/lasp.py
--rw-r--r--   0        0        0     3778 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     6882 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/domain/util.py
--rw-r--r--   0        0        0     7678 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.4.0/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.4.0/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.4.0/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
--rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.4.0/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7915 2023-07-21 01:23:25.924847 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
--rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
--rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
--rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
--rw-r--r--   0        0        0    10027 2023-07-21 01:27:23.154801 ai2_kit-0.4.0/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9073 2023-07-21 01:27:23.154801 ai2_kit-0.4.0/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      953 2023-07-21 01:28:07.314792 ai2_kit-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 ai2_kit-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.0/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.5.0/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.5.0/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.5.0/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
+-rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
+-rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.5.0/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     7307 2023-07-24 07:57:09.456574 ai2_kit-0.5.0/ai2_kit/core/__pycache__/connector.cpython-39.pyc
+-rw-r--r--   0        0        0     9586 2023-07-24 09:28:27.095300 ai2_kit-0.5.0/ai2_kit/core/__pycache__/executor.cpython-39.pyc
+-rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.5.0/ai2_kit/core/__pycache__/future.cpython-39.pyc
+-rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/job.cpython-39.pyc
+-rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.5.0/ai2_kit/core/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0    10069 2023-07-21 03:41:53.042985 ai2_kit-0.5.0/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
+-rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.5.0/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     2611 2023-07-21 03:41:53.282985 ai2_kit-0.5.0/ai2_kit/core/__pycache__/script.cpython-39.pyc
+-rw-r--r--   0        0        0     8116 2023-07-24 09:28:27.215300 ai2_kit-0.5.0/ai2_kit/core/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5745 2023-07-10 01:27:05.779682 ai2_kit-0.5.0/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.0/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.0/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8006 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.0/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.0/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     5900 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.0/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.5.0/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4566 2023-07-24 09:28:27.615300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
+-rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
+-rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0        0        0     1532 2023-07-24 09:28:27.285300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0     5609 2023-07-21 03:41:53.572985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
+-rw-r--r--   0        0        0     5117 2023-07-24 09:28:27.245300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
+-rw-r--r--   0        0        0     6358 2023-07-21 03:41:53.282985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
+-rw-r--r--   0        0        0    12264 2023-07-21 03:41:53.392985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
+-rw-r--r--   0        0        0     9323 2023-07-24 09:28:27.295300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
+-rw-r--r--   0        0        0    10687 2023-07-24 09:28:27.305300 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
+-rw-r--r--   0        0        0      538 2023-07-21 03:41:53.862985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
+-rw-r--r--   0        0        0     3360 2023-07-24 08:47:10.485875 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     6463 2023-07-21 03:41:53.572985 ai2_kit-0.5.0/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
+-rw-r--r--   0        0        0     5225 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0     7895 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.0/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    17292 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0    13582 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.0/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7678 2023-07-21 01:27:23.144801 ai2_kit-0.5.0/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.0/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.0/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.5.0/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.5.0/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
+-rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.0/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.0/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7937 2023-07-24 09:28:27.095300 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
+-rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
+-rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.0/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      953 2023-07-24 09:30:29.085274 ai2_kit-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.0/PKG-INFO
```

### Comparing `ai2_kit-0.4.0/LICENSE` & `ai2_kit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/README.md` & `ai2_kit-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 Note that instead of running global `ai2-kit` command, you should run `./ai2-kit` to run the command from source.
 
 ## Manuals
 
 ### Domain Specific Tools
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
-* [CLL MLP Training Workflow](doc/manual/cll-workflow.md)
+* CLL MLP Training Workflow: [English](doc/manual/cll-workflow.md), [中文](doc/manual/cll-workflow.zh.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ### Build-in Functionalities
 * [Checkpoint Mechanism](doc/manual/checkpoint.md)
 * [ASE Toolkit](doc/manual/ase.md)
 * [Tips](doc/manual/tips.md)
```

### Comparing `ai2_kit-0.4.0/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.5.0/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/artifact.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/artifact.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/cmd.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/connector.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/connector.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb  6 09:01:27 2023 UTC, .py size: 5766 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e7c1 e063 8616 0000  a..........c....
+00000000: 610d 0d0a 0000 0000 830b ba64 8616 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 5a0e 6400  m.Z...d.d.l.Z.d.
```

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/executor.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/executor.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul  6 07:55:32 2023 UTC, .py size: 7939 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7473 a664 031f 0000  a.......ts.d....
+00000000: 610d 0d0a 0000 0000 8c43 be64 461f 0000  a........C.dF...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5401 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6400 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -541,59 +541,60 @@
 000021c0: 0000 0072 1f00 0000 7220 0000 0072 1500  ...r....r ...r..
 000021d0: 0000 7222 0000 0072 1900 0000 7265 0000  ..r"...r....re..
 000021e0: 0072 9000 0000 7223 0000 0072 2300 0000  .r....r#...r#...
 000021f0: 7223 0000 0072 2400 0000 728a 0000 00ce  r#...r$...r.....
 00002200: 0000 0073 0400 0000 0801 1604 728a 0000  ...s........r...
 00002210: 0072 7400 0000 2901 7236 0000 0063 0200  .rt...).r6...c..
 00002220: 0000 0000 0000 0000 0000 0400 0000 0800  ................
-00002230: 0000 4300 0000 734c 0000 0074 00a0 0174  ..C...sL...t...t
+00002230: 0000 4300 0000 734e 0000 0074 00a0 0174  ..C...sN...t...t
 00002240: 02a0 0374 046a 057c 0074 046a 0664 018d  ...t.j.|.t.j.d..
 00002250: 0264 02a1 02a1 017d 0264 0364 0474 077c  .d.....}.d.d.t.|
-00002260: 0283 019b 0064 059d 0364 0674 077c 0183  .....d...d.t.|..
-00002270: 019b 0064 079d 0364 0867 047d 0364 09a0  ...d...d.g.}.d..
-00002280: 087c 03a1 0153 0029 0a4e 2901 da08 7072  .|...S.).N)...pr
-00002290: 6f74 6f63 6f6c e905 0000 007a 2769 6d70  otocol.....z'imp
-000022a0: 6f72 7420 6261 7365 3634 2c62 7a32 2c73  ort base64,bz2,s
-000022b0: 7973 2c63 6c6f 7564 7069 636b 6c65 2061  ys,cloudpickle a
-000022c0: 7320 6370 7a2b 723d 6370 2e6c 6f61 6473  s cpz+r=cp.loads
-000022d0: 2862 7a32 2e64 6563 6f6d 7072 6573 7328  (bz2.decompress(
-000022e0: 6261 7365 3634 2e62 3634 6465 636f 6465  base64.b64decode
-000022f0: 287a 0529 2929 2829 7a06 7072 696e 7428  (z.)))()z.print(
-00002300: 7a5d 2b62 6173 6536 342e 6236 3465 6e63  z]+base64.b64enc
-00002310: 6f64 6528 627a 322e 636f 6d70 7265 7373  ode(bz2.compress
-00002320: 2863 702e 6475 6d70 7328 722c 2070 726f  (cp.dumps(r, pro
-00002330: 746f 636f 6c3d 6370 2e44 4546 4155 4c54  tocol=cp.DEFAULT
-00002340: 5f50 524f 544f 434f 4c29 2c35 2929 2e64  _PROTOCOL),5)).d
-00002350: 6563 6f64 6528 2761 7363 6969 2729 297a  ecode('ascii'))z
-00002360: 1273 7973 2e73 7464 6f75 742e 666c 7573  .sys.stdout.flus
-00002370: 6828 29fa 013b 2909 727c 0000 00da 0962  h()..;).r|.....b
-00002380: 3634 656e 636f 6465 727a 0000 00da 0863  64encoderz.....c
-00002390: 6f6d 7072 6573 7372 7800 0000 da05 6475  ompressrx.....du
-000023a0: 6d70 735a 1044 4546 4155 4c54 5f50 524f  mpsZ.DEFAULT_PRO
-000023b0: 544f 434f 4cda 0472 6570 7272 5200 0000  TOCOL..reprrR...
-000023c0: 2904 7236 0000 0072 7500 0000 5a09 6475  ).r6...ru...Z.du
-000023d0: 6d70 6564 5f66 6e72 3300 0000 7223 0000  mped_fnr3...r#..
-000023e0: 0072 2300 0000 7224 0000 0072 7600 0000  .r#...r$...rv...
-000023f0: e000 0000 730e 0000 0000 011e 0202 010e  ....s...........
-00002400: 010e 0102 fc04 0672 7600 0000 2901 7274  .......rv...).rt
-00002410: 0000 0029 3072 1b00 0000 7202 0000 0072  ...)0r....r....r
-00002420: 0300 0000 7204 0000 0072 0500 0000 5a03  ....r....r....Z.
-00002430: 6a6f 6272 0600 0000 724d 0000 0072 0700  jobr....rM...r..
-00002440: 0000 7261 0000 0072 0800 0000 7209 0000  ..ra...r....r...
-00002450: 0072 0a00 0000 720b 0000 00da 0475 7469  .r....r......uti
-00002460: 6c72 0c00 0000 da03 6c6f 6772 0d00 0000  lr......logr....
-00002470: 721e 0000 0072 5800 0000 da08 7079 6461  r....rX.....pyda
-00002480: 6e74 6963 720f 0000 00da 0674 7970 696e  nticr......typin
-00002490: 6772 1000 0000 7211 0000 0072 1200 0000  gr....r....r....
-000024a0: 7213 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-000024b0: 0361 6263 7216 0000 0072 1700 0000 5a06  .abcr....r....Z.
-000024c0: 696e 766f 6b65 7218 0000 0072 5100 0000  invoker....rQ...
-000024d0: 726c 0000 0072 7c00 0000 727a 0000 0072  rl...r|...rz...r
-000024e0: 7800 0000 7219 0000 0072 2200 0000 5a0b  x...r....r"...Z.
-000024f0: 4578 6563 7574 6f72 4d61 7072 2500 0000  ExecutorMapr%...
-00002500: 7227 0000 0072 5c00 0000 7289 0000 0072  r'...r\...r....r
-00002510: 8a00 0000 7276 0000 0072 2300 0000 7223  ....rv...r#...r#
-00002520: 0000 0072 2300 0000 7224 0000 00da 083c  ...r#...r$.....<
-00002530: 6d6f 6475 6c65 3e01 0000 0073 2e00 0000  module>....s....
-00002540: 1801 0c01 0c01 1801 0c01 0c02 0803 0c01  ................
-00002550: 2001 1001 0c01 0801 0801 0801 0801 0803   ...............
-00002560: 1006 0c02 0c02 103d 106b 1206 0e12       .......=.k....
+00002260: 0283 019b 0064 059d 0364 0664 0774 077c  .....d...d.d.t.|
+00002270: 0183 019b 0064 089d 0364 0667 057d 0364  .....d...d.g.}.d
+00002280: 09a0 087c 03a1 0153 0029 0a4e 2901 da08  ...|...S.).N)...
+00002290: 7072 6f74 6f63 6f6c e905 0000 007a 2769  protocol.....z'i
+000022a0: 6d70 6f72 7420 6261 7365 3634 2c62 7a32  mport base64,bz2
+000022b0: 2c73 7973 2c63 6c6f 7564 7069 636b 6c65  ,sys,cloudpickle
+000022c0: 2061 7320 6370 7a2b 723d 6370 2e6c 6f61   as cpz+r=cp.loa
+000022d0: 6473 2862 7a32 2e64 6563 6f6d 7072 6573  ds(bz2.decompres
+000022e0: 7328 6261 7365 3634 2e62 3634 6465 636f  s(base64.b64deco
+000022f0: 6465 287a 0529 2929 2829 7a12 7379 732e  de(z.)))()z.sys.
+00002300: 7374 646f 7574 2e66 6c75 7368 2829 7a06  stdout.flush()z.
+00002310: 7072 696e 7428 7a5d 2b62 6173 6536 342e  print(z]+base64.
+00002320: 6236 3465 6e63 6f64 6528 627a 322e 636f  b64encode(bz2.co
+00002330: 6d70 7265 7373 2863 702e 6475 6d70 7328  mpress(cp.dumps(
+00002340: 722c 2070 726f 746f 636f 6c3d 6370 2e44  r, protocol=cp.D
+00002350: 4546 4155 4c54 5f50 524f 544f 434f 4c29  EFAULT_PROTOCOL)
+00002360: 2c35 2929 2e64 6563 6f64 6528 2761 7363  ,5)).decode('asc
+00002370: 6969 2729 29fa 013b 2909 727c 0000 00da  ii'))..;).r|....
+00002380: 0962 3634 656e 636f 6465 727a 0000 00da  .b64encoderz....
+00002390: 0863 6f6d 7072 6573 7372 7800 0000 da05  .compressrx.....
+000023a0: 6475 6d70 735a 1044 4546 4155 4c54 5f50  dumpsZ.DEFAULT_P
+000023b0: 524f 544f 434f 4cda 0472 6570 7272 5200  ROTOCOL..reprrR.
+000023c0: 0000 2904 7236 0000 0072 7500 0000 5a09  ..).r6...ru...Z.
+000023d0: 6475 6d70 6564 5f66 6e72 3300 0000 7223  dumped_fnr3...r#
+000023e0: 0000 0072 2300 0000 7224 0000 0072 7600  ...r#...r$...rv.
+000023f0: 0000 e000 0000 7310 0000 0000 011e 0202  ......s.........
+00002400: 010e 0102 010e 0102 fb04 0772 7600 0000  ...........rv...
+00002410: 2901 7274 0000 0029 3072 1b00 0000 7202  ).rt...)0r....r.
+00002420: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
+00002430: 0000 5a03 6a6f 6272 0600 0000 724d 0000  ..Z.jobr....rM..
+00002440: 0072 0700 0000 7261 0000 0072 0800 0000  .r....ra...r....
+00002450: 7209 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
+00002460: 0475 7469 6c72 0c00 0000 da03 6c6f 6772  .utilr......logr
+00002470: 0d00 0000 721e 0000 0072 5800 0000 da08  ....r....rX.....
+00002480: 7079 6461 6e74 6963 720f 0000 00da 0674  pydanticr......t
+00002490: 7970 696e 6772 1000 0000 7211 0000 0072  ypingr....r....r
+000024a0: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
+000024b0: 0000 00da 0361 6263 7216 0000 0072 1700  .....abcr....r..
+000024c0: 0000 5a06 696e 766f 6b65 7218 0000 0072  ..Z.invoker....r
+000024d0: 5100 0000 726c 0000 0072 7c00 0000 727a  Q...rl...r|...rz
+000024e0: 0000 0072 7800 0000 7219 0000 0072 2200  ...rx...r....r".
+000024f0: 0000 5a0b 4578 6563 7574 6f72 4d61 7072  ..Z.ExecutorMapr
+00002500: 2500 0000 7227 0000 0072 5c00 0000 7289  %...r'...r\...r.
+00002510: 0000 0072 8a00 0000 7276 0000 0072 2300  ...r....rv...r#.
+00002520: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
+00002530: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00002540: 2e00 0000 1801 0c01 0c01 1801 0c01 0c02  ................
+00002550: 0803 0c01 2001 1001 0c01 0801 0801 0801  .... ...........
+00002560: 0801 0803 1006 0c02 0c02 103d 106b 1206  ...........=.k..
+00002570: 0e12                                     ..
```

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/future.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/future.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/job.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/job.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 20 07:00:17 2023 UTC, .py size: 9587 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 81db b864 7325 0000  a..........ds%..
+00000000: 610d 0d0a 0000 0000 fbde b964 7325 0000  a..........ds%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 f400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 5a08 6400 6404 6c09 5a09 6400 6404 6c0a  Z.d.d.l.Z.d.d.l.
 00000070: 5a0a 6400 6404 6c0b 5a0b 6400 6404 6c0c  Z.d.d.l.Z.d.d.l.
```

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/script.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/script.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jul 19 02:49:54 2023 UTC, .py size: 2363 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 524f b764 3b09 0000  a.......RO.d;...
+00000000: 610d 0d0a 0000 0000 fbde b964 3b09 0000  a..........d;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 5a06 6413 6405 6406 8401 5a07  d.l.Z.d.d.d...Z.
 00000060: 6508 6407 9c01 6408 6409 8404 5a09 4700  e.d...d.d...Z.G.
 00000070: 640a 640b 8400 640b 6501 8303 5a0a 4700  d.d...d.e...Z.G.
```

### Comparing `ai2_kit-0.4.0/ai2_kit/core/__pycache__/util.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/core/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul 18 07:59:30 2023 UTC, .py size: 5050 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,427 +1,508 @@
-00000000: 610d 0d0a 0000 0000 6246 b664 ba13 0000  a.......bF.d....
+00000000: 610d 0d0a 0000 0000 8c43 be64 0c17 0000  a........C.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 7601 0000 6400  .....@...sv...d.
+00000020: 0009 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 6400 6405 6c0a 5a0a 6400  m.Z...d.d.l.Z.d.
-00000070: 6405 6c0b 5a0b 6400 6405 6c0c 5a0c 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6405 6c0d 5a0d 6400 6405 6c0e 5a0e 6400  d.l.Z.d.d.l.Z.d.
-00000090: 6405 6c0f 5a0f 6406 6407 6c10 6d11 5a11  d.l.Z.d.d.l.m.Z.
-000000a0: 0100 6511 6512 8301 5a13 6514 8300 5a15  ..e.e...Z.e...Z.
-000000b0: 6408 6409 8400 5a16 6503 640a 9c01 640b  d.d...Z.e.d...d.
-000000c0: 640c 8404 5a17 6505 6503 1900 640d 9c01  d...Z.e.e...d...
-000000d0: 640e 640f 8404 5a18 6410 6411 8400 5a19  d.d...Z.d.d...Z.
-000000e0: 6506 651a 1900 6506 651a 1900 6412 9c02  e.e...e.e...d...
-000000f0: 6413 6414 8404 5a1b 6507 6415 8301 5a1c  d.d...Z.e.d...Z.
-00000100: 6506 6506 651c 1900 1900 6506 651c 1900  e.e.e.....e.e...
-00000110: 6412 9c02 6416 6417 8404 5a1d 651a 651a  d...d.d...Z.e.e.
-00000120: 6418 9c02 6419 641a 8404 5a1e 6506 651c  d...d.d...Z.e.e.
-00000130: 1900 651f 6506 6506 651c 1900 1900 641b  ..e.e.e.e.....d.
-00000140: 9c03 641c 641d 8404 5a20 651a 651a 6418  ..d.d...Z e.e.d.
-00000150: 9c02 641e 641f 8404 5a21 651c 651c 6420  ..d.d...Z!e.e.d 
-00000160: 9c02 6421 6422 8404 5a22 4700 6423 6424  ..d!d"..Z"G.d#d$
-00000170: 8400 6424 8302 5a23 4700 6425 6426 8400  ..d$..Z#G.d%d&..
-00000180: 6426 8302 5a24 6427 6428 8400 5a25 6525  d&..Z$d'd(..Z%e%
-00000190: 8300 5c06 5a26 5a27 5a28 5a29 5a2a 5a2b  ..\.Z&Z'Z(Z)Z*Z+
-000001a0: 6405 5300 2929 e900 0000 0029 01da 0459  d.S.)).....)...Y
-000001b0: 414d 4c29 01da 0450 6174 6829 03da 0554  AML)...Path)...T
-000001c0: 7570 6c65 da04 4c69 7374 da07 5479 7065  uple..List..Type
-000001d0: 5661 72a9 01da 0566 6965 6c64 4ee9 0100  Var....fieldN...
-000001e0: 0000 2901 da0a 6765 745f 6c6f 6767 6572  ..)...get_logger
-000001f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000200: 0004 0000 0003 0000 0073 1200 0000 7400  .........s....t.
-00000210: 8700 6601 6401 6402 8408 6403 8d01 5300  ..f.d.d...d...S.
-00000220: 2904 4e63 0000 0000 0000 0000 0000 0000  ).Nc............
-00000230: 0000 0000 0300 0000 1300 0000 730a 0000  ............s...
-00000240: 0074 00a0 0088 00a1 0153 00a9 014e 2901  .t.......S...N).
-00000250: da04 636f 7079 a900 a901 da03 6f62 6a72  ..copy......objr
-00000260: 0d00 0000 fa2c 2f68 6f6d 652f 6865 6e72  .....,/home/henr
-00000270: 792f 7372 632f 6169 322d 6b69 742f 6169  y/src/ai2-kit/ai
-00000280: 325f 6b69 742f 636f 7265 2f75 7469 6c2e  2_kit/core/util.
-00000290: 7079 da08 3c6c 616d 6264 613e 1500 0000  py..<lambda>....
-000002a0: f300 0000 007a 2764 6566 6175 6c74 5f6d  .....z'default_m
-000002b0: 7574 6162 6c65 5f66 6965 6c64 2e3c 6c6f  utable_field.<lo
-000002c0: 6361 6c73 3e2e 3c6c 616d 6264 613e 2901  cals>.<lambda>).
-000002d0: da0f 6465 6661 756c 745f 6661 6374 6f72  ..default_factor
-000002e0: 7972 0700 0000 720e 0000 0072 0d00 0000  yr....r....r....
-000002f0: 720e 0000 0072 1000 0000 da15 6465 6661  r....r......defa
-00000300: 756c 745f 6d75 7461 626c 655f 6669 656c  ult_mutable_fiel
-00000310: 6414 0000 0073 0200 0000 0001 7214 0000  d....s......r...
-00000320: 0029 01da 0470 6174 6863 0100 0000 0000  .)...pathc......
-00000330: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000340: 0000 7328 0000 0074 0064 0164 028d 017d  ..s(...t.d.d...}
-00000350: 0174 01a0 027c 01a1 0101 0074 03a0 027c  .t...|.....t...|
-00000360: 01a1 0101 007c 01a0 047c 00a1 0153 0029  .....|...|...S.)
-00000370: 034e da04 7361 6665 2901 da03 7479 7029  .N..safe)...typ)
-00000380: 0572 0200 0000 da07 4a6f 696e 5461 67da  .r......JoinTag.
-00000390: 0872 6567 6973 7465 72da 0752 6561 6454  .register..ReadT
-000003a0: 6167 da04 6c6f 6164 2902 7215 0000 00da  ag..load).r.....
-000003b0: 0479 616d 6c72 0d00 0000 720d 0000 0072  .yamlr....r....r
-000003c0: 1000 0000 da0e 6c6f 6164 5f79 616d 6c5f  ......load_yaml_
-000003d0: 6669 6c65 1800 0000 7308 0000 0000 010a  file....s.......
-000003e0: 010a 010a 0172 1d00 0000 2901 da05 7061  .....r....)...pa
-000003f0: 7468 7363 0000 0000 0000 0000 0000 0000  thsc............
-00000400: 0300 0000 0600 0000 4700 0000 732e 0000  ........G...s...
-00000410: 0069 007d 017c 0044 005d 207d 0274 0064  .i.}.|.D.] }.t.d
-00000420: 017c 0283 0201 0074 017c 0174 0274 037c  .|.....t.|.t.t.|
-00000430: 0283 0183 0183 027d 0171 087c 0153 0029  .......}.q.|.S.)
-00000440: 024e 7a10 6c6f 6164 2079 616d 6c20 6669  .Nz.load yaml fi
-00000450: 6c65 3a20 2904 da05 7072 696e 74da 0a6d  le: )...print..m
-00000460: 6572 6765 5f64 6963 7472 1d00 0000 7203  erge_dictr....r.
-00000470: 0000 0029 0372 1e00 0000 da01 6472 1500  ...).r......dr..
-00000480: 0000 720d 0000 0072 0d00 0000 7210 0000  ..r....r....r...
-00000490: 00da 0f6c 6f61 645f 7961 6d6c 5f66 696c  ...load_yaml_fil
-000004a0: 6573 1f00 0000 730a 0000 0000 0104 0108  es....s.........
-000004b0: 010a 0114 0172 2200 0000 6300 0000 0000  .....r"...c.....
-000004c0: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
-000004d0: 0000 0073 0800 0000 7400 a001 a100 5300  ...s....t.....S.
-000004e0: 2901 7a0a 7368 6f72 7420 7575 6964 2902  ).z.short uuid).
-000004f0: da09 7368 6f72 7475 7569 64da 0475 7569  ..shortuuid..uui
-00000500: 6472 0d00 0000 720d 0000 0072 0d00 0000  dr....r....r....
-00000510: 7210 0000 00da 0673 5f75 7569 6427 0000  r......s_uuid'..
-00000520: 0073 0200 0000 0002 7225 0000 0029 02da  .s......r%...)..
-00000530: 016c da06 7265 7475 726e 6301 0000 0000  .l..returnc.....
-00000540: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00000550: 0000 0073 1000 0000 7400 7401 7402 7c00  ...s....t.t.t.|.
-00000560: 8301 8301 8301 5300 2901 7a1d 7265 6d6f  ......S.).z.remo
-00000570: 7665 2064 7570 6c69 6361 7465 2073 7472  ve duplicate str
-00000580: 2061 6e64 2073 6f72 7429 03da 046c 6973   and sort)...lis
-00000590: 74da 0673 6f72 7465 64da 0373 6574 a901  t..sorted..set..
-000005a0: 7226 0000 0072 0d00 0000 720d 0000 0072  r&...r....r....r
-000005b0: 1000 0000 da14 736f 7274 5f75 6e69 7175  ......sort_uniqu
-000005c0: 655f 7374 725f 6c69 7374 2c00 0000 7302  e_str_list,...s.
-000005d0: 0000 0000 0272 2c00 0000 da01 5463 0100  .....r,.....Tc..
-000005e0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000005f0: 0000 4300 0000 730e 0000 0064 0164 0284  ..C...s....d.d..
-00000600: 007c 0044 0083 0153 0029 034e 6301 0000  .|.D...S.).Nc...
-00000610: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000620: 0053 0000 0073 1a00 0000 6700 7c00 5d12  .S...s....g.|.].
-00000630: 7d01 7c01 4400 5d08 7d02 7c02 9103 710c  }.|.D.].}.|...q.
-00000640: 7104 5300 720d 0000 0072 0d00 0000 2903  q.S.r....r....).
-00000650: da02 2e30 da07 7375 626c 6973 74da 0469  ...0..sublist..i
-00000660: 7465 6d72 0d00 0000 720d 0000 0072 1000  temr....r....r..
-00000670: 0000 da0a 3c6c 6973 7463 6f6d 703e 3500  ....<listcomp>5.
-00000680: 0000 7212 0000 007a 1b66 6c61 7474 656e  ..r....z.flatten
-00000690: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000006a0: 6f6d 703e 720d 0000 0072 2b00 0000 720d  omp>r....r+...r.
-000006b0: 0000 0072 0d00 0000 7210 0000 00da 0766  ...r....r......f
-000006c0: 6c61 7474 656e 3400 0000 7302 0000 0000  latten4...s.....
-000006d0: 0172 3200 0000 2902 da01 7372 2700 0000  .r2...)...sr'...
-000006e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000006f0: 0004 0000 0043 0000 0073 1200 0000 7c00  .....C...s....|.
-00000700: 6a00 6600 6900 7401 6a02 a401 8e01 5300  j.f.i.t.j.....S.
-00000710: 720b 0000 0029 03da 0666 6f72 6d61 74da  r....)...format.
-00000720: 026f 73da 0765 6e76 6972 6f6e 2901 7233  .os..environ).r3
-00000730: 0000 0072 0d00 0000 720d 0000 0072 1000  ...r....r....r..
-00000740: 0000 da11 666f 726d 6174 5f65 6e76 5f73  ....format_env_s
-00000750: 7472 696e 6738 0000 0073 0200 0000 0001  tring8...s......
-00000760: 7237 0000 0029 0372 2600 0000 da01 6e72  r7...).r&.....nr
-00000770: 2700 0000 6302 0000 0000 0000 0000 0000  '...c...........
-00000780: 0002 0000 0003 0000 0003 0000 0073 2c00  .............s,.
-00000790: 0000 7400 7401 8801 8301 7c01 8302 5c02  ..t.t.....|...\.
-000007a0: 8900 8902 8700 8701 8702 6603 6401 6402  ..........f.d.d.
-000007b0: 8408 7402 7c01 8301 4400 8301 5300 2903  ..t.|...D...S.).
-000007c0: 7a18 7370 6c69 7420 6c69 7374 2069 6e74  z.split list int
-000007d0: 6f20 6e20 6368 756e 6b73 6301 0000 0000  o n chunksc.....
-000007e0: 0000 0000 0000 0002 0000 0008 0000 0013  ................
-000007f0: 0000 0073 3c00 0000 6700 7c00 5d34 7d01  ...s<...g.|.]4}.
-00000800: 8801 7c01 8800 1400 7400 7c01 8802 8302  ..|.....t.|.....
-00000810: 1700 7c01 6400 1700 8800 1400 7400 7c01  ..|.d.......t.|.
-00000820: 6400 1700 8802 8302 1700 8502 1900 9102  d...............
-00000830: 7104 5300 2901 7209 0000 0029 01da 036d  q.S.).r....)...m
-00000840: 696e a902 722e 0000 00da 0169 a903 da01  in..r......i....
-00000850: 6b72 2600 0000 da01 6d72 0d00 0000 7210  kr&.....mr....r.
-00000860: 0000 0072 3100 0000 4000 0000 7212 0000  ...r1...@...r...
-00000870: 007a 1e6c 6973 745f 7370 6c69 742e 3c6c  .z.list_split.<l
-00000880: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000890: 3e29 03da 0664 6976 6d6f 64da 036c 656e  >)...divmod..len
-000008a0: da05 7261 6e67 6529 0272 2600 0000 7238  ..range).r&...r8
-000008b0: 0000 0072 0d00 0000 723c 0000 0072 1000  ...r....r<...r..
-000008c0: 0000 da0a 6c69 7374 5f73 706c 6974 3c00  ....list_split<.
-000008d0: 0000 7304 0000 0000 0312 0172 4200 0000  ..s........rB...
-000008e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000008f0: 0005 0000 0043 0000 0073 2c00 0000 7400  .....C...s,...t.
-00000900: a001 7c00 a002 6401 a101 a101 a003 a100  ..|...d.........
-00000910: 7d01 7404 a005 7c01 a101 a006 6401 a101  }.t...|.....d...
-00000920: 6402 6403 8502 1900 5300 2904 7a11 7368  d.d.....S.).z.sh
-00000930: 6f72 7420 6861 7368 2073 7472 696e 677a  ort hash stringz
-00000940: 0575 7466 2d38 4ee9 feff ffff 2907 da07  .utf-8N.....)...
-00000950: 6861 7368 6c69 62da 0473 6861 31da 0665  hashlib..sha1..e
-00000960: 6e63 6f64 65da 0664 6967 6573 74da 0662  ncode..digest..b
-00000970: 6173 6536 34da 1175 726c 7361 6665 5f62  ase64..urlsafe_b
-00000980: 3634 656e 636f 6465 da06 6465 636f 6465  64encode..decode
-00000990: 2902 7233 0000 0072 4700 0000 720d 0000  ).r3...rG...r...
-000009a0: 0072 0d00 0000 7210 0000 00da 0a73 686f  .r....r......sho
-000009b0: 7274 5f68 6173 6843 0000 0073 0400 0000  rt_hashC...s....
-000009c0: 0002 1402 724b 0000 0029 02da 0576 616c  ....rK...)...val
-000009d0: 7565 7227 0000 0063 0100 0000 0000 0000  uer'...c........
-000009e0: 0000 0000 0100 0000 0100 0000 c300 0000  ................
-000009f0: 7304 0000 007c 0053 0072 0b00 0000 720d  s....|.S.r....r.
-00000a00: 0000 0029 0172 4c00 0000 720d 0000 0072  ...).rL...r....r
-00000a10: 0d00 0000 7210 0000 00da 0c74 6f5f 6177  ....r......to_aw
-00000a20: 6169 7461 626c 654a 0000 0073 0200 0000  aitableJ...s....
-00000a30: 0001 724d 0000 0063 0000 0000 0000 0000  ..rM...c........
-00000a40: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000a50: 733e 0000 0065 005a 0164 005a 0264 015a  s>...e.Z.d.Z.d.Z
-00000a60: 0364 025a 0465 0564 0364 0484 0083 015a  .d.Z.e.d.d.....Z
-00000a70: 0665 0564 0564 0684 0083 015a 0765 0565  .e.d.d.....Z.e.e
-00000a80: 0864 079c 0164 0864 0984 0483 015a 0964  .d...d.d.....Z.d
-00000a90: 0a53 0029 0b72 1800 0000 7a1f 6120 7461  .S.).r....z.a ta
-00000aa0: 6720 746f 206a 6f69 6e20 7374 7269 6e67  g to join string
-00000ab0: 7320 696e 2061 206c 6973 747a 0521 6a6f  s in a listz.!jo
-00000ac0: 696e 6303 0000 0000 0000 0000 0000 0004  inc.............
-00000ad0: 0000 0004 0000 0043 0000 0073 1e00 0000  .......C...s....
-00000ae0: 7c01 a000 7c02 a101 7d03 6401 a001 6402  |...|...}.d...d.
-00000af0: 6403 8400 7c03 4400 8301 a101 5300 2904  d...|.D.....S.).
-00000b00: 4eda 0063 0100 0000 0000 0000 0000 0000  N..c............
-00000b10: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-00000b20: 0067 007c 005d 0c7d 0174 007c 0183 0191  .g.|.].}.t.|....
-00000b30: 0271 0453 0072 0d00 0000 2901 da03 7374  .q.S.r....)...st
-00000b40: 7272 3a00 0000 720d 0000 0072 0d00 0000  rr:...r....r....
-00000b50: 7210 0000 0072 3100 0000 5600 0000 7212  r....r1...V...r.
-00000b60: 0000 007a 254a 6f69 6e54 6167 2e66 726f  ...z%JoinTag.fro
-00000b70: 6d5f 7961 6d6c 2e3c 6c6f 6361 6c73 3e2e  m_yaml.<locals>.
-00000b80: 3c6c 6973 7463 6f6d 703e 2902 da12 636f  <listcomp>)...co
-00000b90: 6e73 7472 7563 745f 7365 7175 656e 6365  nstruct_sequence
-00000ba0: da04 6a6f 696e 2904 da03 636c 73da 0b63  ..join)...cls..c
-00000bb0: 6f6e 7374 7275 6374 6f72 da04 6e6f 6465  onstructor..node
-00000bc0: da03 7365 7172 0d00 0000 720d 0000 0072  ..seqr....r....r
-00000bd0: 1000 0000 da09 6672 6f6d 5f79 616d 6c53  ......from_yamlS
-00000be0: 0000 0073 0400 0000 0002 0a01 7a11 4a6f  ...s........z.Jo
-00000bf0: 696e 5461 672e 6672 6f6d 5f79 616d 6c63  inTag.from_yamlc
-00000c00: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000c10: 0400 0000 4300 0000 730e 0000 007c 01a0  ....C...s....|..
-00000c20: 007c 006a 017c 02a1 0253 0072 0b00 0000  .|.j.|...S.r....
-00000c30: a902 da12 7265 7072 6573 656e 745f 7365  ....represent_se
-00000c40: 7175 656e 6365 da08 7961 6d6c 5f74 6167  quence..yaml_tag
-00000c50: a903 7252 0000 00da 0664 756d 7065 72da  ..rR.....dumper.
-00000c60: 0464 6174 6172 0d00 0000 720d 0000 0072  .datar....r....r
-00000c70: 1000 0000 da07 746f 5f79 616d 6c58 0000  ......to_yamlX..
-00000c80: 0073 0200 0000 0003 7a0f 4a6f 696e 5461  .s......z.JoinTa
-00000c90: 672e 746f 5f79 616d 6ca9 0172 1c00 0000  g.to_yaml..r....
-00000ca0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000cb0: 0003 0000 0043 0000 0073 0e00 0000 7c01  .....C...s....|.
-00000cc0: a000 7c00 a101 0100 6400 5300 720b 0000  ..|.....d.S.r...
-00000cd0: 00a9 015a 0e72 6567 6973 7465 725f 636c  ...Z.register_cl
-00000ce0: 6173 73a9 0272 5200 0000 721c 0000 0072  ass..rR...r....r
-00000cf0: 0d00 0000 720d 0000 0072 1000 0000 7219  ....r....r....r.
-00000d00: 0000 005d 0000 0073 0200 0000 0002 7a10  ...]...s......z.
-00000d10: 4a6f 696e 5461 672e 7265 6769 7374 6572  JoinTag.register
-00000d20: 4ea9 0ada 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
-00000d30: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000d40: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00000d50: 7259 0000 00da 0b63 6c61 7373 6d65 7468  rY.....classmeth
-00000d60: 6f64 7256 0000 0072 5d00 0000 7202 0000  odrV...r]...r...
-00000d70: 0072 1900 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000d80: 720d 0000 0072 1000 0000 7218 0000 004e  r....r....r....N
-00000d90: 0000 0073 1000 0000 0801 0402 0402 0201  ...s............
-00000da0: 0a04 0201 0a04 0201 7218 0000 0063 0000  ........r....c..
-00000db0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000dc0: 0000 4000 0000 733e 0000 0065 005a 0164  ..@...s>...e.Z.d
-00000dd0: 005a 0264 015a 0364 025a 0465 0564 0364  .Z.d.Z.d.Z.e.d.d
-00000de0: 0484 0083 015a 0665 0564 0564 0684 0083  .....Z.e.d.d....
-00000df0: 015a 0765 0565 0864 079c 0164 0864 0984  .Z.e.e.d...d.d..
-00000e00: 0483 015a 0964 0a53 0029 0b72 1a00 0000  ...Z.d.S.).r....
-00000e10: 7a1e 6120 7461 6720 746f 2072 6561 6420  z.a tag to read 
-00000e20: 7374 7269 6e67 2066 726f 6d20 6669 6c65  string from file
-00000e30: 7a05 2172 6561 6463 0300 0000 0000 0000  z.!readc........
-00000e40: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
-00000e50: 734c 0000 007c 01a0 007c 02a1 017d 0374  sL...|...|...}.t
-00000e60: 016a 026a 037c 038e 007d 0474 047c 0464  .j.j.|...}.t.|.d
-00000e70: 0183 028f 187d 057c 05a0 05a1 0057 0002  .....}.|.....W..
-00000e80: 0064 0004 0004 0083 0301 0053 0031 0073  .d.........S.1.s
-00000e90: 3e30 0001 0001 0001 0059 0001 0064 0053  >0.......Y...d.S
-00000ea0: 0029 024e da01 7229 0672 5000 0000 7235  .).N..r).rP...r5
-00000eb0: 0000 0072 1500 0000 7251 0000 00da 046f  ...r....rQ.....o
-00000ec0: 7065 6eda 0472 6561 6429 0672 5200 0000  pen..read).rR...
-00000ed0: 7253 0000 0072 5400 0000 7255 0000 0072  rS...rT...rU...r
-00000ee0: 1500 0000 da01 6672 0d00 0000 720d 0000  ......fr....r...
-00000ef0: 0072 1000 0000 7256 0000 0067 0000 0073  .r....rV...g...s
-00000f00: 0800 0000 0002 0a01 0c01 0c01 7a11 5265  ............z.Re
-00000f10: 6164 5461 672e 6672 6f6d 5f79 616d 6c63  adTag.from_yamlc
-00000f20: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000f30: 0400 0000 4300 0000 730e 0000 007c 01a0  ....C...s....|..
-00000f40: 007c 006a 017c 02a1 0253 0072 0b00 0000  .|.j.|...S.r....
-00000f50: 7257 0000 0072 5a00 0000 720d 0000 0072  rW...rZ...r....r
-00000f60: 0d00 0000 7210 0000 0072 5d00 0000 6e00  ....r....r]...n.
-00000f70: 0000 7302 0000 0000 037a 0f52 6561 6454  ..s......z.ReadT
-00000f80: 6167 2e74 6f5f 7961 6d6c 725e 0000 0063  ag.to_yamlr^...c
-00000f90: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000fa0: 0300 0000 4300 0000 730e 0000 007c 01a0  ....C...s....|..
-00000fb0: 007c 00a1 0101 0064 0053 0072 0b00 0000  .|.....d.S.r....
-00000fc0: 725f 0000 0072 6000 0000 720d 0000 0072  r_...r`...r....r
-00000fd0: 0d00 0000 7210 0000 0072 1900 0000 7300  ....r....r....s.
-00000fe0: 0000 7302 0000 0000 027a 1052 6561 6454  ..s......z.ReadT
-00000ff0: 6167 2e72 6567 6973 7465 724e 7261 0000  ag.registerNra..
-00001000: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00001010: 7210 0000 0072 1a00 0000 6200 0000 7310  r....r....b...s.
-00001020: 0000 0008 0104 0204 0202 010a 0602 010a  ................
-00001030: 0402 0172 1a00 0000 6300 0000 0000 0000  ...r....c.......
-00001040: 0000 0000 0003 0000 0006 0000 0003 0000  ................
-00001050: 0073 7400 0000 6411 7400 7400 6402 9c02  .st...d.t.t.d...
-00001060: 8702 6601 6403 6404 840d 8902 7401 6601  ..f.d.d.....t.f.
-00001070: 7400 7402 7403 1900 6405 9c02 6406 6407  t.t.t...d...d.d.
-00001080: 8405 7d00 7400 7402 7403 1900 6405 9c02  ..}.t.t.t...d...
-00001090: 6408 6409 8404 7d01 640a 640b 8400 8900  d.d...}.d.d.....
-000010a0: 6412 640c 640d 8401 8901 6413 8700 8701  d.d.d.....d.....
-000010b0: 6602 640f 6410 8409 7d02 8802 7c00 7c01  f.d.d...}...|.|.
-000010c0: 8800 8801 7c02 6606 5300 2914 7a44 636c  ....|.f.S.).zDcl
-000010d0: 6f75 6470 6963 6b6c 6520 636f 6d70 6174  oudpickle compat
-000010e0: 6962 6c65 3a20 6874 7470 733a 2f2f 7374  ible: https://st
-000010f0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
-00001100: 7175 6573 7469 6f6e 732f 3735 3239 3237  questions/752927
-00001110: 3639 4e29 02da 026c 6fda 0272 6f63 0300  69N)...lo..roc..
-00001120: 0000 0000 0000 0000 0000 0600 0000 0500  ................
-00001130: 0000 1300 0000 7386 0000 007c 0264 0175  ......s....|.d.u
-00001140: 0072 0c67 007d 027c 01a0 00a1 0044 005d  .r.g.}.|.....D.]
-00001150: 6c5c 027d 037d 047c 037c 0076 0072 787c  l\.}.}.|.|.v.rx|
-00001160: 0274 017c 0383 0167 0117 007d 0574 027c  .t.|...g...}.t.|
-00001170: 007c 0319 0074 0383 0272 5c74 027c 0474  .|...t...r\t.|.t
-00001180: 0383 0272 5c88 007c 007c 0319 007c 047c  ...r\..|.|...|.|
-00001190: 0583 0301 0071 8074 0464 02a0 057c 05a1  .....q.t.d...|..
-000011a0: 0164 0317 0083 0101 007c 047c 007c 033c  .d.......|.|.|.<
-000011b0: 0071 147c 047c 007c 033c 0071 147c 0053  .q.|.|.|.<.q.|.S
-000011c0: 0029 047a 7a0a 2020 2020 2020 2020 4d65  .).zz.        Me
-000011d0: 7267 6520 7477 6f20 6469 6374 2c20 7468  rge two dict, th
-000011e0: 6520 6c65 6674 2064 6963 7420 7769 6c6c  e left dict will
-000011f0: 2062 6520 6f76 6572 7269 6464 656e 2e0a   be overridden..
-00001200: 2020 2020 2020 2020 4e6f 7465 3a20 6c69          Note: li
-00001210: 7374 2077 696c 6c20 6265 2072 6570 6c61  st will be repla
-00001220: 6365 6420 696e 7374 6561 6420 6f66 206d  ced instead of m
-00001230: 6572 6765 642e 0a20 2020 2020 2020 204e  erged..        N
-00001240: da01 2e7a 1420 6861 7320 6265 656e 206f  ...z. has been o
-00001250: 7665 7272 6964 6465 6e29 06da 0569 7465  verridden)...ite
-00001260: 6d73 724f 0000 00da 0a69 7369 6e73 7461  msrO.....isinsta
-00001270: 6e63 65da 0464 6963 7472 1f00 0000 7251  nce..dictr....rQ
-00001280: 0000 0029 0672 6b00 0000 726c 0000 0072  ...).rk...rl...r
-00001290: 1500 0000 da03 6b65 7972 4c00 0000 da0c  ......keyrL.....
-000012a0: 6375 7272 656e 745f 7061 7468 2901 7220  current_path).r 
-000012b0: 0000 0072 0d00 0000 7210 0000 0072 2000  ...r....r....r .
-000012c0: 0000 7b00 0000 7316 0000 0000 0508 0104  ..{...s.........
-000012d0: 0110 0108 010e 0118 0112 0212 010a 020a  ................
-000012e0: 017a 2d5f 5f65 7870 6f72 745f 7265 6d6f  .z-__export_remo
-000012f0: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
-00001300: 6361 6c73 3e2e 6d65 7267 655f 6469 6374  cals>.merge_dict
-00001310: 2902 7221 0000 00da 046b 6579 7363 0300  ).r!.....keysc..
-00001320: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00001330: 0000 5300 0000 732e 0000 007c 0144 005d  ..S...s....|.D.]
-00001340: 247d 037c 037c 0076 0172 207c 0274 0075  $}.|.|.v.r |.t.u
-00001350: 0172 207c 0202 0001 0053 007c 007c 0319  .r |.....S.|.|..
-00001360: 007d 0071 047c 0053 0029 017a 1a67 6574  .}.q.|.S.).z.get
-00001370: 2076 616c 7565 2066 726f 6d20 6e65 7374   value from nest
-00001380: 6564 2064 6963 7429 01da 0545 4d50 5459  ed dict)...EMPTY
-00001390: 2904 7221 0000 0072 7300 0000 da07 6465  ).r!...rs.....de
-000013a0: 6661 756c 7472 7100 0000 720d 0000 0072  faultrq...r....r
-000013b0: 0d00 0000 7210 0000 00da 0f64 6963 745f  ....r......dict_
-000013c0: 6e65 7374 6564 5f67 6574 8e00 0000 730a  nested_get....s.
-000013d0: 0000 0000 0208 0110 0108 010a 017a 325f  .............z2_
-000013e0: 5f65 7870 6f72 745f 7265 6d6f 7465 5f66  _export_remote_f
-000013f0: 756e 6374 696f 6e73 2e3c 6c6f 6361 6c73  unctions.<locals
-00001400: 3e2e 6469 6374 5f6e 6573 7465 645f 6765  >.dict_nested_ge
-00001410: 7463 0300 0000 0000 0000 0000 0000 0400  tc..............
-00001420: 0000 0400 0000 5300 0000 732a 0000 007c  ......S...s*...|
-00001430: 0164 0164 0285 0219 0044 005d 0c7d 037c  .d.d.....D.].}.|
-00001440: 007c 0319 007d 0071 0c7c 027c 007c 0164  .|...}.q.|.|.|.d
-00001450: 0219 003c 0064 0153 0029 037a 1873 6574  ...<.d.S.).z.set
-00001460: 2076 616c 7565 2074 6f20 6e65 7374 6564   value to nested
-00001470: 2064 6963 744e e9ff ffff ff72 0d00 0000   dictN.....r....
-00001480: 2904 7221 0000 0072 7300 0000 724c 0000  ).r!...rs...rL..
-00001490: 0072 7100 0000 720d 0000 0072 0d00 0000  .rq...r....r....
-000014a0: 7210 0000 00da 0f64 6963 745f 6e65 7374  r......dict_nest
-000014b0: 6564 5f73 6574 9600 0000 7306 0000 0000  ed_set....s.....
-000014c0: 0210 010a 017a 325f 5f65 7870 6f72 745f  .....z2__export_
-000014d0: 7265 6d6f 7465 5f66 756e 6374 696f 6e73  remote_functions
-000014e0: 2e3c 6c6f 6361 6c73 3e2e 6469 6374 5f6e  .<locals>.dict_n
-000014f0: 6573 7465 645f 7365 7463 0200 0000 0000  ested_setc......
-00001500: 0000 0000 0000 0200 0000 0300 0000 1300  ................
-00001510: 0000 733c 0000 007c 0164 016b 0173 147c  ..s<...|.d.k.s.|
-00001520: 0174 0088 0183 016b 0472 1888 0153 0074  .t.....k.r...S.t
-00001530: 0088 0183 017c 011b 0089 0087 0087 0166  .....|.........f
-00001540: 0264 0264 0384 0874 017c 0183 0144 0083  .d.d...t.|...D..
-00001550: 0153 0029 044e 7201 0000 0063 0100 0000  .S.).Nr....c....
-00001560: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00001570: 1300 0000 731c 0000 0067 007c 005d 147d  ....s....g.|.].}
-00001580: 0188 0174 007c 0188 0014 0083 0119 0091  ...t.|..........
-00001590: 0271 0453 0072 0d00 0000 2901 da03 696e  .q.S.r....)...in
-000015a0: 7472 3a00 0000 a902 da08 696e 7465 7276  tr:.......interv
-000015b0: 616c 7226 0000 0072 0d00 0000 7210 0000  alr&...r....r...
-000015c0: 0072 3100 0000 a100 0000 7212 0000 007a  .r1.......r....z
-000015d0: 475f 5f65 7870 6f72 745f 7265 6d6f 7465  G__export_remote
-000015e0: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
-000015f0: 6c73 3e2e 6c69 7374 5f65 7665 6e5f 7361  ls>.list_even_sa
-00001600: 6d70 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c  mple.<locals>.<l
-00001610: 6973 7463 6f6d 703e 2902 7240 0000 0072  istcomp>).r@...r
-00001620: 4100 0000 2902 7226 0000 00da 0473 697a  A...).r&.....siz
-00001630: 6572 0d00 0000 727a 0000 0072 1000 0000  er....rz...r....
-00001640: da10 6c69 7374 5f65 7665 6e5f 7361 6d70  ..list_even_samp
-00001650: 6c65 9c00 0000 7308 0000 0000 0114 0104  le....s.........
-00001660: 020c 017a 335f 5f65 7870 6f72 745f 7265  ...z3__export_re
-00001670: 6d6f 7465 5f66 756e 6374 696f 6e73 2e3c  mote_functions.<
-00001680: 6c6f 6361 6c73 3e2e 6c69 7374 5f65 7665  locals>.list_eve
-00001690: 6e5f 7361 6d70 6c65 6303 0000 0000 0000  n_samplec.......
-000016a0: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
-000016b0: 0073 2600 0000 7c02 6400 7500 7210 7400  .s&...|.d.u.r.t.
-000016c0: 7c00 8301 7d02 7401 a002 7c02 a101 0100  |...}.t...|.....
-000016d0: 7401 a003 7c00 7c01 a102 5300 720b 0000  t...|.|...S.r...
-000016e0: 0029 0472 4000 0000 da06 7261 6e64 6f6d  .).r@.....random
-000016f0: da04 7365 6564 da06 7361 6d70 6c65 2903  ..seed..sample).
-00001700: 7226 0000 0072 7c00 0000 727f 0000 0072  r&...r|...r....r
-00001710: 0d00 0000 720d 0000 0072 1000 0000 da12  ....r....r......
-00001720: 6c69 7374 5f72 616e 646f 6d5f 7361 6d70  list_random_samp
-00001730: 6c65 a300 0000 7308 0000 0000 0108 0108  le....s.........
-00001740: 010a 017a 355f 5f65 7870 6f72 745f 7265  ...z5__export_re
-00001750: 6d6f 7465 5f66 756e 6374 696f 6e73 2e3c  mote_functions.<
-00001760: 6c6f 6361 6c73 3e2e 6c69 7374 5f72 616e  locals>.list_ran
-00001770: 646f 6d5f 7361 6d70 6c65 da04 6576 656e  dom_sample..even
-00001780: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00001790: 0004 0000 001b 0000 0073 5200 0000 7c02  .........sR...|.
-000017a0: 6401 6b02 7212 8800 7c00 7c01 8302 5300  d.k.r...|.|...S.
-000017b0: 7c02 6402 6b02 722c 8801 7c00 7c01 6602  |.d.k.r,..|.|.f.
-000017c0: 6900 7c03 a401 8e01 5300 7c02 6403 6b02  i.|.....S.|.d.k.
-000017d0: 7240 7c00 6400 7c01 8502 1900 5300 7400  r@|.d.|.....S.t.
-000017e0: 6404 7c02 9b00 9d02 8301 8201 6400 5300  d.|.........d.S.
-000017f0: 2905 4e72 8200 0000 727e 0000 00da 0874  ).Nr....r~.....t
-00001800: 7275 6e63 6174 657a 1655 6e6b 6e6f 776e  runcatez.Unknown
-00001810: 2073 616d 706c 6520 6d65 7468 6f64 2029   sample method )
-00001820: 01da 0a56 616c 7565 4572 726f 7229 0472  ...ValueError).r
-00001830: 2600 0000 727c 0000 00da 066d 6574 686f  &...r|.....metho
-00001840: 64da 066b 7761 7267 7329 0272 7d00 0000  d..kwargs).r}...
-00001850: 7281 0000 0072 0d00 0000 7210 0000 00da  r....r....r.....
-00001860: 0b6c 6973 745f 7361 6d70 6c65 a900 0000  .list_sample....
-00001870: 730e 0000 0000 0108 010a 0108 0112 0108  s...............
-00001880: 010c 027a 2e5f 5f65 7870 6f72 745f 7265  ...z.__export_re
-00001890: 6d6f 7465 5f66 756e 6374 696f 6e73 2e3c  mote_functions.<
-000018a0: 6c6f 6361 6c73 3e2e 6c69 7374 5f73 616d  locals>.list_sam
-000018b0: 706c 6529 014e 2901 4e29 0172 8200 0000  ple).N).N).r....
-000018c0: 2904 7270 0000 0072 7400 0000 7205 0000  ).rp...rt...r...
-000018d0: 0072 4f00 0000 2903 7276 0000 0072 7800  .rO...).rv...rx.
-000018e0: 0000 7287 0000 0072 0d00 0000 2903 727d  ..r....r....).r}
-000018f0: 0000 0072 8100 0000 7220 0000 0072 1000  ...r....r ...r..
-00001900: 0000 da19 5f5f 6578 706f 7274 5f72 656d  ....__export_rem
-00001910: 6f74 655f 6675 6e63 7469 6f6e 7378 0000  ote_functionsx..
-00001920: 0073 1a00 0000 0003 1613 1808 1406 0807  .s..............
-00001930: 0a06 100c 0201 0201 0201 0201 0201 02fa  ................
-00001940: 7288 0000 0029 2c5a 0b72 7561 6d65 6c2e  r....),Z.ruamel.
-00001950: 7961 6d6c 7202 0000 00da 0770 6174 686c  yamlr......pathl
-00001960: 6962 7203 0000 00da 0674 7970 696e 6772  ibr......typingr
-00001970: 0400 0000 7205 0000 0072 0600 0000 da0b  ....r....r......
-00001980: 6461 7461 636c 6173 7365 7372 0800 0000  dataclassesr....
-00001990: 7223 0000 0072 4400 0000 7248 0000 0072  r#...rD...rH...r
-000019a0: 0c00 0000 7235 0000 0072 7e00 0000 da03  ....r5...r~.....
-000019b0: 6c6f 6772 0a00 0000 7262 0000 00da 066c  logr....rb.....l
-000019c0: 6f67 6765 72da 066f 626a 6563 7472 7400  ogger..objectrt.
-000019d0: 0000 7214 0000 0072 1d00 0000 7222 0000  ..r....r....r"..
-000019e0: 0072 2500 0000 724f 0000 0072 2c00 0000  .r%...rO...r,...
-000019f0: 722d 0000 0072 3200 0000 7237 0000 0072  r-...r2...r7...r
-00001a00: 7900 0000 7242 0000 0072 4b00 0000 724d  y...rB...rK...rM
-00001a10: 0000 0072 1800 0000 721a 0000 0072 8800  ...r....r....r..
-00001a20: 0000 7220 0000 0072 7600 0000 7278 0000  ..r ...rv...rx..
-00001a30: 0072 7d00 0000 7281 0000 0072 8700 0000  .r}...r....r....
-00001a40: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00001a50: 1000 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00001a60: 0000 7346 0000 000c 010c 0114 010c 0208  ..sF............
-00001a70: 0108 0108 0108 0108 0108 020c 0208 0206  ................
-00001a80: 0308 040e 0712 0808 0518 0508 031c 0410  ................
-00001a90: 041e 0710 0710 040e 140e 1608 4d04 f902  ............M...
-00001aa0: 0102 0102 0102 0102 0102 0102 fa         .............
+00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6406 6c0c 5a0c 6400 6406 6c0d  ..d.d.l.Z.d.d.l.
+00000080: 5a0d 6400 6406 6c0e 5a0e 6400 6406 6c0f  Z.d.d.l.Z.d.d.l.
+00000090: 5a0f 6400 6406 6c10 5a10 6400 6406 6c11  Z.d.d.l.Z.d.d.l.
+000000a0: 5a11 6400 6406 6c12 5a12 6407 6408 6c13  Z.d.d.l.Z.d.d.l.
+000000b0: 6d14 5a14 0100 6514 6515 8301 5a16 6517  m.Z...e.e...Z.e.
+000000c0: 8300 5a18 6409 640a 8400 5a19 6503 640b  ..Z.d.d...Z.e.d.
+000000d0: 9c01 640c 640d 8404 5a1a 6505 6503 1900  ..d.d...Z.e.e...
+000000e0: 640e 9c01 640f 6410 8404 5a1b 6411 6412  d...d.d...Z.d.d.
+000000f0: 8400 5a1c 6506 651d 1900 6506 651d 1900  ..Z.e.e...e.e...
+00000100: 6413 9c02 6414 6415 8404 5a1e 6507 6416  d...d.d...Z.e.d.
+00000110: 8301 5a1f 6506 6506 651f 1900 1900 6506  ..Z.e.e.e.....e.
+00000120: 651f 1900 6413 9c02 6417 6418 8404 5a20  e...d...d.d...Z 
+00000130: 651d 651d 6419 9c02 641a 641b 8404 5a21  e.e.d...d.d...Z!
+00000140: 6506 651f 1900 6522 6506 6506 651f 1900  e.e...e"e.e.e...
+00000150: 1900 641c 9c03 641d 641e 8404 5a23 651d  ..d...d.d...Z#e.
+00000160: 651d 6419 9c02 641f 6420 8404 5a24 651f  e.d...d.d ..Z$e.
+00000170: 651f 6421 9c02 6422 6423 8404 5a25 4700  e.d!..d"d#..Z%G.
+00000180: 6424 6425 8400 6425 8302 5a26 4700 6426  d$d%..d%..Z&G.d&
+00000190: 6427 8400 6427 8302 5a27 6428 6429 8400  d'..d'..Z'd(d)..
+000001a0: 5a28 6528 8300 5c09 5a29 5a2a 5a2b 5a2c  Z(e(..\.Z)Z*Z+Z,
+000001b0: 5a2d 5a2e 5a2f 5a30 5a31 6406 5300 292a  Z-Z.Z/Z0Z1d.S.)*
+000001c0: e900 0000 0029 01da 0459 414d 4c29 01da  .....)...YAML)..
+000001d0: 0450 6174 6829 03da 0554 7570 6c65 da04  .Path)...Tuple..
+000001e0: 4c69 7374 da07 5479 7065 5661 72a9 01da  List..TypeVar...
+000001f0: 0566 6965 6c64 a901 da0b 7a69 705f 6c6f  .field....zip_lo
+00000200: 6e67 6573 744e e901 0000 0029 01da 0a67  ngestN.....)...g
+00000210: 6574 5f6c 6f67 6765 7263 0100 0000 0000  et_loggerc......
+00000220: 0000 0000 0000 0100 0000 0400 0000 0300  ................
+00000230: 0000 7312 0000 0074 0087 0066 0164 0164  ..s....t...f.d.d
+00000240: 0284 0864 038d 0153 0029 044e 6300 0000  ...d...S.).Nc...
+00000250: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000260: 0013 0000 0073 0a00 0000 7400 a000 8800  .....s....t.....
+00000270: a101 5300 a901 4e29 01da 0463 6f70 79a9  ..S...N)...copy.
+00000280: 00a9 01da 036f 626a 720f 0000 00fa 2c2f  .....objr.....,/
+00000290: 686f 6d65 2f68 656e 7279 2f73 7263 2f61  home/henry/src/a
+000002a0: 6932 2d6b 6974 2f61 6932 5f6b 6974 2f63  i2-kit/ai2_kit/c
+000002b0: 6f72 652f 7574 696c 2e70 79da 083c 6c61  ore/util.py..<la
+000002c0: 6d62 6461 3e17 0000 00f3 0000 0000 7a27  mbda>.........z'
+000002d0: 6465 6661 756c 745f 6d75 7461 626c 655f  default_mutable_
+000002e0: 6669 656c 642e 3c6c 6f63 616c 733e 2e3c  field.<locals>.<
+000002f0: 6c61 6d62 6461 3e29 01da 0f64 6566 6175  lambda>)...defau
+00000300: 6c74 5f66 6163 746f 7279 7207 0000 0072  lt_factoryr....r
+00000310: 1000 0000 720f 0000 0072 1000 0000 7212  ....r....r....r.
+00000320: 0000 00da 1564 6566 6175 6c74 5f6d 7574  .....default_mut
+00000330: 6162 6c65 5f66 6965 6c64 1600 0000 7302  able_field....s.
+00000340: 0000 0000 0172 1600 0000 2901 da04 7061  .....r....)...pa
+00000350: 7468 6301 0000 0000 0000 0000 0000 0002  thc.............
+00000360: 0000 0003 0000 0043 0000 0073 2800 0000  .......C...s(...
+00000370: 7400 6401 6402 8d01 7d01 7401 a002 7c01  t.d.d...}.t...|.
+00000380: a101 0100 7403 a002 7c01 a101 0100 7c01  ....t...|.....|.
+00000390: a004 7c00 a101 5300 2903 4eda 0473 6166  ..|...S.).N..saf
+000003a0: 6529 01da 0374 7970 2905 7202 0000 00da  e)...typ).r.....
+000003b0: 074a 6f69 6e54 6167 da08 7265 6769 7374  .JoinTag..regist
+000003c0: 6572 da07 5265 6164 5461 67da 046c 6f61  er..ReadTag..loa
+000003d0: 6429 0272 1700 0000 da04 7961 6d6c 720f  d).r......yamlr.
+000003e0: 0000 0072 0f00 0000 7212 0000 00da 0e6c  ...r....r......l
+000003f0: 6f61 645f 7961 6d6c 5f66 696c 651a 0000  oad_yaml_file...
+00000400: 0073 0800 0000 0001 0a01 0a01 0a01 721f  .s............r.
+00000410: 0000 0029 01da 0570 6174 6873 6300 0000  ...)...pathsc...
+00000420: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+00000430: 0047 0000 0073 2e00 0000 6900 7d01 7c00  .G...s....i.}.|.
+00000440: 4400 5d20 7d02 7400 6401 7c02 8302 0100  D.] }.t.d.|.....
+00000450: 7401 7c01 7402 7403 7c02 8301 8301 8302  t.|.t.t.|.......
+00000460: 7d01 7108 7c01 5300 2902 4e7a 106c 6f61  }.q.|.S.).Nz.loa
+00000470: 6420 7961 6d6c 2066 696c 653a 2029 04da  d yaml file: )..
+00000480: 0570 7269 6e74 da0a 6d65 7267 655f 6469  .print..merge_di
+00000490: 6374 721f 0000 0072 0300 0000 2903 7220  ctr....r....).r 
+000004a0: 0000 00da 0164 7217 0000 0072 0f00 0000  .....dr....r....
+000004b0: 720f 0000 0072 1200 0000 da0f 6c6f 6164  r....r......load
+000004c0: 5f79 616d 6c5f 6669 6c65 7321 0000 0073  _yaml_files!...s
+000004d0: 0a00 0000 0001 0401 0801 0a01 1401 7224  ..............r$
+000004e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000004f0: 0000 0000 0200 0000 4300 0000 7308 0000  ........C...s...
+00000500: 0074 00a0 01a1 0053 0029 017a 0a73 686f  .t.....S.).z.sho
+00000510: 7274 2075 7569 6429 02da 0973 686f 7274  rt uuid)...short
+00000520: 7575 6964 da04 7575 6964 720f 0000 0072  uuid..uuidr....r
+00000530: 0f00 0000 720f 0000 0072 1200 0000 da06  ....r....r......
+00000540: 735f 7575 6964 2900 0000 7302 0000 0000  s_uuid)...s.....
+00000550: 0272 2700 0000 2902 da01 6cda 0672 6574  .r'...)...l..ret
+00000560: 7572 6e63 0100 0000 0000 0000 0000 0000  urnc............
+00000570: 0100 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+00000580: 0074 0074 0174 027c 0083 0183 0183 0153  .t.t.t.|.......S
+00000590: 0029 017a 1d72 656d 6f76 6520 6475 706c  .).z.remove dupl
+000005a0: 6963 6174 6520 7374 7220 616e 6420 736f  icate str and so
+000005b0: 7274 2903 da04 6c69 7374 da06 736f 7274  rt)...list..sort
+000005c0: 6564 da03 7365 74a9 0172 2800 0000 720f  ed..set..r(...r.
+000005d0: 0000 0072 0f00 0000 7212 0000 00da 1473  ...r....r......s
+000005e0: 6f72 745f 756e 6971 7565 5f73 7472 5f6c  ort_unique_str_l
+000005f0: 6973 742e 0000 0073 0200 0000 0002 722e  ist....s......r.
+00000600: 0000 00da 0154 6301 0000 0000 0000 0000  .....Tc.........
+00000610: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000620: 0e00 0000 6401 6402 8400 7c00 4400 8301  ....d.d...|.D...
+00000630: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000640: 0000 0300 0000 0400 0000 5300 0000 731a  ..........S...s.
+00000650: 0000 0067 007c 005d 127d 017c 0144 005d  ...g.|.].}.|.D.]
+00000660: 087d 027c 0291 0371 0c71 0453 0072 0f00  .}.|...q.q.S.r..
+00000670: 0000 720f 0000 0029 03da 022e 305a 0773  ..r....)....0Z.s
+00000680: 7562 6c69 7374 da04 6974 656d 720f 0000  ublist..itemr...
+00000690: 0072 0f00 0000 7212 0000 00da 0a3c 6c69  .r....r......<li
+000006a0: 7374 636f 6d70 3e37 0000 0072 1400 0000  stcomp>7...r....
+000006b0: 7a1b 666c 6174 7465 6e2e 3c6c 6f63 616c  z.flatten.<local
+000006c0: 733e 2e3c 6c69 7374 636f 6d70 3e72 0f00  s>.<listcomp>r..
+000006d0: 0000 722d 0000 0072 0f00 0000 720f 0000  ..r-...r....r...
+000006e0: 0072 1200 0000 da07 666c 6174 7465 6e36  .r......flatten6
+000006f0: 0000 0073 0200 0000 0001 7233 0000 0029  ...s......r3...)
+00000700: 02da 0173 7229 0000 0063 0100 0000 0000  ...sr)...c......
+00000710: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000720: 0000 7312 0000 007c 006a 0066 0069 0074  ..s....|.j.f.i.t
+00000730: 016a 02a4 018e 0153 0072 0d00 0000 2903  .j.....S.r....).
+00000740: da06 666f 726d 6174 da02 6f73 da07 656e  ..format..os..en
+00000750: 7669 726f 6e29 0172 3400 0000 720f 0000  viron).r4...r...
+00000760: 0072 0f00 0000 7212 0000 00da 1166 6f72  .r....r......for
+00000770: 6d61 745f 656e 765f 7374 7269 6e67 3a00  mat_env_string:.
+00000780: 0000 7302 0000 0000 0172 3800 0000 2903  ..s......r8...).
+00000790: 7228 0000 00da 016e 7229 0000 0063 0200  r(.....nr)...c..
+000007a0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000007b0: 0000 0300 0000 732c 0000 0074 0074 0188  ......s,...t.t..
+000007c0: 0183 017c 0183 025c 0289 0089 0287 0087  ...|...\........
+000007d0: 0187 0266 0364 0164 0284 0874 027c 0183  ...f.d.d...t.|..
+000007e0: 0144 0083 0153 0029 037a 1873 706c 6974  .D...S.).z.split
+000007f0: 206c 6973 7420 696e 746f 206e 2063 6875   list into n chu
+00000800: 6e6b 7363 0100 0000 0000 0000 0000 0000  nksc............
+00000810: 0200 0000 0800 0000 1300 0000 733c 0000  ............s<..
+00000820: 0067 007c 005d 347d 0188 017c 0188 0014  .g.|.]4}...|....
+00000830: 0074 007c 0188 0283 0217 007c 0164 0017  .t.|.......|.d..
+00000840: 0088 0014 0074 007c 0164 0017 0088 0283  .....t.|.d......
+00000850: 0217 0085 0219 0091 0271 0453 0029 0172  .........q.S.).r
+00000860: 0b00 0000 2901 da03 6d69 6ea9 0272 3000  ....)...min..r0.
+00000870: 0000 da01 69a9 03da 016b 7228 0000 00da  ....i....kr(....
+00000880: 016d 720f 0000 0072 1200 0000 7232 0000  .mr....r....r2..
+00000890: 0042 0000 0072 1400 0000 7a1e 6c69 7374  .B...r....z.list
+000008a0: 5f73 706c 6974 2e3c 6c6f 6361 6c73 3e2e  _split.<locals>.
+000008b0: 3c6c 6973 7463 6f6d 703e 2903 da06 6469  <listcomp>)...di
+000008c0: 766d 6f64 da03 6c65 6eda 0572 616e 6765  vmod..len..range
+000008d0: 2902 7228 0000 0072 3900 0000 720f 0000  ).r(...r9...r...
+000008e0: 0072 3d00 0000 7212 0000 00da 0a6c 6973  .r=...r......lis
+000008f0: 745f 7370 6c69 743e 0000 0073 0400 0000  t_split>...s....
+00000900: 0003 1201 7243 0000 0063 0100 0000 0000  ....rC...c......
+00000910: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+00000920: 0000 732c 0000 0074 00a0 017c 00a0 0264  ..s,...t...|...d
+00000930: 01a1 01a1 01a0 03a1 007d 0174 04a0 057c  .........}.t...|
+00000940: 01a1 01a0 0664 01a1 0164 0264 0385 0219  .....d...d.d....
+00000950: 0053 0029 047a 1173 686f 7274 2068 6173  .S.).z.short has
+00000960: 6820 7374 7269 6e67 fa05 7574 662d 384e  h string..utf-8N
+00000970: e9fe ffff ff29 07da 0768 6173 686c 6962  .....)...hashlib
+00000980: da04 7368 6131 da06 656e 636f 6465 da06  ..sha1..encode..
+00000990: 6469 6765 7374 da06 6261 7365 3634 da11  digest..base64..
+000009a0: 7572 6c73 6166 655f 6236 3465 6e63 6f64  urlsafe_b64encod
+000009b0: 65da 0664 6563 6f64 6529 0272 3400 0000  e..decode).r4...
+000009c0: 7249 0000 0072 0f00 0000 720f 0000 0072  rI...r....r....r
+000009d0: 1200 0000 da0a 7368 6f72 745f 6861 7368  ......short_hash
+000009e0: 4500 0000 7304 0000 0000 0214 0272 4d00  E...s........rM.
+000009f0: 0000 2902 da05 7661 6c75 6572 2900 0000  ..)...valuer)...
+00000a00: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000a10: 0001 0000 00c3 0000 0073 0400 0000 7c00  .........s....|.
+00000a20: 5300 720d 0000 0072 0f00 0000 2901 724e  S.r....r....).rN
+00000a30: 0000 0072 0f00 0000 720f 0000 0072 1200  ...r....r....r..
+00000a40: 0000 da0c 746f 5f61 7761 6974 6162 6c65  ....to_awaitable
+00000a50: 4c00 0000 7302 0000 0000 0172 4f00 0000  L...s......rO...
+00000a60: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000a70: 0004 0000 0040 0000 0073 3e00 0000 6500  .....@...s>...e.
+00000a80: 5a01 6400 5a02 6401 5a03 6402 5a04 6505  Z.d.Z.d.Z.d.Z.e.
+00000a90: 6403 6404 8400 8301 5a06 6505 6405 6406  d.d.....Z.e.d.d.
+00000aa0: 8400 8301 5a07 6505 6508 6407 9c01 6408  ....Z.e.e.d...d.
+00000ab0: 6409 8404 8301 5a09 640a 5300 290b 721a  d.....Z.d.S.).r.
+00000ac0: 0000 007a 1f61 2074 6167 2074 6f20 6a6f  ...z.a tag to jo
+00000ad0: 696e 2073 7472 696e 6773 2069 6e20 6120  in strings in a 
+00000ae0: 6c69 7374 7a05 216a 6f69 6e63 0300 0000  listz.!joinc....
+00000af0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000b00: 4300 0000 731e 0000 007c 01a0 007c 02a1  C...s....|...|..
+00000b10: 017d 0364 01a0 0164 0264 0384 007c 0344  .}.d...d.d...|.D
+00000b20: 0083 01a1 0153 0029 044e da00 6301 0000  .....S.).N..c...
+00000b30: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000b40: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
+00000b50: 7d01 7400 7c01 8301 9102 7104 5300 720f  }.t.|.....q.S.r.
+00000b60: 0000 0029 01da 0373 7472 723b 0000 0072  ...)...strr;...r
+00000b70: 0f00 0000 720f 0000 0072 1200 0000 7232  ....r....r....r2
+00000b80: 0000 0058 0000 0072 1400 0000 7a25 4a6f  ...X...r....z%Jo
+00000b90: 696e 5461 672e 6672 6f6d 5f79 616d 6c2e  inTag.from_yaml.
+00000ba0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00000bb0: 6d70 3e29 02da 1263 6f6e 7374 7275 6374  mp>)...construct
+00000bc0: 5f73 6571 7565 6e63 65da 046a 6f69 6e29  _sequence..join)
+00000bd0: 04da 0363 6c73 da0b 636f 6e73 7472 7563  ...cls..construc
+00000be0: 746f 72da 046e 6f64 65da 0373 6571 720f  tor..node..seqr.
+00000bf0: 0000 0072 0f00 0000 7212 0000 00da 0966  ...r....r......f
+00000c00: 726f 6d5f 7961 6d6c 5500 0000 7304 0000  rom_yamlU...s...
+00000c10: 0000 020a 017a 114a 6f69 6e54 6167 2e66  .....z.JoinTag.f
+00000c20: 726f 6d5f 7961 6d6c 6303 0000 0000 0000  rom_yamlc.......
+00000c30: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000c40: 0073 0e00 0000 7c01 a000 7c00 6a01 7c02  .s....|...|.j.|.
+00000c50: a102 5300 720d 0000 00a9 02da 1272 6570  ..S.r........rep
+00000c60: 7265 7365 6e74 5f73 6571 7565 6e63 65da  resent_sequence.
+00000c70: 0879 616d 6c5f 7461 67a9 0372 5400 0000  .yaml_tag..rT...
+00000c80: da06 6475 6d70 6572 da04 6461 7461 720f  ..dumper..datar.
+00000c90: 0000 0072 0f00 0000 7212 0000 00da 0774  ...r....r......t
+00000ca0: 6f5f 7961 6d6c 5a00 0000 7302 0000 0000  o_yamlZ...s.....
+00000cb0: 037a 0f4a 6f69 6e54 6167 2e74 6f5f 7961  .z.JoinTag.to_ya
+00000cc0: 6d6c a901 721e 0000 0063 0200 0000 0000  ml..r....c......
+00000cd0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000ce0: 0000 730e 0000 007c 01a0 007c 00a1 0101  ..s....|...|....
+00000cf0: 0064 0053 0072 0d00 0000 a901 5a0e 7265  .d.S.r......Z.re
+00000d00: 6769 7374 6572 5f63 6c61 7373 a902 7254  gister_class..rT
+00000d10: 0000 0072 1e00 0000 720f 0000 0072 0f00  ...r....r....r..
+00000d20: 0000 7212 0000 0072 1b00 0000 5f00 0000  ..r....r...._...
+00000d30: 7302 0000 0000 027a 104a 6f69 6e54 6167  s......z.JoinTag
+00000d40: 2e72 6567 6973 7465 724e a90a da08 5f5f  .registerN....__
+00000d50: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000d60: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000d70: da07 5f5f 646f 635f 5f72 5b00 0000 da0b  ..__doc__r[.....
+00000d80: 636c 6173 736d 6574 686f 6472 5800 0000  classmethodrX...
+00000d90: 725f 0000 0072 0200 0000 721b 0000 0072  r_...r....r....r
+00000da0: 0f00 0000 720f 0000 0072 0f00 0000 7212  ....r....r....r.
+00000db0: 0000 0072 1a00 0000 5000 0000 7310 0000  ...r....P...s...
+00000dc0: 0008 0104 0204 0202 010a 0402 010a 0402  ................
+00000dd0: 0172 1a00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000de0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+00000df0: 3e00 0000 6500 5a01 6400 5a02 6401 5a03  >...e.Z.d.Z.d.Z.
+00000e00: 6402 5a04 6505 6403 6404 8400 8301 5a06  d.Z.e.d.d.....Z.
+00000e10: 6505 6405 6406 8400 8301 5a07 6505 6508  e.d.d.....Z.e.e.
+00000e20: 6407 9c01 6408 6409 8404 8301 5a09 640a  d...d.d.....Z.d.
+00000e30: 5300 290b 721c 0000 007a 1e61 2074 6167  S.).r....z.a tag
+00000e40: 2074 6f20 7265 6164 2073 7472 696e 6720   to read string 
+00000e50: 6672 6f6d 2066 696c 657a 0521 7265 6164  from filez.!read
+00000e60: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+00000e70: 0008 0000 0043 0000 0073 4c00 0000 7c01  .....C...sL...|.
+00000e80: a000 7c02 a101 7d03 7401 6a02 6a03 7c03  ..|...}.t.j.j.|.
+00000e90: 8e00 7d04 7404 7c04 6401 8302 8f18 7d05  ..}.t.|.d.....}.
+00000ea0: 7c05 a005 a100 5700 0200 6400 0400 0400  |.....W...d.....
+00000eb0: 8303 0100 5300 3100 733e 3000 0100 0100  ....S.1.s>0.....
+00000ec0: 0100 5900 0100 6400 5300 2902 4eda 0172  ..Y...d.S.).N..r
+00000ed0: 2906 7252 0000 0072 3600 0000 7217 0000  ).rR...r6...r...
+00000ee0: 0072 5300 0000 da04 6f70 656e da04 7265  .rS.....open..re
+00000ef0: 6164 2906 7254 0000 0072 5500 0000 7256  ad).rT...rU...rV
+00000f00: 0000 0072 5700 0000 7217 0000 00da 0166  ...rW...r......f
+00000f10: 720f 0000 0072 0f00 0000 7212 0000 0072  r....r....r....r
+00000f20: 5800 0000 6900 0000 7308 0000 0000 020a  X...i...s.......
+00000f30: 010c 010c 017a 1152 6561 6454 6167 2e66  .....z.ReadTag.f
+00000f40: 726f 6d5f 7961 6d6c 6303 0000 0000 0000  rom_yamlc.......
+00000f50: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000f60: 0073 0e00 0000 7c01 a000 7c00 6a01 7c02  .s....|...|.j.|.
+00000f70: a102 5300 720d 0000 0072 5900 0000 725c  ..S.r....rY...r\
+00000f80: 0000 0072 0f00 0000 720f 0000 0072 1200  ...r....r....r..
+00000f90: 0000 725f 0000 0070 0000 0073 0200 0000  ..r_...p...s....
+00000fa0: 0003 7a0f 5265 6164 5461 672e 746f 5f79  ..z.ReadTag.to_y
+00000fb0: 616d 6c72 6000 0000 6302 0000 0000 0000  amlr`...c.......
+00000fc0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000fd0: 0073 0e00 0000 7c01 a000 7c00 a101 0100  .s....|...|.....
+00000fe0: 6400 5300 720d 0000 0072 6100 0000 7262  d.S.r....ra...rb
+00000ff0: 0000 0072 0f00 0000 720f 0000 0072 1200  ...r....r....r..
+00001000: 0000 721b 0000 0075 0000 0073 0200 0000  ..r....u...s....
+00001010: 0002 7a10 5265 6164 5461 672e 7265 6769  ..z.ReadTag.regi
+00001020: 7374 6572 4e72 6300 0000 720f 0000 0072  sterNrc...r....r
+00001030: 0f00 0000 720f 0000 0072 1200 0000 721c  ....r....r....r.
+00001040: 0000 0064 0000 0073 1000 0000 0801 0402  ...d...s........
+00001050: 0402 0201 0a06 0201 0a04 0201 721c 0000  ............r...
+00001060: 0063 0000 0000 0000 0000 0000 0000 0600  .c..............
+00001070: 0000 0900 0000 0300 0000 739a 0000 0064  ..........s....d
+00001080: 1874 0074 0064 029c 0287 0266 0164 0364  .t.t.d.....f.d.d
+00001090: 0484 0d89 0274 0166 0174 0074 0274 0319  .....t.f.t.t.t..
+000010a0: 0064 059c 0264 0664 0784 057d 0074 0074  .d...d.d...}.t.t
+000010b0: 0274 0319 0064 059c 0264 0864 0984 047d  .t...d...d.d...}
+000010c0: 0164 0a64 0b84 0089 0064 1964 0c64 0d84  .d.d.....d.d.d..
+000010d0: 0189 0164 1a87 0087 0166 0264 0f64 1084  ...d.....f.d.d..
+000010e0: 097d 0264 1164 1284 007d 0374 0074 0364  .}.d.d...}.t.t.d
+000010f0: 139c 0264 1464 1584 047d 0464 1664 1784  ...d.d...}.d.d..
+00001100: 007d 0588 027c 007c 0188 0088 017c 027c  .}...|.|.....|.|
+00001110: 037c 047c 0566 0953 0029 1b7a 4463 6c6f  .|.|.f.S.).zDclo
+00001120: 7564 7069 636b 6c65 2063 6f6d 7061 7469  udpickle compati
+00001130: 626c 653a 2068 7474 7073 3a2f 2f73 7461  ble: https://sta
+00001140: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
+00001150: 7565 7374 696f 6e73 2f37 3532 3932 3736  uestions/7529276
+00001160: 394e 2902 da02 6c6f da02 726f 6303 0000  9N)...lo..roc...
+00001170: 0000 0000 0000 0000 0006 0000 0005 0000  ................
+00001180: 0013 0000 0073 8600 0000 7c02 6401 7500  .....s....|.d.u.
+00001190: 720c 6700 7d02 7c01 a000 a100 4400 5d6c  r.g.}.|.....D.]l
+000011a0: 5c02 7d03 7d04 7c03 7c00 7600 7278 7c02  \.}.}.|.|.v.rx|.
+000011b0: 7401 7c03 8301 6701 1700 7d05 7402 7c00  t.|...g...}.t.|.
+000011c0: 7c03 1900 7403 8302 725c 7402 7c04 7403  |...t...r\t.|.t.
+000011d0: 8302 725c 8800 7c00 7c03 1900 7c04 7c05  ..r\..|.|...|.|.
+000011e0: 8303 0100 7180 7404 6402 a005 7c05 a101  ....q.t.d...|...
+000011f0: 6403 1700 8301 0100 7c04 7c00 7c03 3c00  d.......|.|.|.<.
+00001200: 7114 7c04 7c00 7c03 3c00 7114 7c00 5300  q.|.|.|.<.q.|.S.
+00001210: 2904 7a7a 0a20 2020 2020 2020 204d 6572  ).zz.        Mer
+00001220: 6765 2074 776f 2064 6963 742c 2074 6865  ge two dict, the
+00001230: 206c 6566 7420 6469 6374 2077 696c 6c20   left dict will 
+00001240: 6265 206f 7665 7272 6964 6465 6e2e 0a20  be overridden.. 
+00001250: 2020 2020 2020 204e 6f74 653a 206c 6973         Note: lis
+00001260: 7420 7769 6c6c 2062 6520 7265 706c 6163  t will be replac
+00001270: 6564 2069 6e73 7465 6164 206f 6620 6d65  ed instead of me
+00001280: 7267 6564 2e0a 2020 2020 2020 2020 4eda  rged..        N.
+00001290: 012e 7a14 2068 6173 2062 6565 6e20 6f76  ..z. has been ov
+000012a0: 6572 7269 6464 656e 2906 da05 6974 656d  erridden)...item
+000012b0: 7372 5100 0000 da0a 6973 696e 7374 616e  srQ.....isinstan
+000012c0: 6365 da04 6469 6374 7221 0000 0072 5300  ce..dictr!...rS.
+000012d0: 0000 2906 726d 0000 0072 6e00 0000 7217  ..).rm...rn...r.
+000012e0: 0000 00da 036b 6579 724e 0000 005a 0c63  .....keyrN...Z.c
+000012f0: 7572 7265 6e74 5f70 6174 6829 0172 2200  urrent_path).r".
+00001300: 0000 720f 0000 0072 1200 0000 7222 0000  ..r....r....r"..
+00001310: 007d 0000 0073 1600 0000 0005 0801 0401  .}...s..........
+00001320: 1001 0801 0e01 1801 1202 1201 0a02 0a01  ................
+00001330: 7a2d 5f5f 6578 706f 7274 5f72 656d 6f74  z-__export_remot
+00001340: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
+00001350: 616c 733e 2e6d 6572 6765 5f64 6963 7429  als>.merge_dict)
+00001360: 0272 2300 0000 da04 6b65 7973 6303 0000  .r#.....keysc...
+00001370: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00001380: 0053 0000 0073 2e00 0000 7c01 4400 5d24  .S...s....|.D.]$
+00001390: 7d03 7c03 7c00 7601 7220 7c02 7400 7501  }.|.|.v.r |.t.u.
+000013a0: 7220 7c02 0200 0100 5300 7c00 7c03 1900  r |.....S.|.|...
+000013b0: 7d00 7104 7c00 5300 2901 7a1a 6765 7420  }.q.|.S.).z.get 
+000013c0: 7661 6c75 6520 6672 6f6d 206e 6573 7465  value from neste
+000013d0: 6420 6469 6374 2901 da05 454d 5054 5929  d dict)...EMPTY)
+000013e0: 0472 2300 0000 7274 0000 00da 0764 6566  .r#...rt.....def
+000013f0: 6175 6c74 7273 0000 0072 0f00 0000 720f  aultrs...r....r.
+00001400: 0000 0072 1200 0000 da0f 6469 6374 5f6e  ...r......dict_n
+00001410: 6573 7465 645f 6765 7490 0000 0073 0a00  ested_get....s..
+00001420: 0000 0002 0801 1001 0801 0a01 7a32 5f5f  ............z2__
+00001430: 6578 706f 7274 5f72 656d 6f74 655f 6675  export_remote_fu
+00001440: 6e63 7469 6f6e 732e 3c6c 6f63 616c 733e  nctions.<locals>
+00001450: 2e64 6963 745f 6e65 7374 6564 5f67 6574  .dict_nested_get
+00001460: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00001470: 0004 0000 0053 0000 0073 2a00 0000 7c01  .....S...s*...|.
+00001480: 6401 6402 8502 1900 4400 5d0c 7d03 7c00  d.d.....D.].}.|.
+00001490: 7c03 1900 7d00 710c 7c02 7c00 7c01 6402  |...}.q.|.|.|.d.
+000014a0: 1900 3c00 6401 5300 2903 7a18 7365 7420  ..<.d.S.).z.set 
+000014b0: 7661 6c75 6520 746f 206e 6573 7465 6420  value to nested 
+000014c0: 6469 6374 4ee9 ffff ffff 720f 0000 0029  dictN.....r....)
+000014d0: 0472 2300 0000 7274 0000 0072 4e00 0000  .r#...rt...rN...
+000014e0: 7273 0000 0072 0f00 0000 720f 0000 0072  rs...r....r....r
+000014f0: 1200 0000 da0f 6469 6374 5f6e 6573 7465  ......dict_neste
+00001500: 645f 7365 7498 0000 0073 0600 0000 0002  d_set....s......
+00001510: 1001 0a01 7a32 5f5f 6578 706f 7274 5f72  ....z2__export_r
+00001520: 656d 6f74 655f 6675 6e63 7469 6f6e 732e  emote_functions.
+00001530: 3c6c 6f63 616c 733e 2e64 6963 745f 6e65  <locals>.dict_ne
+00001540: 7374 6564 5f73 6574 6302 0000 0000 0000  sted_setc.......
+00001550: 0000 0000 0002 0000 0003 0000 0013 0000  ................
+00001560: 0073 3c00 0000 7c01 6401 6b01 7314 7c01  .s<...|.d.k.s.|.
+00001570: 7400 8801 8301 6b04 7218 8801 5300 7400  t.....k.r...S.t.
+00001580: 8801 8301 7c01 1b00 8900 8700 8701 6602  ....|.........f.
+00001590: 6402 6403 8408 7401 7c01 8301 4400 8301  d.d...t.|...D...
+000015a0: 5300 2904 4e72 0100 0000 6301 0000 0000  S.).Nr....c.....
+000015b0: 0000 0000 0000 0002 0000 0006 0000 0013  ................
+000015c0: 0000 0073 1c00 0000 6700 7c00 5d14 7d01  ...s....g.|.].}.
+000015d0: 8801 7400 7c01 8800 1400 8301 1900 9102  ..t.|...........
+000015e0: 7104 5300 720f 0000 0029 01da 0369 6e74  q.S.r....)...int
+000015f0: 723b 0000 00a9 02da 0869 6e74 6572 7661  r;.......interva
+00001600: 6c72 2800 0000 720f 0000 0072 1200 0000  lr(...r....r....
+00001610: 7232 0000 00a3 0000 0072 1400 0000 7a47  r2.......r....zG
+00001620: 5f5f 6578 706f 7274 5f72 656d 6f74 655f  __export_remote_
+00001630: 6675 6e63 7469 6f6e 732e 3c6c 6f63 616c  functions.<local
+00001640: 733e 2e6c 6973 745f 6576 656e 5f73 616d  s>.list_even_sam
+00001650: 706c 652e 3c6c 6f63 616c 733e 2e3c 6c69  ple.<locals>.<li
+00001660: 7374 636f 6d70 3e29 0272 4100 0000 7242  stcomp>).rA...rB
+00001670: 0000 0029 0272 2800 0000 da04 7369 7a65  ...).r(.....size
+00001680: 720f 0000 0072 7b00 0000 7212 0000 00da  r....r{...r.....
+00001690: 106c 6973 745f 6576 656e 5f73 616d 706c  .list_even_sampl
+000016a0: 659e 0000 0073 0800 0000 0001 1401 0402  e....s..........
+000016b0: 0c01 7a33 5f5f 6578 706f 7274 5f72 656d  ..z3__export_rem
+000016c0: 6f74 655f 6675 6e63 7469 6f6e 732e 3c6c  ote_functions.<l
+000016d0: 6f63 616c 733e 2e6c 6973 745f 6576 656e  ocals>.list_even
+000016e0: 5f73 616d 706c 6563 0300 0000 0000 0000  _samplec........
+000016f0: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
+00001700: 7326 0000 007c 0264 0075 0072 1074 007c  s&...|.d.u.r.t.|
+00001710: 0083 017d 0274 01a0 027c 02a1 0101 0074  ...}.t...|.....t
+00001720: 01a0 037c 007c 01a1 0253 0072 0d00 0000  ...|.|...S.r....
+00001730: 2904 7241 0000 00da 0672 616e 646f 6dda  ).rA.....random.
+00001740: 0473 6565 64da 0673 616d 706c 6529 0372  .seed..sample).r
+00001750: 2800 0000 727d 0000 0072 8000 0000 720f  (...r}...r....r.
+00001760: 0000 0072 0f00 0000 7212 0000 00da 126c  ...r....r......l
+00001770: 6973 745f 7261 6e64 6f6d 5f73 616d 706c  ist_random_sampl
+00001780: 65a5 0000 0073 0800 0000 0001 0801 0801  e....s..........
+00001790: 0a01 7a35 5f5f 6578 706f 7274 5f72 656d  ..z5__export_rem
+000017a0: 6f74 655f 6675 6e63 7469 6f6e 732e 3c6c  ote_functions.<l
+000017b0: 6f63 616c 733e 2e6c 6973 745f 7261 6e64  ocals>.list_rand
+000017c0: 6f6d 5f73 616d 706c 65da 0465 7665 6e63  om_sample..evenc
+000017d0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+000017e0: 0400 0000 1b00 0000 7352 0000 007c 0264  ........sR...|.d
+000017f0: 016b 0272 1288 007c 007c 0183 0253 007c  .k.r...|.|...S.|
+00001800: 0264 026b 0272 2c88 017c 007c 0166 0269  .d.k.r,..|.|.f.i
+00001810: 007c 03a4 018e 0153 007c 0264 036b 0272  .|.....S.|.d.k.r
+00001820: 407c 0064 007c 0185 0219 0053 0074 0064  @|.d.|.....S.t.d
+00001830: 047c 029b 009d 0283 0182 0164 0053 0029  .|.........d.S.)
+00001840: 054e 7283 0000 0072 7f00 0000 da08 7472  .Nr....r......tr
+00001850: 756e 6361 7465 7a16 556e 6b6e 6f77 6e20  uncatez.Unknown 
+00001860: 7361 6d70 6c65 206d 6574 686f 6420 2901  sample method ).
+00001870: da0a 5661 6c75 6545 7272 6f72 2904 7228  ..ValueError).r(
+00001880: 0000 0072 7d00 0000 da06 6d65 7468 6f64  ...r}.....method
+00001890: da06 6b77 6172 6773 2902 727e 0000 0072  ..kwargs).r~...r
+000018a0: 8200 0000 720f 0000 0072 1200 0000 da0b  ....r....r......
+000018b0: 6c69 7374 5f73 616d 706c 65ab 0000 0073  list_sample....s
+000018c0: 0e00 0000 0001 0801 0a01 0801 1201 0801  ................
+000018d0: 0c02 7a2e 5f5f 6578 706f 7274 5f72 656d  ..z.__export_rem
+000018e0: 6f74 655f 6675 6e63 7469 6f6e 732e 3c6c  ote_functions.<l
+000018f0: 6f63 616c 733e 2e6c 6973 745f 7361 6d70  ocals>.list_samp
+00001900: 6c65 6301 0000 0000 0000 0000 0000 0001  lec.............
+00001910: 0000 0003 0000 0053 0000 0073 1200 0000  .......S...s....
+00001920: 6401 6402 8400 7400 7c00 8e00 4400 8301  d.d...t.|...D...
+00001930: 5300 2903 6140 0100 000a 2020 2020 2020  S.).a@....      
+00001940: 2020 666c 6174 2061 206c 6973 7420 6f66    flat a list of
+00001950: 206c 6973 7473 2061 6e64 2065 6e73 7572   lists and ensur
+00001960: 6520 7468 6520 6f75 7470 7574 2072 6573  e the output res
+00001970: 756c 7420 6469 7374 7269 6275 7465 6420  ult distributed 
+00001980: 6576 656e 6c79 0a20 2020 2020 2020 203e  evenly.        >
+00001990: 3e3e 2066 6c61 745f 6576 656e 6c79 285b  >> flat_evenly([
+000019a0: 5b31 2c20 322c 2033 5d2c 205b 342c 2035  [1, 2, 3], [4, 5
+000019b0: 2c20 365d 2c20 5b37 2c20 382c 2039 5d5d  , 6], [7, 8, 9]]
+000019c0: 290a 2020 2020 2020 2020 5b31 2c20 342c  ).        [1, 4,
+000019d0: 2037 2c20 322c 2035 2c20 382c 2033 2c20   7, 2, 5, 8, 3, 
+000019e0: 362c 2039 5d0a 2020 2020 2020 2020 5265  6, 9].        Re
+000019f0: 663a 2068 7474 7073 3a2f 2f73 7461 636b  f: https://stack
+00001a00: 6f76 6572 666c 6f77 2e63 6f6d 2f71 7565  overflow.com/que
+00001a10: 7374 696f 6e73 2f37 3637 3531 3137 312f  stions/76751171/
+00001a20: 686f 772d 746f 2d66 6c61 742d 612d 6c69  how-to-flat-a-li
+00001a30: 7374 2d6f 662d 6c69 7374 732d 616e 642d  st-of-lists-and-
+00001a40: 656e 7375 7265 2d74 6865 2d6f 7574 7075  ensure-the-outpu
+00001a50: 742d 7265 7375 6c74 2d64 6973 7472 6962  t-result-distrib
+00001a60: 7574 6564 2d65 7665 6e6c 792d 696e 2d70  uted-evenly-in-p
+00001a70: 0a20 2020 2020 2020 2063 0100 0000 0000  .        c......
+00001a80: 0000 0000 0000 0300 0000 0500 0000 5300  ..............S.
+00001a90: 0000 7322 0000 0067 007c 005d 1a7d 017c  ..s"...g.|.].}.|
+00001aa0: 0144 005d 107d 027c 0264 0075 0172 0c7c  .D.].}.|.d.u.r.|
+00001ab0: 0291 0371 0c71 0453 0072 0d00 0000 720f  ...q.q.S.r....r.
+00001ac0: 0000 0029 0372 3000 0000 da03 7475 70da  ...).r0.....tup.
+00001ad0: 0165 720f 0000 0072 0f00 0000 7212 0000  .er....r....r...
+00001ae0: 0072 3200 0000 bc00 0000 7214 0000 007a  .r2.......r....z
+00001af0: 425f 5f65 7870 6f72 745f 7265 6d6f 7465  B__export_remote
+00001b00: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
+00001b10: 6c73 3e2e 666c 6174 5f65 7665 6e6c 792e  ls>.flat_evenly.
+00001b20: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001b30: 6d70 3e72 0900 0000 2901 5a0d 6c69 7374  mp>r....).Z.list
+00001b40: 5f6f 665f 6c69 7374 7372 0f00 0000 720f  _of_listsr....r.
+00001b50: 0000 0072 1200 0000 da0b 666c 6174 5f65  ...r......flat_e
+00001b60: 7665 6e6c 79b5 0000 0073 0200 0000 0007  venly....s......
+00001b70: 7a2e 5f5f 6578 706f 7274 5f72 656d 6f74  z.__export_remot
+00001b80: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
+00001b90: 616c 733e 2e66 6c61 745f 6576 656e 6c79  als>.flat_evenly
+00001ba0: 2902 7211 0000 0072 1700 0000 6302 0000  ).r....r....c...
+00001bb0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+00001bc0: 0053 0000 0073 4200 0000 7400 7c01 6401  .S...sB...t.|.d.
+00001bd0: 6402 6403 8d03 8f20 7d02 7401 6a02 7c00  d.d.... }.t.j.|.
+00001be0: 7c02 6404 6405 8d03 0100 5700 6400 0400  |.d.d.....W.d...
+00001bf0: 0400 8303 0100 6e10 3100 7334 3000 0100  ......n.1.s40...
+00001c00: 0100 0100 5900 0100 6400 5300 2906 4eda  ....Y...d.S.).N.
+00001c10: 0177 7244 0000 0029 01da 0865 6e63 6f64  .wrD...)...encod
+00001c20: 696e 67e9 0200 0000 2901 da06 696e 6465  ing.....)...inde
+00001c30: 6e74 2903 726a 0000 00da 046a 736f 6eda  nt).rj.....json.
+00001c40: 0464 756d 7029 0372 1100 0000 7217 0000  .dump).r....r...
+00001c50: 0072 6c00 0000 720f 0000 0072 0f00 0000  .rl...r....r....
+00001c60: 7212 0000 00da 0964 756d 705f 6a73 6f6e  r......dump_json
+00001c70: bf00 0000 7304 0000 0000 0110 017a 2c5f  ....s........z,_
+00001c80: 5f65 7870 6f72 745f 7265 6d6f 7465 5f66  _export_remote_f
+00001c90: 756e 6374 696f 6e73 2e3c 6c6f 6361 6c73  unctions.<locals
+00001ca0: 3e2e 6475 6d70 5f6a 736f 6e63 0000 0000  >.dump_jsonc....
+00001cb0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00001cc0: 5300 0000 7320 0000 0064 0164 006c 007d  S...s ...d.d.l.}
+00001cd0: 007c 006a 01a0 02a1 0001 007c 006a 03a0  .|.j.......|.j..
+00001ce0: 02a1 0001 0064 0053 0029 024e 7201 0000  .....d.S.).Nr...
+00001cf0: 0029 04da 0373 7973 da06 7374 646f 7574  .)...sys..stdout
+00001d00: da05 666c 7573 68da 0673 7464 6572 7229  ..flush..stderr)
+00001d10: 0172 9300 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00001d20: 7212 0000 00da 0b66 6c75 7368 5f73 7464  r......flush_std
+00001d30: 696f c300 0000 7306 0000 0000 0108 010a  io....s.........
+00001d40: 017a 2e5f 5f65 7870 6f72 745f 7265 6d6f  .z.__export_remo
+00001d50: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
+00001d60: 6361 6c73 3e2e 666c 7573 685f 7374 6469  cals>.flush_stdi
+00001d70: 6f29 014e 2901 4e29 0172 8300 0000 2904  o).N).N).r....).
+00001d80: 7272 0000 0072 7500 0000 7205 0000 0072  rr...ru...r....r
+00001d90: 5100 0000 2906 7277 0000 0072 7900 0000  Q...).rw...ry...
+00001da0: 7288 0000 0072 8b00 0000 7292 0000 0072  r....r....r....r
+00001db0: 9700 0000 720f 0000 0029 0372 7e00 0000  ....r....).r~...
+00001dc0: 7282 0000 0072 2200 0000 7212 0000 00da  r....r"...r.....
+00001dd0: 195f 5f65 7870 6f72 745f 7265 6d6f 7465  .__export_remote
+00001de0: 5f66 756e 6374 696f 6e73 7a00 0000 7326  _functionsz...s&
+00001df0: 0000 0000 0316 1318 0814 0608 070a 0610  ................
+00001e00: 0a08 0a10 0408 0802 0102 0102 0102 0102  ................
+00001e10: 0102 0102 0102 0102 f772 9800 0000 2932  .........r....)2
+00001e20: 5a0b 7275 616d 656c 2e79 616d 6c72 0200  Z.ruamel.yamlr..
+00001e30: 0000 da07 7061 7468 6c69 6272 0300 0000  ....pathlibr....
+00001e40: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
+00001e50: 0000 7206 0000 00da 0b64 6174 6163 6c61  ..r......datacla
+00001e60: 7373 6573 7208 0000 00da 0969 7465 7274  ssesr......itert
+00001e70: 6f6f 6c73 720a 0000 0072 2500 0000 7246  oolsr....r%...rF
+00001e80: 0000 0072 4a00 0000 720e 0000 0072 3600  ...rJ...r....r6.
+00001e90: 0000 727f 0000 0072 9000 0000 da03 6c6f  ..r....r......lo
+00001ea0: 6772 0c00 0000 7264 0000 00da 066c 6f67  gr....rd.....log
+00001eb0: 6765 72da 066f 626a 6563 7472 7500 0000  ger..objectru...
+00001ec0: 7216 0000 0072 1f00 0000 7224 0000 0072  r....r....r$...r
+00001ed0: 2700 0000 7251 0000 0072 2e00 0000 722f  '...rQ...r....r/
+00001ee0: 0000 0072 3300 0000 7238 0000 0072 7a00  ...r3...r8...rz.
+00001ef0: 0000 7243 0000 0072 4d00 0000 724f 0000  ..rC...rM...rO..
+00001f00: 0072 1a00 0000 721c 0000 0072 9800 0000  .r....r....r....
+00001f10: 7222 0000 0072 7700 0000 7279 0000 0072  r"...rw...ry...r
+00001f20: 7e00 0000 7282 0000 0072 8800 0000 728b  ~...r....r....r.
+00001f30: 0000 0072 9200 0000 7297 0000 0072 0f00  ...r....r....r..
+00001f40: 0000 720f 0000 0072 0f00 0000 7212 0000  ..r....r....r...
+00001f50: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001f60: 5000 0000 0c01 0c01 1401 0c01 0c02 0801  P...............
+00001f70: 0801 0801 0801 0801 0801 0802 0c02 0802  ................
+00001f80: 0603 0804 0e07 1208 0805 1805 0803 1c04  ................
+00001f90: 1004 1e07 1007 1004 0e14 0e16 0867 04f6  .............g..
+00001fa0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001fb0: 0201 02f7                                ....
```

### Comparing `ai2_kit-0.4.0/ai2_kit/core/artifact.py` & `ai2_kit-0.5.0/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/checkpoint.py` & `ai2_kit-0.5.0/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/connector.py` & `ai2_kit-0.5.0/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/executor.py` & `ai2_kit-0.5.0/ai2_kit/core/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,11 +222,12 @@
 
 
 def fn_to_script(fn: Callable, delimiter='@'):
     dumped_fn = base64.b64encode(bz2.compress(cloudpickle.dumps(fn, protocol=cloudpickle.DEFAULT_PROTOCOL), 5))
     script = [
         f'''import base64,bz2,sys,cloudpickle as cp''',
         f'''r=cp.loads(bz2.decompress(base64.b64decode({repr(dumped_fn)})))()''',
+        f'''sys.stdout.flush()''',  # ensure all output is printed
         f'''print({repr(delimiter)}+base64.b64encode(bz2.compress(cp.dumps(r, protocol=cp.DEFAULT_PROTOCOL),5)).decode('ascii'))''',
         f'''sys.stdout.flush()''',  # ensure all output is printed
     ]
     return ';'.join(script)
```

### Comparing `ai2_kit-0.4.0/ai2_kit/core/job.py` & `ai2_kit-0.5.0/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/queue_system.py` & `ai2_kit-0.5.0/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/resource_manager.py` & `ai2_kit-0.5.0/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/script.py` & `ai2_kit-0.5.0/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/core/util.py` & `ai2_kit-0.5.0/ai2_kit/core/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from ruamel.yaml import YAML
 from pathlib import Path
 from typing import Tuple, List, TypeVar
 from dataclasses import field
+from itertools import zip_longest
 
 import shortuuid
 import hashlib
 import base64
 import copy
 import os
 import random
+import json
 
 from .log import get_logger
 
 logger = get_logger(__name__)
 
 EMPTY = object()
 
@@ -172,26 +174,52 @@
         elif method == 'random':
             return list_random_sample(l, size, **kwargs)
         elif method == 'truncate':
             return l[:size]
         else:
             raise ValueError(f'Unknown sample method {method}')
 
+    def flat_evenly(list_of_lists):
+        """
+        flat a list of lists and ensure the output result distributed evenly
+        >>> flat_evenly([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
+        [1, 4, 7, 2, 5, 8, 3, 6, 9]
+        Ref: https://stackoverflow.com/questions/76751171/how-to-flat-a-list-of-lists-and-ensure-the-output-result-distributed-evenly-in-p
+        """
+        return [e for tup in zip_longest(*list_of_lists) for e in tup if e is not None]
+
+
+    def dump_json(obj: dict, path: str):
+        with open(path, 'w', encoding='utf-8') as f:
+            json.dump(obj, f, indent=2)
+
+    def flush_stdio():
+        import sys
+        sys.stdout.flush()
+        sys.stderr.flush()
+
+
     # export functions
     return (
         merge_dict,
         dict_nested_get,
         dict_nested_set,
         list_even_sample,
         list_random_sample,
         list_sample,
+        flat_evenly,
+        dump_json,
+        flush_stdio,
     )
 
 
 (
     merge_dict,
     dict_nested_get,
     dict_nested_set,
     list_even_sample,
     list_random_sample,
     list_sample,
+    flat_evenly,
+    dump_json,
+    flush_stdio,
 ) = __export_remote_functions()
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/cll.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cll.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/common.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/constant.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/constant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jul 19 08:27:40 2023 UTC, .py size: 1650 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,96 @@
-00000000: 610d 0d0a 0000 0000 7c9e b764 7206 0000  a.......|..dr...
+00000000: 610d 0d0a 0000 0000 8c43 be64 0d07 0000  a........C.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000f 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
+00000020: 000f 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 5a07 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6409 5a09 640a 5a0a 640b 5a0b 640c  Z.d.Z.d.Z.d.Z.d.
 00000060: 640d 640e 640f 6410 6411 6412 6413 6413  d.d.d.d.d.d.d.d.
 00000070: 640e 6414 6415 6416 6417 6418 9c0e 5a0c  d.d.d.d.d.d...Z.
 00000080: 6419 5a0d 641a 641b 641c 641d 641e 641f  d.Z.d.d.d.d.d.d.
 00000090: 9c05 5a0e 641a 641b 6420 6420 6412 641d  ..Z.d.d.d d d.d.
-000000a0: 6421 641c 641d 641e 6422 9c0a 5a0f 641a  d!d.d.d.d"..Z.d.
-000000b0: 5300 2923 7a0a 6d6f 6465 6c2e 636b 7074  S.)#z.model.ckpt
-000000c0: 7a0a 6c63 7572 7665 2e6f 7574 7a0d 7469  z.lcurve.outz.ti
-000000d0: 6d65 6c69 6e65 2e6a 736f 6e7a 0a69 6e70  meline.jsonz.inp
-000000e0: 7574 2e6a 736f 6e7a 0f66 726f 7a65 6e5f  ut.jsonz.frozen_
-000000f0: 6d6f 6465 6c2e 7062 7a11 6f72 6967 696e  model.pbz.origin
-00000100: 616c 5f6d 6f64 656c 2e70 627a 0e6d 6f64  al_model.pbz.mod
-00000110: 656c 5f64 6576 692e 6f75 747a 126d 6f64  el_devi.outz.mod
-00000120: 656c 5f64 6576 695f 6e65 752e 6f75 747a  el_devi_neu.outz
-00000130: 126d 6f64 656c 5f64 6576 695f 7265 642e  .model_devi_red.
-00000140: 6f75 74da 0474 7261 6a7a 0a2e 6c61 6d6d  out..trajz..lamm
-00000150: 7073 7472 6a5a 1064 756d 7073 5f63 6c61  pstrjZ.dumps_cla
-00000160: 7373 6966 6965 64e9 0f00 0000 e914 0000  ssified.........
-00000170: 0069 2c01 0000 e90a 0000 00e9 0800 0000  .i,.............
-00000180: 6733 3333 3333 33e3 3f67 0000 0000 0000  g333333.?g......
-00000190: e03f 679a 9999 9999 99a9 3fda 0154 e900  .?g.......?..T..
-000001a0: 0000 00e9 ffff ffff da01 4629 0e5a 0852  ..........F).Z.R
-000001b0: 756e 5f74 7970 657a 0c53 5357 2e53 5357  un_typez.SSW.SSW
-000001c0: 7374 6570 737a 0853 5357 2e54 656d 707a  stepsz.SSW.Tempz
-000001d0: 0653 5357 2e4e 477a 0b53 5357 2e4e 475f  .SSW.NGz.SSW.NG_
-000001e0: 6365 6c6c 7a0b 5353 572e 6473 5f61 746f  cellz.SSW.ds_ato
-000001f0: 6d7a 0b53 5357 2e64 735f 6365 6c6c 7a08  mz.SSW.ds_cellz.
-00000200: 5353 572e 6674 6f6c 7a0a 5353 572e 7374  SSW.ftolz.SSW.st
-00000210: 7274 6f6c 7a0e 5353 572e 4d61 784f 7074  rtolz.SSW.MaxOpt
-00000220: 7374 6570 7a0e 5353 572e 7072 696e 7465  stepz.SSW.printe
-00000230: 7665 7279 7a0f 5353 572e 7072 696e 7473  veryz.SSW.prints
-00000240: 656c 6563 747a 0e53 5357 2e70 7269 6e74  electz.SSW.print
-00000250: 6465 6c61 797a 0a53 5357 2e6f 7574 7075  delayz.SSW.outpu
-00000260: 747a ad75 6e69 7473 2020 2020 2020 2020  tz.units        
-00000270: 2020 206d 6574 616c 0a62 6f75 6e64 6172     metal.boundar
-00000280: 7920 2020 2020 2020 2070 2070 2070 0a61  y        p p p.a
-00000290: 746f 6d5f 7374 796c 6520 2020 2020 2061  tom_style      a
-000002a0: 746f 6d69 630a 6174 6f6d 5f6d 6f64 6966  tomic.atom_modif
-000002b0: 7920 6d61 7020 7965 730a 0a24 2472 6561  y map yes..$$rea
-000002c0: 645f 6461 7461 5f73 6563 7469 6f6e 0a0a  d_data_section..
-000002d0: 2424 666f 7263 655f 6669 656c 645f 7365  $$force_field_se
-000002e0: 6374 696f 6e0a 0a63 6f6d 7075 7465 2070  ction..compute p
-000002f0: 6572 6174 6f6d 2061 6c6c 2070 7265 7373  eratom all press
-00000300: 7572 6520 4e55 4c4c 2076 6972 6961 6c0a  ure NULL virial.
-00000310: 4e67 0000 0000 0000 0c40 da07 6176 6572  Ng.......@..aver
-00000320: 6167 6546 e901 0000 0029 05da 0670 7265  ageF.....)...pre
-00000330: 7365 74da 0572 5f63 7574 da0c 7265 6475  set..r_cut..redu
-00000340: 6365 725f 7479 7065 da0c 656c 656d 656e  cer_type..elemen
-00000350: 745f 7769 7365 da04 7a65 7461 e906 0000  t_wise..zeta....
-00000360: 00da 0367 746f 290a 720c 0000 0072 0d00  ...gto).r....r..
-00000370: 0000 da05 6e5f 6d61 78da 056c 5f6d 6178  ....n_max..l_max
-00000380: da05 7369 676d 61da 0963 726f 7373 6f76  ..sigma..crossov
-00000390: 6572 da03 7262 6672 0e00 0000 720f 0000  er..rbfr....r...
-000003a0: 0072 1000 0000 2910 5a12 4450 5f43 4845  .r....).Z.DP_CHE
-000003b0: 434b 504f 494e 545f 4649 4c45 5a0c 4450  CKPOINT_FILEZ.DP
-000003c0: 5f44 4953 505f 4649 4c45 5a11 4450 5f50  _DISP_FILEZ.DP_P
-000003d0: 524f 4649 4c49 4e47 5f46 494c 455a 0d44  ROFILING_FILEZ.D
-000003e0: 505f 494e 5055 545f 4649 4c45 5a0f 4450  P_INPUT_FILEZ.DP
-000003f0: 5f46 524f 5a45 4e5f 4d4f 4445 4c5a 1144  _FROZEN_MODELZ.D
-00000400: 505f 4f52 4947 494e 414c 5f4d 4f44 454c  P_ORIGINAL_MODEL
-00000410: 5a0e 4d4f 4445 4c5f 4445 5649 5f4f 5554  Z.MODEL_DEVI_OUT
-00000420: 5a12 4d4f 4445 4c5f 4445 5649 5f4e 4555  Z.MODEL_DEVI_NEU
-00000430: 5f4f 5554 5a12 4d4f 4445 4c5f 4445 5649  _OUTZ.MODEL_DEVI
-00000440: 5f52 4544 5f4f 5554 5a0f 4c41 4d4d 5053  _RED_OUTZ.LAMMPS
-00000450: 5f54 5241 4a5f 4449 525a 124c 414d 4d50  _TRAJ_DIRZ.LAMMP
-00000460: 535f 5452 414a 5f53 5546 4649 585a 174c  S_TRAJ_SUFFIXZ.L
-00000470: 414d 4d50 535f 4455 4d50 535f 434c 4153  AMMPS_DUMPS_CLAS
-00000480: 5349 4649 4544 5a0f 4445 4641 554c 545f  SIFIEDZ.DEFAULT_
-00000490: 4c41 5350 5f49 4e5a 2244 4546 4155 4c54  LASP_INZ"DEFAULT
-000004a0: 5f4c 414d 4d50 535f 5445 4d50 4c41 5445  _LAMMPS_TEMPLATE
-000004b0: 5f46 4f52 5f44 505f 5353 575a 1644 4546  _FOR_DP_SSWZ.DEF
-000004c0: 4155 4c54 5f41 5341 505f 4153 4346 5f44  AULT_ASAP_ASCF_D
-000004d0: 4553 43da 1644 4546 4155 4c54 5f41 5341  ESC..DEFAULT_ASA
-000004e0: 505f 534f 4150 5f44 4553 43a9 0072 1900  P_SOAP_DESC..r..
-000004f0: 0000 7219 0000 00fa 322f 686f 6d65 2f68  ..r.....2/home/h
-00000500: 656e 7279 2f73 7263 2f61 6932 2d6b 6974  enry/src/ai2-kit
-00000510: 2f61 6932 5f6b 6974 2f64 6f6d 6169 6e2f  /ai2_kit/domain/
-00000520: 636f 6e73 7461 6e74 2e70 79da 083c 6d6f  constant.py..<mo
-00000530: 6475 6c65 3e01 0000 0073 5800 0000 0401  dule>....sX.....
-00000540: 0401 0401 0401 0401 0402 0401 0401 0402  ................
-00000550: 0401 0401 0404 0201 0201 0201 0201 0201  ................
-00000560: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000570: 02f2 0612 040f 0203 0202 0201 0201 02f8  ................
-00000580: 060d 0204 0201 0201 0201 0202 0201 0202  ................
-00000590: 0201 0201 02f1                           ......
+000000a0: 6421 641c 641d 641e 6422 9c0a 5a0f 6423  d!d.d.d.d"..Z.d#
+000000b0: 6424 6425 6426 9c02 6427 9c02 5a10 641a  d$d%d&..d'..Z.d.
+000000c0: 5300 2928 7a0a 6d6f 6465 6c2e 636b 7074  S.)(z.model.ckpt
+000000d0: 7a0a 6c63 7572 7665 2e6f 7574 7a0d 7469  z.lcurve.outz.ti
+000000e0: 6d65 6c69 6e65 2e6a 736f 6e7a 0a69 6e70  meline.jsonz.inp
+000000f0: 7574 2e6a 736f 6e7a 0f66 726f 7a65 6e5f  ut.jsonz.frozen_
+00000100: 6d6f 6465 6c2e 7062 7a11 6f72 6967 696e  model.pbz.origin
+00000110: 616c 5f6d 6f64 656c 2e70 627a 0e6d 6f64  al_model.pbz.mod
+00000120: 656c 5f64 6576 692e 6f75 747a 126d 6f64  el_devi.outz.mod
+00000130: 656c 5f64 6576 695f 6e65 752e 6f75 747a  el_devi_neu.outz
+00000140: 126d 6f64 656c 5f64 6576 695f 7265 642e  .model_devi_red.
+00000150: 6f75 74da 0474 7261 6a7a 0a2e 6c61 6d6d  out..trajz..lamm
+00000160: 7073 7472 6ada 0f73 656c 6563 746f 725f  pstrj..selector_
+00000170: 6f75 7470 7574 e90f 0000 00e9 1400 0000  output..........
+00000180: 692c 0100 00e9 0a00 0000 e908 0000 0067  i,.............g
+00000190: 3333 3333 3333 e33f 6700 0000 0000 00e0  333333.?g.......
+000001a0: 3f67 9a99 9999 9999 a93f da01 54e9 0000  ?g.......?..T...
+000001b0: 0000 e9ff ffff ffda 0146 290e 5a08 5275  .........F).Z.Ru
+000001c0: 6e5f 7479 7065 7a0c 5353 572e 5353 5773  n_typez.SSW.SSWs
+000001d0: 7465 7073 7a08 5353 572e 5465 6d70 7a06  tepsz.SSW.Tempz.
+000001e0: 5353 572e 4e47 7a0b 5353 572e 4e47 5f63  SSW.NGz.SSW.NG_c
+000001f0: 656c 6c7a 0b53 5357 2e64 735f 6174 6f6d  ellz.SSW.ds_atom
+00000200: 7a0b 5353 572e 6473 5f63 656c 6c7a 0853  z.SSW.ds_cellz.S
+00000210: 5357 2e66 746f 6c7a 0a53 5357 2e73 7472  SW.ftolz.SSW.str
+00000220: 746f 6c7a 0e53 5357 2e4d 6178 4f70 7473  tolz.SSW.MaxOpts
+00000230: 7465 707a 0e53 5357 2e70 7269 6e74 6576  tepz.SSW.printev
+00000240: 6572 797a 0f53 5357 2e70 7269 6e74 7365  eryz.SSW.printse
+00000250: 6c65 6374 7a0e 5353 572e 7072 696e 7464  lectz.SSW.printd
+00000260: 656c 6179 7a0a 5353 572e 6f75 7470 7574  elayz.SSW.output
+00000270: 7aad 756e 6974 7320 2020 2020 2020 2020  z.units         
+00000280: 2020 6d65 7461 6c0a 626f 756e 6461 7279    metal.boundary
+00000290: 2020 2020 2020 2020 7020 7020 700a 6174          p p p.at
+000002a0: 6f6d 5f73 7479 6c65 2020 2020 2020 6174  om_style      at
+000002b0: 6f6d 6963 0a61 746f 6d5f 6d6f 6469 6679  omic.atom_modify
+000002c0: 206d 6170 2079 6573 0a0a 2424 7265 6164   map yes..$$read
+000002d0: 5f64 6174 615f 7365 6374 696f 6e0a 0a24  _data_section..$
+000002e0: 2466 6f72 6365 5f66 6965 6c64 5f73 6563  $force_field_sec
+000002f0: 7469 6f6e 0a0a 636f 6d70 7574 6520 7065  tion..compute pe
+00000300: 7261 746f 6d20 616c 6c20 7072 6573 7375  ratom all pressu
+00000310: 7265 204e 554c 4c20 7669 7269 616c 0a4e  re NULL virial.N
+00000320: 6700 0000 0000 000c 40da 0761 7665 7261  g.......@..avera
+00000330: 6765 46e9 0100 0000 2905 da06 7072 6573  geF.....)...pres
+00000340: 6574 da05 725f 6375 74da 0c72 6564 7563  et..r_cut..reduc
+00000350: 6572 5f74 7970 65da 0c65 6c65 6d65 6e74  er_type..element
+00000360: 5f77 6973 65da 047a 6574 61e9 0600 0000  _wise..zeta.....
+00000370: 5a03 6774 6f29 0a72 0d00 0000 720e 0000  Z.gto).r....r...
+00000380: 005a 056e 5f6d 6178 5a05 6c5f 6d61 78da  .Z.n_maxZ.l_max.
+00000390: 0573 6967 6d61 5a09 6372 6f73 736f 7665  .sigmaZ.crossove
+000003a0: 725a 0372 6266 720f 0000 0072 1000 0000  rZ.rbfr....r....
+000003b0: 7211 0000 005a 0350 4341 e903 0000 0054  r....Z.PCA.....T
+000003c0: 2902 da0c 6e5f 636f 6d70 6f6e 656e 7473  )...n_components
+000003d0: 5a0b 7363 616c 6563 656e 7465 7229 02da  Z.scalecenter)..
+000003e0: 0474 7970 65da 0970 6172 616d 6574 6572  .type..parameter
+000003f0: 2911 da12 4450 5f43 4845 434b 504f 494e  )...DP_CHECKPOIN
+00000400: 545f 4649 4c45 da0c 4450 5f44 4953 505f  T_FILE..DP_DISP_
+00000410: 4649 4c45 da11 4450 5f50 524f 4649 4c49  FILE..DP_PROFILI
+00000420: 4e47 5f46 494c 45da 0d44 505f 494e 5055  NG_FILE..DP_INPU
+00000430: 545f 4649 4c45 da0f 4450 5f46 524f 5a45  T_FILE..DP_FROZE
+00000440: 4e5f 4d4f 4445 4cda 1144 505f 4f52 4947  N_MODEL..DP_ORIG
+00000450: 494e 414c 5f4d 4f44 454c da0e 4d4f 4445  INAL_MODEL..MODE
+00000460: 4c5f 4445 5649 5f4f 5554 5a12 4d4f 4445  L_DEVI_OUTZ.MODE
+00000470: 4c5f 4445 5649 5f4e 4555 5f4f 5554 5a12  L_DEVI_NEU_OUTZ.
+00000480: 4d4f 4445 4c5f 4445 5649 5f52 4544 5f4f  MODEL_DEVI_RED_O
+00000490: 5554 5a0f 4c41 4d4d 5053 5f54 5241 4a5f  UTZ.LAMMPS_TRAJ_
+000004a0: 4449 525a 124c 414d 4d50 535f 5452 414a  DIRZ.LAMMPS_TRAJ
+000004b0: 5f53 5546 4649 585a 0f53 454c 4543 544f  _SUFFIXZ.SELECTO
+000004c0: 525f 4f55 5450 5554 5a0f 4445 4641 554c  R_OUTPUTZ.DEFAUL
+000004d0: 545f 4c41 5350 5f49 4e5a 2244 4546 4155  T_LASP_INZ"DEFAU
+000004e0: 4c54 5f4c 414d 4d50 535f 5445 4d50 4c41  LT_LAMMPS_TEMPLA
+000004f0: 5445 5f46 4f52 5f44 505f 5353 575a 1644  TE_FOR_DP_SSWZ.D
+00000500: 4546 4155 4c54 5f41 5341 505f 4153 4346  EFAULT_ASAP_ASCF
+00000510: 5f44 4553 435a 1644 4546 4155 4c54 5f41  _DESCZ.DEFAULT_A
+00000520: 5341 505f 534f 4150 5f44 4553 435a 1844  SAP_SOAP_DESCZ.D
+00000530: 4546 4155 4c54 5f41 5341 505f 5043 415f  EFAULT_ASAP_PCA_
+00000540: 5245 4455 4345 52a9 0072 1f00 0000 721f  REDUCER..r....r.
+00000550: 0000 00fa 322f 686f 6d65 2f68 656e 7279  ....2/home/henry
+00000560: 2f73 7263 2f61 6932 2d6b 6974 2f61 6932  /src/ai2-kit/ai2
+00000570: 5f6b 6974 2f64 6f6d 6169 6e2f 636f 6e73  _kit/domain/cons
+00000580: 7461 6e74 2e70 79da 083c 6d6f 6475 6c65  tant.py..<module
+00000590: 3e01 0000 0073 6200 0000 0401 0401 0401  >....sb.........
+000005a0: 0401 0401 0402 0401 0401 0402 0401 0402  ................
+000005b0: 0404 0201 0201 0201 0201 0201 0201 0201  ................
+000005c0: 0201 0201 0201 0201 0201 0201 02f2 0612  ................
+000005d0: 040f 0203 0202 0201 0201 02f8 060d 0204  ................
+000005e0: 0201 0201 0201 0202 0201 0202 0201 0201  ................
+000005f0: 02f1 0613 0202 0201 02fe 04fe            ............
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:22:42 2023 UTC, .py size: 6585 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e2dd b964 b919 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 fbde b964 b919 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6400 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/data.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:01:13 2023 UTC, .py size: 6679 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,374 +1,320 @@
-00000000: 610d 0d0a 0000 0000 d9d8 b964 171a 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 8c43 be64 4e15 0000  a........C.dN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
-00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0c 0100 6400 6406 6c0d 5a09 6400  m.Z...d.d.l.Z.d.
-00000080: 6406 6c0e 5a0e 6407 6408 6c0f 6d10 5a10  d.l.Z.d.d.l.m.Z.
-00000090: 6d11 5a11 6d12 5a12 0100 6409 640a 8400  m.Z.m.Z...d.d...
-000000a0: 5a13 6513 8300 5c06 5a14 5a15 5a16 5a17  Z.e...\.Z.Z.Z.Z.
-000000b0: 5a18 5a19 6406 5300 290b e900 0000 0029  Z.Z.d.S.)......)
-000000c0: 02da 0841 7274 6966 6163 74da 0c41 7274  ...Artifact..Art
-000000d0: 6966 6163 7444 6963 7429 01da 0f64 6963  ifactDict)...dic
-000000e0: 745f 6e65 7374 6564 5f67 6574 2903 da04  t_nested_get)...
-000000f0: 4c69 7374 da05 5475 706c 65da 084f 7074  List..Tuple..Opt
-00000100: 696f 6e61 6c29 01da 0541 746f 6d73 2901  ional)...Atoms).
-00000110: da0a 6974 656d 6765 7474 6572 4ee9 0100  ..itemgetterN...
-00000120: 0000 2903 da0f 4c41 4d4d 5053 5f54 5241  ..)...LAMMPS_TRA
-00000130: 4a5f 4449 52da 124c 414d 4d50 535f 5452  J_DIR..LAMMPS_TR
-00000140: 414a 5f53 5546 4649 58da 174c 414d 4d50  AJ_SUFFIX..LAMMP
-00000150: 535f 4455 4d50 535f 434c 4153 5349 4649  S_DUMPS_CLASSIFI
-00000160: 4544 6300 0000 0000 0000 0000 0000 0003  EDc.............
-00000170: 0000 0006 0000 0003 0000 0073 de00 0000  ...........s....
-00000180: 4700 6401 6402 8400 6402 8302 8900 7400  G.d.d...d.....t.
-00000190: 7401 7402 1900 6403 9c02 8700 6601 6404  t.t...d.....f.d.
-000001a0: 6405 840c 8903 7400 7401 7403 7404 1900  d.....t.t.t.t...
-000001b0: 1900 6403 9c02 6406 6407 8404 8901 7403  ..d...d.d.....t.
-000001c0: 7405 1900 7403 7402 1900 7403 7406 7405  t...t.t...t.t.t.
-000001d0: 7407 6602 1900 1900 6408 9c03 8700 8701  t.f.....d.......
-000001e0: 8703 6603 6409 640a 840c 8902 7407 7406  ..f.d.d.....t.t.
-000001f0: 7403 7402 1900 7403 7403 7408 1900 1900  t.t...t.t.t.....
-00000200: 6602 1900 640b 9c02 640c 640d 8404 7d00  f...d...d.d...}.
-00000210: 7402 7403 7402 1900 7403 7405 1900 640e  t.t.t...t.t...d.
-00000220: 9c03 8700 8703 6602 640f 6410 840c 7d01  ......f.d.d...}.
-00000230: 7403 7405 1900 7402 7403 7402 1900 6411  t.t...t.t.t...d.
-00000240: 9c03 8702 6601 6412 6413 840c 7d02 8802  ....f.d.d...}...
-00000250: 7c00 7c01 7c02 8800 8803 6606 5300 2914  |.|.|.....f.S.).
-00000260: 7a20 776f 726b 6172 6f75 6e64 2066 6f72  z workaround for
-00000270: 2063 6c6f 7564 7069 636b 6c65 2069 7373   cloudpickle iss
-00000280: 7565 6300 0000 0000 0000 0000 0000 0000  uec.............
-00000290: 0000 0001 0000 0040 0000 0073 3400 0000  .......@...s4...
-000002a0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-000002b0: 6403 5a05 6404 5a06 6405 5a07 6406 5a08  d.Z.d.Z.d.Z.d.Z.
-000002c0: 6407 5a09 6408 5a0a 6409 5a0b 640a 5a0c  d.Z.d.Z.d.Z.d.Z.
-000002d0: 640b 5300 290c 7a2d 5f5f 6578 706f 7274  d.S.).z-__export
-000002e0: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
-000002f0: 732e 3c6c 6f63 616c 733e 2e44 6174 6146  s.<locals>.DataF
-00000300: 6f72 6d61 747a 0f63 7032 6b2f 6f75 7470  ormatz.cp2k/outp
-00000310: 7574 5f64 6972 7a0f 7661 7370 2f6f 7574  ut_dirz.vasp/out
-00000320: 7075 745f 6469 727a 116c 616d 6d70 732f  put_dirz.lammps/
-00000330: 6f75 7470 7574 5f64 6972 7a11 6465 6570  output_dirz.deep
-00000340: 6d64 2f6f 7574 7075 745f 6469 727a 0a64  md/output_dirz.d
-00000350: 6565 706d 642f 6e70 797a 166c 6173 702b  eepmd/npyz.lasp+
-00000360: 6c61 6d6d 7073 2f6f 7574 7075 745f 6469  lammps/output_di
-00000370: 72fa 0b63 7032 6b2f 6f75 7470 7574 7a08  r..cp2k/outputz.
-00000380: 7661 7370 2f78 6d6c da06 6578 7478 797a  vasp/xml..extxyz
-00000390: 7a0b 7661 7370 2f70 6f73 6361 724e 290d  z.vasp/poscarN).
-000003a0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000003b0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000003c0: 6d65 5f5f da0f 4350 324b 5f4f 5554 5055  me__..CP2K_OUTPU
-000003d0: 545f 4449 52da 0f56 4153 505f 4f55 5450  T_DIR..VASP_OUTP
-000003e0: 5554 5f44 4952 da11 4c41 4d4d 5053 5f4f  UT_DIR..LAMMPS_O
-000003f0: 5554 5055 545f 4449 52da 1144 4545 504d  UTPUT_DIR..DEEPM
-00000400: 445f 4f55 5450 5554 5f44 4952 da0a 4445  D_OUTPUT_DIR..DE
-00000410: 4550 4d44 5f4e 5059 da13 4c41 5350 5f4c  EPMD_NPY..LASP_L
-00000420: 414d 4d50 535f 4f55 545f 4449 525a 0b43  AMMPS_OUT_DIRZ.C
-00000430: 5032 4b5f 4f55 5450 5554 5a08 5641 5350  P2K_OUTPUTZ.VASP
-00000440: 5f58 4d4c da06 4558 5458 595a da0b 5641  _XML..EXTXYZ..VA
-00000450: 5350 5f50 4f53 4341 52a9 0072 1b00 0000  SP_POSCAR..r....
-00000460: 721b 0000 00fa 2e2f 686f 6d65 2f68 656e  r....../home/hen
-00000470: 7279 2f73 7263 2f61 6932 2d6b 6974 2f61  ry/src/ai2-kit/a
-00000480: 6932 5f6b 6974 2f64 6f6d 6169 6e2f 6461  i2_kit/domain/da
-00000490: 7461 2e70 79da 0a44 6174 6146 6f72 6d61  ta.py..DataForma
-000004a0: 7411 0000 0073 1400 0000 0802 0401 0401  t....s..........
-000004b0: 0401 0401 0401 0403 0401 0403 0401 721d  ..............r.
-000004c0: 0000 0029 02da 0861 7274 6966 6163 74da  ...)...artifact.
-000004d0: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
-000004e0: 0000 0000 0400 0000 0400 0000 1300 0000  ................
-000004f0: 7370 0000 007c 00a0 0064 01a1 017d 0174  sp...|...d...}.t
-00000500: 017c 0174 0283 0273 264a 0064 0274 037c  .|.t...s&J.d.t.|
-00000510: 0183 019b 009d 0283 0182 0174 046a 05a0  ...........t.j..
-00000520: 067c 01a1 017d 027c 00a0 0064 03a1 017d  .|...}.|...d...}
-00000530: 037c 0372 4e74 017c 0374 0283 0272 4e7c  .|.rNt.|.t...rN|
-00000540: 0353 007c 02a0 0764 04a1 0172 5e88 006a  .S.|...d...r^..j
-00000550: 0853 0064 057c 0276 0072 6c88 006a 0953  .S.d.|.v.rl..j.S
-00000560: 0064 0653 0029 077a 960a 2020 2020 2020  .d.S.).z..      
-00000570: 2020 4765 7420 286f 7220 6775 6573 7329    Get (or guess)
-00000580: 2064 6174 6120 7479 7065 2066 726f 6d20   data type from 
-00000590: 6172 7469 6661 6374 2064 6963 740a 2020  artifact dict.  
-000005a0: 2020 2020 2020 4e6f 7465 3a20 5468 6520        Note: The 
-000005b0: 7265 6173 6f6e 206f 6620 7573 696e 6720  reason of using 
-000005c0: 6469 6374 2069 6e73 7465 6164 206f 6620  dict instead of 
-000005d0: 4172 7469 6661 6374 2069 7320 4172 7469  Artifact is Arti
-000005e0: 6661 6374 2069 7320 6e6f 7420 7069 636b  fact is not pick
-000005f0: 6c65 6162 6c65 0a20 2020 2020 2020 20da  leable.        .
-00000600: 0375 726c 7a15 7572 6c20 6d75 7374 2062  .urlz.url must b
-00000610: 6520 7374 722c 2067 6f74 20da 0666 6f72  e str, got ..for
-00000620: 6d61 747a 042e 7879 7a5a 0650 4f53 4341  matz..xyzZ.POSCA
-00000630: 524e 290a da03 6765 74da 0a69 7369 6e73  RN)...get..isins
-00000640: 7461 6e63 65da 0373 7472 da04 7479 7065  tance..str..type
-00000650: da02 6f73 da04 7061 7468 da08 6261 7365  ..os..path..base
-00000660: 6e61 6d65 da08 656e 6473 7769 7468 7219  name..endswithr.
-00000670: 0000 0072 1a00 0000 2904 721e 0000 0072  ...r....).r....r
-00000680: 2000 0000 da09 6669 6c65 5f6e 616d 6572   .....file_namer
-00000690: 2100 0000 2901 721d 0000 0072 1b00 0000  !...).r....r....
-000006a0: 721c 0000 00da 0f67 6574 5f64 6174 615f  r......get_data_
-000006b0: 666f 726d 6174 2300 0000 7316 0000 0000  format#...s.....
-000006c0: 050a 011c 020c 010a 010e 0104 010a 0106  ................
-000006d0: 0108 0106 017a 325f 5f65 7870 6f72 745f  .....z2__export_
-000006e0: 7265 6d6f 7465 5f66 756e 6374 696f 6e73  remote_functions
-000006f0: 2e3c 6c6f 6361 6c73 3e2e 6765 745f 6461  .<locals>.get_da
-00000700: 7461 5f66 6f72 6d61 7463 0100 0000 0000  ta_formatc......
-00000710: 0000 0000 0000 0100 0000 0500 0000 5300  ..............S.
-00000720: 0000 7312 0000 0074 007c 0064 0174 0164  ..s....t.|.d.t.d
-00000730: 0267 0364 0083 0353 0029 034e da05 6174  .g.d...S.).N..at
-00000740: 7472 73da 0873 656c 6563 7465 6429 0272  trs..selected).r
-00000750: 0400 0000 720d 0000 0029 0172 1e00 0000  ....r....).r....
-00000760: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-00000770: 115f 6765 745f 7365 6c65 6374 6564 5f69  ._get_selected_i
-00000780: 6473 3600 0000 7302 0000 0000 017a 345f  ds6...s......z4_
-00000790: 5f65 7870 6f72 745f 7265 6d6f 7465 5f66  _export_remote_f
-000007a0: 756e 6374 696f 6e73 2e3c 6c6f 6361 6c73  unctions.<locals
-000007b0: 3e2e 5f67 6574 5f73 656c 6563 7465 645f  >._get_selected_
-000007c0: 6964 7329 03da 0961 7274 6966 6163 7473  ids)...artifacts
-000007d0: da08 7479 7065 5f6d 6170 721f 0000 0063  ..type_mapr....c
-000007e0: 0200 0000 0000 0000 0000 0000 0b00 0000  ................
-000007f0: 0900 0000 1300 0000 734a 0100 0067 007d  ........sJ...g.}
-00000800: 027c 0044 0090 015d 3a89 0088 0388 0083  .|.D...]:.......
-00000810: 017d 0388 0064 0119 007d 0488 0288 0083  .}...d...}......
-00000820: 017d 057c 0388 016a 006b 0272 4474 016a  .}.|...j.k.rDt.j
-00000830: 026a 037c 0464 0264 0364 048d 037d 066e  .j.|.d.d.d...}.n
-00000840: e87c 0388 016a 046b 0272 6274 016a 026a  .|...j.k.rbt.j.j
-00000850: 037c 0464 0264 0564 048d 037d 066e ca7c  .|.d.d.d...}.n.|
-00000860: 0388 016a 056b 0272 cc7c 0564 0075 0173  ...j.k.r.|.d.u.s
-00000870: 844a 0064 0688 009b 0064 079d 0383 0182  .J.d.....d......
-00000880: 0167 007d 067c 0544 005d 3c7d 0774 066a  .g.}.|.D.]<}.t.j
-00000890: 07a0 087c 0474 097c 079b 0074 0a9b 009d  ...|.t.|...t....
-000008a0: 02a1 037d 0874 016a 026a 037c 0864 0264  ...}.t.j.j.|.d.d
-000008b0: 0864 097c 0164 0a8d 057d 097c 06a0 0b7c  .d.|.d...}.|...|
-000008c0: 09a1 0101 0071 8c6e 607c 0388 016a 0c6b  .....q.n`|...j.k
-000008d0: 0290 0172 1e7c 0564 0075 0173 f04a 0064  ...r.|.d.u.s.J.d
-000008e0: 0688 009b 0064 079d 0383 0182 0174 066a  .....d.......t.j
-000008f0: 07a0 087c 0464 0ba1 027d 0a74 0d74 0e7c  ...|.d...}.t.t.|
-00000900: 058e 0074 016a 026a 037c 0a64 0264 0564  ...t.j.j.|.d.d.d
-00000910: 048d 0383 0183 017d 066e 0e74 0f64 0c7c  .......}.n.t.d.|
-00000920: 039b 009d 0283 0182 017c 02a0 0b87 0066  .........|.....f
-00000930: 0164 0d64 0e84 087c 0644 0083 01a1 0101  .d.d...|.D......
-00000940: 0071 087c 0253 0029 0f4e 7220 0000 00fa  .q.|.S.).Nr ....
-00000950: 013a da04 7661 7370 2901 7221 0000 0072  .:..vasp).r!...r
-00000960: 0f00 0000 7a09 6172 7469 6661 6374 207a  ....z.artifact z
-00000970: 1220 6973 206e 6f74 2063 6c61 7373 6966  . is not classif
-00000980: 6965 647a 106c 616d 6d70 732d 6475 6d70  iedz.lammps-dump
-00000990: 2d74 6578 7446 2903 7221 0000 00da 056f  -textF).r!.....o
-000009a0: 7264 6572 da09 7370 6563 6f72 6465 727a  rder..specorderz
-000009b0: 0874 7261 6a2e 7879 7a7a 1975 6e73 7570  .traj.xyzz.unsup
-000009c0: 706f 7274 6564 2064 6174 6120 666f 726d  ported data form
-000009d0: 6174 3a20 6301 0000 0000 0000 0000 0000  at: c...........
-000009e0: 0002 0000 0003 0000 0033 0000 0073 1600  .........3...s..
-000009f0: 0000 7c00 5d0e 7d01 8800 7c01 6602 5600  ..|.].}...|.f.V.
-00000a00: 0100 7102 6400 5300 a901 4e72 1b00 0000  ..q.d.S...Nr....
-00000a10: 2902 da02 2e30 da05 6174 6f6d 73a9 01da  )....0..atoms...
-00000a20: 0161 721b 0000 0072 1c00 0000 da09 3c67  .ar....r......<g
-00000a30: 656e 6578 7072 3e51 0000 00f3 0000 0000  enexpr>Q........
-00000a40: 7a4c 5f5f 6578 706f 7274 5f72 656d 6f74  zL__export_remot
-00000a50: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
-00000a60: 616c 733e 2e61 7274 6966 6163 7473 5f74  als>.artifacts_t
-00000a70: 6f5f 6173 655f 6174 6f6d 732e 3c6c 6f63  o_ase_atoms.<loc
-00000a80: 616c 733e 2e3c 6765 6e65 7870 723e 2910  als>.<genexpr>).
-00000a90: 721a 0000 00da 0361 7365 da02 696f da04  r......ase..io..
-00000aa0: 7265 6164 7219 0000 0072 1500 0000 7226  readr....r....r&
-00000ab0: 0000 0072 2700 0000 da04 6a6f 696e 720b  ...r'.....joinr.
-00000ac0: 0000 0072 0c00 0000 da06 6578 7465 6e64  ...r......extend
-00000ad0: 7218 0000 00da 046c 6973 7472 0900 0000  r......listr....
-00000ae0: da0a 5661 6c75 6545 7272 6f72 290b 722f  ..ValueError).r/
-00000af0: 0000 0072 3000 0000 da07 7265 7375 6c74  ...r0.....result
-00000b00: 73da 0b64 6174 615f 666f 726d 6174 7220  s..data_formatr 
-00000b10: 0000 005a 0c73 656c 6563 7465 645f 6964  ...Z.selected_id
-00000b20: 73da 0a61 746f 6d73 5f6c 6973 745a 0764  s..atoms_listZ.d
-00000b30: 756d 705f 6964 5a09 6475 6d70 5f66 696c  ump_idZ.dump_fil
-00000b40: 65da 0464 756d 705a 0974 7261 6a5f 6669  e..dumpZ.traj_fi
-00000b50: 6c65 2903 721d 0000 0072 2e00 0000 722b  le).r....r....r+
-00000b60: 0000 0072 3800 0000 721c 0000 00da 1661  ...r8...r......a
-00000b70: 7274 6966 6163 7473 5f74 6f5f 6173 655f  rtifacts_to_ase_
-00000b80: 6174 6f6d 733a 0000 0073 2e00 0000 0001  atoms:...s......
-00000b90: 0401 0a01 0801 0801 0801 0a01 1401 0a01  ................
-00000ba0: 1401 0a01 1801 0401 0801 1801 1601 0e01  ................
-00000bb0: 0c01 1801 0e01 2002 0e01 1a01 7a39 5f5f  ...... .....z9__
-00000bc0: 6578 706f 7274 5f72 656d 6f74 655f 6675  export_remote_fu
-00000bd0: 6e63 7469 6f6e 732e 3c6c 6f63 616c 733e  nctions.<locals>
-00000be0: 2e61 7274 6966 6163 7473 5f74 6f5f 6173  .artifacts_to_as
-00000bf0: 655f 6174 6f6d 7329 0272 3700 0000 721f  e_atoms).r7...r.
-00000c00: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000c10: 0300 0000 0200 0000 5300 0000 7326 0000  ........S...s&..
-00000c20: 0064 0164 0284 007c 0044 0083 017d 0164  .d.d...|.D...}.d
-00000c30: 0364 0284 007c 006a 0044 0083 017d 027c  .d...|.j.D...}.|
-00000c40: 017c 0266 0253 0029 044e 6301 0000 0000  .|.f.S.).Nc.....
-00000c50: 0000 0000 0000 0002 0000 0007 0000 0053  ...............S
-00000c60: 0000 0073 2c00 0000 6700 7c00 5d24 7d01  ...s,...g.|.]$}.
-00000c70: 7c01 6a00 6400 1700 6400 a001 6401 6402  |.j.d...d...d.d.
-00000c80: 8400 7c01 6a02 4400 8301 a101 1700 9102  ..|.j.D.........
-00000c90: 7104 5300 2903 fa01 2063 0100 0000 0000  q.S.)... c......
-00000ca0: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
-00000cb0: 0000 7316 0000 007c 005d 0e7d 0174 007c  ..s....|.].}.t.|
-00000cc0: 0183 0156 0001 0071 0264 0053 0072 3500  ...V...q.d.S.r5.
-00000cd0: 0000 2901 7224 0000 0029 0272 3600 0000  ..).r$...).r6...
-00000ce0: da01 7872 1b00 0000 721b 0000 0072 1c00  ..xr....r....r..
-00000cf0: 0000 723a 0000 0056 0000 0072 3b00 0000  ..r:...V...r;...
-00000d00: 7a5d 5f5f 6578 706f 7274 5f72 656d 6f74  z]__export_remot
-00000d10: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
-00000d20: 616c 733e 2e61 7365 5f61 746f 6d73 5f74  als>.ase_atoms_t
-00000d30: 6f5f 6370 326b 5f69 6e70 7574 5f64 6174  o_cp2k_input_dat
-00000d40: 612e 3c6c 6f63 616c 733e 2e3c 6c69 7374  a.<locals>.<list
-00000d50: 636f 6d70 3e2e 3c67 656e 6578 7072 3e29  comp>.<genexpr>)
-00000d60: 03da 0673 796d 626f 6c72 3f00 0000 da08  ...symbolr?.....
-00000d70: 706f 7369 7469 6f6e 2902 7236 0000 005a  position).r6...Z
-00000d80: 0461 746f 6d72 1b00 0000 721b 0000 0072  .atomr....r....r
-00000d90: 1c00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00000da0: 5600 0000 723b 0000 007a 535f 5f65 7870  V...r;...zS__exp
-00000db0: 6f72 745f 7265 6d6f 7465 5f66 756e 6374  ort_remote_funct
-00000dc0: 696f 6e73 2e3c 6c6f 6361 6c73 3e2e 6173  ions.<locals>.as
-00000dd0: 655f 6174 6f6d 735f 746f 5f63 7032 6b5f  e_atoms_to_cp2k_
-00000de0: 696e 7075 745f 6461 7461 2e3c 6c6f 6361  input_data.<loca
-00000df0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
-00000e00: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000e10: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00000e20: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
-00000e30: 721b 0000 0029 0172 4100 0000 2902 7236  r....).rA...).r6
-00000e40: 0000 00da 0372 6f77 721b 0000 0072 1b00  .....rowr....r..
-00000e50: 0000 721c 0000 0072 4c00 0000 5700 0000  ..r....rL...W...
-00000e60: 723b 0000 0029 01da 0463 656c 6c29 0372  r;...)...cell).r
-00000e70: 3700 0000 da06 636f 6f72 6473 724e 0000  7.....coordsrN..
-00000e80: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000e90: da1c 6173 655f 6174 6f6d 735f 746f 5f63  ..ase_atoms_to_c
-00000ea0: 7032 6b5f 696e 7075 745f 6461 7461 5500  p2k_input_dataU.
-00000eb0: 0000 7306 0000 0000 010e 0110 017a 3f5f  ..s..........z?_
-00000ec0: 5f65 7870 6f72 745f 7265 6d6f 7465 5f66  _export_remote_f
-00000ed0: 756e 6374 696f 6e73 2e3c 6c6f 6361 6c73  unctions.<locals
-00000ee0: 3e2e 6173 655f 6174 6f6d 735f 746f 5f63  >.ase_atoms_to_c
-00000ef0: 7032 6b5f 696e 7075 745f 6461 7461 2903  p2k_input_data).
-00000f00: da08 6261 7365 5f64 6972 7230 0000 00da  ..base_dirr0....
-00000f10: 0764 6174 6173 6574 6303 0000 0000 0000  .datasetc.......
-00000f20: 0000 0000 0010 0000 000b 0000 0013 0000  ................
-00000f30: 0073 9c01 0000 6401 6400 6c00 7d03 6401  .s....d.d.l.}.d.
-00000f40: 6402 6c01 6d02 7d04 0100 6700 7d05 7c02  d.l.m.}...g.}.|.
-00000f50: 4400 5dc6 7d06 8801 7c06 8301 7d07 6400  D.].}...|...}.d.
-00000f60: 7d08 7a56 7c07 8800 6a03 6b02 7258 7c03  }.zV|...j.k.rX|.
-00000f70: 6a04 7405 6a06 a007 7c06 6403 1900 6404  j.t.j...|.d...d.
-00000f80: a102 6405 7c01 6406 8d03 7d08 6e28 7c07  ..d.|.d...}.n(|.
-00000f90: 8800 6a08 6b02 7280 7c03 6a04 7405 6a06  ..j.k.r.|.j.t.j.
-00000fa0: a007 7c06 6403 1900 6407 a102 6408 7c01  ..|.d...d...d.|.
-00000fb0: 6406 8d03 7d08 5700 6e3c 0400 7409 79be  d...}.W.n<..t.y.
-00000fc0: 0100 7d09 0100 7a24 740a 6409 7c06 6403  ..}...z$t.d.|.d.
-00000fd0: 1900 9b00 640a 7c09 9b00 9d04 8301 0100  ....d.|.........
-00000fe0: 5700 5900 6400 7d09 7e09 6e0a 6400 7d09  W.Y.d.}.~.n.d.}.
-00000ff0: 7e09 3000 3000 7c08 6400 7501 721c 740b  ~.0.0.|.d.u.r.t.
-00001000: 7c08 8301 6401 6b04 721c 7c05 a00c 7c06  |...d.k.r.|...|.
-00001010: 7c08 6602 a101 0100 711c 6700 7d0a 740d  |.f.....q.g.}.t.
-00001020: 7c04 7c05 640b 640c 8400 640d 8d02 8301  |.|.d.d...d.....
-00001030: 4400 5d9a 5c02 7d0b 5c02 7d0c 7d0d 740e  D.].\.}.\.}.}.t.
-00001040: 7c0d 8301 7d0d 6401 740b 7c0d 8301 6b02  |...}.d.t.|...k.
-00001050: 9001 7220 71fc 7405 6a06 a007 7c00 7c0c  ..r q.t.j...|.|.
-00001060: a00f 640e 640f a102 a102 7d0e 7c0d 6401  ..d.d.....}.|.d.
-00001070: 1900 6410 1900 7d08 7c0d 6410 6400 8502  ..d...}.|.d.d...
-00001080: 1900 4400 5d12 7d0f 7c08 7c0f 6410 1900  ..D.].}.|.|.d...
-00001090: 3700 7d08 9001 714e 7c08 6a10 7c0e 740b  7.}...qN|.j.|.t.
-000010a0: 7c08 8301 7c01 6411 8d03 0100 7c0a a00c  |...|.d.....|...
-000010b0: 7c0e 8800 6a11 7c0d 6401 1900 6401 1900  |...j.|.d...d...
-000010c0: 6412 1900 6413 9c03 a101 0100 71fc 7c0a  d...d.......q.|.
-000010d0: 5300 2914 4e72 0100 0000 2901 da07 6772  S.).Nr....)...gr
-000010e0: 6f75 7062 7972 2000 0000 da06 6f75 7470  oupbyr .....outp
-000010f0: 7574 720e 0000 0029 02da 0366 6d74 7230  utr....)...fmtr0
-00001100: 0000 005a 064f 5554 4341 527a 0b76 6173  ...Z.OUTCARz.vas
-00001110: 702f 6f75 7463 6172 7a0f 6661 696c 6564  p/outcarz.failed
-00001120: 2074 6f20 6c6f 6164 207a 023a 2063 0100   to load z.: c..
-00001130: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001140: 0000 5300 0000 7310 0000 007c 0064 0119  ..S...s....|.d..
-00001150: 0064 0219 0064 0319 0053 0029 044e 7201  .d...d...S.).Nr.
-00001160: 0000 0072 2c00 0000 da08 616e 6365 7374  ...r,.....ancest
-00001170: 6f72 721b 0000 0029 0172 4900 0000 721b  orr....).rI...r.
-00001180: 0000 0072 1b00 0000 721c 0000 00da 083c  ...r....r......<
-00001190: 6c61 6d62 6461 3e75 0000 0072 3b00 0000  lambda>u...r;...
-000011a0: 7a4a 5f5f 6578 706f 7274 5f72 656d 6f74  zJ__export_remot
-000011b0: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
-000011c0: 616c 733e 2e63 6f6e 7665 7274 5f74 6f5f  als>.convert_to_
-000011d0: 6465 6570 6d64 5f6e 7079 2e3c 6c6f 6361  deepmd_npy.<loca
-000011e0: 6c73 3e2e 3c6c 616d 6264 613e 2901 da03  ls>.<lambda>)...
-000011f0: 6b65 79fa 012f da01 5f72 0a00 0000 2902  key../.._r....).
-00001200: 5a08 7365 745f 7369 7a65 7230 0000 0072  Z.set_sizer0...r
-00001210: 2c00 0000 2903 7220 0000 0072 2100 0000  ,...).r ...r!...
-00001220: 722c 0000 0029 12da 0664 7064 6174 61da  r,...)...dpdata.
-00001230: 0969 7465 7274 6f6f 6c73 7253 0000 0072  .itertoolsrS...r
-00001240: 1300 0000 5a0d 4c61 6265 6c65 6453 7973  ....Z.LabeledSys
-00001250: 7465 6d72 2600 0000 7227 0000 0072 3f00  temr&...r'...r?.
-00001260: 0000 7214 0000 00da 0945 7863 6570 7469  ..r......Excepti
-00001270: 6f6e da05 7072 696e 74da 036c 656e da06  on..print..len..
-00001280: 6170 7065 6e64 da09 656e 756d 6572 6174  append..enumerat
-00001290: 6572 4100 0000 da07 7265 706c 6163 655a  erA.....replaceZ
-000012a0: 0d74 6f5f 6465 6570 6d64 5f6e 7079 7217  .to_deepmd_npyr.
-000012b0: 0000 0029 1072 5100 0000 7230 0000 0072  ...).rQ...r0...r
-000012c0: 5200 0000 725b 0000 0072 5300 0000 5a0e  R...r[...rS...Z.
-000012d0: 6470 5f73 7973 7465 6d5f 6c69 7374 da04  dp_system_list..
-000012e0: 6461 7461 7244 0000 005a 0964 705f 7379  datarD...Z.dp_sy
-000012f0: 7374 656d da01 65da 0b6f 7574 7075 745f  stem..e..output_
-00001300: 6469 7273 da01 6972 5800 0000 5a0f 6470  dirs..irX...Z.dp
-00001310: 5f73 7973 7465 6d5f 6772 6f75 705a 0a6f  _system_groupZ.o
-00001320: 7574 7075 745f 6469 72da 0469 7465 6d29  utput_dir..item)
-00001330: 0272 1d00 0000 722b 0000 0072 1b00 0000  .r....r+...r....
-00001340: 721c 0000 00da 1563 6f6e 7665 7274 5f74  r......convert_t
-00001350: 6f5f 6465 6570 6d64 5f6e 7079 5b00 0000  o_deepmd_npy[...
-00001360: 733c 0000 0000 0508 010c 0204 0108 0108  s<..............
-00001370: 0104 0102 010a 0120 010a 0122 010e 012e  ....... ..."....
-00001380: 0314 0110 0204 0220 0108 010e 0102 0216  ....... ........
-00001390: 020c 0110 0110 0214 0206 0104 010e fe0a  ................
-000013a0: 037a 385f 5f65 7870 6f72 745f 7265 6d6f  .z8__export_remo
-000013b0: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
-000013c0: 6361 6c73 3e2e 636f 6e76 6572 745f 746f  cals>.convert_to
-000013d0: 5f64 6565 706d 645f 6e70 7929 03da 0773  _deepmd_npy)...s
-000013e0: 7973 7465 6d73 7251 0000 0072 3000 0000  ystemsrQ...r0...
-000013f0: 6303 0000 0000 0000 0000 0000 0009 0000  c...............
-00001400: 0007 0000 0013 0000 0073 6800 0000 6700  .........sh...g.
-00001410: 7d03 8800 7c00 7c02 6401 8d02 7d04 7400  }...|.|.d...}.t.
-00001420: 7c04 8301 4400 5d4a 5c02 7d05 5c02 7d06  |...D.]J\.}.\.}.
-00001430: 7d07 7401 6a02 a003 7c01 7c05 6402 9b04  }.t.j...|.|.d...
-00001440: 6403 9d02 a102 7d08 7404 6a05 6a06 7c08  d.....}.t.j.j.|.
-00001450: 7c07 6404 7c02 6405 8d04 0100 7c03 a007  |.d.|.d.....|...
-00001460: 7c08 7c06 6406 1900 6407 9c02 a101 0100  |.|.d...d.......
-00001470: 7118 7c03 5300 2908 4e29 0172 3000 0000  q.|.S.).N).r0...
-00001480: 5a03 3036 647a 0c2e 6c61 6d6d 7073 2e64  Z.06dz..lammps.d
-00001490: 6174 617a 0b6c 616d 6d70 732d 6461 7461  ataz.lammps-data
-000014a0: 2902 7221 0000 0072 3400 0000 722c 0000  ).r!...r4...r,..
-000014b0: 0029 0272 2000 0000 722c 0000 0029 0872  .).r ...r,...).r
-000014c0: 6100 0000 7226 0000 0072 2700 0000 723f  a...r&...r'...r?
-000014d0: 0000 0072 3c00 0000 723d 0000 00da 0577  ...r<...r=.....w
-000014e0: 7269 7465 7260 0000 0029 0972 6900 0000  riter`...).ri...
-000014f0: 7251 0000 0072 3000 0000 5a0a 6461 7461  rQ...r0...Z.data
-00001500: 5f66 696c 6573 7245 0000 0072 6600 0000  _filesrE...rf...
-00001510: 721e 0000 0072 3700 0000 5a09 6461 7461  r....r7...Z.data
-00001520: 5f66 696c 6529 0172 4700 0000 721b 0000  _file).rG...r...
-00001530: 0072 1c00 0000 da1c 636f 6e76 6572 745f  .r......convert_
-00001540: 746f 5f6c 616d 6d70 735f 696e 7075 745f  to_lammps_input_
-00001550: 6461 7461 8800 0000 7314 0000 0000 0104  data....s.......
-00001560: 010c 0114 0116 0114 0104 0102 0106 fe0a  ................
-00001570: 047a 3f5f 5f65 7870 6f72 745f 7265 6d6f  .z?__export_remo
-00001580: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
-00001590: 6361 6c73 3e2e 636f 6e76 6572 745f 746f  cals>.convert_to
-000015a0: 5f6c 616d 6d70 735f 696e 7075 745f 6461  _lammps_input_da
-000015b0: 7461 2909 da04 6469 6374 7207 0000 0072  ta)...dictr....r
-000015c0: 2400 0000 7205 0000 00da 0369 6e74 7203  $...r......intr.
-000015d0: 0000 0072 0600 0000 7208 0000 00da 0566  ...r....r......f
-000015e0: 6c6f 6174 2903 7250 0000 0072 6800 0000  loat).rP...rh...
-000015f0: 726b 0000 0072 1b00 0000 2904 721d 0000  rk...r....).r...
-00001600: 0072 2e00 0000 7247 0000 0072 2b00 0000  .r....rG...r+...
-00001610: 721c 0000 00da 195f 5f65 7870 6f72 745f  r......__export_
-00001620: 7265 6d6f 7465 5f66 756e 6374 696f 6e73  remote_functions
-00001630: 0e00 0000 7322 0000 0000 030e 1218 1318  ....s"..........
-00001640: 042e 1b24 0702 0106 0106 fd12 2d1e 0d02  ...$........-...
-00001650: 0102 0102 0102 0102 0102 fa72 6f00 0000  ...........ro...
-00001660: 291a da15 6169 325f 6b69 742e 636f 7265  )...ai2_kit.core
-00001670: 2e61 7274 6966 6163 7472 0200 0000 7203  .artifactr....r.
-00001680: 0000 00da 1161 6932 5f6b 6974 2e63 6f72  .....ai2_kit.cor
-00001690: 652e 7574 696c 7204 0000 00da 0674 7970  e.utilr......typ
-000016a0: 696e 6772 0500 0000 7206 0000 0072 0700  ingr....r....r..
-000016b0: 0000 723c 0000 0072 0800 0000 da08 6f70  ..r<...r......op
-000016c0: 6572 6174 6f72 7209 0000 005a 0661 7365  eratorr....Z.ase
-000016d0: 2e69 6f72 2600 0000 da08 636f 6e73 7461  .ior&.....consta
-000016e0: 6e74 720b 0000 0072 0c00 0000 720d 0000  ntr....r....r...
-000016f0: 0072 6f00 0000 7247 0000 0072 5000 0000  .ro...rG...rP...
-00001700: 7268 0000 0072 6b00 0000 721d 0000 0072  rh...rk...r....r
-00001710: 2b00 0000 721b 0000 0072 1b00 0000 721b  +...r....r....r.
-00001720: 0000 0072 1c00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001730: 653e 0100 0000 7324 0000 0010 010c 0214  e>....s$........
-00001740: 010c 020c 0108 0108 0214 0308 7f00 1704  ................
-00001750: f902 0102 0102 0102 0102 0102 0102 fa    ...............
+00000020: 0006 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
+00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
+00000060: 5a06 6400 6404 6c09 5a09 6405 6406 8400  Z.d.d.l.Z.d.d...
+00000070: 5a0a 650a 8300 5c06 5a0b 5a0c 5a0d 5a0e  Z.e...\.Z.Z.Z.Z.
+00000080: 5a0f 5a10 6404 5300 2907 e900 0000 0029  Z.Z.d.S.)......)
+00000090: 01da 0c41 7274 6966 6163 7444 6963 7429  ...ArtifactDict)
+000000a0: 03da 044c 6973 74da 0554 7570 6c65 da08  ...List..Tuple..
+000000b0: 4f70 7469 6f6e 616c 2901 da05 4174 6f6d  Optional)...Atom
+000000c0: 734e 6300 0000 0000 0000 0000 0000 0003  sNc.............
+000000d0: 0000 0006 0000 0003 0000 0073 c400 0000  ...........s....
+000000e0: 4700 6401 6402 8400 6402 8302 8900 7400  G.d.d...d.....t.
+000000f0: 7401 7402 1900 6403 9c02 8700 6601 6404  t.t...d.....f.d.
+00000100: 6405 840c 8902 7403 7404 1900 7403 7402  d.....t.t...t.t.
+00000110: 1900 7403 7405 7404 7406 6602 1900 1900  ..t.t.t.t.f.....
+00000120: 6406 9c03 8700 8702 6602 6407 6408 840c  d.......f.d.d...
+00000130: 8901 7406 7405 7403 7402 1900 7403 7403  ..t.t.t.t...t.t.
+00000140: 7407 1900 1900 6602 1900 6409 9c02 640a  t.....f...d...d.
+00000150: 640b 8404 7d00 7402 7403 7402 1900 7403  d...}.t.t.t...t.
+00000160: 7404 1900 640c 9c03 8700 8702 6602 640d  t...d.......f.d.
+00000170: 640e 840c 7d01 7403 7404 1900 7402 7403  d...}.t.t...t.t.
+00000180: 7402 1900 640f 9c03 8701 6601 6410 6411  t...d.....f.d.d.
+00000190: 840c 7d02 8801 7c00 7c01 7c02 8800 8802  ..}...|.|.|.....
+000001a0: 6606 5300 2912 7a20 776f 726b 6172 6f75  f.S.).z workarou
+000001b0: 6e64 2066 6f72 2063 6c6f 7564 7069 636b  nd for cloudpick
+000001c0: 6c65 2069 7373 7565 6300 0000 0000 0000  le issuec.......
+000001d0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+000001e0: 0073 3400 0000 6500 5a01 6400 5a02 6401  .s4...e.Z.d.Z.d.
+000001f0: 5a03 6402 5a04 6403 5a05 6404 5a06 6405  Z.d.Z.d.Z.d.Z.d.
+00000200: 5a07 6406 5a08 6407 5a09 6408 5a0a 6409  Z.d.Z.d.Z.d.Z.d.
+00000210: 5a0b 640a 5a0c 640b 5300 290c 7a2d 5f5f  Z.d.Z.d.S.).z-__
+00000220: 6578 706f 7274 5f72 656d 6f74 655f 6675  export_remote_fu
+00000230: 6e63 7469 6f6e 732e 3c6c 6f63 616c 733e  nctions.<locals>
+00000240: 2e44 6174 6146 6f72 6d61 747a 0f63 7032  .DataFormatz.cp2
+00000250: 6b2f 6f75 7470 7574 5f64 6972 7a0f 7661  k/output_dirz.va
+00000260: 7370 2f6f 7574 7075 745f 6469 727a 116c  sp/output_dirz.l
+00000270: 616d 6d70 732f 6f75 7470 7574 5f64 6972  ammps/output_dir
+00000280: 7a11 6465 6570 6d64 2f6f 7574 7075 745f  z.deepmd/output_
+00000290: 6469 727a 0a64 6565 706d 642f 6e70 797a  dirz.deepmd/npyz
+000002a0: 166c 6173 702b 6c61 6d6d 7073 2f6f 7574  .lasp+lammps/out
+000002b0: 7075 745f 6469 72fa 0b63 7032 6b2f 6f75  put_dir..cp2k/ou
+000002c0: 7470 7574 7a08 7661 7370 2f78 6d6c da06  tputz.vasp/xml..
+000002d0: 6578 7478 797a 7a0b 7661 7370 2f70 6f73  extxyzz.vasp/pos
+000002e0: 6361 724e 290d da08 5f5f 6e61 6d65 5f5f  carN)...__name__
+000002f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000300: 7175 616c 6e61 6d65 5f5f da0f 4350 324b  qualname__..CP2K
+00000310: 5f4f 5554 5055 545f 4449 52da 0f56 4153  _OUTPUT_DIR..VAS
+00000320: 505f 4f55 5450 5554 5f44 4952 5a11 4c41  P_OUTPUT_DIRZ.LA
+00000330: 4d4d 5053 5f4f 5554 5055 545f 4449 52da  MMPS_OUTPUT_DIR.
+00000340: 1144 4545 504d 445f 4f55 5450 5554 5f44  .DEEPMD_OUTPUT_D
+00000350: 4952 da0a 4445 4550 4d44 5f4e 5059 5a13  IR..DEEPMD_NPYZ.
+00000360: 4c41 5350 5f4c 414d 4d50 535f 4f55 545f  LASP_LAMMPS_OUT_
+00000370: 4449 525a 0b43 5032 4b5f 4f55 5450 5554  DIRZ.CP2K_OUTPUT
+00000380: 5a08 5641 5350 5f58 4d4c da06 4558 5458  Z.VASP_XML..EXTX
+00000390: 595a da0b 5641 5350 5f50 4f53 4341 52a9  YZ..VASP_POSCAR.
+000003a0: 0072 1200 0000 7212 0000 00fa 2e2f 686f  .r....r....../ho
+000003b0: 6d65 2f68 656e 7279 2f73 7263 2f61 6932  me/henry/src/ai2
+000003c0: 2d6b 6974 2f61 6932 5f6b 6974 2f64 6f6d  -kit/ai2_kit/dom
+000003d0: 6169 6e2f 6461 7461 2e70 79da 0a44 6174  ain/data.py..Dat
+000003e0: 6146 6f72 6d61 740d 0000 0073 1400 0000  aFormat....s....
+000003f0: 0802 0401 0401 0401 0401 0401 0403 0401  ................
+00000400: 0403 0401 7214 0000 0029 02da 0861 7274  ....r....)...art
+00000410: 6966 6163 74da 0672 6574 7572 6e63 0100  ifact..returnc..
+00000420: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00000430: 0000 1300 0000 7370 0000 007c 00a0 0064  ......sp...|...d
+00000440: 01a1 017d 0174 017c 0174 0283 0273 264a  ...}.t.|.t...s&J
+00000450: 0064 0274 037c 0183 019b 009d 0283 0182  .d.t.|..........
+00000460: 0174 046a 05a0 067c 01a1 017d 027c 00a0  .t.j...|...}.|..
+00000470: 0064 03a1 017d 037c 0372 4e74 017c 0374  .d...}.|.rNt.|.t
+00000480: 0283 0272 4e7c 0353 007c 02a0 0764 04a1  ...rN|.S.|...d..
+00000490: 0172 5e88 006a 0853 0064 057c 0276 0072  .r^..j.S.d.|.v.r
+000004a0: 6c88 006a 0953 0064 0653 0029 077a 960a  l..j.S.d.S.).z..
+000004b0: 2020 2020 2020 2020 4765 7420 286f 7220          Get (or 
+000004c0: 6775 6573 7329 2064 6174 6120 7479 7065  guess) data type
+000004d0: 2066 726f 6d20 6172 7469 6661 6374 2064   from artifact d
+000004e0: 6963 740a 2020 2020 2020 2020 4e6f 7465  ict.        Note
+000004f0: 3a20 5468 6520 7265 6173 6f6e 206f 6620  : The reason of 
+00000500: 7573 696e 6720 6469 6374 2069 6e73 7465  using dict inste
+00000510: 6164 206f 6620 4172 7469 6661 6374 2069  ad of Artifact i
+00000520: 7320 4172 7469 6661 6374 2069 7320 6e6f  s Artifact is no
+00000530: 7420 7069 636b 6c65 6162 6c65 0a20 2020  t pickleable.   
+00000540: 2020 2020 20da 0375 726c 7a15 7572 6c20       ..urlz.url 
+00000550: 6d75 7374 2062 6520 7374 722c 2067 6f74  must be str, got
+00000560: 20da 0666 6f72 6d61 747a 042e 7879 7a5a   ..formatz..xyzZ
+00000570: 0650 4f53 4341 524e 290a da03 6765 74da  .POSCARN)...get.
+00000580: 0a69 7369 6e73 7461 6e63 65da 0373 7472  .isinstance..str
+00000590: da04 7479 7065 da02 6f73 da04 7061 7468  ..type..os..path
+000005a0: da08 6261 7365 6e61 6d65 da08 656e 6473  ..basename..ends
+000005b0: 7769 7468 7210 0000 0072 1100 0000 2904  withr....r....).
+000005c0: 7215 0000 0072 1700 0000 da09 6669 6c65  r....r......file
+000005d0: 5f6e 616d 6572 1800 0000 2901 7214 0000  _namer....).r...
+000005e0: 0072 1200 0000 7213 0000 00da 0f67 6574  .r....r......get
+000005f0: 5f64 6174 615f 666f 726d 6174 1f00 0000  _data_format....
+00000600: 7316 0000 0000 050a 011c 020c 010a 010e  s...............
+00000610: 0104 010a 0106 0108 0106 017a 325f 5f65  ...........z2__e
+00000620: 7870 6f72 745f 7265 6d6f 7465 5f66 756e  xport_remote_fun
+00000630: 6374 696f 6e73 2e3c 6c6f 6361 6c73 3e2e  ctions.<locals>.
+00000640: 6765 745f 6461 7461 5f66 6f72 6d61 7429  get_data_format)
+00000650: 03da 0961 7274 6966 6163 7473 da08 7479  ...artifacts..ty
+00000660: 7065 5f6d 6170 7216 0000 0063 0200 0000  pe_mapr....c....
+00000670: 0000 0000 0000 0000 0600 0000 0600 0000  ................
+00000680: 1300 0000 7384 0000 0067 007d 027c 0044  ....s....g.}.|.D
+00000690: 005d 7689 0088 0288 0083 017d 0388 0064  .]v........}...d
+000006a0: 0119 007d 047c 0388 016a 006b 0272 3a74  ...}.|...j.k.r:t
+000006b0: 016a 026a 037c 0464 0264 0364 048d 037d  .j.j.|.d.d.d...}
+000006c0: 056e 2c7c 0388 016a 046b 0272 5874 016a  .n,|...j.k.rXt.j
+000006d0: 026a 037c 0464 0264 0564 048d 037d 056e  .j.|.d.d.d...}.n
+000006e0: 0e74 0564 067c 039b 009d 0283 0182 017c  .t.d.|.........|
+000006f0: 02a0 0687 0066 0164 0764 0884 087c 0544  .....f.d.d...|.D
+00000700: 0083 01a1 0101 0071 087c 0253 0029 094e  .......q.|.S.).N
+00000710: 7217 0000 00fa 013a da04 7661 7370 2901  r......:..vasp).
+00000720: 7218 0000 0072 0800 0000 7a19 756e 7375  r....r....z.unsu
+00000730: 7070 6f72 7465 6420 6461 7461 2066 6f72  pported data for
+00000740: 6d61 743a 2063 0100 0000 0000 0000 0000  mat: c..........
+00000750: 0000 0200 0000 0300 0000 3300 0000 7316  ..........3...s.
+00000760: 0000 007c 005d 0e7d 0188 007c 0166 0256  ...|.].}...|.f.V
+00000770: 0001 0071 0264 0053 00a9 014e 7212 0000  ...q.d.S...Nr...
+00000780: 0029 02da 022e 30da 0561 746f 6d73 a901  .)....0..atoms..
+00000790: da01 6172 1200 0000 7213 0000 00da 093c  ..ar....r......<
+000007a0: 6765 6e65 7870 723e 3d00 0000 f300 0000  genexpr>=.......
+000007b0: 007a 4c5f 5f65 7870 6f72 745f 7265 6d6f  .zL__export_remo
+000007c0: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
+000007d0: 6361 6c73 3e2e 6172 7469 6661 6374 735f  cals>.artifacts_
+000007e0: 746f 5f61 7365 5f61 746f 6d73 2e3c 6c6f  to_ase_atoms.<lo
+000007f0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
+00000800: 0772 1100 0000 da03 6173 65da 0269 6fda  .r......ase..io.
+00000810: 0472 6561 6472 1000 0000 da0a 5661 6c75  .readr......Valu
+00000820: 6545 7272 6f72 da06 6578 7465 6e64 2906  eError..extend).
+00000830: 7223 0000 0072 2400 0000 da07 7265 7375  r#...r$.....resu
+00000840: 6c74 73da 0b64 6174 615f 666f 726d 6174  lts..data_format
+00000850: 7217 0000 00da 0a61 746f 6d73 5f6c 6973  r......atoms_lis
+00000860: 74a9 0272 1400 0000 7222 0000 0072 2a00  t..r....r"...r*.
+00000870: 0000 7213 0000 00da 1661 7274 6966 6163  ..r......artifac
+00000880: 7473 5f74 6f5f 6173 655f 6174 6f6d 7332  ts_to_ase_atoms2
+00000890: 0000 0073 1600 0000 0001 0401 0801 0801  ...s............
+000008a0: 0801 0a01 1401 0a01 1402 0e01 1a01 7a39  ..............z9
+000008b0: 5f5f 6578 706f 7274 5f72 656d 6f74 655f  __export_remote_
+000008c0: 6675 6e63 7469 6f6e 732e 3c6c 6f63 616c  functions.<local
+000008d0: 733e 2e61 7274 6966 6163 7473 5f74 6f5f  s>.artifacts_to_
+000008e0: 6173 655f 6174 6f6d 7329 0272 2900 0000  ase_atoms).r)...
+000008f0: 7216 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000900: 0000 0300 0000 0200 0000 5300 0000 7326  ..........S...s&
+00000910: 0000 0064 0164 0284 007c 0044 0083 017d  ...d.d...|.D...}
+00000920: 0164 0364 0284 007c 006a 0044 0083 017d  .d.d...|.j.D...}
+00000930: 027c 017c 0266 0253 0029 044e 6301 0000  .|.|.f.S.).Nc...
+00000940: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+00000950: 0053 0000 0073 2c00 0000 6700 7c00 5d24  .S...s,...g.|.]$
+00000960: 7d01 7c01 6a00 6400 1700 6400 a001 6401  }.|.j.d...d...d.
+00000970: 6402 8400 7c01 6a02 4400 8301 a101 1700  d...|.j.D.......
+00000980: 9102 7104 5300 2903 fa01 2063 0100 0000  ..q.S.)... c....
+00000990: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000009a0: 7300 0000 7316 0000 007c 005d 0e7d 0174  s...s....|.].}.t
+000009b0: 007c 0183 0156 0001 0071 0264 0053 0072  .|...V...q.d.S.r
+000009c0: 2700 0000 2901 721b 0000 0029 0272 2800  '...).r....).r(.
+000009d0: 0000 da01 7872 1200 0000 7212 0000 0072  ....xr....r....r
+000009e0: 1300 0000 722c 0000 0042 0000 0072 2d00  ....r,...B...r-.
+000009f0: 0000 7a5d 5f5f 6578 706f 7274 5f72 656d  ..z]__export_rem
+00000a00: 6f74 655f 6675 6e63 7469 6f6e 732e 3c6c  ote_functions.<l
+00000a10: 6f63 616c 733e 2e61 7365 5f61 746f 6d73  ocals>.ase_atoms
+00000a20: 5f74 6f5f 6370 326b 5f69 6e70 7574 5f64  _to_cp2k_input_d
+00000a30: 6174 612e 3c6c 6f63 616c 733e 2e3c 6c69  ata.<locals>.<li
+00000a40: 7374 636f 6d70 3e2e 3c67 656e 6578 7072  stcomp>.<genexpr
+00000a50: 3e29 03da 0673 796d 626f 6cda 046a 6f69  >)...symbol..joi
+00000a60: 6eda 0870 6f73 6974 696f 6e29 0272 2800  n..position).r(.
+00000a70: 0000 5a04 6174 6f6d 7212 0000 0072 1200  ..Z.atomr....r..
+00000a80: 0000 7213 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00000a90: 6d70 3e42 0000 0072 2d00 0000 7a53 5f5f  mp>B...r-...zS__
+00000aa0: 6578 706f 7274 5f72 656d 6f74 655f 6675  export_remote_fu
+00000ab0: 6e63 7469 6f6e 732e 3c6c 6f63 616c 733e  nctions.<locals>
+00000ac0: 2e61 7365 5f61 746f 6d73 5f74 6f5f 6370  .ase_atoms_to_cp
+00000ad0: 326b 5f69 6e70 7574 5f64 6174 612e 3c6c  2k_input_data.<l
+00000ae0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000af0: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+00000b00: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00000b10: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
+00000b20: 0453 0072 1200 0000 2901 da04 6c69 7374  .S.r....)...list
+00000b30: 2902 7228 0000 00da 0372 6f77 7212 0000  ).r(.....rowr...
+00000b40: 0072 1200 0000 7213 0000 0072 3d00 0000  .r....r....r=...
+00000b50: 4300 0000 722d 0000 0029 01da 0463 656c  C...r-...)...cel
+00000b60: 6c29 0372 2900 0000 da06 636f 6f72 6473  l).r).....coords
+00000b70: 7240 0000 0072 1200 0000 7212 0000 0072  r@...r....r....r
+00000b80: 1300 0000 da1c 6173 655f 6174 6f6d 735f  ......ase_atoms_
+00000b90: 746f 5f63 7032 6b5f 696e 7075 745f 6461  to_cp2k_input_da
+00000ba0: 7461 4100 0000 7306 0000 0000 010e 0110  taA...s.........
+00000bb0: 017a 3f5f 5f65 7870 6f72 745f 7265 6d6f  .z?__export_remo
+00000bc0: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
+00000bd0: 6361 6c73 3e2e 6173 655f 6174 6f6d 735f  cals>.ase_atoms_
+00000be0: 746f 5f63 7032 6b5f 696e 7075 745f 6461  to_cp2k_input_da
+00000bf0: 7461 2903 da08 6261 7365 5f64 6972 7224  ta)...base_dirr$
+00000c00: 0000 00da 0764 6174 6173 6574 6303 0000  .....datasetc...
+00000c10: 0000 0000 0000 0000 0010 0000 000b 0000  ................
+00000c20: 0013 0000 0073 9c01 0000 6401 6400 6c00  .....s....d.d.l.
+00000c30: 7d03 6401 6402 6c01 6d02 7d04 0100 6700  }.d.d.l.m.}...g.
+00000c40: 7d05 7c02 4400 5dc6 7d06 8801 7c06 8301  }.|.D.].}...|...
+00000c50: 7d07 6400 7d08 7a56 7c07 8800 6a03 6b02  }.d.}.zV|...j.k.
+00000c60: 7258 7c03 6a04 7405 6a06 a007 7c06 6403  rX|.j.t.j...|.d.
+00000c70: 1900 6404 a102 6405 7c01 6406 8d03 7d08  ..d...d.|.d...}.
+00000c80: 6e28 7c07 8800 6a08 6b02 7280 7c03 6a04  n(|...j.k.r.|.j.
+00000c90: 7405 6a06 a007 7c06 6403 1900 6407 a102  t.j...|.d...d...
+00000ca0: 6408 7c01 6406 8d03 7d08 5700 6e3c 0400  d.|.d...}.W.n<..
+00000cb0: 7409 79be 0100 7d09 0100 7a24 740a 6409  t.y...}...z$t.d.
+00000cc0: 7c06 6403 1900 9b00 640a 7c09 9b00 9d04  |.d.....d.|.....
+00000cd0: 8301 0100 5700 5900 6400 7d09 7e09 6e0a  ....W.Y.d.}.~.n.
+00000ce0: 6400 7d09 7e09 3000 3000 7c08 6400 7501  d.}.~.0.0.|.d.u.
+00000cf0: 721c 740b 7c08 8301 6401 6b04 721c 7c05  r.t.|...d.k.r.|.
+00000d00: a00c 7c06 7c08 6602 a101 0100 711c 6700  ..|.|.f.....q.g.
+00000d10: 7d0a 740d 7c04 7c05 640b 640c 8400 640d  }.t.|.|.d.d...d.
+00000d20: 8d02 8301 4400 5d9a 5c02 7d0b 5c02 7d0c  ....D.].\.}.\.}.
+00000d30: 7d0d 740e 7c0d 8301 7d0d 6401 740b 7c0d  }.t.|...}.d.t.|.
+00000d40: 8301 6b02 9001 7220 71fc 7405 6a06 a007  ..k...r q.t.j...
+00000d50: 7c00 7c0c a00f 640e 640f a102 a102 7d0e  |.|...d.d.....}.
+00000d60: 7c0d 6401 1900 6410 1900 7d08 7c0d 6410  |.d...d...}.|.d.
+00000d70: 6400 8502 1900 4400 5d12 7d0f 7c08 7c0f  d.....D.].}.|.|.
+00000d80: 6410 1900 3700 7d08 9001 714e 7c08 6a10  d...7.}...qN|.j.
+00000d90: 7c0e 740b 7c08 8301 7c01 6411 8d03 0100  |.t.|...|.d.....
+00000da0: 7c0a a00c 7c0e 8800 6a11 7c0d 6401 1900  |...|...j.|.d...
+00000db0: 6401 1900 6412 1900 6413 9c03 a101 0100  d...d...d.......
+00000dc0: 71fc 7c0a 5300 2914 4e72 0100 0000 2901  q.|.S.).Nr....).
+00000dd0: da07 6772 6f75 7062 7972 1700 0000 da06  ..groupbyr......
+00000de0: 6f75 7470 7574 7207 0000 0029 02da 0366  outputr....)...f
+00000df0: 6d74 7224 0000 005a 064f 5554 4341 527a  mtr$...Z.OUTCARz
+00000e00: 0b76 6173 702f 6f75 7463 6172 7a0f 6661  .vasp/outcarz.fa
+00000e10: 696c 6564 2074 6f20 6c6f 6164 207a 023a  iled to load z.:
+00000e20: 2063 0100 0000 0000 0000 0000 0000 0100   c..............
+00000e30: 0000 0200 0000 5300 0000 7310 0000 007c  ......S...s....|
+00000e40: 0064 0119 0064 0219 0064 0319 0053 0029  .d...d...d...S.)
+00000e50: 044e 7201 0000 00da 0561 7474 7273 da08  .Nr......attrs..
+00000e60: 616e 6365 7374 6f72 7212 0000 0029 0172  ancestorr....).r
+00000e70: 3900 0000 7212 0000 0072 1200 0000 7213  9...r....r....r.
+00000e80: 0000 00da 083c 6c61 6d62 6461 3e61 0000  .....<lambda>a..
+00000e90: 0072 2d00 0000 7a4a 5f5f 6578 706f 7274  .r-...zJ__export
+00000ea0: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
+00000eb0: 732e 3c6c 6f63 616c 733e 2e63 6f6e 7665  s.<locals>.conve
+00000ec0: 7274 5f74 6f5f 6465 6570 6d64 5f6e 7079  rt_to_deepmd_npy
+00000ed0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00000ee0: 613e 2901 da03 6b65 79fa 012f da01 5fe9  a>)...key../.._.
+00000ef0: 0100 0000 2902 5a08 7365 745f 7369 7a65  ....).Z.set_size
+00000f00: 7224 0000 0072 4800 0000 2903 7217 0000  r$...rH...).r...
+00000f10: 0072 1800 0000 7248 0000 0029 12da 0664  .r....rH...)...d
+00000f20: 7064 6174 61da 0969 7465 7274 6f6f 6c73  pdata..itertools
+00000f30: 7245 0000 0072 0c00 0000 5a0d 4c61 6265  rE...r....Z.Labe
+00000f40: 6c65 6453 7973 7465 6d72 1d00 0000 721e  ledSystemr....r.
+00000f50: 0000 0072 3b00 0000 720d 0000 00da 0945  ...r;...r......E
+00000f60: 7863 6570 7469 6f6e da05 7072 696e 74da  xception..print.
+00000f70: 036c 656e da06 6170 7065 6e64 da09 656e  .len..append..en
+00000f80: 756d 6572 6174 6572 3e00 0000 da07 7265  umerater>.....re
+00000f90: 706c 6163 655a 0d74 6f5f 6465 6570 6d64  placeZ.to_deepmd
+00000fa0: 5f6e 7079 720f 0000 0029 1072 4300 0000  _npyr....).rC...
+00000fb0: 7224 0000 0072 4400 0000 724f 0000 0072  r$...rD...rO...r
+00000fc0: 4500 0000 5a0e 6470 5f73 7973 7465 6d5f  E...Z.dp_system_
+00000fd0: 6c69 7374 da04 6461 7461 7234 0000 005a  list..datar4...Z
+00000fe0: 0964 705f 7379 7374 656d da01 65da 0b6f  .dp_system..e..o
+00000ff0: 7574 7075 745f 6469 7273 da01 6972 4b00  utput_dirs..irK.
+00001000: 0000 5a0f 6470 5f73 7973 7465 6d5f 6772  ..Z.dp_system_gr
+00001010: 6f75 705a 0a6f 7574 7075 745f 6469 72da  oupZ.output_dir.
+00001020: 0469 7465 6d72 3600 0000 7212 0000 0072  .itemr6...r....r
+00001030: 1300 0000 da15 636f 6e76 6572 745f 746f  ......convert_to
+00001040: 5f64 6565 706d 645f 6e70 7947 0000 0073  _deepmd_npyG...s
+00001050: 3c00 0000 0005 0801 0c02 0401 0801 0801  <...............
+00001060: 0401 0201 0a01 2001 0a01 2201 0e01 2e03  ...... ...".....
+00001070: 1401 1002 0402 2001 0801 0e01 0202 1602  ...... .........
+00001080: 0c01 1001 1002 1402 0601 0401 0efe 0a03  ................
+00001090: 7a38 5f5f 6578 706f 7274 5f72 656d 6f74  z8__export_remot
+000010a0: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
+000010b0: 616c 733e 2e63 6f6e 7665 7274 5f74 6f5f  als>.convert_to_
+000010c0: 6465 6570 6d64 5f6e 7079 2903 da07 7379  deepmd_npy)...sy
+000010d0: 7374 656d 7372 4300 0000 7224 0000 0063  stemsrC...r$...c
+000010e0: 0300 0000 0000 0000 0000 0000 0900 0000  ................
+000010f0: 0700 0000 1300 0000 7368 0000 0067 007d  ........sh...g.}
+00001100: 0388 007c 007c 0264 018d 027d 0474 007c  ...|.|.d...}.t.|
+00001110: 0483 0144 005d 4a5c 027d 055c 027d 067d  ...D.]J\.}.\.}.}
+00001120: 0774 016a 02a0 037c 017c 0564 029b 0464  .t.j...|.|.d...d
+00001130: 039d 02a1 027d 0874 046a 056a 067c 087c  .....}.t.j.j.|.|
+00001140: 0764 047c 0264 058d 0401 007c 03a0 077c  .d.|.d.....|...|
+00001150: 087c 0664 0619 0064 079c 02a1 0101 0071  .|.d...d.......q
+00001160: 187c 0353 0029 084e 2901 7224 0000 005a  .|.S.).N).r$...Z
+00001170: 0330 3664 7a0c 2e6c 616d 6d70 732e 6461  .06dz..lammps.da
+00001180: 7461 7a0b 6c61 6d6d 7073 2d64 6174 6129  taz.lammps-data)
+00001190: 0272 1800 0000 5a09 7370 6563 6f72 6465  .r....Z.specorde
+000011a0: 7272 4800 0000 2902 7217 0000 0072 4800  rrH...).r....rH.
+000011b0: 0000 2908 7255 0000 0072 1d00 0000 721e  ..).rU...r....r.
+000011c0: 0000 0072 3b00 0000 722e 0000 0072 2f00  ...r;...r....r/.
+000011d0: 0000 da05 7772 6974 6572 5400 0000 2909  ....writerT...).
+000011e0: 725d 0000 0072 4300 0000 7224 0000 005a  r]...rC...r$...Z
+000011f0: 0a64 6174 615f 6669 6c65 7372 3500 0000  .data_filesr5...
+00001200: 725a 0000 0072 1500 0000 7229 0000 005a  rZ...r....r)...Z
+00001210: 0964 6174 615f 6669 6c65 2901 7237 0000  .data_file).r7..
+00001220: 0072 1200 0000 7213 0000 00da 1c63 6f6e  .r....r......con
+00001230: 7665 7274 5f74 6f5f 6c61 6d6d 7073 5f69  vert_to_lammps_i
+00001240: 6e70 7574 5f64 6174 6174 0000 0073 1400  nput_datat...s..
+00001250: 0000 0001 0401 0c01 1401 1601 1401 0401  ................
+00001260: 0201 06fe 0a04 7a3f 5f5f 6578 706f 7274  ......z?__export
+00001270: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
+00001280: 732e 3c6c 6f63 616c 733e 2e63 6f6e 7665  s.<locals>.conve
+00001290: 7274 5f74 6f5f 6c61 6d6d 7073 5f69 6e70  rt_to_lammps_inp
+000012a0: 7574 5f64 6174 6129 08da 0464 6963 7472  ut_data)...dictr
+000012b0: 0500 0000 721b 0000 0072 0300 0000 7202  ....r....r....r.
+000012c0: 0000 0072 0400 0000 7206 0000 00da 0566  ...r....r......f
+000012d0: 6c6f 6174 2903 7242 0000 0072 5c00 0000  loat).rB...r\...
+000012e0: 725f 0000 0072 1200 0000 2903 7214 0000  r_...r....).r...
+000012f0: 0072 3700 0000 7222 0000 0072 1300 0000  .r7...r"...r....
+00001300: da19 5f5f 6578 706f 7274 5f72 656d 6f74  ..__export_remot
+00001310: 655f 6675 6e63 7469 6f6e 730a 0000 0073  e_functions....s
+00001320: 2000 0000 0003 0e12 1813 2c0f 2407 0201   .........,.$...
+00001330: 0601 06fd 122d 1e0d 0201 0201 0201 0201  .....-..........
+00001340: 0201 02fa 7262 0000 0029 11da 1561 6932  ....rb...)...ai2
+00001350: 5f6b 6974 2e63 6f72 652e 6172 7469 6661  _kit.core.artifa
+00001360: 6374 7202 0000 00da 0674 7970 696e 6772  ctr......typingr
+00001370: 0300 0000 7204 0000 0072 0500 0000 722e  ....r....r....r.
+00001380: 0000 0072 0600 0000 5a06 6173 652e 696f  ...r....Z.ase.io
+00001390: 721d 0000 0072 6200 0000 7237 0000 0072  r....rb...r7...r
+000013a0: 4200 0000 725c 0000 0072 5f00 0000 7214  B...r\...r_...r.
+000013b0: 0000 0072 2200 0000 7212 0000 0072 1200  ...r"...r....r..
+000013c0: 0000 7212 0000 0072 1300 0000 da08 3c6d  ..r....r......<m
+000013d0: 6f64 756c 653e 0100 0000 731e 0000 000c  odule>....s.....
+000013e0: 0214 010c 0208 0108 0308 7f00 0704 f902  ................
+000013f0: 0102 0102 0102 0102 0102 0102 fa         .............
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:23:03 2023 UTC, .py size: 7895 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 f7dd b964 d71e 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 fbde b964 d71e 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e01 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/iface.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/iface.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:22:33 2023 UTC, .py size: 17292 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d9dd b964 8c43 0000  a..........d.C..
+00000000: 610d 0d0a 0000 0000 fbde b964 8c43 0000  a..........d.C..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 fe01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:10:08 2023 UTC, .py size: 9028 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 f0da b964 4423 0000  a..........dD#..
+00000000: 610d 0d0a 0000 0000 8c43 be64 5623 0000  a........C.dV#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6406 6c0e  m.Z.m.Z...d.d.l.
@@ -199,385 +199,385 @@
 00000c60: 726c 2902 7242 0000 00da 016d 721e 0000  rl).rB.....mr...
 00000c70: 0072 1e00 0000 721f 0000 0072 4400 0000  .r....r....rD...
 00000c80: 6200 0000 7245 0000 0029 07da 0773 7973  b...rE...)...sys
 00000c90: 7465 6d73 722f 0000 0072 3000 0000 da0c  temsr/...r0.....
 00000ca0: 6c61 7370 5f69 6e5f 6461 7461 da09 6470  lasp_in_data..dp
 00000cb0: 5f6d 6f64 656c 73da 156c 616d 6d70 735f  _models..lammps_
 00000cc0: 696e 7075 745f 7465 6d70 6c61 7465 da08  input_template..
-00000cd0: 6261 7365 5f64 6972 7a1a 2031 203e 3e20  base_dirz. 1 >> 
-00000ce0: 6c61 7370 2e6f 7574 203e 3e20 6c61 7370  lasp.out >> lasp
-00000cf0: 2e65 7272 7247 0000 0072 2700 0000 2903  .errrG...r'...).
-00000d00: da03 6377 64da 0363 6d64 da0a 6368 6563  ..cwd..cmd..chec
-00000d10: 6b70 6f69 6e74 2902 da08 7465 6d70 6c61  kpoint)...templa
-00000d20: 7465 da05 7374 6570 737a 0f71 7565 7565  te..stepsz.queue
-00000d30: 2d6a 6f62 2f6c 6173 702f fa01 3a29 0272  -job/lasp/..:).r
-00000d40: 4e00 0000 da0e 6368 6563 6b70 6f69 6e74  N.....checkpoint
-00000d50: 5f6b 6579 e902 0000 0029 01da 096d 6178  _key.....)...max
-00000d60: 5f74 7269 6573 6301 0000 0000 0000 0000  _triesc.........
-00000d70: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00000d80: 1400 0000 6700 7c00 5d0c 7d01 7c01 6400  ....g.|.].}.|.d.
-00000d90: 1900 9102 7104 5300 7246 0000 0072 1e00  ....q.S.rF...r..
-00000da0: 0000 7241 0000 0072 1e00 0000 721e 0000  ..rA...r....r...
-00000db0: 0072 1f00 0000 7244 0000 007c 0000 0072  .r....rD...|...r
-00000dc0: 4500 0000 2901 da09 7461 736b 5f64 6972  E...)...task_dir
-00000dd0: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
-00000de0: 0000 0900 0000 1300 0000 7336 0000 0067  ..........s6...g
-00000df0: 007c 005d 2e7d 0174 006a 017c 0164 0019  .|.].}.t.j.|.d..
-00000e00: 0088 006a 0274 036a 0469 007c 0164 0119  ...j.t.j.i.|.d..
-00000e10: 00a5 0164 0264 0369 01a5 0164 048d 0491  ...d.d.i...d....
-00000e20: 0271 0453 0029 0572 4700 0000 da05 6174  .q.S.).rG.....at
-00000e30: 7472 73da 0974 7261 6a5f 6669 6c65 fa08  trs..traj_file..
-00000e40: 7472 616a 2e78 797a 2904 7247 0000 00da  traj.xyz).rG....
-00000e50: 0865 7865 6375 746f 72da 0666 6f72 6d61  .executor..forma
-00000e60: 7472 5800 0000 2905 7205 0000 00da 026f  trX...).r......o
-00000e70: 66da 046e 616d 6572 1600 0000 da13 4c41  f..namer......LA
-00000e80: 5350 5f4c 414d 4d50 535f 4f55 545f 4449  SP_LAMMPS_OUT_DI
-00000e90: 52a9 0272 4200 0000 da08 7461 736b 5f64  R..rB.....task_d
-00000ea0: 6972 a901 725b 0000 0072 1e00 0000 721f  ir..r[...r....r.
-00000eb0: 0000 0072 4400 0000 7e00 0000 730e 0000  ...rD...~...s...
-00000ec0: 0006 0602 fb04 0106 0104 0104 0112 fc72  ...............r
-00000ed0: 3800 0000 2925 da10 7265 736f 7572 6365  8...)%..resource
-00000ee0: 5f6d 616e 6167 6572 da10 6465 6661 756c  _manager..defaul
-00000ef0: 745f 6578 6563 7574 6f72 da02 6f73 da04  t_executor..os..
-00000f00: 7061 7468 da04 6a6f 696e da08 776f 726b  path..join..work
-00000f10: 5f64 6972 da0b 7061 7468 5f70 7265 6669  _dir..path_prefi
-00000f20: 78da 0f73 6574 7570 5f77 6f72 6b73 7061  x..setup_workspa
-00000f30: 6365 da11 7265 736f 6c76 655f 6172 7469  ce..resolve_arti
-00000f40: 6661 6374 7372 2e00 0000 7224 0000 0072  factsr....r$...r
-00000f50: 0a00 0000 da04 636f 7079 da08 6465 6570  ......copy..deep
-00000f60: 636f 7079 7212 0000 0072 1800 0000 7223  copyr....r....r#
-00000f70: 0000 0072 2100 0000 da0a 5661 6c75 6545  ...r!.....ValueE
-00000f80: 7272 6f72 da0d 7275 6e5f 7079 7468 6f6e  rror..run_python
-00000f90: 5f66 6eda 136d 616b 655f 6c61 7370 5f74  _fn..make_lasp_t
-00000fa0: 6173 6b5f 6469 7273 722f 0000 0072 3000  ask_dirsr/...r0.
-00000fb0: 0000 7231 0000 0072 2800 0000 da06 6170  ..r1...r(.....ap
-00000fc0: 7065 6e64 7203 0000 00da 0965 6e75 6d65  pendr......enume
-00000fd0: 7261 7465 7209 0000 0072 2b00 0000 7204  rater....r+...r.
-00000fe0: 0000 0072 2900 0000 da06 7375 626d 6974  ...r).....submit
-00000ff0: da06 7265 6e64 6572 7208 0000 00da 1470  ..renderr......p
-00001000: 726f 6365 7373 5f6c 6173 705f 6f75 7470  rocess_lasp_outp
-00001010: 7574 7372 3400 0000 2911 723b 0000 0072  utsr4...).r;...r
-00001020: 3c00 0000 7268 0000 00da 0974 6173 6b73  <...rh.....tasks
-00001030: 5f64 6972 7249 0000 0072 4a00 0000 724c  _dirrI...rJ...rL
-00001040: 0000 0072 5700 0000 7228 0000 0072 5200  ...rW...r(...rR.
-00001050: 0000 7261 0000 00da 046a 6f62 73da 0169  ..ra.....jobs..i
-00001060: da0b 7374 6570 735f 6772 6f75 70da 0673  ..steps_group..s
-00001070: 6372 6970 74da 036a 6f62 7235 0000 0072  cript..jobr5...r
-00001080: 1e00 0000 7262 0000 0072 1f00 0000 da08  ....rb...r......
-00001090: 636c 6c5f 6c61 7370 4700 0000 7354 0000  cll_laspG...sT..
-000010a0: 0000 0108 0312 0110 0310 0314 0108 0108  ................
-000010b0: 0204 010e 0108 010e 0208 0308 010c 0108  ................
-000010c0: 0102 010e 0102 0102 fa06 0a0e 0104 0108  ................
-000010d0: 011a 0304 011a 0106 0104 0102 0106 0102  ................
-000010e0: fe06 040c 010e ff06 020e 0112 031a 020a  ................
-000010f0: 0602 fa06 0772 7c00 0000 6300 0000 0000  .....r|...c.....
-00001100: 0000 0000 0000 0003 0000 0009 0000 0003  ................
-00001110: 0000 0073 8600 0000 6401 6402 6c00 6d01  ...s....d.d.l.m.
-00001120: 7d00 0100 4700 6403 6404 8400 6404 7c00  }...G.d.d...d.|.
-00001130: 8303 8900 7402 7403 1900 7404 7405 7402  ....t.t...t.t.t.
-00001140: 7405 1900 7402 7406 1900 7402 7405 1900  t...t.t...t.t...
-00001150: 7407 7405 1900 7402 7403 1900 6405 9c08  t.t...t.t...d...
-00001160: 8700 6601 6406 6407 840c 7d01 6410 7405  ..f.d.d...}.d.t.
-00001170: 6409 9c01 640a 640b 8405 8901 6411 7402  d...d.d.....d.t.
-00001180: 7405 1900 7408 640d 9c02 8701 6601 640e  t...t.d.....f.d.
-00001190: 640f 840d 7d02 7c01 7c02 6602 5300 2912  d...}.|.|.f.S.).
-000011a0: 4e72 0100 0000 2901 da08 5465 6d70 6c61  Nr....)...Templa
-000011b0: 7465 6300 0000 0000 0000 0000 0000 0000  tec.............
-000011c0: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
-000011d0: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
-000011e0: 2903 7a36 5f5f 6578 706f 7274 5f72 656d  ).z6__export_rem
-000011f0: 6f74 655f 6675 6e63 7469 6f6e 732e 3c6c  ote_functions.<l
-00001200: 6f63 616c 733e 2e4c 616d 6d70 7349 6e70  ocals>.LammpsInp
-00001210: 7574 5465 6d70 6c61 7465 7a02 2424 4e29  utTemplatez.$$N)
-00001220: 0472 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001230: da09 6465 6c69 6d69 7465 7272 1e00 0000  ..delimiterr....
-00001240: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-00001250: 134c 616d 6d70 7349 6e70 7574 5465 6d70  .LammpsInputTemp
-00001260: 6c61 7465 8c00 0000 7302 0000 0008 0172  late....s......r
-00001270: 7f00 0000 2908 7249 0000 0072 4a00 0000  ....).rI...rJ...
-00001280: 724d 0000 0072 2f00 0000 7230 0000 0072  rM...r/...r0...r
-00001290: 4b00 0000 724c 0000 0072 3600 0000 6307  K...rL...r6...c.
-000012a0: 0000 0000 0000 0000 0000 0014 0000 0009  ................
-000012b0: 0000 0013 0000 0073 b401 0000 7400 7c00  .......s....t.|.
-000012c0: 7c03 6401 8d02 7d07 6402 6700 0200 7d08  |.d...}.d.g...}.
-000012d0: 7d09 7c07 4400 9001 5d92 5c02 7d0a 7d0b  }.|.D...].\.}.}.
-000012e0: 7401 6a02 a003 7c02 6403 7c08 6404 9b04  t.j...|.d.|.d...
-000012f0: 9d02 a102 7d0c 7401 6a04 7c0c 6405 6406  ....}.t.j.|.d.d.
-00001300: 8d02 0100 6407 a003 6408 6409 8400 7c01  ....d...d.d...|.
-00001310: a005 a100 4400 8301 a101 7d0d 7406 7401  ....D.....}.t.t.
-00001320: 6a02 a003 7c0c 640a a102 640b 640c 640d  j...|.d...d.d.d.
-00001330: 8d03 8f1a 7d0e 7c0e a007 7c0d a101 0100  ....}.|...|.....
-00001340: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
-00001350: 7398 3000 0100 0100 0100 5900 0100 7408  s.0.......Y...t.
-00001360: 6a09 6a07 7401 6a02 a003 7c0c 640e a102  j.j.t.j...|.d...
-00001370: 7c0b 640f 6410 8d03 0100 7c06 6400 7501  |.d.d.....|.d.u.
-00001380: 9001 728a 7401 6a02 a003 7c0c 6411 a102  ..r.t.j...|.d...
-00001390: 7d0f 7408 6a09 6a07 7c0f 7c0b 6412 7c03  }.t.j.j.|.|.d.|.
-000013a0: 6413 8d04 0100 6407 a003 6414 7c0f 9b00  d.....d...d.|...
-000013b0: 9d02 6701 6415 6416 8400 740a 7c04 8301  ..g.d.d...t.|...
-000013c0: 4400 8301 a201 a101 7d10 6407 a003 6417  D.......}.d...d.
-000013d0: 6418 a003 7c05 a101 9b00 6419 740b 9b00  d...|.....d.t...
-000013e0: 9d04 641a 6702 a101 7d11 8800 7c06 8301  ..d.g...}...|...
-000013f0: 6a0c 7c10 7c11 641b 8d02 7d12 7401 6a02  j.|.|.d...}.t.j.
-00001400: a003 7c0c 641c a102 7d13 7406 7c13 640b  ..|.d...}.t.|.d.
-00001410: 640c 640d 8d03 8f1a 7d0e 7c0e a007 7c12  d.d.....}.|...|.
-00001420: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00001430: 6e12 3100 9001 737e 3000 0100 0100 0100  n.1...s~0.......
-00001440: 5900 0100 6e08 740d 641d 8301 8201 7c09  Y...n.t.d.....|.
-00001450: a00e 7c0c 7c0a 641e 1900 641f 9c02 a101  ..|.|.d...d.....
-00001460: 0100 7c08 6420 3700 7d08 711a 7c09 5300  ..|.d 7.}.q.|.S.
-00001470: 2921 4e29 0172 2f00 0000 7201 0000 005a  )!N).r/...r....Z
-00001480: 0574 6173 6b5f 5a02 3036 5429 01da 0865  .task_Z.06T)...e
-00001490: 7869 7374 5f6f 6bda 010a 6301 0000 0000  xist_ok...c.....
-000014a0: 0000 0000 0000 0003 0000 0005 0000 0053  ...............S
-000014b0: 0000 0073 2000 0000 6700 7c00 5d18 5c02  ...s ...g.|.].\.
-000014c0: 7d01 7d02 7c01 6400 9b04 6401 7c02 9b00  }.}.|.d...d.|...
-000014d0: 9d03 9102 7104 5300 2902 5a02 3332 fa01  ....q.S.).Z.32..
-000014e0: 2072 1e00 0000 2903 7242 0000 00da 016b   r....).rB.....k
-000014f0: da01 7672 1e00 0000 721e 0000 0072 1f00  ..vr....r....r..
-00001500: 0000 7244 0000 009f 0000 0072 4500 0000  ..rD.......rE...
-00001510: 7a4a 5f5f 6578 706f 7274 5f72 656d 6f74  zJ__export_remot
-00001520: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
-00001530: 616c 733e 2e6d 616b 655f 6c61 7370 5f74  als>.make_lasp_t
-00001540: 6173 6b5f 6469 7273 2e3c 6c6f 6361 6c73  ask_dirs.<locals
-00001550: 3e2e 3c6c 6973 7463 6f6d 703e 7a07 6c61  >.<listcomp>z.la
-00001560: 7370 2e69 6eda 0177 7a05 7574 662d 3829  sp.in..wz.utf-8)
-00001570: 01da 0865 6e63 6f64 696e 677a 086c 6173  ...encodingz.las
-00001580: 702e 7374 72fa 0864 6d6f 6c2d 6172 63a9  p.str..dmol-arc.
-00001590: 0172 5c00 0000 7a0b 6c61 6d6d 7073 2e64  .r\...z.lammps.d
-000015a0: 6174 617a 0b6c 616d 6d70 732d 6461 7461  ataz.lammps-data
-000015b0: 2902 725c 0000 00da 0973 7065 636f 7264  ).r\.....specord
-000015c0: 6572 7a0a 7265 6164 5f64 6174 6120 6301  erz.read_data c.
-000015d0: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-000015e0: 0000 0073 0000 0073 2600 0000 7c00 5d1e  ...s...s&...|.].
-000015f0: 5c02 7d01 7d02 6400 7c01 6401 1700 9b00  \.}.}.d.|.d.....
-00001600: 6402 7c02 9b00 9d04 5600 0100 7102 6403  d.|.....V...q.d.
-00001610: 5300 2904 7a05 6d61 7373 2072 0f00 0000  S.).z.mass r....
-00001620: 7282 0000 004e 721e 0000 0029 0372 4200  r....Nr....).rB.
-00001630: 0000 7278 0000 0072 4800 0000 721e 0000  ..rx...rH...r...
-00001640: 0072 1e00 0000 721f 0000 00da 093c 6765  .r....r......<ge
-00001650: 6e65 7870 723e ab00 0000 7245 0000 007a  nexpr>....rE...z
-00001660: 495f 5f65 7870 6f72 745f 7265 6d6f 7465  I__export_remote
-00001670: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
-00001680: 6c73 3e2e 6d61 6b65 5f6c 6173 705f 7461  ls>.make_lasp_ta
-00001690: 736b 5f64 6972 732e 3c6c 6f63 616c 733e  sk_dirs.<locals>
-000016a0: 2e3c 6765 6e65 7870 723e 7a12 7061 6972  .<genexpr>z.pair
-000016b0: 5f73 7479 6c65 2064 6565 706d 6420 7282  _style deepmd r.
-000016c0: 0000 007a 0a20 6f75 745f 6669 6c65 207a  ...z. out_file z
-000016d0: 0e70 6169 725f 636f 6566 6620 2a20 2a29  .pair_coeff * *)
-000016e0: 02da 1172 6561 645f 6461 7461 5f73 6563  ...read_data_sec
-000016f0: 7469 6f6e da13 666f 7263 655f 6669 656c  tion..force_fiel
-00001700: 645f 7365 6374 696f 6e7a 0969 6e2e 7369  d_sectionz.in.si
-00001710: 6d70 6c65 723f 0000 0072 5800 0000 2902  mpler?...rX...).
-00001720: 7247 0000 0072 5800 0000 720f 0000 0029  rG...rX...r....)
-00001730: 0f72 1500 0000 7265 0000 0072 6600 0000  .r....re...rf...
-00001740: 7267 0000 00da 086d 616b 6564 6972 73da  rg.....makedirs.
-00001750: 0569 7465 6d73 da04 6f70 656e da05 7772  .items..open..wr
-00001760: 6974 65da 0361 7365 da02 696f 7272 0000  ite..ase..iorr..
-00001770: 0072 1400 0000 da0a 7375 6273 7469 7475  .r......substitu
-00001780: 7465 726e 0000 0072 7100 0000 2914 7249  tern...rq...).rI
-00001790: 0000 0072 4a00 0000 724d 0000 0072 2f00  ...rJ...rM...r/.
-000017a0: 0000 7230 0000 0072 4b00 0000 724c 0000  ..r0...rK...rL..
-000017b0: 00da 0a69 6e70 7574 5f64 6174 6172 7800  ...input_datarx.
-000017c0: 0000 7257 0000 00da 0861 7274 6966 6163  ..rW.....artifac
-000017d0: 74da 0561 746f 6d73 7261 0000 005a 0c6c  t..atomsra...Z.l
-000017e0: 6173 705f 696e 5f74 6578 74da 0166 da09  asp_in_text..f..
-000017f0: 6461 7461 5f66 696c 6572 8b00 0000 728c  data_filer....r.
-00001800: 0000 00da 0c6c 616d 6d70 735f 696e 7075  .....lammps_inpu
-00001810: 745a 116c 616d 6d70 735f 696e 7075 745f  tZ.lammps_input_
-00001820: 6669 6c65 2901 727f 0000 0072 1e00 0000  file).r....r....
-00001830: 721f 0000 0072 7000 0000 8f00 0000 7340  r....rp.......s@
-00001840: 0000 0000 080c 020a 010e 0216 010e 0218  ................
-00001850: 011a 0128 021c 010a 020e 0114 0204 0108  ...(............
-00001860: ff02 0210 fe06 0404 0114 0102 fe06 0408  ................
-00001870: 0102 0102 fe06 040e 0110 012c 0208 0114  ...........,....
-00001880: 010a 017a 365f 5f65 7870 6f72 745f 7265  ...z6__export_re
-00001890: 6d6f 7465 5f66 756e 6374 696f 6e73 2e3c  mote_functions.<
-000018a0: 6c6f 6361 6c73 3e2e 6d61 6b65 5f6c 6173  locals>.make_las
-000018b0: 705f 7461 736b 5f64 6972 7372 5a00 0000  p_task_dirsrZ...
-000018c0: 2901 7261 0000 0063 0200 0000 0000 0000  ).ra...c........
-000018d0: 0000 0000 0f00 0000 0800 0000 5300 0000  ............S...
-000018e0: 7300 0200 0074 006a 01a0 027c 0064 01a1  s....t.j...|.d..
-000018f0: 027d 0274 006a 01a0 027c 0064 02a1 027d  .}.t.j...|.d...}
-00001900: 0374 036a 046a 057c 0264 0364 0464 058d  .t.j.j.|.d.d.d..
-00001910: 037d 0474 067c 0264 0683 028f 267d 0574  .}.t.|.d....&}.t
-00001920: 0764 0764 0884 007c 05a0 08a1 0044 0083  .d.d...|.....D..
-00001930: 0183 017d 0657 0064 0904 0004 0083 0301  ...}.W.d........
-00001940: 006e 1031 0073 6430 0001 0001 0001 0059  .n.1.sd0.......Y
-00001950: 0001 0074 067c 0364 0683 028f 3c7d 057c  ...t.|.d....<}.|
-00001960: 05a0 08a1 007d 0774 0764 0a64 0884 007c  .....}.t.d.d...|
-00001970: 0744 0083 0183 017d 0874 0764 0b64 0884  .D.....}.t.d.d..
-00001980: 007c 0744 0083 0183 017d 0957 0064 0904  .|.D.....}.W.d..
-00001990: 0004 0083 0301 006e 1031 0073 ba30 0001  .......n.1.s.0..
-000019a0: 0001 0001 0059 0001 0067 007d 0a74 097c  .....Y...g.}.t.|
-000019b0: 0683 0144 005d 585c 027d 0b7d 0c74 0a7c  ...D.]X\.}.}.t.|
-000019c0: 0883 0164 0c6b 0472 d074 0b6a 0c7c 0c7c  ...d.k.r.t.j.|.|
-000019d0: 0864 0c19 0064 0c64 0d64 0e8d 0472 d07c  .d...d.d.d...r.|
-000019e0: 0974 0a7c 0a83 0119 007c 047c 0b19 006a  .t.|.....|.|...j
-000019f0: 0d64 0f3c 007c 0aa0 0e7c 047c 0b19 00a1  .d.<.|...|.|....
-00001a00: 0101 007c 08a0 0f64 0ca1 0101 0071 d074  ...|...d.....q.t
-00001a10: 036a 046a 1074 006a 01a0 027c 007c 01a1  .j.j.t.j...|.|..
-00001a20: 027c 0a64 1064 058d 0301 0074 006a 01a0  .|.d.d.....t.j..
-00001a30: 027c 0074 11a1 027d 0d67 007d 0774 067c  .|.t...}.g.}.t.|
-00001a40: 0d64 0683 028f 527d 0574 097c 0583 0144  .d....R}.t.|...D
-00001a50: 005d 385c 027d 0b7d 0e7c 0b64 0c6b 0490  .]8\.}.}.|.d.k..
-00001a60: 0172 9874 12a0 1364 117c 0b64 1218 0064  .r.t...d.|.d...d
-00001a70: 139b 0464 149d 027c 0ea1 037d 0e7c 07a0  ...d...|...}.|..
-00001a80: 0e7c 0ea1 0101 0090 0171 6c57 0064 0904  .|.......qlW.d..
-00001a90: 0004 0083 0301 006e 1231 0090 0173 bc30  .......n.1...s.0
-00001aa0: 0001 0001 0001 0059 0001 0074 067c 0d64  .......Y...t.|.d
-00001ab0: 1583 028f 1a7d 057c 05a0 147c 07a1 0101  .....}.|...|....
-00001ac0: 0057 0064 0904 0004 0083 0301 006e 1231  .W.d.........n.1
-00001ad0: 0090 0173 f230 0001 0001 0001 0059 0001  ...s.0.......Y..
-00001ae0: 0064 0953 0029 1661 0c01 0000 0a20 2020  .d.S.).a.....   
-00001af0: 2020 2020 2041 6c69 676e 206c 6173 7020       Align lasp 
-00001b00: 6f75 7470 7574 2077 6974 6820 6d6f 6465  output with mode
-00001b10: 6c5f 6465 7669 2072 6563 6f72 6473 2e0a  l_devi records..
-00001b20: 0a20 2020 2020 2020 2041 7320 616c 6c73  .        As alls
-00001b30: 7472 2e61 7263 2063 6f6e 7461 696e 7320  tr.arc contains 
-00001b40: 616c 6c20 7468 6520 7374 7275 6374 7572  all the structur
-00001b50: 6573 2067 656e 6572 6174 6564 2062 7920  es generated by 
-00001b60: 4c41 5350 2c0a 2020 2020 2020 2020 7765  LASP,.        we
-00001b70: 206e 6565 6420 746f 2075 7365 2074 6865   need to use the
-00001b80: 2072 6573 756c 7420 6f66 206c 6173 702e   result of lasp.
-00001b90: 6f75 7420 666f 7220 616c 6967 6e6d 656e  out for alignmen
-00001ba0: 742e 0a0a 2020 2020 2020 2020 5468 6520  t...        The 
-00001bb0: 666f 6c6c 6f77 696e 6720 636f 6465 2069  following code i
-00001bc0: 7320 636f 7079 2066 726f 6d20 4368 6563  s copy from Chec
-00001bd0: 4d61 7465 2c20 6d61 7920 6e65 6564 2074  Mate, may need t
-00001be0: 6f20 6265 2072 6566 6163 746f 7265 640a  o be refactored.
-00001bf0: 2020 2020 2020 2020 7a0a 616c 6c73 7472          z.allstr
-00001c00: 2e61 7263 7a08 6c61 7370 2e6f 7574 7253  .arcz.lasp.outrS
-00001c10: 0000 0072 8700 0000 7288 0000 00da 0172  ...r....r......r
-00001c20: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001c30: 0006 0000 0073 0000 0073 3800 0000 7c00  .....s...s8...|.
-00001c40: 5d30 7d01 6400 7c01 7600 7202 7400 7401  ]0}.d.|.v.r.t.t.
-00001c50: 7c01 6401 6402 8502 1900 a002 a100 a003  |.d.d...........
-00001c60: a100 6403 1900 8301 6404 8302 5600 0100  ..d.....d...V...
-00001c70: 7102 6401 5300 2905 5a06 456e 6572 6779  q.d.S.).Z.Energy
-00001c80: 4ee9 4900 0000 e9fe ffff ffe9 0600 0000  N.I.............
-00001c90: a904 da05 726f 756e 6472 3200 0000 da05  ....roundr2.....
-00001ca0: 7374 7269 70da 0573 706c 6974 a902 7242  strip..split..rB
-00001cb0: 0000 00da 046c 696e 6572 1e00 0000 721e  .....liner....r.
-00001cc0: 0000 0072 1f00 0000 728a 0000 00cd 0000  ...r....r.......
-00001cd0: 0072 4500 0000 7a49 5f5f 6578 706f 7274  .rE...zI__export
-00001ce0: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
-00001cf0: 732e 3c6c 6f63 616c 733e 2e70 726f 6365  s.<locals>.proce
-00001d00: 7373 5f6c 6173 705f 6f75 7470 7574 2e3c  ss_lasp_output.<
-00001d10: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-00001d20: 3e4e 6301 0000 0000 0000 0000 0000 0002  >Nc.............
-00001d30: 0000 0006 0000 0073 0000 0073 3800 0000  .......s...s8...
-00001d40: 7c00 5d30 7d01 6400 7c01 7600 7202 7400  |.]0}.d.|.v.r.t.
-00001d50: 7401 7c01 6401 6402 8502 1900 a002 a100  t.|.d.d.........
-00001d60: a003 a100 6403 1900 8301 6404 8302 5600  ....d.....d...V.
-00001d70: 0100 7102 6401 5300 2905 fa0c 456e 6572  ..q.d.S.)...Ener
-00001d80: 6779 2c66 6f72 6365 4e72 9b00 0000 7255  gy,forceNr....rU
-00001d90: 0000 0072 9d00 0000 729e 0000 0072 a200  ...r....r....r..
-00001da0: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00001db0: 0072 8a00 0000 d000 0000 7245 0000 0063  .r........rE...c
-00001dc0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001dd0: 0600 0000 7300 0000 7338 0000 007c 005d  ....s...s8...|.]
-00001de0: 307d 0164 007c 0176 0072 0274 0074 017c  0}.d.|.v.r.t.t.|
-00001df0: 0164 0164 0285 0219 00a0 02a1 00a0 03a1  .d.d............
-00001e00: 0064 0319 0083 0164 0483 0256 0001 0071  .d.....d...V...q
-00001e10: 0264 0153 0029 0572 a400 0000 4e72 9b00  .d.S.).r....Nr..
-00001e20: 0000 720f 0000 0072 9d00 0000 729e 0000  ..r....r....r...
-00001e30: 0072 a200 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00001e40: 721f 0000 0072 8a00 0000 d100 0000 7245  r....r........rE
-00001e50: 0000 0072 0100 0000 672d 431c ebe2 361a  ...r....g-C...6.
-00001e60: 3f29 02da 0472 746f 6cda 0461 746f 6c5a  ?)...rtol..atolZ
-00001e70: 0a73 7377 5f65 6e65 7267 79da 0665 7874  .ssw_energy..ext
-00001e80: 7879 7a7a 075e 5c73 2b5c 642b 720f 0000  xyzz.^\s+\d+r...
-00001e90: 007a 033e 3132 7282 0000 0072 8500 0000  .z.>12r....r....
-00001ea0: 2915 7265 0000 0072 6600 0000 7267 0000  ).re...rf...rg..
-00001eb0: 0072 9100 0000 7292 0000 00da 0472 6561  .r....r......rea
-00001ec0: 6472 8f00 0000 da04 6c69 7374 da09 7265  dr......list..re
-00001ed0: 6164 6c69 6e65 7372 7200 0000 da03 6c65  adlinesrr.....le
-00001ee0: 6eda 026e 70da 0769 7363 6c6f 7365 da04  n..np..isclose..
-00001ef0: 696e 666f 7271 0000 00da 0370 6f70 7290  inforq.....popr.
-00001f00: 0000 0072 1400 0000 da02 7265 da03 7375  ...r......re..su
-00001f10: 62da 0a77 7269 7465 6c69 6e65 7329 0f72  b..writelines).r
-00001f20: 6100 0000 da09 6669 6c65 5f6e 616d 655a  a.....file_nameZ
-00001f30: 0c61 6c6c 5f73 7472 5f66 696c 655a 0d6c  .all_str_fileZ.l
-00001f40: 6173 705f 6f75 745f 6669 6c65 5a08 616c  asp_out_fileZ.al
-00001f50: 6c5f 7374 7273 7297 0000 005a 0661 6c6c  l_strsr....Z.all
-00001f60: 5f71 73da 056c 696e 6573 5a07 7472 616a  _qs..linesZ.traj
-00001f70: 5f71 735a 0774 7261 6a5f 6573 5a09 7472  _qsZ.traj_esZ.tr
-00001f80: 616a 5f73 7472 7372 7800 0000 da01 715a  aj_strsrx.....qZ
-00001f90: 0f6d 6f64 656c 5f64 6576 695f 6669 6c65  .model_devi_file
-00001fa0: 72a3 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00001fb0: 1f00 0000 da13 7072 6f63 6573 735f 6c61  ......process_la
-00001fc0: 7370 5f6f 7574 7075 74bf 0000 0073 3200  sp_output....s2.
-00001fd0: 0000 0009 0e01 0e01 1202 0c01 3401 0c01  ............4...
-00001fe0: 0801 1201 3002 0401 1002 2201 1601 0e01  ....0.....".....
-00001ff0: 0c02 1c02 0e01 0401 0c01 1001 0a02 1a01  ................
-00002000: 2e01 0c01 7a36 5f5f 6578 706f 7274 5f72  ....z6__export_r
-00002010: 656d 6f74 655f 6675 6e63 7469 6f6e 732e  emote_functions.
-00002020: 3c6c 6f63 616c 733e 2e70 726f 6365 7373  <locals>.process
-00002030: 5f6c 6173 705f 6f75 7470 7574 e904 0000  _lasp_output....
-00002040: 00a9 0272 5700 0000 da07 776f 726b 6572  ...rW.....worker
-00002050: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00002060: 0000 0400 0000 1300 0000 732c 0000 0064  ..........s,...d
-00002070: 0164 006c 0089 0088 006a 017c 0164 028d  .d.l.....j.|.d..
-00002080: 0187 0087 0166 0264 0364 0484 087c 0044  .....f.d.d...|.D
-00002090: 0083 0183 0101 0064 0053 0029 054e 7201  .......d.S.).Nr.
-000020a0: 0000 0029 015a 066e 5f6a 6f62 7363 0100  ...).Z.n_jobsc..
-000020b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000020c0: 0000 3300 0000 731c 0000 007c 005d 147d  ..3...s....|.].}
-000020d0: 0188 00a0 0088 01a1 017c 0183 0156 0001  .........|...V..
-000020e0: 0071 0264 0053 0072 3700 0000 2901 5a07  .q.d.S.r7...).Z.
-000020f0: 6465 6c61 7965 6472 6000 0000 2902 da06  delayedr`...)...
-00002100: 6a6f 626c 6962 72b6 0000 0072 1e00 0000  joblibr....r....
-00002110: 721f 0000 0072 8a00 0000 ea00 0000 7304  r....r........s.
-00002120: 0000 0004 0202 ff7a 4a5f 5f65 7870 6f72  .......zJ__expor
-00002130: 745f 7265 6d6f 7465 5f66 756e 6374 696f  t_remote_functio
-00002140: 6e73 2e3c 6c6f 6361 6c73 3e2e 7072 6f63  ns.<locals>.proc
-00002150: 6573 735f 6c61 7370 5f6f 7574 7075 7473  ess_lasp_outputs
-00002160: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00002170: 7072 3e29 0272 ba00 0000 5a08 5061 7261  pr>).r....Z.Para
-00002180: 6c6c 656c 72b8 0000 0029 0172 b600 0000  llelr....).r....
-00002190: 2901 72ba 0000 0072 1f00 0000 7275 0000  ).r....r....ru..
-000021a0: 00e8 0000 0073 0800 0000 0001 0801 1602  .....s..........
-000021b0: 02fe 7a37 5f5f 6578 706f 7274 5f72 656d  ..z7__export_rem
-000021c0: 6f74 655f 6675 6e63 7469 6f6e 732e 3c6c  ote_functions.<l
-000021d0: 6f63 616c 733e 2e70 726f 6365 7373 5f6c  ocals>.process_l
-000021e0: 6173 705f 6f75 7470 7574 7329 0172 5a00  asp_outputs).rZ.
-000021f0: 0000 2901 72b7 0000 0029 09da 0673 7472  ..).r....)...str
-00002200: 696e 6772 7d00 0000 720b 0000 0072 0600  ingr}...r....r..
-00002210: 0000 7225 0000 0072 1c00 0000 7232 0000  ..r%...r....r2..
-00002220: 0072 0c00 0000 722c 0000 0029 0372 7d00  .r....r,...).r}.
-00002230: 0000 7270 0000 0072 7500 0000 721e 0000  ..rp...ru...r...
-00002240: 0029 0272 7f00 0000 72b6 0000 0072 1f00  .).r....r....r..
-00002250: 0000 da19 5f5f 6578 706f 7274 5f72 656d  ....__export_rem
-00002260: 6f74 655f 6675 6e63 7469 6f6e 7388 0000  ote_functions...
-00002270: 0073 2000 0000 0002 0c02 1003 0601 0201  .s .............
-00002280: 0201 0601 0601 0601 0601 06f9 1030 1029  .............0.)
-00002290: 1a09 0201 02fe 72bc 0000 0029 31da 1361  ......r....)1..a
-000022a0: 6932 5f6b 6974 2e63 6f72 652e 7363 7269  i2_kit.core.scri
-000022b0: 7074 7202 0000 0072 0300 0000 7204 0000  ptr....r....r...
-000022c0: 00da 1561 6932 5f6b 6974 2e63 6f72 652e  ...ai2_kit.core.
-000022d0: 6172 7469 6661 6374 7205 0000 0072 0600  artifactr....r..
-000022e0: 0000 da10 6169 325f 6b69 742e 636f 7265  ....ai2_kit.core
-000022f0: 2e6c 6f67 7207 0000 005a 1061 6932 5f6b  .logr....Z.ai2_k
-00002300: 6974 2e63 6f72 652e 6a6f 6272 0800 0000  it.core.jobr....
-00002310: da11 6169 325f 6b69 742e 636f 7265 2e75  ..ai2_kit.core.u
-00002320: 7469 6c72 0900 0000 720a 0000 00da 0674  tilr....r......t
-00002330: 7970 696e 6772 0b00 0000 720c 0000 00da  ypingr....r.....
-00002340: 0870 7964 616e 7469 6372 0d00 0000 da0b  .pydanticr......
-00002350: 6461 7461 636c 6173 7365 7372 0e00 0000  dataclassesr....
-00002360: da05 6e75 6d70 7972 ac00 0000 da06 6173  ..numpyr......as
-00002370: 652e 696f 7291 0000 0072 6c00 0000 7265  e.ior....rl...re
-00002380: 0000 0072 b000 0000 da05 6966 6163 6572  ...r......ifacer
-00002390: 1000 0000 7211 0000 00da 0863 6f6e 7374  ....r......const
-000023a0: 616e 7472 1200 0000 7213 0000 0072 1400  antr....r....r..
-000023b0: 0000 da04 6461 7461 7215 0000 0072 1600  ....datar....r..
-000023c0: 0000 7219 0000 00da 066c 6f67 6765 7272  ..r......loggerr
-000023d0: 1700 0000 7226 0000 0072 2d00 0000 7233  ....r&...r-...r3
-000023e0: 0000 0072 3400 0000 727c 0000 0072 bc00  ...r4...r|...r..
-000023f0: 0000 7270 0000 0072 7500 0000 721e 0000  ..rp...ru...r...
-00002400: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00002410: da08 3c6d 6f64 756c 653e 0100 0000 733e  ..<module>....s>
-00002420: 0000 0014 0110 010c 010c 0110 0210 010c  ................
-00002430: 010c 0208 0108 0108 0108 0108 0210 0114  ................
-00002440: 0110 0308 0310 1310 0602 0110 0702 0112  ................
-00002450: 0402 0112 0710 4108 7104 fd02 0102 0102  ......A.q.......
-00002460: fe                                       .
+00000cd0: 6261 7365 5f64 6972 7a18 2031 203e 206c  base_dirz. 1 > l
+00000ce0: 6173 702e 6f75 7420 3e20 6c61 7370 2e65  asp.out > lasp.e
+00000cf0: 7272 7247 0000 0072 2700 0000 2903 da03  rrrG...r'...)...
+00000d00: 6377 64da 0363 6d64 da0a 6368 6563 6b70  cwd..cmd..checkp
+00000d10: 6f69 6e74 2902 da08 7465 6d70 6c61 7465  oint)...template
+00000d20: da05 7374 6570 737a 0f71 7565 7565 2d6a  ..stepsz.queue-j
+00000d30: 6f62 2f6c 6173 702f fa01 3a29 0272 4e00  ob/lasp/..:).rN.
+00000d40: 0000 da0e 6368 6563 6b70 6f69 6e74 5f6b  ....checkpoint_k
+00000d50: 6579 e902 0000 0029 01da 096d 6178 5f74  ey.....)...max_t
+00000d60: 7269 6573 6301 0000 0000 0000 0000 0000  riesc...........
+00000d70: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00000d80: 0000 6700 7c00 5d0c 7d01 7c01 6400 1900  ..g.|.].}.|.d...
+00000d90: 9102 7104 5300 7246 0000 0072 1e00 0000  ..q.S.rF...r....
+00000da0: 7241 0000 0072 1e00 0000 721e 0000 0072  rA...r....r....r
+00000db0: 1f00 0000 7244 0000 007c 0000 0072 4500  ....rD...|...rE.
+00000dc0: 0000 2901 da09 7461 736b 5f64 6972 7363  ..)...task_dirsc
+00000dd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000de0: 0900 0000 1300 0000 7336 0000 0067 007c  ........s6...g.|
+00000df0: 005d 2e7d 0174 006a 017c 0164 0019 0088  .].}.t.j.|.d....
+00000e00: 006a 0274 036a 0469 007c 0164 0119 00a5  .j.t.j.i.|.d....
+00000e10: 0164 0264 0369 01a5 0164 048d 0491 0271  .d.d.i...d.....q
+00000e20: 0453 0029 0572 4700 0000 da05 6174 7472  .S.).rG.....attr
+00000e30: 735a 0f73 7472 7563 7475 7265 735f 6669  sZ.structures_fi
+00000e40: 6c65 fa0e 7374 7275 6374 7572 6573 2e78  le..structures.x
+00000e50: 797a 2904 7247 0000 00da 0865 7865 6375  yz).rG.....execu
+00000e60: 746f 72da 0666 6f72 6d61 7472 5800 0000  tor..formatrX...
+00000e70: 2905 7205 0000 00da 026f 66da 046e 616d  ).r......of..nam
+00000e80: 6572 1600 0000 da13 4c41 5350 5f4c 414d  er......LASP_LAM
+00000e90: 4d50 535f 4f55 545f 4449 52a9 0272 4200  MPS_OUT_DIR..rB.
+00000ea0: 0000 da08 7461 736b 5f64 6972 a901 725a  ....task_dir..rZ
+00000eb0: 0000 0072 1e00 0000 721f 0000 0072 4400  ...r....r....rD.
+00000ec0: 0000 7e00 0000 730e 0000 0006 0602 fb04  ..~...s.........
+00000ed0: 0106 0104 0104 0112 fc72 3800 0000 2925  .........r8...)%
+00000ee0: da10 7265 736f 7572 6365 5f6d 616e 6167  ..resource_manag
+00000ef0: 6572 da10 6465 6661 756c 745f 6578 6563  er..default_exec
+00000f00: 7574 6f72 da02 6f73 da04 7061 7468 da04  utor..os..path..
+00000f10: 6a6f 696e da08 776f 726b 5f64 6972 da0b  join..work_dir..
+00000f20: 7061 7468 5f70 7265 6669 78da 0f73 6574  path_prefix..set
+00000f30: 7570 5f77 6f72 6b73 7061 6365 da11 7265  up_workspace..re
+00000f40: 736f 6c76 655f 6172 7469 6661 6374 7372  solve_artifactsr
+00000f50: 2e00 0000 7224 0000 0072 0a00 0000 da04  ....r$...r......
+00000f60: 636f 7079 da08 6465 6570 636f 7079 7212  copy..deepcopyr.
+00000f70: 0000 0072 1800 0000 7223 0000 0072 2100  ...r....r#...r!.
+00000f80: 0000 da0a 5661 6c75 6545 7272 6f72 da0d  ....ValueError..
+00000f90: 7275 6e5f 7079 7468 6f6e 5f66 6eda 136d  run_python_fn..m
+00000fa0: 616b 655f 6c61 7370 5f74 6173 6b5f 6469  ake_lasp_task_di
+00000fb0: 7273 722f 0000 0072 3000 0000 7231 0000  rsr/...r0...r1..
+00000fc0: 0072 2800 0000 da06 6170 7065 6e64 7203  .r(.....appendr.
+00000fd0: 0000 00da 0965 6e75 6d65 7261 7465 7209  .....enumerater.
+00000fe0: 0000 0072 2b00 0000 7204 0000 0072 2900  ...r+...r....r).
+00000ff0: 0000 da06 7375 626d 6974 da06 7265 6e64  ....submit..rend
+00001000: 6572 7208 0000 00da 1470 726f 6365 7373  err......process
+00001010: 5f6c 6173 705f 6f75 7470 7574 7372 3400  _lasp_outputsr4.
+00001020: 0000 2911 723b 0000 0072 3c00 0000 7267  ..).r;...r<...rg
+00001030: 0000 00da 0974 6173 6b73 5f64 6972 7249  .....tasks_dirrI
+00001040: 0000 0072 4a00 0000 724c 0000 0072 5700  ...rJ...rL...rW.
+00001050: 0000 7228 0000 0072 5200 0000 7260 0000  ..r(...rR...r`..
+00001060: 00da 046a 6f62 73da 0169 da0b 7374 6570  ...jobs..i..step
+00001070: 735f 6772 6f75 70da 0673 6372 6970 74da  s_group..script.
+00001080: 036a 6f62 7235 0000 0072 1e00 0000 7261  .jobr5...r....ra
+00001090: 0000 0072 1f00 0000 da08 636c 6c5f 6c61  ...r......cll_la
+000010a0: 7370 4700 0000 7354 0000 0000 0108 0312  spG...sT........
+000010b0: 0110 0310 0314 0108 0108 0204 010e 0108  ................
+000010c0: 010e 0208 0308 010c 0108 0102 010e 0102  ................
+000010d0: 0102 fa06 0a0e 0104 0108 011a 0304 011a  ................
+000010e0: 0106 0104 0102 0106 0102 fe06 040c 010e  ................
+000010f0: ff06 020e 0112 031a 020a 0602 fa06 0772  ...............r
+00001100: 7b00 0000 6300 0000 0000 0000 0000 0000  {...c...........
+00001110: 0003 0000 0009 0000 0003 0000 0073 8600  .............s..
+00001120: 0000 6401 6402 6c00 6d01 7d00 0100 4700  ..d.d.l.m.}...G.
+00001130: 6403 6404 8400 6404 7c00 8303 8900 7402  d.d...d.|.....t.
+00001140: 7403 1900 7404 7405 7402 7405 1900 7402  t...t.t.t.t...t.
+00001150: 7406 1900 7402 7405 1900 7407 7405 1900  t...t.t...t.t...
+00001160: 7402 7403 1900 6405 9c08 8700 6601 6406  t.t...d.....f.d.
+00001170: 6407 840c 7d01 6410 7405 6409 9c01 640a  d...}.d.t.d...d.
+00001180: 640b 8405 8901 6411 7402 7405 1900 7408  d.....d.t.t...t.
+00001190: 640d 9c02 8701 6601 640e 640f 840d 7d02  d.....f.d.d...}.
+000011a0: 7c01 7c02 6602 5300 2912 4e72 0100 0000  |.|.f.S.).Nr....
+000011b0: 2901 da08 5465 6d70 6c61 7465 6300 0000  )...Templatec...
+000011c0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+000011d0: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
+000011e0: 5a02 6401 5a03 6402 5300 2903 7a36 5f5f  Z.d.Z.d.S.).z6__
+000011f0: 6578 706f 7274 5f72 656d 6f74 655f 6675  export_remote_fu
+00001200: 6e63 7469 6f6e 732e 3c6c 6f63 616c 733e  nctions.<locals>
+00001210: 2e4c 616d 6d70 7349 6e70 7574 5465 6d70  .LammpsInputTemp
+00001220: 6c61 7465 7a02 2424 4e29 0472 1900 0000  latez.$$N).r....
+00001230: 721a 0000 0072 1b00 0000 da09 6465 6c69  r....r......deli
+00001240: 6d69 7465 7272 1e00 0000 721e 0000 0072  miterr....r....r
+00001250: 1e00 0000 721f 0000 00da 134c 616d 6d70  ....r......Lammp
+00001260: 7349 6e70 7574 5465 6d70 6c61 7465 8c00  sInputTemplate..
+00001270: 0000 7302 0000 0008 0172 7e00 0000 2908  ..s......r~...).
+00001280: 7249 0000 0072 4a00 0000 724d 0000 0072  rI...rJ...rM...r
+00001290: 2f00 0000 7230 0000 0072 4b00 0000 724c  /...r0...rK...rL
+000012a0: 0000 0072 3600 0000 6307 0000 0000 0000  ...r6...c.......
+000012b0: 0000 0000 0014 0000 0009 0000 0013 0000  ................
+000012c0: 0073 b401 0000 7400 7c00 7c03 6401 8d02  .s....t.|.|.d...
+000012d0: 7d07 6402 6700 0200 7d08 7d09 7c07 4400  }.d.g...}.}.|.D.
+000012e0: 9001 5d92 5c02 7d0a 7d0b 7401 6a02 a003  ..].\.}.}.t.j...
+000012f0: 7c02 6403 7c08 6404 9b04 9d02 a102 7d0c  |.d.|.d.......}.
+00001300: 7401 6a04 7c0c 6405 6406 8d02 0100 6407  t.j.|.d.d.....d.
+00001310: a003 6408 6409 8400 7c01 a005 a100 4400  ..d.d...|.....D.
+00001320: 8301 a101 7d0d 7406 7401 6a02 a003 7c0c  ....}.t.t.j...|.
+00001330: 640a a102 640b 640c 640d 8d03 8f1a 7d0e  d...d.d.d.....}.
+00001340: 7c0e a007 7c0d a101 0100 5700 6400 0400  |...|.....W.d...
+00001350: 0400 8303 0100 6e10 3100 7398 3000 0100  ......n.1.s.0...
+00001360: 0100 0100 5900 0100 7408 6a09 6a07 7401  ....Y...t.j.j.t.
+00001370: 6a02 a003 7c0c 640e a102 7c0b 640f 6410  j...|.d...|.d.d.
+00001380: 8d03 0100 7c06 6400 7501 9001 728a 7401  ....|.d.u...r.t.
+00001390: 6a02 a003 7c0c 6411 a102 7d0f 7408 6a09  j...|.d...}.t.j.
+000013a0: 6a07 7c0f 7c0b 6412 7c03 6413 8d04 0100  j.|.|.d.|.d.....
+000013b0: 6407 a003 6414 7c0f 9b00 9d02 6701 6415  d...d.|.....g.d.
+000013c0: 6416 8400 740a 7c04 8301 4400 8301 a201  d...t.|...D.....
+000013d0: a101 7d10 6407 a003 6417 6418 a003 7c05  ..}.d...d.d...|.
+000013e0: a101 9b00 6419 740b 9b00 9d04 641a 6702  ....d.t.....d.g.
+000013f0: a101 7d11 8800 7c06 8301 6a0c 7c10 7c11  ..}...|...j.|.|.
+00001400: 641b 8d02 7d12 7401 6a02 a003 7c0c 641c  d...}.t.j...|.d.
+00001410: a102 7d13 7406 7c13 640b 640c 640d 8d03  ..}.t.|.d.d.d...
+00001420: 8f1a 7d0e 7c0e a007 7c12 a101 0100 5700  ..}.|...|.....W.
+00001430: 6400 0400 0400 8303 0100 6e12 3100 9001  d.........n.1...
+00001440: 737e 3000 0100 0100 0100 5900 0100 6e08  s~0.......Y...n.
+00001450: 740d 641d 8301 8201 7c09 a00e 7c0c 7c0a  t.d.....|...|.|.
+00001460: 641e 1900 641f 9c02 a101 0100 7c08 6420  d...d.......|.d 
+00001470: 3700 7d08 711a 7c09 5300 2921 4e29 0172  7.}.q.|.S.)!N).r
+00001480: 2f00 0000 7201 0000 005a 0574 6173 6b5f  /...r....Z.task_
+00001490: 5a02 3036 5429 01da 0865 7869 7374 5f6f  Z.06T)...exist_o
+000014a0: 6bda 010a 6301 0000 0000 0000 0000 0000  k...c...........
+000014b0: 0003 0000 0005 0000 0053 0000 0073 2000  .........S...s .
+000014c0: 0000 6700 7c00 5d18 5c02 7d01 7d02 7c01  ..g.|.].\.}.}.|.
+000014d0: 6400 9b04 6401 7c02 9b00 9d03 9102 7104  d...d.|.......q.
+000014e0: 5300 2902 5a02 3332 fa01 2072 1e00 0000  S.).Z.32.. r....
+000014f0: 2903 7242 0000 00da 016b da01 7672 1e00  ).rB.....k..vr..
+00001500: 0000 721e 0000 0072 1f00 0000 7244 0000  ..r....r....rD..
+00001510: 009f 0000 0072 4500 0000 7a4a 5f5f 6578  .....rE...zJ__ex
+00001520: 706f 7274 5f72 656d 6f74 655f 6675 6e63  port_remote_func
+00001530: 7469 6f6e 732e 3c6c 6f63 616c 733e 2e6d  tions.<locals>.m
+00001540: 616b 655f 6c61 7370 5f74 6173 6b5f 6469  ake_lasp_task_di
+00001550: 7273 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  rs.<locals>.<lis
+00001560: 7463 6f6d 703e 7a07 6c61 7370 2e69 6eda  tcomp>z.lasp.in.
+00001570: 0177 7a05 7574 662d 3829 01da 0865 6e63  .wz.utf-8)...enc
+00001580: 6f64 696e 677a 086c 6173 702e 7374 72fa  odingz.lasp.str.
+00001590: 0864 6d6f 6c2d 6172 63a9 0172 5b00 0000  .dmol-arc..r[...
+000015a0: 7a0b 6c61 6d6d 7073 2e64 6174 617a 0b6c  z.lammps.dataz.l
+000015b0: 616d 6d70 732d 6461 7461 2902 725b 0000  ammps-data).r[..
+000015c0: 00da 0973 7065 636f 7264 6572 7a0a 7265  ...specorderz.re
+000015d0: 6164 5f64 6174 6120 6301 0000 0000 0000  ad_data c.......
+000015e0: 0000 0000 0003 0000 0005 0000 0073 0000  .............s..
+000015f0: 0073 2600 0000 7c00 5d1e 5c02 7d01 7d02  .s&...|.].\.}.}.
+00001600: 6400 7c01 6401 1700 9b00 6402 7c02 9b00  d.|.d.....d.|...
+00001610: 9d04 5600 0100 7102 6403 5300 2904 7a05  ..V...q.d.S.).z.
+00001620: 6d61 7373 2072 0f00 0000 7281 0000 004e  mass r....r....N
+00001630: 721e 0000 0029 0372 4200 0000 7277 0000  r....).rB...rw..
+00001640: 0072 4800 0000 721e 0000 0072 1e00 0000  .rH...r....r....
+00001650: 721f 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
+00001660: ab00 0000 7245 0000 007a 495f 5f65 7870  ....rE...zI__exp
+00001670: 6f72 745f 7265 6d6f 7465 5f66 756e 6374  ort_remote_funct
+00001680: 696f 6e73 2e3c 6c6f 6361 6c73 3e2e 6d61  ions.<locals>.ma
+00001690: 6b65 5f6c 6173 705f 7461 736b 5f64 6972  ke_lasp_task_dir
+000016a0: 732e 3c6c 6f63 616c 733e 2e3c 6765 6e65  s.<locals>.<gene
+000016b0: 7870 723e 7a12 7061 6972 5f73 7479 6c65  xpr>z.pair_style
+000016c0: 2064 6565 706d 6420 7281 0000 007a 0a20   deepmd r....z. 
+000016d0: 6f75 745f 6669 6c65 207a 0e70 6169 725f  out_file z.pair_
+000016e0: 636f 6566 6620 2a20 2a29 02da 1172 6561  coeff * *)...rea
+000016f0: 645f 6461 7461 5f73 6563 7469 6f6e da13  d_data_section..
+00001700: 666f 7263 655f 6669 656c 645f 7365 6374  force_field_sect
+00001710: 696f 6e7a 0969 6e2e 7369 6d70 6c65 723f  ionz.in.simpler?
+00001720: 0000 0072 5800 0000 2902 7247 0000 0072  ...rX...).rG...r
+00001730: 5800 0000 720f 0000 0029 0f72 1500 0000  X...r....).r....
+00001740: 7264 0000 0072 6500 0000 7266 0000 00da  rd...re...rf....
+00001750: 086d 616b 6564 6972 73da 0569 7465 6d73  .makedirs..items
+00001760: da04 6f70 656e da05 7772 6974 65da 0361  ..open..write..a
+00001770: 7365 da02 696f 7271 0000 0072 1400 0000  se..iorq...r....
+00001780: da0a 7375 6273 7469 7475 7465 726d 0000  ..substituterm..
+00001790: 0072 7000 0000 2914 7249 0000 0072 4a00  .rp...).rI...rJ.
+000017a0: 0000 724d 0000 0072 2f00 0000 7230 0000  ..rM...r/...r0..
+000017b0: 0072 4b00 0000 724c 0000 00da 0a69 6e70  .rK...rL.....inp
+000017c0: 7574 5f64 6174 6172 7700 0000 7257 0000  ut_datarw...rW..
+000017d0: 00da 0861 7274 6966 6163 74da 0561 746f  ...artifact..ato
+000017e0: 6d73 7260 0000 005a 0c6c 6173 705f 696e  msr`...Z.lasp_in
+000017f0: 5f74 6578 74da 0166 da09 6461 7461 5f66  _text..f..data_f
+00001800: 696c 6572 8a00 0000 728b 0000 00da 0c6c  iler....r......l
+00001810: 616d 6d70 735f 696e 7075 745a 116c 616d  ammps_inputZ.lam
+00001820: 6d70 735f 696e 7075 745f 6669 6c65 2901  mps_input_file).
+00001830: 727e 0000 0072 1e00 0000 721f 0000 0072  r~...r....r....r
+00001840: 6f00 0000 8f00 0000 7340 0000 0000 080c  o.......s@......
+00001850: 020a 010e 0216 010e 0218 011a 0128 021c  .............(..
+00001860: 010a 020e 0114 0204 0108 ff02 0210 fe06  ................
+00001870: 0404 0114 0102 fe06 0408 0102 0102 fe06  ................
+00001880: 040e 0110 012c 0208 0114 010a 017a 365f  .....,.......z6_
+00001890: 5f65 7870 6f72 745f 7265 6d6f 7465 5f66  _export_remote_f
+000018a0: 756e 6374 696f 6e73 2e3c 6c6f 6361 6c73  unctions.<locals
+000018b0: 3e2e 6d61 6b65 5f6c 6173 705f 7461 736b  >.make_lasp_task
+000018c0: 5f64 6972 7372 5900 0000 2901 7260 0000  _dirsrY...).r`..
+000018d0: 0063 0200 0000 0000 0000 0000 0000 0f00  .c..............
+000018e0: 0000 0800 0000 5300 0000 7300 0200 0074  ......S...s....t
+000018f0: 006a 01a0 027c 0064 01a1 027d 0274 006a  .j...|.d...}.t.j
+00001900: 01a0 027c 0064 02a1 027d 0374 036a 046a  ...|.d...}.t.j.j
+00001910: 057c 0264 0364 0464 058d 037d 0474 067c  .|.d.d.d...}.t.|
+00001920: 0264 0683 028f 267d 0574 0764 0764 0884  .d....&}.t.d.d..
+00001930: 007c 05a0 08a1 0044 0083 0183 017d 0657  .|.....D.....}.W
+00001940: 0064 0904 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+00001950: 6430 0001 0001 0001 0059 0001 0074 067c  d0.......Y...t.|
+00001960: 0364 0683 028f 3c7d 057c 05a0 08a1 007d  .d....<}.|.....}
+00001970: 0774 0764 0a64 0884 007c 0744 0083 0183  .t.d.d...|.D....
+00001980: 017d 0874 0764 0b64 0884 007c 0744 0083  .}.t.d.d...|.D..
+00001990: 0183 017d 0957 0064 0904 0004 0083 0301  ...}.W.d........
+000019a0: 006e 1031 0073 ba30 0001 0001 0001 0059  .n.1.s.0.......Y
+000019b0: 0001 0067 007d 0a74 097c 0683 0144 005d  ...g.}.t.|...D.]
+000019c0: 585c 027d 0b7d 0c74 0a7c 0883 0164 0c6b  X\.}.}.t.|...d.k
+000019d0: 0472 d074 0b6a 0c7c 0c7c 0864 0c19 0064  .r.t.j.|.|.d...d
+000019e0: 0c64 0d64 0e8d 0472 d07c 0974 0a7c 0a83  .d.d...r.|.t.|..
+000019f0: 0119 007c 047c 0b19 006a 0d64 0f3c 007c  ...|.|...j.d.<.|
+00001a00: 0aa0 0e7c 047c 0b19 00a1 0101 007c 08a0  ...|.|.......|..
+00001a10: 0f64 0ca1 0101 0071 d074 036a 046a 1074  .d.....q.t.j.j.t
+00001a20: 006a 01a0 027c 007c 01a1 027c 0a64 1064  .j...|.|...|.d.d
+00001a30: 058d 0301 0074 006a 01a0 027c 0074 11a1  .....t.j...|.t..
+00001a40: 027d 0d67 007d 0774 067c 0d64 0683 028f  .}.g.}.t.|.d....
+00001a50: 527d 0574 097c 0583 0144 005d 385c 027d  R}.t.|...D.]8\.}
+00001a60: 0b7d 0e7c 0b64 0c6b 0490 0172 9874 12a0  .}.|.d.k...r.t..
+00001a70: 1364 117c 0b64 1218 0064 139b 0464 149d  .d.|.d...d...d..
+00001a80: 027c 0ea1 037d 0e7c 07a0 0e7c 0ea1 0101  .|...}.|...|....
+00001a90: 0090 0171 6c57 0064 0904 0004 0083 0301  ...qlW.d........
+00001aa0: 006e 1231 0090 0173 bc30 0001 0001 0001  .n.1...s.0......
+00001ab0: 0059 0001 0074 067c 0d64 1583 028f 1a7d  .Y...t.|.d.....}
+00001ac0: 057c 05a0 147c 07a1 0101 0057 0064 0904  .|...|.....W.d..
+00001ad0: 0004 0083 0301 006e 1231 0090 0173 f230  .......n.1...s.0
+00001ae0: 0001 0001 0001 0059 0001 0064 0953 0029  .......Y...d.S.)
+00001af0: 1661 0c01 0000 0a20 2020 2020 2020 2041  .a.....        A
+00001b00: 6c69 676e 206c 6173 7020 6f75 7470 7574  lign lasp output
+00001b10: 2077 6974 6820 6d6f 6465 6c5f 6465 7669   with model_devi
+00001b20: 2072 6563 6f72 6473 2e0a 0a20 2020 2020   records...     
+00001b30: 2020 2041 7320 616c 6c73 7472 2e61 7263     As allstr.arc
+00001b40: 2063 6f6e 7461 696e 7320 616c 6c20 7468   contains all th
+00001b50: 6520 7374 7275 6374 7572 6573 2067 656e  e structures gen
+00001b60: 6572 6174 6564 2062 7920 4c41 5350 2c0a  erated by LASP,.
+00001b70: 2020 2020 2020 2020 7765 206e 6565 6420          we need 
+00001b80: 746f 2075 7365 2074 6865 2072 6573 756c  to use the resul
+00001b90: 7420 6f66 206c 6173 702e 6f75 7420 666f  t of lasp.out fo
+00001ba0: 7220 616c 6967 6e6d 656e 742e 0a0a 2020  r alignment...  
+00001bb0: 2020 2020 2020 5468 6520 666f 6c6c 6f77        The follow
+00001bc0: 696e 6720 636f 6465 2069 7320 636f 7079  ing code is copy
+00001bd0: 2066 726f 6d20 4368 6563 4d61 7465 2c20   from ChecMate, 
+00001be0: 6d61 7920 6e65 6564 2074 6f20 6265 2072  may need to be r
+00001bf0: 6566 6163 746f 7265 640a 2020 2020 2020  efactored.      
+00001c00: 2020 7a0a 616c 6c73 7472 2e61 7263 7a08    z.allstr.arcz.
+00001c10: 6c61 7370 2e6f 7574 7253 0000 0072 8600  lasp.outrS...r..
+00001c20: 0000 7287 0000 00da 0172 6301 0000 0000  ..r......rc.....
+00001c30: 0000 0000 0000 0002 0000 0006 0000 0073  ...............s
+00001c40: 0000 0073 3800 0000 7c00 5d30 7d01 6400  ...s8...|.]0}.d.
+00001c50: 7c01 7600 7202 7400 7401 7c01 6401 6402  |.v.r.t.t.|.d.d.
+00001c60: 8502 1900 a002 a100 a003 a100 6403 1900  ............d...
+00001c70: 8301 6404 8302 5600 0100 7102 6401 5300  ..d...V...q.d.S.
+00001c80: 2905 5a06 456e 6572 6779 4ee9 4900 0000  ).Z.EnergyN.I...
+00001c90: e9fe ffff ffe9 0600 0000 a904 da05 726f  ..............ro
+00001ca0: 756e 6472 3200 0000 da05 7374 7269 70da  undr2.....strip.
+00001cb0: 0573 706c 6974 a902 7242 0000 00da 046c  .split..rB.....l
+00001cc0: 696e 6572 1e00 0000 721e 0000 0072 1f00  iner....r....r..
+00001cd0: 0000 7289 0000 00cd 0000 0072 4500 0000  ..r........rE...
+00001ce0: 7a49 5f5f 6578 706f 7274 5f72 656d 6f74  zI__export_remot
+00001cf0: 655f 6675 6e63 7469 6f6e 732e 3c6c 6f63  e_functions.<loc
+00001d00: 616c 733e 2e70 726f 6365 7373 5f6c 6173  als>.process_las
+00001d10: 705f 6f75 7470 7574 2e3c 6c6f 6361 6c73  p_output.<locals
+00001d20: 3e2e 3c67 656e 6578 7072 3e4e 6301 0000  >.<genexpr>Nc...
+00001d30: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00001d40: 0073 0000 0073 3800 0000 7c00 5d30 7d01  .s...s8...|.]0}.
+00001d50: 6400 7c01 7600 7202 7400 7401 7c01 6401  d.|.v.r.t.t.|.d.
+00001d60: 6402 8502 1900 a002 a100 a003 a100 6403  d.............d.
+00001d70: 1900 8301 6404 8302 5600 0100 7102 6401  ....d...V...q.d.
+00001d80: 5300 2905 fa0c 456e 6572 6779 2c66 6f72  S.)...Energy,for
+00001d90: 6365 4e72 9a00 0000 7255 0000 0072 9c00  ceNr....rU...r..
+00001da0: 0000 729d 0000 0072 a100 0000 721e 0000  ..r....r....r...
+00001db0: 0072 1e00 0000 721f 0000 0072 8900 0000  .r....r....r....
+00001dc0: d000 0000 7245 0000 0063 0100 0000 0000  ....rE...c......
+00001dd0: 0000 0000 0000 0200 0000 0600 0000 7300  ..............s.
+00001de0: 0000 7338 0000 007c 005d 307d 0164 007c  ..s8...|.]0}.d.|
+00001df0: 0176 0072 0274 0074 017c 0164 0164 0285  .v.r.t.t.|.d.d..
+00001e00: 0219 00a0 02a1 00a0 03a1 0064 0319 0083  ...........d....
+00001e10: 0164 0483 0256 0001 0071 0264 0153 0029  .d...V...q.d.S.)
+00001e20: 0572 a300 0000 4e72 9a00 0000 720f 0000  .r....Nr....r...
+00001e30: 0072 9c00 0000 729d 0000 0072 a100 0000  .r....r....r....
+00001e40: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00001e50: 8900 0000 d100 0000 7245 0000 0072 0100  ........rE...r..
+00001e60: 0000 672d 431c ebe2 361a 3f29 02da 0472  ..g-C...6.?)...r
+00001e70: 746f 6cda 0461 746f 6c5a 0a73 7377 5f65  tol..atolZ.ssw_e
+00001e80: 6e65 7267 79da 0665 7874 7879 7a7a 075e  nergy..extxyzz.^
+00001e90: 5c73 2b5c 642b 720f 0000 007a 033e 3132  \s+\d+r....z.>12
+00001ea0: 7281 0000 0072 8400 0000 2915 7264 0000  r....r....).rd..
+00001eb0: 0072 6500 0000 7266 0000 0072 9000 0000  .re...rf...r....
+00001ec0: 7291 0000 00da 0472 6561 6472 8e00 0000  r......readr....
+00001ed0: da04 6c69 7374 da09 7265 6164 6c69 6e65  ..list..readline
+00001ee0: 7372 7100 0000 da03 6c65 6eda 026e 70da  srq.....len..np.
+00001ef0: 0769 7363 6c6f 7365 da04 696e 666f 7270  .isclose..inforp
+00001f00: 0000 00da 0370 6f70 728f 0000 0072 1400  .....popr....r..
+00001f10: 0000 da02 7265 da03 7375 62da 0a77 7269  ....re..sub..wri
+00001f20: 7465 6c69 6e65 7329 0f72 6000 0000 da09  telines).r`.....
+00001f30: 6669 6c65 5f6e 616d 655a 0c61 6c6c 5f73  file_nameZ.all_s
+00001f40: 7472 5f66 696c 655a 0d6c 6173 705f 6f75  tr_fileZ.lasp_ou
+00001f50: 745f 6669 6c65 5a08 616c 6c5f 7374 7273  t_fileZ.all_strs
+00001f60: 7296 0000 005a 0661 6c6c 5f71 73da 056c  r....Z.all_qs..l
+00001f70: 696e 6573 5a07 7472 616a 5f71 735a 0774  inesZ.traj_qsZ.t
+00001f80: 7261 6a5f 6573 5a09 7472 616a 5f73 7472  raj_esZ.traj_str
+00001f90: 7372 7700 0000 da01 715a 0f6d 6f64 656c  srw.....qZ.model
+00001fa0: 5f64 6576 695f 6669 6c65 72a2 0000 0072  _devi_filer....r
+00001fb0: 1e00 0000 721e 0000 0072 1f00 0000 da13  ....r....r......
+00001fc0: 7072 6f63 6573 735f 6c61 7370 5f6f 7574  process_lasp_out
+00001fd0: 7075 74bf 0000 0073 3200 0000 0009 0e01  put....s2.......
+00001fe0: 0e01 1202 0c01 3401 0c01 0801 1201 3002  ......4.......0.
+00001ff0: 0401 1002 2201 1601 0e01 0c02 1c02 0e01  ...."...........
+00002000: 0401 0c01 1001 0a02 1a01 2e01 0c01 7a36  ..............z6
+00002010: 5f5f 6578 706f 7274 5f72 656d 6f74 655f  __export_remote_
+00002020: 6675 6e63 7469 6f6e 732e 3c6c 6f63 616c  functions.<local
+00002030: 733e 2e70 726f 6365 7373 5f6c 6173 705f  s>.process_lasp_
+00002040: 6f75 7470 7574 e904 0000 00a9 0272 5700  output.......rW.
+00002050: 0000 da07 776f 726b 6572 7363 0200 0000  ....workersc....
+00002060: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002070: 1300 0000 732c 0000 0064 0164 006c 0089  ....s,...d.d.l..
+00002080: 0088 006a 017c 0164 028d 0187 0087 0166  ...j.|.d.......f
+00002090: 0264 0364 0484 087c 0044 0083 0183 0101  .d.d...|.D......
+000020a0: 0064 0053 0029 054e 7201 0000 0029 015a  .d.S.).Nr....).Z
+000020b0: 066e 5f6a 6f62 7363 0100 0000 0000 0000  .n_jobsc........
+000020c0: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
+000020d0: 731c 0000 007c 005d 147d 0188 00a0 0088  s....|.].}......
+000020e0: 01a1 017c 0183 0156 0001 0071 0264 0053  ...|...V...q.d.S
+000020f0: 0072 3700 0000 2901 5a07 6465 6c61 7965  .r7...).Z.delaye
+00002100: 6472 5f00 0000 2902 da06 6a6f 626c 6962  dr_...)...joblib
+00002110: 72b5 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00002120: 8900 0000 ea00 0000 7304 0000 0004 0202  ........s.......
+00002130: ff7a 4a5f 5f65 7870 6f72 745f 7265 6d6f  .zJ__export_remo
+00002140: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
+00002150: 6361 6c73 3e2e 7072 6f63 6573 735f 6c61  cals>.process_la
+00002160: 7370 5f6f 7574 7075 7473 2e3c 6c6f 6361  sp_outputs.<loca
+00002170: 6c73 3e2e 3c67 656e 6578 7072 3e29 0272  ls>.<genexpr>).r
+00002180: b900 0000 5a08 5061 7261 6c6c 656c 72b7  ....Z.Parallelr.
+00002190: 0000 0029 0172 b500 0000 2901 72b9 0000  ...).r....).r...
+000021a0: 0072 1f00 0000 7274 0000 00e8 0000 0073  .r....rt.......s
+000021b0: 0800 0000 0001 0801 1602 02fe 7a37 5f5f  ............z7__
+000021c0: 6578 706f 7274 5f72 656d 6f74 655f 6675  export_remote_fu
+000021d0: 6e63 7469 6f6e 732e 3c6c 6f63 616c 733e  nctions.<locals>
+000021e0: 2e70 726f 6365 7373 5f6c 6173 705f 6f75  .process_lasp_ou
+000021f0: 7470 7574 7329 0172 5900 0000 2901 72b6  tputs).rY...).r.
+00002200: 0000 0029 09da 0673 7472 696e 6772 7c00  ...)...stringr|.
+00002210: 0000 720b 0000 0072 0600 0000 7225 0000  ..r....r....r%..
+00002220: 0072 1c00 0000 7232 0000 0072 0c00 0000  .r....r2...r....
+00002230: 722c 0000 0029 0372 7c00 0000 726f 0000  r,...).r|...ro..
+00002240: 0072 7400 0000 721e 0000 0029 0272 7e00  .rt...r....).r~.
+00002250: 0000 72b5 0000 0072 1f00 0000 da19 5f5f  ..r....r......__
+00002260: 6578 706f 7274 5f72 656d 6f74 655f 6675  export_remote_fu
+00002270: 6e63 7469 6f6e 7388 0000 0073 2000 0000  nctions....s ...
+00002280: 0002 0c02 1003 0601 0201 0201 0601 0601  ................
+00002290: 0601 0601 06f9 1030 1029 1a09 0201 02fe  .......0.)......
+000022a0: 72bb 0000 0029 31da 1361 6932 5f6b 6974  r....)1..ai2_kit
+000022b0: 2e63 6f72 652e 7363 7269 7074 7202 0000  .core.scriptr...
+000022c0: 0072 0300 0000 7204 0000 00da 1561 6932  .r....r......ai2
+000022d0: 5f6b 6974 2e63 6f72 652e 6172 7469 6661  _kit.core.artifa
+000022e0: 6374 7205 0000 0072 0600 0000 da10 6169  ctr....r......ai
+000022f0: 325f 6b69 742e 636f 7265 2e6c 6f67 7207  2_kit.core.logr.
+00002300: 0000 005a 1061 6932 5f6b 6974 2e63 6f72  ...Z.ai2_kit.cor
+00002310: 652e 6a6f 6272 0800 0000 da11 6169 325f  e.jobr......ai2_
+00002320: 6b69 742e 636f 7265 2e75 7469 6c72 0900  kit.core.utilr..
+00002330: 0000 720a 0000 00da 0674 7970 696e 6772  ..r......typingr
+00002340: 0b00 0000 720c 0000 00da 0870 7964 616e  ....r......pydan
+00002350: 7469 6372 0d00 0000 da0b 6461 7461 636c  ticr......datacl
+00002360: 6173 7365 7372 0e00 0000 da05 6e75 6d70  assesr......nump
+00002370: 7972 ab00 0000 da06 6173 652e 696f 7290  yr......ase.ior.
+00002380: 0000 0072 6b00 0000 7264 0000 0072 af00  ...rk...rd...r..
+00002390: 0000 da05 6966 6163 6572 1000 0000 7211  ....ifacer....r.
+000023a0: 0000 00da 0863 6f6e 7374 616e 7472 1200  .....constantr..
+000023b0: 0000 7213 0000 0072 1400 0000 da04 6461  ..r....r......da
+000023c0: 7461 7215 0000 0072 1600 0000 7219 0000  tar....r....r...
+000023d0: 00da 066c 6f67 6765 7272 1700 0000 7226  ...loggerr....r&
+000023e0: 0000 0072 2d00 0000 7233 0000 0072 3400  ...r-...r3...r4.
+000023f0: 0000 727b 0000 0072 bb00 0000 726f 0000  ..r{...r....ro..
+00002400: 0072 7400 0000 721e 0000 0072 1e00 0000  .rt...r....r....
+00002410: 721e 0000 0072 1f00 0000 da08 3c6d 6f64  r....r......<mod
+00002420: 756c 653e 0100 0000 733e 0000 0014 0110  ule>....s>......
+00002430: 010c 010c 0110 0210 010c 010c 0208 0108  ................
+00002440: 0108 0108 0108 0210 0114 0110 0308 0310  ................
+00002450: 1310 0602 0110 0702 0112 0402 0112 0710  ................
+00002460: 4108 7104 fd02 0102 0102 fe              A.q........
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/updater.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/updater.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:20:56 2023 UTC, .py size: 186 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 78dd b964 ba00 0000  a.......x..d....
+00000000: 610d 0d0a 0000 0000 fbde b964 ba00 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 4700  m.Z.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6501 8303 5a06 6405  d.d...d.e...Z.d.
 00000060: 5300 2906 e900 0000 0029 01da 0942 6173  S.)......)...Bas
 00000070: 654d 6f64 656c 2903 da08 4f70 7469 6f6e  eModel)...Option
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/util.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul  6 07:55:32 2023 UTC, .py size: 6882 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7473 a664 e21a 0000  a.......ts.d....
+00000000: 610d 0d0a 0000 0000 533a be64 e21a 0000  a.......S:.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6502 8300 5c04 5a03 5a04  d...Z.e...\.Z.Z.
 00000050: 5a05 5a06 6401 5300 2904 e900 0000 004e  Z.Z.d.S.)......N
 00000060: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
 00000070: 0004 0000 0003 0000 0073 5a00 0000 7400  .........sZ...t.
@@ -72,15 +72,15 @@
 00000470: da05 7374 7269 70da 0573 706c 6974 7208  ..strip..splitr.
 00000480: 0000 0072 0600 0000 da07 6973 6469 6769  ...r......isdigi
 00000490: 7472 0700 0000 da06 6170 7065 6e64 da04  tr......append..
 000004a0: 6a6f 696e 2908 da02 6670 5a0b 7365 745f  join)...fpZ.set_
 000004b0: 7061 7474 6572 6eda 0976 6172 6961 626c  pattern..variabl
 000004c0: 6573 da0c 6f75 7470 7574 5f6c 696e 6573  es..output_lines
 000004d0: da04 6c69 6e65 5a09 7365 745f 6d61 7463  ..lineZ.set_matc
-000004e0: 6872 0900 0000 5a09 7661 725f 7661 6c75  hr....Z.var_valu
+000004e0: 6872 0900 0000 da09 7661 725f 7661 6c75  hr......var_valu
 000004f0: 6572 0b00 0000 720b 0000 0072 0c00 0000  er....r....r....
 00000500: da12 7072 6f63 6573 735f 6370 326b 5f6d  ..process_cp2k_m
 00000510: 6163 726f 1d00 0000 7324 0000 0000 020e  acro....s$......
 00000520: 0204 0104 0208 0208 010e 0204 0102 020a  ................
 00000530: 0104 020a 010e 030c 0210 0308 0202 030c  ................
 00000540: 037a 355f 5f65 7870 6f72 745f 7265 6d6f  .z5__export_remo
 00000550: 7465 5f66 756e 6374 696f 6e73 2e3c 6c6f  te_functions.<lo
@@ -127,25 +127,25 @@
 000007e0: 1300 0000 7324 0000 0088 017c 0083 015c  ....s$.....|...\
 000007f0: 027d 017d 0288 027c 027c 0183 027d 0388  .}.}...|.|...}..
 00000800: 0074 00a0 017c 03a1 0183 0153 00a9 014e  .t...|.....S...N
 00000810: a902 da02 696f da08 5374 7269 6e67 494f  ....io..StringIO
 00000820: 2904 721b 0000 0072 1c00 0000 5a0e 7072  ).r....r....Z.pr
 00000830: 6f63 6573 7365 645f 7465 7874 5a10 7375  ocessed_textZ.su
 00000840: 6273 7469 7475 7465 645f 7465 7874 2903  bstituted_text).
-00000850: 722d 0000 0072 1f00 0000 7212 0000 0072  r-...r....r....r
+00000850: 722e 0000 0072 2000 0000 7212 0000 0072  r....r ...r....r
 00000860: 0b00 0000 720c 0000 00da 0f6c 6f61 645f  ....r......load_
 00000870: 6370 326b 5f69 6e70 7574 7400 0000 7306  cp2k_inputt...s.
 00000880: 0000 0000 010c 010a 017a 325f 5f65 7870  .........z2__exp
 00000890: 6f72 745f 7265 6d6f 7465 5f66 756e 6374  ort_remote_funct
 000008a0: 696f 6e73 2e3c 6c6f 6361 6c73 3e2e 6c6f  ions.<locals>.lo
 000008b0: 6164 5f63 7032 6b5f 696e 7075 7463 0100  ad_cp2k_inputc..
 000008c0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
 000008d0: 0000 1300 0000 730e 0000 0088 0074 00a0  ......s......t..
-000008e0: 017c 00a1 0183 0153 0072 2e00 0000 722f  .|.....S.r....r/
-000008f0: 0000 0029 01da 0474 6578 7429 0172 3200  ...)...text).r2.
+000008e0: 017c 00a1 0183 0153 0072 2f00 0000 7230  .|.....S.r/...r0
+000008f0: 0000 0029 01da 0474 6578 7429 0172 3300  ...)...text).r3.
 00000900: 0000 720b 0000 0072 0c00 0000 da10 6c6f  ..r....r......lo
 00000910: 6164 735f 6370 326b 5f69 6e70 7574 7900  ads_cp2k_inputy.
 00000920: 0000 7302 0000 0000 017a 335f 5f65 7870  ..s......z3__exp
 00000930: 6f72 745f 7265 6d6f 7465 5f66 756e 6374  ort_remote_funct
 00000940: 696f 6e73 2e3c 6c6f 6361 6c73 3e2e 6c6f  ions.<locals>.lo
 00000950: 6164 735f 6370 326b 5f69 6e70 7574 6301  ads_cp2k_inputc.
 00000960: 0000 0000 0000 0000 0000 0001 0000 0004  ................
@@ -158,53 +158,53 @@
 000009d0: 5d68 5c02 7d02 7d03 7401 7c03 7402 8302  ]h\.}.}.t.|.t...
 000009e0: 7254 8801 a003 6401 7c01 1400 6402 7c02  rT....d.|...d.|.
 000009f0: 9b00 9d02 1700 a101 0100 8800 7c03 7c01  ............|.|.
 00000a00: 6403 1700 8302 0100 8801 a003 6401 7c01  d...........d.|.
 00000a10: 1400 6404 1700 a101 0100 7108 8801 a003  ..d.......q.....
 00000a20: 6401 7c01 1400 7c02 9b00 6405 7c03 9b00  d.|...|...d.|...
 00000a30: 9d03 1700 a101 0100 7108 6400 5300 2906  ........q.d.S.).
-00000a40: 4e72 2200 0000 7220 0000 00e9 0300 0000  Nr"...r ........
+00000a40: 4e72 2300 0000 7221 0000 00e9 0300 0000  Nr#...r!........
 00000a50: 7a04 2645 4e44 7a02 2020 2904 da05 6974  z.&ENDz.  )...it
 00000a60: 656d 73da 0a69 7369 6e73 7461 6e63 65da  ems..isinstance.
 00000a70: 0464 6963 7472 1900 0000 2904 5a0c 7365  .dictr....).Z.se
 00000a80: 6374 696f 6e5f 6469 6374 da06 696e 6465  ction_dict..inde
-00000a90: 6e74 da03 6b65 7972 2c00 0000 a902 da0c  nt..keyr,.......
+00000a90: 6e74 da03 6b65 7972 2d00 0000 a902 da0c  nt..keyr-.......
 00000aa0: 6475 6d70 5f73 6563 7469 6f6e 721d 0000  dump_sectionr...
-00000ab0: 0072 0b00 0000 720c 0000 0072 3c00 0000  .r....r....r<...
+00000ab0: 0072 0b00 0000 720c 0000 0072 3d00 0000  .r....r....r=...
 00000ac0: 8100 0000 730c 0000 0000 0210 020a 0218  ....s...........
 00000ad0: 020e 0214 037a 495f 5f65 7870 6f72 745f  .....zI__export_
 00000ae0: 7265 6d6f 7465 5f66 756e 6374 696f 6e73  remote_functions
 00000af0: 2e3c 6c6f 6361 6c73 3e2e 6475 6d70 735f  .<locals>.dumps_
 00000b00: 6370 326b 5f69 6e70 7574 2e3c 6c6f 6361  cp2k_input.<loca
 00000b10: 6c73 3e2e 6475 6d70 5f73 6563 7469 6f6e  ls>.dump_section
 00000b20: 7214 0000 0029 0172 0100 0000 2901 721a  r....).r....).r.
 00000b30: 0000 0029 01da 0a69 6e70 7574 5f64 6963  ...)...input_dic
-00000b40: 7472 0b00 0000 723b 0000 0072 0c00 0000  tr....r;...r....
+00000b40: 7472 0b00 0000 723c 0000 0072 0c00 0000  tr....r<...r....
 00000b50: da10 6475 6d70 735f 6370 326b 5f69 6e70  ..dumps_cp2k_inp
 00000b60: 7574 7d00 0000 7308 0000 0000 0204 0210  ut}...s.........
 00000b70: 0f08 027a 335f 5f65 7870 6f72 745f 7265  ...z3__export_re
 00000b80: 6d6f 7465 5f66 756e 6374 696f 6e73 2e3c  mote_functions.<
 00000b90: 6c6f 6361 6c73 3e2e 6475 6d70 735f 6370  locals>.dumps_cp
 00000ba0: 326b 5f69 6e70 7574 6302 0000 0000 0000  2k_inputc.......
 00000bb0: 0000 0000 0002 0000 0004 0000 0013 0000  ................
 00000bc0: 0073 1200 0000 7c01 a000 8800 7c00 8301  .s....|.....|...
-00000bd0: a101 0100 6400 5300 722e 0000 0029 01da  ....d.S.r....)..
-00000be0: 0577 7269 7465 2902 723d 0000 0072 1b00  .write).r=...r..
-00000bf0: 0000 2901 723e 0000 0072 0b00 0000 720c  ..).r>...r....r.
+00000bd0: a101 0100 6400 5300 722f 0000 0029 01da  ....d.S.r/...)..
+00000be0: 0577 7269 7465 2902 723e 0000 0072 1b00  .write).r>...r..
+00000bf0: 0000 2901 723f 0000 0072 0b00 0000 720c  ..).r?...r....r.
 00000c00: 0000 00da 0f64 756d 705f 6370 326b 5f69  .....dump_cp2k_i
 00000c10: 6e70 7574 9400 0000 7302 0000 0000 017a  nput....s......z
 00000c20: 325f 5f65 7870 6f72 745f 7265 6d6f 7465  2__export_remote
 00000c30: 5f66 756e 6374 696f 6e73 2e3c 6c6f 6361  _functions.<loca
 00000c40: 6c73 3e2e 6475 6d70 5f63 7032 6b5f 696e  ls>.dump_cp2k_in
-00000c50: 7075 7429 0172 3800 0000 2902 7234 0000  put).r8...).r4..
-00000c60: 0072 4000 0000 720b 0000 0029 0572 3e00  .r@...r....).r>.
-00000c70: 0000 7232 0000 0072 2d00 0000 721f 0000  ..r2...r-...r...
+00000c50: 7075 7429 0172 3900 0000 2902 7235 0000  put).r9...).r5..
+00000c60: 0072 4100 0000 720b 0000 0029 0572 3f00  .rA...r....).r?.
+00000c70: 0000 7233 0000 0072 2e00 0000 7220 0000  ..r3...r....r ..
 00000c80: 0072 1200 0000 720c 0000 00da 195f 5f65  .r....r......__e
 00000c90: 7870 6f72 745f 7265 6d6f 7465 5f66 756e  xport_remote_fun
 00000ca0: 6374 696f 6e73 0400 0000 7310 0000 0000  ctions....s.....
 00000cb0: 020e 1708 2508 3210 050c 0408 170c 0372  ....%.2........r
-00000cc0: 4100 0000 2907 7230 0000 0072 0e00 0000  A...).r0...r....
-00000cd0: 7241 0000 0072 4000 0000 723e 0000 0072  rA...r@...r>...r
-00000ce0: 3200 0000 7234 0000 0072 0b00 0000 720b  2...r4...r....r.
+00000cc0: 4200 0000 2907 7231 0000 0072 0e00 0000  B...).r1...r....
+00000cd0: 7242 0000 0072 4100 0000 723f 0000 0072  rB...rA...r?...r
+00000ce0: 3300 0000 7235 0000 0072 0b00 0000 720b  3...r5...r....r.
 00000cf0: 0000 0072 0b00 0000 720c 0000 00da 083c  ...r....r......<
 00000d00: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
 00000d10: 0801 0802 087f 001a 04fd 0201 0401 04fe  ................
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:22:50 2023 UTC, .py size: 7678 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 eadd b964 fe1d 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 fbde b964 fe1d 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7201 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/asap.py` & `ai2_kit-0.5.0/ai2_kit/domain/asap.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,152 +3,146 @@
 from asaplib.hypers.hyper_soap import universal_soap_hyper
 from asaplib.hypers.hyper_acsf import universal_acsf_hyper
 from asaplib.reducedim.dim_reducer import Dimension_Reducers
 from asaplib.cluster.ml_cluster_fit import LAIO_DB, sklearn_DB
 
 from scipy.spatial.distance import cdist
 
-from ai2_kit.core.util import merge_dict
-from ai2_kit.core.log import get_logger
-import copy
 import numpy as np
 
-logger = get_logger(__name__)
 
+def __export_remote_functions():
 
-def get_descriptor(asapxyz: ASAPXYZ, setting: dict, keep_atomic=False, n_process=4, path_prefix='./asap-descriptor'):
-    descriptor_spec = get_descriptor_spec(asapxyz, setting)
-    asapxyz.compute_global_descriptors(
-        desc_spec_dict = descriptor_spec,
-        keep_atomic = keep_atomic,
-        n_process = n_process,
-    )
-    asapxyz.save_state(path_prefix)
+    def get_descriptor(asapxyz: ASAPXYZ, setting: dict, keep_atomic=False, n_process=4, path_prefix='./asap-descriptor'):
 
-    global_descriptors = asapxyz.fetch_computed_descriptors(list(descriptor_spec.keys()))
-    atomic_descriptors = asapxyz.fetch_computed_atomic_descriptors(list(descriptor_spec.keys())) if keep_atomic else None
-    return global_descriptors, atomic_descriptors
-
-
-def get_descriptor_spec(asapxyz: ASAPXYZ, setting: dict):
-    descriptor_type = setting.get('type', 'SOAP').upper()
-    assert descriptor_type in ['SOAP', 'ACSF', 'CM'], f'Unknown descriptor type {descriptor_type}'
-
-    if descriptor_type == 'CM':
-        return {'cm': {'type': 'CM'}}
-
-    reducer_spec = dict(set_reducer(
-        setting['reducer_type'],
-        setting['element_wise'],
-        setting['zeta'],
-    ))
-
-    if descriptor_type == 'ACSF':
-        atomic_descriptor_spec = get_acsf_atomic_descriptor_spec(asapxyz, setting)
-    elif descriptor_type == 'SOAP':
-        atomic_descriptor_spec = get_soap_atomic_descriptor_spec(asapxyz, setting)
-
-    descriptor_spec = {}
-    for k, v in atomic_descriptor_spec.items():  # type: ignore
-        descriptor_spec[k] = {
-            'atomic_descriptor': {k: v},
-            'reducer_function': reducer_spec,
-        }
-    return descriptor_spec
+        descriptor_spec = get_descriptor_spec(asapxyz, setting)
+        asapxyz.compute_global_descriptors(
+            desc_spec_dict = descriptor_spec,
+            keep_atomic = keep_atomic,
+            n_process = n_process,
+        )
+        asapxyz.save_state(path_prefix)
+
+        global_descriptors = asapxyz.fetch_computed_descriptors(list(descriptor_spec.keys()))
+        atomic_descriptors = asapxyz.fetch_computed_atomic_descriptors(list(descriptor_spec.keys())) if keep_atomic else None
+        return global_descriptors, atomic_descriptors
+
+
+    def get_descriptor_spec(asapxyz: ASAPXYZ, setting: dict):
+        descriptor_type, params = None, None
+        for key in ['soap', 'acsf', 'cm']:
+            params = setting.get(key, None)
+            if params is not None:
+                descriptor_type = key
+                break
+        else:
+            raise ValueError('Unknown descriptor type')
+
+
+        if descriptor_type == 'cm':
+            return {'cm': {'type': 'CM'}}
+
+        reducer_spec = dict(set_reducer(
+            params['reducer_type'],
+            params['element_wise'],
+            params['zeta'],
+        ))
+
+        if descriptor_type == 'acsf':
+            atomic_descriptor_spec = get_acsf_atomic_descriptor_spec(asapxyz, params)
+        elif descriptor_type == 'soap':
+            atomic_descriptor_spec = get_soap_atomic_descriptor_spec(asapxyz, params)
+
+        descriptor_spec = {}
+        for k, v in atomic_descriptor_spec.items():  # type: ignore
+            descriptor_spec[k] = {
+                'atomic_descriptor': {k: v},
+                'reducer_function': reducer_spec,
+            }
+        return descriptor_spec
 
 
-def get_soap_atomic_descriptor_spec(asapxyz: ASAPXYZ, setting: dict):
-    preset = setting['preset']
-    if preset is None:
-       atomic_descriptor_spec = {
-            'soap1': {
-                'type': 'SOAP',
-                'cutoff': setting['r_cut'],
-                'n': setting['n_max'],
-                'l': setting['l_max'],
-                'atom_gaussian_width': setting['sigma'],
+    def get_soap_atomic_descriptor_spec(asapxyz: ASAPXYZ, params: dict):
+        preset = params['preset']
+        if preset is None:
+           atomic_descriptor_spec = {
+                'soap1': {
+                    'type': 'SOAP',
+                    'cutoff': params['r_cut'],
+                    'n': params['n_max'],
+                    'l': params['l_max'],
+                    'atom_gaussian_width': params['sigma'],
+                }
             }
-        }
-    else:
-        atomic_descriptor_spec = universal_soap_hyper(asapxyz.get_global_species(), preset, dump=False)
+        else:
+            atomic_descriptor_spec = universal_soap_hyper(asapxyz.get_global_species(), preset, dump=False)
 
-    for k in atomic_descriptor_spec.keys():
-        atomic_descriptor_spec[k]['rbf'] = setting['rbf']
-        atomic_descriptor_spec[k]['crossover'] = setting['crossover']
-
-    return atomic_descriptor_spec
-
-
-def get_acsf_atomic_descriptor_spec(asapxyz: ASAPXYZ, setting: dict):
-    preset = setting['preset']
-    facsf_param = setting['r_cut'] if preset is None else preset
-    return universal_acsf_hyper(asapxyz.get_global_species(), facsf_param, dump=False)
-
-
-def reduce_dimension(descriptors: np.ndarray, setting: dict):
-    reducer = Dimension_Reducers(setting)
-    reduced_descriptors = reducer.fit_transform(descriptors)
-    return reduced_descriptors
-
-
-def get_dbscan_trainer(descriptor: np.ndarray, metric='euclidean', eps=None, min_samples=2, eval_sample=50):
-    if eps is None:
-        n = len(descriptor)
-        sample = descriptor[np.random.choice(n, min(n, eval_sample), replace=False)]
-        # FIXME: the method to estimate eps is strange
-        eps = np.percentile(cdist(sample, descriptor, metric), min(100 * 10. / n, 100))  # type: ignore
-    return sklearn_DB(eps, min_samples, metrictype=metric)
-
-
-def get_fdb_trainer():
-    return LAIO_DB()
-
-
-def get_cluster(asapxyz: ASAPXYZ, descriptors: np.ndarray, trainer, path_prefix='./asap-cluster'):
-    options = {
-        'prefix': path_prefix,
-        'savexyz': False,
-        'savetxt': False,
-    }
-    labels: np.ndarray = cluster_process(asapxyz, trainer, descriptors, options)  # type: ignore
-
-    groups = {}
-    index = np.arange(len(labels))
-    for label in set(labels):
-        groups[label] = index[labels == label]
-    return groups
-
-
-def test(path: str):
-    from .constant import DEFAULT_ASAP_SOAP_DESC
-    asapxyz = ASAPXYZ(path)
-    setting = merge_dict(copy.deepcopy(DEFAULT_ASAP_SOAP_DESC), {'type': 'soap', 'preset': 'minimal'})
-    global_descriptors, atomic_descriptor = get_descriptor(asapxyz, setting, keep_atomic=False)
-    dim_reducer_setting = {
-        'pca': {
-            'type': 'PCA',
-            'parameter': {
-                'n_components': 3,
-                'scalecenter': True,
-            }
-        }
-    }
-    dim_reducer_setting = {
-        'tsne': {
-            'type': 'TSNE',
-            'parameter': {
-                'perplexity': 30,
-                'early_exaggeration': 12,
-                'learning_rate': 200,
-                'metric': 'euclidean',
-            }
+        for k in atomic_descriptor_spec.keys():
+            atomic_descriptor_spec[k]['rbf'] = params['rbf']
+            atomic_descriptor_spec[k]['crossover'] = params['crossover']
+
+        return atomic_descriptor_spec
+
+
+    def get_acsf_atomic_descriptor_spec(asapxyz: ASAPXYZ, params: dict):
+        preset = params['preset']
+        facsf_param = params['r_cut'] if preset is None else preset
+        return universal_acsf_hyper(asapxyz.get_global_species(), facsf_param, dump=False)
+
+
+    def reduce_dimension(descriptors: np.ndarray, setting: dict):
+        reducer = Dimension_Reducers(setting)
+        reduced_descriptors = reducer.fit_transform(descriptors)
+        return reduced_descriptors
+
+
+    def get_dbscan_trainer(descriptor: np.ndarray, metric='euclidean', eps=None, min_samples=2, eval_sample=50):
+        if eps is None:
+            n = len(descriptor)
+            sample = descriptor[np.random.choice(n, min(n, eval_sample), replace=False)]
+            # FIXME: the method to estimate eps is strange
+            eps = np.percentile(cdist(sample, descriptor, metric), min(100 * 10. / n, 100))  # type: ignore
+        return sklearn_DB(eps, min_samples, metrictype=metric)
+
+
+    def get_laio_db_trainer(**kwargs):
+        return LAIO_DB(**kwargs)
+
+
+    def get_trainer(descriptor: np.ndarray, setting: dict):
+        dbscan_setting = setting.get('dbscan', None)
+        if dbscan_setting is not None:
+            return get_dbscan_trainer(descriptor, **dbscan_setting)
+        laiodb_setting = setting.get('laiodb', None)
+        if laiodb_setting is not None:
+            return get_laio_db_trainer(**laiodb_setting)
+        raise ValueError('Unknown trainer type')
+
+
+    def get_cluster(asapxyz: ASAPXYZ, descriptors: np.ndarray, trainer, path_prefix='./asap-cluster'):
+        options = {
+            'prefix': path_prefix,
+            'savexyz': False,
+            'savetxt': False,
         }
-    }
-    reduced_descriptors = reduce_dimension(global_descriptors, dim_reducer_setting)
-    trainer = get_dbscan_trainer(global_descriptors)
-    r = get_cluster(asapxyz, reduced_descriptors, trainer)
-    print(r)
+        labels: np.ndarray = cluster_process(asapxyz, trainer, descriptors, options)  # type: ignore
+
+        groups = {}
+        index = np.arange(len(labels))
+        for label in set(labels):
+            groups[label] = index[labels == label]
+        return groups
+
+    return (
+        get_descriptor,
+        reduce_dimension,
+        get_trainer,
+        get_cluster,
+    )
 
 
-if __name__ == '__main__':
-    import fire
-    fire.Fire(test)
+(
+    get_descriptor,
+    reduce_dimension,
+    get_trainer,
+    get_cluster,
+) = __export_remote_functions()
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/constant.py` & `ai2_kit-0.5.0/ai2_kit/domain/constant.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 MODEL_DEVI_OUT = 'model_devi.out'
 MODEL_DEVI_NEU_OUT = 'model_devi_neu.out'
 MODEL_DEVI_RED_OUT = 'model_devi_red.out'
 
 LAMMPS_TRAJ_DIR = 'traj'
 LAMMPS_TRAJ_SUFFIX = '.lammpstrj'
-LAMMPS_DUMPS_CLASSIFIED = 'dumps_classified'
+
+SELECTOR_OUTPUT = 'selector_output'
 
 
 DEFAULT_LASP_IN = {
     "Run_type": 15,
     "SSW.SSWsteps": 20,
     "SSW.Temp": 300,
     "SSW.NG": 10,
@@ -72,7 +73,14 @@
     'rbf': 'gto',
 
     'reducer_type': 'average',
     'element_wise': False,
     'zeta': 1,
 }
 
+DEFAULT_ASAP_PCA_REDUCER = {
+    'type': 'PCA',
+            'parameter': {
+                'n_components': 3,
+                'scalecenter': True,
+            }
+}
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/cp2k.py` & `ai2_kit-0.5.0/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/data.py` & `ai2_kit-0.5.0/ai2_kit/domain/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from ai2_kit.core.artifact import Artifact, ArtifactDict
-from ai2_kit.core.util import dict_nested_get
+from ai2_kit.core.artifact import ArtifactDict
 
 from typing import List, Tuple, Optional
 from ase import Atoms
 
-from operator import itemgetter
 import ase.io
 import os
 
-from .constant import LAMMPS_TRAJ_DIR, LAMMPS_TRAJ_SUFFIX, LAMMPS_DUMPS_CLASSIFIED
-
 
 def __export_remote_functions():
     """workaround for cloudpickle issue"""
 
     class DataFormat:
         # customize data format
         CP2K_OUTPUT_DIR = 'cp2k/output_dir'
@@ -47,39 +43,23 @@
         if file_name.endswith('.xyz'):
             return DataFormat.EXTXYZ
         if 'POSCAR' in file_name:
             return DataFormat.VASP_POSCAR
         return None
 
 
-    def _get_selected_ids(artifact: dict) -> Optional[List[int]]:
-        return dict_nested_get(artifact, ['attrs', LAMMPS_DUMPS_CLASSIFIED, 'selected'], None)  # type: ignore
-
-
     def artifacts_to_ase_atoms(artifacts: List[ArtifactDict], type_map: List[str]) -> List[Tuple[ArtifactDict, Atoms]]:
         results = []
         for a in artifacts:
             data_format = get_data_format(a)  # type: ignore
             url = a['url']
-            selected_ids = _get_selected_ids(a)  # type: ignore
             if data_format == DataFormat.VASP_POSCAR:
                 atoms_list = ase.io.read(url, ':', format='vasp')
             elif data_format == DataFormat.EXTXYZ:
                 atoms_list = ase.io.read(url, ':', format='extxyz')
-            elif data_format == DataFormat.LAMMPS_OUTPUT_DIR:
-                assert selected_ids is not None, f'artifact {a} is not classified'
-                atoms_list = []
-                for dump_id in selected_ids:
-                    dump_file = os.path.join(url, LAMMPS_TRAJ_DIR, f'{dump_id}{LAMMPS_TRAJ_SUFFIX}')
-                    dump = ase.io.read(dump_file, ':', format='lammps-dump-text', order=False, specorder=type_map)
-                    atoms_list.extend(dump)
-            elif data_format == DataFormat.LASP_LAMMPS_OUT_DIR:
-                assert selected_ids is not None, f'artifact {a} is not classified'
-                traj_file = os.path.join(url, 'traj.xyz')
-                atoms_list = list(itemgetter(*selected_ids)(ase.io.read(traj_file, ':', format='extxyz')))  # type: ignore
             else:
                 raise ValueError(f'unsupported data format: {data_format}')
             results.extend((a, atoms) for atoms in atoms_list)
         return results
 
 
     def ase_atoms_to_cp2k_input_data(atoms: Atoms) -> Tuple[List[str], List[List[float]]]:
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/deepmd.py` & `ai2_kit-0.5.0/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/iface.py` & `ai2_kit-0.5.0/ai2_kit/domain/iface.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/lammps.py` & `ai2_kit-0.5.0/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/lasp.py` & `ai2_kit-0.5.0/ai2_kit/domain/lasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         lasp_in_data=lasp_in_data,
         dp_models=[m.url for m in input.models],
         lammps_input_template=lammps_input_template,
         base_dir=tasks_dir,
     )
 
     # generate steps
-    lasp_cmd = f'{ctx.config.lasp_cmd} 1 >> lasp.out >> lasp.err'
+    lasp_cmd = f'{ctx.config.lasp_cmd} 1 > lasp.out > lasp.err'
     steps = []
     for task_dir in task_dirs :
         steps.append(BashStep(cwd=task_dir['url'], cmd=lasp_cmd, checkpoint='lasp'))
 
     # submit jobs by the number of concurrency
     jobs = []
     for i, steps_group in enumerate(list_split(steps, ctx.config.concurrency)):
@@ -124,15 +124,15 @@
     executor.run_python_fn(process_lasp_outputs)(task_dirs=[a['url'] for a in task_dirs])
 
     output_dirs = [
         Artifact.of(
             url=task_dir['url'],
             executor=executor.name,
             format=DataFormat.LASP_LAMMPS_OUT_DIR,
-            attrs={ **task_dir['attrs'],  'traj_file': 'traj.xyz'},
+            attrs={ **task_dir['attrs'],  'structures_file': 'structures.xyz'},
         ) for task_dir in task_dirs]  # type: ignore
     return CllLaspOutput(output_dirs=output_dirs)
 
 
 def __export_remote_functions():
 
     from string import Template
@@ -184,15 +184,15 @@
             else:
                 raise ValueError('At least one potential should be specified.')
             task_dirs.append({'url': task_dir, 'attrs': artifact['attrs']})
             i += 1
         return task_dirs
 
 
-    def process_lasp_output(task_dir: str, file_name='traj.xyz'):
+    def process_lasp_output(task_dir: str, file_name='structures.xyz'):
         """
         Align lasp output with model_devi records.
 
         As allstr.arc contains all the structures generated by LASP,
         we need to use the result of lasp.out for alignment.
 
         The following code is copy from ChecMate, may need to be refactored
@@ -219,15 +219,15 @@
         ase.io.write(os.path.join(task_dir, file_name), traj_strs, format='extxyz')
         # edit model_devi.out
         model_devi_file = os.path.join(task_dir, MODEL_DEVI_OUT)
         lines = []
         with open(model_devi_file, "r") as f:
             for i, line in enumerate(f):
                 if i > 0:
-                    # replace step 0 with step i so that it can be aligned with traj.xyz
+                    # replace step 0 with step i so that it can be aligned with structures
                     line = re.sub(r'^\s+\d+', f'{i-1:>12} ', line)   #
                 lines.append(line)
         with open(model_devi_file, "w") as f:
             f.writelines(lines)
 
     def process_lasp_outputs(task_dirs: List[str], workers: int = 4):
         import joblib
```

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/util.py` & `ai2_kit-0.5.0/ai2_kit/domain/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/domain/vasp.py` & `ai2_kit-0.5.0/ai2_kit/domain/vasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/main.py` & `ai2_kit-0.5.0/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/tool/__pycache__/ase.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/tool/__pycache__/ase.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/tool/ase.py` & `ai2_kit-0.5.0/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul 21 01:22:55 2023 UTC, .py size: 10016 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 efdd b964 2027 0000  a..........d '..
+00000000: 610d 0d0a 0000 0000 8c43 be64 5027 0000  a........C.dP'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5601 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
@@ -273,21 +273,21 @@
 00001100: 0072 1f00 0000 da0c 7275 6e5f 776f 726b  .r......run_work
 00001110: 666c 6f77 5900 0000 731e 0000 0000 0508  flowY...s.......
 00001120: 0108 0208 010a 020a 0110 0108 0108 020c  ................
 00001130: 0102 0104 0104 0102 fd06 0572 4600 0000  ...........rF...
 00001140: 2904 7244 0000 0072 4500 0000 723c 0000  ).rD...rE...r<..
 00001150: 0072 3d00 0000 6304 0000 0000 0000 0000  .r=...c.........
 00001160: 0000 001f 0000 0008 0000 00c3 0000 0073  ...............s
-00001170: 0204 0000 7c00 6a00 7c02 1900 6a01 7d04  ....|.j.|...j.}.
+00001170: 0404 0000 7c00 6a00 7c02 1900 6a01 7d04  ....|.j.|...j.}.
 00001180: 7402 a003 7c00 6a04 a101 7d05 6400 7d06  t...|.j...}.d.}.
 00001190: 6400 7d07 6400 7d08 6400 7d09 6401 7d0a  d.}.d.}.d.}.d.}.
-000011a0: 7405 a006 6401 a101 4400 9003 5dc4 7d0b  t...d...D...].}.
+000011a0: 7405 a006 6401 a101 4400 9003 5dc6 7d0b  t...d...D...].}.
 000011b0: 7407 a008 7c05 a101 7d0c 7c0b 7c0c 6a09  t...|...}.|.|.j.
 000011c0: 6a0a 6b05 726a 740b a00c 6402 7c0b 9b00  j.k.rjt...d.|...
-000011d0: 6403 9d03 a101 0100 0100 9003 71fe 7c0c  d...........q.|.
+000011d0: 6403 9d03 a101 0100 0100 9004 7100 7c0c  d...........q.|.
 000011e0: 6a09 6a0d 7d0d 7c0c 6a09 6a0e 7d0e 740f  j.j.}.|.j.j.}.t.
 000011f0: 6a10 a011 7c03 6404 7c0b 6405 9b04 9d02  j...|.d.|.d.....
 00001200: a102 7d0f 6404 7c0b 6405 9b04 9d02 7d10  ..}.d.|.d.....}.
 00001210: 7c0c 6a12 6a13 9001 721a 7c04 6a12 6a13  |.j.j...r.|.j.j.
 00001220: 9001 721a 7413 6a14 7c0c 6a12 6a13 7c0d  ..r.t.j.|.j.j.|.
 00001230: 7c07 6400 7500 72c8 6700 6e06 7c07 a015  |.d.u.r.g.n.|...
 00001240: a100 7c0b 6401 6b04 6406 8d04 7d11 7413  ..|.d.k.d...}.t.
@@ -301,16 +301,16 @@
 000012c0: a100 7c0b 6401 6b04 6406 8d04 7d13 7419  ..|.d.k.d...}.t.
 000012d0: 6a1b 7c04 6a12 6a19 740f 6a10 a011 7c0f  j.|.j.j.t.j...|.
 000012e0: 640a a102 7c01 6408 8d03 7d14 7417 7c10  d...|.d...}.t.|.
 000012f0: 9b00 640b 9d02 8301 7419 6a1c 8301 7c13  ..d.....t.j...|.
 00001300: 7c14 8302 4900 6400 4800 7d06 6e08 741d  |...I.d.H.}.n.t.
 00001310: 640c 8301 8201 7c0b 6401 6b04 9001 72ce  d.....|.d.k...r.
 00001320: 741e 7c06 a01f a100 8301 6401 6b02 9001  t.|.......d.k...
-00001330: 72ce 740b a00c 640d a101 0100 0100 9003  r.t...d.........
-00001340: 71fe 7c0c 6a20 6a21 9002 724a 7421 6a22  q.|.j j!..rJt!j"
+00001330: 72ce 740b a00c 640d a101 0100 0100 9004  r.t...d.........
+00001340: 7100 7c0c 6a20 6a21 9002 724a 7421 6a22  q.|.j j!..rJt!j"
 00001350: 7c0c 6a20 6a21 7c0d 7c08 6400 7500 9001  |.j j!|.|.d.u...
 00001360: 72f2 6700 6e06 7c08 a023 a100 7c06 a01f  r.g.n.|..#..|...
 00001370: a100 7c0b 6401 6b04 640e 8d05 7d15 7421  ..|.d.k.d...}.t!
 00001380: 6a24 740f 6a10 a011 7c0f 640f a102 7c04  j$t.j...|.d...|.
 00001390: 6a20 6a21 7c01 6410 8d03 7d16 7417 7c10  j j!|.d...}.t.|.
 000013a0: 9b00 6411 9d02 8301 7421 6a25 8301 7c15  ..d.....t!j%..|.
 000013b0: 7c16 8302 4900 6400 4800 7d08 6e08 741d  |...I.d.H.}.n.t.
@@ -326,170 +326,172 @@
 00001450: 6a2d 9003 723c 742d 6a2e 7c0c 6a26 6a2d  j-..r<t-j.|.j&j-
 00001460: 7c0d 7c0e 7c08 a02a a100 6417 8d04 7d1a  |.|.|..*..d...}.
 00001470: 742d 6a2f 7c04 6a26 6a2d 740f 6a10 a011  t-j/|.j&j-t.j...
 00001480: 7c0f 6418 a102 7c01 6408 8d03 7d1b 7417  |.d...|.d...}.t.
 00001490: 7c10 9b00 6419 9d02 8301 742d 6a30 8301  |...d.....t-j0..
 000014a0: 7c1a 7c1b 8302 4900 6400 4800 7d09 6e08  |.|...I.d.H.}.n.
 000014b0: 741d 641a 8301 8201 7c0c 6a31 6a32 9003  t.d.....|.j1j2..
-000014c0: 72a2 7433 6a34 7c0c 6a31 6a32 7c09 a015  r.t3j4|.j1j2|...
-000014d0: a100 7435 6a36 641b 8d03 7d1c 7433 6a37  ..t5j6d...}.t3j7
-000014e0: 740f 6a10 a011 7c0f 641c a102 7c01 641d  t.j...|.d...|.d.
-000014f0: 8d02 7d1d 7417 7c10 9b00 641e 9d02 8301  ..}.t.|...d.....
-00001500: 7433 6a38 8301 7c1c 7c1d 8302 4900 6400  t3j8..|.|...I.d.
-00001510: 4800 7d07 6e08 741d 641f 8301 8201 7c0c  H.}.n.t.d.....|.
-00001520: 6a39 6a3a 7d1e 7c1e 6a3b 9003 73bc 7136  j9j:}.|.j;..s.q6
-00001530: 7c0a 741e 7c1e 6a3b 8301 6b05 9003 72ce  |.t.|.j;..k...r.
-00001540: 7136 7c07 a03c a100 7c1e 6a3d 6b04 7236  q6|..<..|.j=k.r6
-00001550: 743e 7402 a003 7c00 6a04 a101 7c1e 6a3b  t>t...|.j...|.j;
-00001560: 7c0a 1900 8302 7d05 7c0a 6420 3700 7d0a  |.....}.|.d 7.}.
-00001570: 7136 6400 5300 2921 4e72 0100 0000 7a0a  q6d.S.)!Nr....z.
-00001580: 4974 6572 6174 696f 6e20 7a23 2065 7863  Iteration z# exc
-00001590: 6565 6473 206d 6178 5f69 7465 7273 2c20  eeds max_iters, 
-000015a0: 7374 6f70 2069 7465 7261 7469 6f6e 2e7a  stop iteration.z
-000015b0: 0669 7465 7273 2d5a 0330 3364 2904 7244  .iters-Z.03d).rD
-000015c0: 0000 0072 2900 0000 5a0c 7379 7374 656d  ...r)...Z.system
-000015d0: 5f66 696c 6573 da09 696e 6974 6961 7465  _files..initiate
-000015e0: 647a 0a6c 6162 656c 2d63 7032 6b29 0372  dz.label-cp2k).r
-000015f0: 4400 0000 723d 0000 0072 4500 0000 7a0b  D...r=...rE...z.
-00001600: 2f6c 6162 656c 2d63 7032 6b7a 0a6c 6162  /label-cp2kz.lab
-00001610: 656c 2d76 6173 707a 0b2f 6c61 6265 6c2d  el-vaspz./label-
-00001620: 7661 7370 7a1c 4e6f 206c 6162 656c 206d  vaspz.No label m
-00001630: 6574 686f 6420 6973 2073 7065 6369 6669  ethod is specifi
-00001640: 6564 7a29 4e6f 206e 6577 2064 6174 6120  edz)No new data 
-00001650: 6973 2067 656e 6572 6174 6564 2c20 7374  is generated, st
-00001660: 6f70 2069 7465 7261 7469 6f6e 2e29 0572  op iteration.).r
-00001670: 4400 0000 7229 0000 005a 0b6f 6c64 5f64  D...r)...Z.old_d
-00001680: 6174 6173 6574 5a0b 6e65 775f 6461 7461  atasetZ.new_data
-00001690: 7365 7472 4700 0000 7a0c 7472 6169 6e2d  setrG...z.train-
-000016a0: 6465 6570 6d64 2903 723d 0000 0072 4400  deepmd).r=...rD.
-000016b0: 0000 7245 0000 007a 0d2f 7472 6169 6e2d  ..rE...z./train-
-000016c0: 6465 6570 6d64 7a1c 4e6f 2074 7261 696e  deepmdz.No train
-000016d0: 206d 6574 686f 6420 6973 2073 7065 6369   method is speci
-000016e0: 6669 6564 2901 da06 6d6f 6465 6c73 2904  fied)...models).
-000016f0: 7244 0000 0072 2900 0000 722a 0000 00da  rD...r)...r*....
-00001700: 0a6d 645f 6f70 7469 6f6e 737a 0e65 7870  .md_optionsz.exp
-00001710: 6c6f 7265 2d6c 616d 6d70 737a 0f2f 6578  lore-lammpsz./ex
-00001720: 706c 6f72 652d 6c61 6d6d 7073 2904 7244  plore-lammps).rD
-00001730: 0000 0072 2900 0000 722a 0000 0072 4800  ...r)...r*...rH.
-00001740: 0000 7a0c 6578 706c 6f72 652d 6c61 7370  ..z.explore-lasp
-00001750: 7a0d 2f65 7870 6c6f 7265 2d6c 6173 707a  z./explore-laspz
-00001760: 1e4e 6f20 6578 706c 6f72 6520 6d65 7468  .No explore meth
-00001770: 6f64 2069 7320 7370 6563 6966 6965 6429  od is specified)
-00001780: 0372 4400 0000 5a0f 6d6f 6465 6c5f 6465  .rD...Z.model_de
-00001790: 7669 5f64 6174 615a 176d 6f64 656c 5f64  vi_dataZ.model_d
-000017a0: 6576 695f 6f75 745f 6669 6c65 6e61 6d65  evi_out_filename
-000017b0: 7a12 7365 6c65 6374 6f72 2d74 6872 6573  z.selector-thres
-000017c0: 686f 6c64 2902 723d 0000 0072 4500 0000  hold).r=...rE...
-000017d0: 7a13 2f73 656c 6563 746f 722d 7468 7265  z./selector-thre
-000017e0: 7368 6f6c 647a 1d4e 6f20 7365 6c65 6374  sholdz.No select
-000017f0: 206d 6574 686f 6420 6973 2073 7065 6369   method is speci
-00001800: 6669 6564 e901 0000 0029 3f72 3900 0000  fied.....)?r9...
-00001810: 7227 0000 00da 0463 6f70 79da 0864 6565  r'.....copy..dee
-00001820: 7063 6f70 7972 3b00 0000 da09 6974 6572  pcopyr;.....iter
-00001830: 746f 6f6c 73da 0563 6f75 6e74 7228 0000  tools..countr(..
-00001840: 0072 3f00 0000 7235 0000 0072 2c00 0000  .r?...r5...r,...
-00001850: da06 6c6f 6767 6572 da04 696e 666f 7229  ..logger..infor)
-00001860: 0000 0072 2a00 0000 da02 6f73 da04 7061  ...r*.....os..pa
-00001870: 7468 da04 6a6f 696e 7225 0000 0072 0f00  th..joinr%...r..
-00001880: 0000 5a0c 436c 6c43 7032 6b49 6e70 7574  ..Z.CllCp2kInput
-00001890: 5a16 6765 745f 6d6f 6465 6c5f 6465 7669  Z.get_model_devi
-000018a0: 5f64 6174 6173 6574 5a0e 436c 6c43 7032  _datasetZ.CllCp2
-000018b0: 6b43 6f6e 7465 7874 7209 0000 005a 0863  kContextr....Z.c
-000018c0: 6c6c 5f63 7032 6b72 1000 0000 5a0c 436c  ll_cp2kr....Z.Cl
-000018d0: 6c56 6173 7049 6e70 7574 5a0e 436c 6c56  lVaspInputZ.CllV
-000018e0: 6173 7043 6f6e 7465 7874 5a08 636c 6c5f  aspContextZ.cll_
-000018f0: 7661 7370 7240 0000 00da 036c 656e 5a1a  vaspr@.....lenZ.
-00001900: 6765 745f 6c61 6265 6c65 645f 7379 7374  get_labeled_syst
-00001910: 656d 5f64 6174 6173 6574 7223 0000 0072  em_datasetr#...r
-00001920: 0a00 0000 5a0e 436c 6c44 6565 706d 6449  ....Z.CllDeepmdI
-00001930: 6e70 7574 5a14 6765 745f 7472 6169 6e69  nputZ.get_traini
-00001940: 6e67 5f64 6174 6173 6574 5a10 436c 6c44  ng_datasetZ.CllD
-00001950: 6565 706d 6443 6f6e 7465 7874 5a0a 636c  eepmdContextZ.cl
-00001960: 6c5f 6465 6570 6d64 7224 0000 0072 0c00  l_deepmdr$...r..
-00001970: 0000 5a0e 436c 6c4c 616d 6d70 7349 6e70  ..Z.CllLammpsInp
-00001980: 7574 5a09 4d64 4f70 7469 6f6e 735a 0e67  utZ.MdOptionsZ.g
-00001990: 6574 5f6d 6c70 5f6d 6f64 656c 735a 1043  et_mlp_modelsZ.C
-000019a0: 6c6c 4c61 6d6d 7073 436f 6e74 6578 745a  llLammpsContextZ
-000019b0: 0a63 6c6c 5f6c 616d 6d70 7372 0d00 0000  .cll_lammpsr....
-000019c0: 5a0c 436c 6c4c 6173 7049 6e70 7574 5a0e  Z.CllLaspInputZ.
-000019d0: 436c 6c4c 6173 7043 6f6e 7465 7874 5a08  CllLaspContextZ.
-000019e0: 636c 6c5f 6c61 7370 7236 0000 0072 3100  cll_laspr6...r1.
-000019f0: 0000 720e 0000 005a 1943 6c6c 4d6f 6465  ..r....Z.CllMode
-00001a00: 6c44 6576 6953 656c 6563 746f 7249 6e70  lDeviSelectorInp
-00001a10: 7574 da05 636f 6e73 745a 0e4d 4f44 454c  ut..constZ.MODEL
-00001a20: 5f44 4556 495f 4f55 545a 1a43 6c6c 4d6f  _DEVI_OUTZ.CllMo
-00001a30: 6465 6c44 6576 5365 6c65 6374 6f72 436f  delDevSelectorCo
-00001a40: 6e74 6578 745a 0c63 6c6c 5f73 656c 6563  ntextZ.cll_selec
-00001a50: 746f 7272 3700 0000 7233 0000 00da 0574  torr7...r3.....t
-00001a60: 6162 6c65 5a10 6765 745f 7061 7373 696e  ableZ.get_passin
-00001a70: 675f 7261 7465 5a16 7061 7373 696e 675f  g_rateZ.passing_
-00001a80: 7261 7465 5f74 6872 6573 686f 6c64 7206  rate_thresholdr.
-00001a90: 0000 0029 1f72 4400 0000 7245 0000 0072  ...).rD...rE...r
-00001aa0: 3c00 0000 723d 0000 005a 0e63 6f6e 7465  <...r=...Z.conte
-00001ab0: 7874 5f63 6f6e 6669 675a 1372 6177 5f77  xt_configZ.raw_w
-00001ac0: 6f72 6b66 6c6f 775f 636f 6e66 6967 5a0c  orkflow_configZ.
-00001ad0: 6c61 6265 6c5f 6f75 7470 7574 5a0f 7365  label_outputZ.se
-00001ae0: 6c65 6374 6f72 5f6f 7574 7075 745a 0c74  lector_outputZ.t
-00001af0: 7261 696e 5f6f 7574 7075 745a 0e65 7870  rain_outputZ.exp
-00001b00: 6c6f 7265 5f6f 7574 7075 745a 0d75 7064  lore_outputZ.upd
-00001b10: 6174 655f 6375 7273 6f72 da01 695a 0f77  ate_cursor..iZ.w
-00001b20: 6f72 6b66 6c6f 775f 636f 6e66 6967 7229  orkflow_configr)
-00001b30: 0000 0072 2a00 0000 5a10 6974 6572 5f70  ...r*...Z.iter_p
-00001b40: 6174 685f 7072 6566 6978 5a09 6370 5f70  ath_prefixZ.cp_p
-00001b50: 7265 6669 785a 0a63 7032 6b5f 696e 7075  refixZ.cp2k_inpu
-00001b60: 745a 0c63 7032 6b5f 636f 6e74 6578 745a  tZ.cp2k_contextZ
-00001b70: 0a76 6173 705f 696e 7075 745a 0c76 6173  .vasp_inputZ.vas
-00001b80: 705f 636f 6e74 6578 745a 0c64 6565 706d  p_contextZ.deepm
-00001b90: 645f 696e 7075 745a 0e64 6565 706d 645f  d_inputZ.deepmd_
-00001ba0: 636f 6e74 6578 7472 4900 0000 5a0c 6c61  contextrI...Z.la
-00001bb0: 6d6d 7073 5f69 6e70 7574 5a0e 6c61 6d6d  mmps_inputZ.lamm
-00001bc0: 7073 5f63 6f6e 7465 7874 5a0a 6c61 7370  ps_contextZ.lasp
-00001bd0: 5f69 6e70 7574 5a0c 6c61 7370 5f63 6f6e  _inputZ.lasp_con
-00001be0: 7465 7874 5a0e 7365 6c65 6374 6f72 5f69  textZ.selector_i
-00001bf0: 6e70 7574 5a10 7365 6c65 6374 6f72 5f63  nputZ.selector_c
-00001c00: 6f6e 7465 7874 5a0d 7570 6461 7465 5f63  ontextZ.update_c
-00001c10: 6f6e 6669 6772 1e00 0000 721e 0000 0072  onfigr....r....r
-00001c20: 1f00 0000 7243 0000 0072 0000 0073 e600  ....rC...r...s..
-00001c30: 0000 0001 0c01 0c03 0401 0401 0401 0403  ................
-00001c40: 0403 1003 0a01 0c01 1201 0603 0801 0803  ................
-00001c50: 1602 0c03 1401 0401 0601 0201 1201 06fc  ................
-00001c60: 0606 0401 0601 0c01 02fd 0605 2202 1401  ............"...
-00001c70: 0401 0601 0201 1401 06fc 0606 0401 0601  ................
-00001c80: 0c01 02fd 0605 2203 0803 1c01 0a01 0603  ......".........
-00001c90: 0a01 0401 0601 0201 1401 0601 06fb 0607  ................
-00001ca0: 0401 0c01 0601 02fd 0605 2203 0803 1401  ..........".....
-00001cb0: 0601 06ff 0603 0401 0601 0201 0201 02fc  ................
-00001cc0: 0606 0401 0c01 0601 02fd 0605 2202 1401  ............"...
-00001cd0: 0401 0601 0201 0201 06fc 0606 0401 0601  ................
-00001ce0: 0c01 02fd 0605 2203 0803 0a01 0401 0601  ......".........
-00001cf0: 0601 04fd 0605 0401 0c01 02fe 0604 2203  ..............".
-00001d00: 0803 0803 0801 0202 1001 0203 0e01 0601  ................
-00001d10: 04ff 0201 08ff 0402 7243 0000 00da 085f  ........rC....._
-00001d20: 5f6d 6169 6e5f 5f29 2e5a 1561 6932 5f6b  _main__).Z.ai2_k
-00001d30: 6974 2e63 6f72 652e 6578 6563 7574 6f72  it.core.executor
-00001d40: 7202 0000 005a 1561 6932 5f6b 6974 2e63  r....Z.ai2_kit.c
-00001d50: 6f72 652e 6172 7469 6661 6374 7203 0000  ore.artifactr...
-00001d60: 005a 1061 6932 5f6b 6974 2e63 6f72 652e  .Z.ai2_kit.core.
-00001d70: 6c6f 6772 0400 0000 5a11 6169 325f 6b69  logr....Z.ai2_ki
-00001d80: 742e 636f 7265 2e75 7469 6c72 0500 0000  t.core.utilr....
-00001d90: 7206 0000 005a 1d61 6932 5f6b 6974 2e63  r....Z.ai2_kit.c
-00001da0: 6f72 652e 7265 736f 7572 6365 5f6d 616e  ore.resource_man
-00001db0: 6167 6572 7207 0000 00da 1761 6932 5f6b  agerr......ai2_k
-00001dc0: 6974 2e63 6f72 652e 6368 6563 6b70 6f69  it.core.checkpoi
-00001dd0: 6e74 7208 0000 0072 0900 0000 5a0e 6169  ntr....r....Z.ai
-00001de0: 325f 6b69 742e 646f 6d61 696e 720a 0000  2_kit.domainr...
-00001df0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00001e00: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00001e10: 1100 0000 7255 0000 0072 1200 0000 5a08  ....rU...r....Z.
-00001e20: 7079 6461 6e74 6963 7213 0000 00da 0674  pydanticr......t
-00001e30: 7970 696e 6772 1400 0000 7215 0000 0072  ypingr....r....r
-00001e40: 1600 0000 7217 0000 00da 0466 6972 6572  ....r......firer
-00001e50: 1800 0000 7241 0000 0072 4d00 0000 724b  ....rA...rM...rK
-00001e60: 0000 0072 5100 0000 721a 0000 0072 4f00  ...rQ...r....rO.
-00001e70: 0000 7219 0000 0072 2800 0000 7238 0000  ..r....r(...r8..
-00001e80: 0072 2d00 0000 7246 0000 0072 4300 0000  .r-...rF...rC...
-00001e90: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00001ea0: 1f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00001eb0: 0000 7334 0000 000c 010c 010c 0110 010c  ..s4............
-00001ec0: 0110 012c 0c0c 0118 010c 0208 0108 0108  ...,............
-00001ed0: 0108 0208 0310 1410 1f10 0702 0104 ff0a  ................
-00001ee0: 010c ff0c 1914 7f00 1c0a 02              ...........
+000014c0: 72a4 7433 6a34 7c0c 6a31 6a32 7c09 a015  r.t3j4|.j1j2|...
+000014d0: a100 7435 6a36 7c0d 641b 8d04 7d1c 7433  ..t5j6|.d...}.t3
+000014e0: 6a37 740f 6a10 a011 7c0f 641c a102 7c01  j7t.j...|.d...|.
+000014f0: 641d 8d02 7d1d 7417 7c10 9b00 641e 9d02  d...}.t.|...d...
+00001500: 8301 7433 6a38 8301 7c1c 7c1d 8302 4900  ..t3j8..|.|...I.
+00001510: 6400 4800 7d07 6e08 741d 641f 8301 8201  d.H.}.n.t.d.....
+00001520: 7c0c 6a39 6a3a 7d1e 7c1e 6a3b 9003 73be  |.j9j:}.|.j;..s.
+00001530: 7136 7c0a 741e 7c1e 6a3b 8301 6b05 9003  q6|.t.|.j;..k...
+00001540: 72d0 7136 7c07 a03c a100 7c1e 6a3d 6b04  r.q6|..<..|.j=k.
+00001550: 7236 743e 7402 a003 7c00 6a04 a101 7c1e  r6t>t...|.j...|.
+00001560: 6a3b 7c0a 1900 8302 7d05 7c0a 6420 3700  j;|.....}.|.d 7.
+00001570: 7d0a 7136 6400 5300 2921 4e72 0100 0000  }.q6d.S.)!Nr....
+00001580: 7a0a 4974 6572 6174 696f 6e20 7a23 2065  z.Iteration z# e
+00001590: 7863 6565 6473 206d 6178 5f69 7465 7273  xceeds max_iters
+000015a0: 2c20 7374 6f70 2069 7465 7261 7469 6f6e  , stop iteration
+000015b0: 2e7a 0669 7465 7273 2d5a 0330 3364 2904  .z.iters-Z.03d).
+000015c0: 7244 0000 0072 2900 0000 5a0c 7379 7374  rD...r)...Z.syst
+000015d0: 656d 5f66 696c 6573 da09 696e 6974 6961  em_files..initia
+000015e0: 7465 647a 0a6c 6162 656c 2d63 7032 6b29  tedz.label-cp2k)
+000015f0: 0372 4400 0000 723d 0000 0072 4500 0000  .rD...r=...rE...
+00001600: 7a0b 2f6c 6162 656c 2d63 7032 6b7a 0a6c  z./label-cp2kz.l
+00001610: 6162 656c 2d76 6173 707a 0b2f 6c61 6265  abel-vaspz./labe
+00001620: 6c2d 7661 7370 7a1c 4e6f 206c 6162 656c  l-vaspz.No label
+00001630: 206d 6574 686f 6420 6973 2073 7065 6369   method is speci
+00001640: 6669 6564 7a29 4e6f 206e 6577 2064 6174  fiedz)No new dat
+00001650: 6120 6973 2067 656e 6572 6174 6564 2c20  a is generated, 
+00001660: 7374 6f70 2069 7465 7261 7469 6f6e 2e29  stop iteration.)
+00001670: 0572 4400 0000 7229 0000 005a 0b6f 6c64  .rD...r)...Z.old
+00001680: 5f64 6174 6173 6574 5a0b 6e65 775f 6461  _datasetZ.new_da
+00001690: 7461 7365 7472 4700 0000 7a0c 7472 6169  tasetrG...z.trai
+000016a0: 6e2d 6465 6570 6d64 2903 723d 0000 0072  n-deepmd).r=...r
+000016b0: 4400 0000 7245 0000 007a 0d2f 7472 6169  D...rE...z./trai
+000016c0: 6e2d 6465 6570 6d64 7a1c 4e6f 2074 7261  n-deepmdz.No tra
+000016d0: 696e 206d 6574 686f 6420 6973 2073 7065  in method is spe
+000016e0: 6369 6669 6564 2901 da06 6d6f 6465 6c73  cified)...models
+000016f0: 2904 7244 0000 0072 2900 0000 722a 0000  ).rD...r)...r*..
+00001700: 00da 0a6d 645f 6f70 7469 6f6e 737a 0e65  ...md_optionsz.e
+00001710: 7870 6c6f 7265 2d6c 616d 6d70 737a 0f2f  xplore-lammpsz./
+00001720: 6578 706c 6f72 652d 6c61 6d6d 7073 2904  explore-lammps).
+00001730: 7244 0000 0072 2900 0000 722a 0000 0072  rD...r)...r*...r
+00001740: 4800 0000 7a0c 6578 706c 6f72 652d 6c61  H...z.explore-la
+00001750: 7370 7a0d 2f65 7870 6c6f 7265 2d6c 6173  spz./explore-las
+00001760: 707a 1e4e 6f20 6578 706c 6f72 6520 6d65  pz.No explore me
+00001770: 7468 6f64 2069 7320 7370 6563 6966 6965  thod is specifie
+00001780: 6429 0472 4400 0000 5a0f 6d6f 6465 6c5f  d).rD...Z.model_
+00001790: 6465 7669 5f64 6174 615a 176d 6f64 656c  devi_dataZ.model
+000017a0: 5f64 6576 695f 6f75 745f 6669 6c65 6e61  _devi_out_filena
+000017b0: 6d65 7229 0000 007a 1373 656c 6563 746f  mer)...z.selecto
+000017c0: 722d 6d6f 6465 6c2d 6465 7669 2902 723d  r-model-devi).r=
+000017d0: 0000 0072 4500 0000 7a14 2f73 656c 6563  ...rE...z./selec
+000017e0: 746f 722d 6d6f 6465 6c2d 6465 7669 7a1d  tor-model-deviz.
+000017f0: 4e6f 2073 656c 6563 7420 6d65 7468 6f64  No select method
+00001800: 2069 7320 7370 6563 6966 6965 64e9 0100   is specified...
+00001810: 0000 293f 7239 0000 0072 2700 0000 da04  ..)?r9...r'.....
+00001820: 636f 7079 da08 6465 6570 636f 7079 723b  copy..deepcopyr;
+00001830: 0000 00da 0969 7465 7274 6f6f 6c73 da05  .....itertools..
+00001840: 636f 756e 7472 2800 0000 723f 0000 0072  countr(...r?...r
+00001850: 3500 0000 722c 0000 00da 066c 6f67 6765  5...r,.....logge
+00001860: 72da 0469 6e66 6f72 2900 0000 722a 0000  r..infor)...r*..
+00001870: 00da 026f 73da 0470 6174 68da 046a 6f69  ...os..path..joi
+00001880: 6e72 2500 0000 720f 0000 005a 0c43 6c6c  nr%...r....Z.Cll
+00001890: 4370 326b 496e 7075 745a 1667 6574 5f6d  Cp2kInputZ.get_m
+000018a0: 6f64 656c 5f64 6576 695f 6461 7461 7365  odel_devi_datase
+000018b0: 745a 0e43 6c6c 4370 326b 436f 6e74 6578  tZ.CllCp2kContex
+000018c0: 7472 0900 0000 5a08 636c 6c5f 6370 326b  tr....Z.cll_cp2k
+000018d0: 7210 0000 005a 0c43 6c6c 5661 7370 496e  r....Z.CllVaspIn
+000018e0: 7075 745a 0e43 6c6c 5661 7370 436f 6e74  putZ.CllVaspCont
+000018f0: 6578 745a 0863 6c6c 5f76 6173 7072 4000  extZ.cll_vaspr@.
+00001900: 0000 da03 6c65 6e5a 1a67 6574 5f6c 6162  ....lenZ.get_lab
+00001910: 656c 6564 5f73 7973 7465 6d5f 6461 7461  eled_system_data
+00001920: 7365 7472 2300 0000 720a 0000 005a 0e43  setr#...r....Z.C
+00001930: 6c6c 4465 6570 6d64 496e 7075 745a 1467  llDeepmdInputZ.g
+00001940: 6574 5f74 7261 696e 696e 675f 6461 7461  et_training_data
+00001950: 7365 745a 1043 6c6c 4465 6570 6d64 436f  setZ.CllDeepmdCo
+00001960: 6e74 6578 745a 0a63 6c6c 5f64 6565 706d  ntextZ.cll_deepm
+00001970: 6472 2400 0000 720c 0000 005a 0e43 6c6c  dr$...r....Z.Cll
+00001980: 4c61 6d6d 7073 496e 7075 745a 094d 644f  LammpsInputZ.MdO
+00001990: 7074 696f 6e73 5a0e 6765 745f 6d6c 705f  ptionsZ.get_mlp_
+000019a0: 6d6f 6465 6c73 5a10 436c 6c4c 616d 6d70  modelsZ.CllLammp
+000019b0: 7343 6f6e 7465 7874 5a0a 636c 6c5f 6c61  sContextZ.cll_la
+000019c0: 6d6d 7073 720d 0000 005a 0c43 6c6c 4c61  mmpsr....Z.CllLa
+000019d0: 7370 496e 7075 745a 0e43 6c6c 4c61 7370  spInputZ.CllLasp
+000019e0: 436f 6e74 6578 745a 0863 6c6c 5f6c 6173  ContextZ.cll_las
+000019f0: 7072 3600 0000 7231 0000 0072 0e00 0000  pr6...r1...r....
+00001a00: 5a19 436c 6c4d 6f64 656c 4465 7669 5365  Z.CllModelDeviSe
+00001a10: 6c65 6374 6f72 496e 7075 74da 0563 6f6e  lectorInput..con
+00001a20: 7374 5a0e 4d4f 4445 4c5f 4445 5649 5f4f  stZ.MODEL_DEVI_O
+00001a30: 5554 5a1a 436c 6c4d 6f64 656c 4465 7653  UTZ.CllModelDevS
+00001a40: 656c 6563 746f 7243 6f6e 7465 7874 5a17  electorContextZ.
+00001a50: 636c 6c5f 6d6f 6465 6c5f 6465 7669 5f73  cll_model_devi_s
+00001a60: 656c 6563 746f 7272 3700 0000 7233 0000  electorr7...r3..
+00001a70: 00da 0574 6162 6c65 5a10 6765 745f 7061  ...tableZ.get_pa
+00001a80: 7373 696e 675f 7261 7465 5a16 7061 7373  ssing_rateZ.pass
+00001a90: 696e 675f 7261 7465 5f74 6872 6573 686f  ing_rate_thresho
+00001aa0: 6c64 7206 0000 0029 1f72 4400 0000 7245  ldr....).rD...rE
+00001ab0: 0000 0072 3c00 0000 723d 0000 005a 0e63  ...r<...r=...Z.c
+00001ac0: 6f6e 7465 7874 5f63 6f6e 6669 675a 1372  ontext_configZ.r
+00001ad0: 6177 5f77 6f72 6b66 6c6f 775f 636f 6e66  aw_workflow_conf
+00001ae0: 6967 5a0c 6c61 6265 6c5f 6f75 7470 7574  igZ.label_output
+00001af0: 5a0f 7365 6c65 6374 6f72 5f6f 7574 7075  Z.selector_outpu
+00001b00: 745a 0c74 7261 696e 5f6f 7574 7075 745a  tZ.train_outputZ
+00001b10: 0e65 7870 6c6f 7265 5f6f 7574 7075 745a  .explore_outputZ
+00001b20: 0d75 7064 6174 655f 6375 7273 6f72 da01  .update_cursor..
+00001b30: 695a 0f77 6f72 6b66 6c6f 775f 636f 6e66  iZ.workflow_conf
+00001b40: 6967 7229 0000 0072 2a00 0000 5a10 6974  igr)...r*...Z.it
+00001b50: 6572 5f70 6174 685f 7072 6566 6978 5a09  er_path_prefixZ.
+00001b60: 6370 5f70 7265 6669 785a 0a63 7032 6b5f  cp_prefixZ.cp2k_
+00001b70: 696e 7075 745a 0c63 7032 6b5f 636f 6e74  inputZ.cp2k_cont
+00001b80: 6578 745a 0a76 6173 705f 696e 7075 745a  extZ.vasp_inputZ
+00001b90: 0c76 6173 705f 636f 6e74 6578 745a 0c64  .vasp_contextZ.d
+00001ba0: 6565 706d 645f 696e 7075 745a 0e64 6565  eepmd_inputZ.dee
+00001bb0: 706d 645f 636f 6e74 6578 7472 4900 0000  pmd_contextrI...
+00001bc0: 5a0c 6c61 6d6d 7073 5f69 6e70 7574 5a0e  Z.lammps_inputZ.
+00001bd0: 6c61 6d6d 7073 5f63 6f6e 7465 7874 5a0a  lammps_contextZ.
+00001be0: 6c61 7370 5f69 6e70 7574 5a0c 6c61 7370  lasp_inputZ.lasp
+00001bf0: 5f63 6f6e 7465 7874 5a0e 7365 6c65 6374  _contextZ.select
+00001c00: 6f72 5f69 6e70 7574 5a10 7365 6c65 6374  or_inputZ.select
+00001c10: 6f72 5f63 6f6e 7465 7874 5a0d 7570 6461  or_contextZ.upda
+00001c20: 7465 5f63 6f6e 6669 6772 1e00 0000 721e  te_configr....r.
+00001c30: 0000 0072 1f00 0000 7243 0000 0072 0000  ...r....rC...r..
+00001c40: 0073 e800 0000 0001 0c01 0c03 0401 0401  .s..............
+00001c50: 0401 0403 0403 1003 0a01 0c01 1201 0603  ................
+00001c60: 0801 0803 1602 0c03 1401 0401 0601 0201  ................
+00001c70: 1201 06fc 0606 0401 0601 0c01 02fd 0605  ................
+00001c80: 2202 1401 0401 0601 0201 1401 06fc 0606  "...............
+00001c90: 0401 0601 0c01 02fd 0605 2203 0803 1c01  ..........".....
+00001ca0: 0a01 0603 0a01 0401 0601 0201 1401 0601  ................
+00001cb0: 06fb 0607 0401 0c01 0601 02fd 0605 2203  ..............".
+00001cc0: 0803 1401 0601 06ff 0603 0401 0601 0201  ................
+00001cd0: 0201 02fc 0606 0401 0c01 0601 02fd 0605  ................
+00001ce0: 2202 1401 0401 0601 0201 0201 06fc 0606  "...............
+00001cf0: 0401 0601 0c01 02fd 0605 2203 0803 0a01  ..........".....
+00001d00: 0401 0601 0601 0401 02fc 0606 0401 0c01  ................
+00001d10: 02fe 0604 2203 0803 0803 0801 0202 1001  ...."...........
+00001d20: 0203 0e01 0601 04ff 0201 08ff 0402 7243  ..............rC
+00001d30: 0000 00da 085f 5f6d 6169 6e5f 5f29 2e5a  .....__main__).Z
+00001d40: 1561 6932 5f6b 6974 2e63 6f72 652e 6578  .ai2_kit.core.ex
+00001d50: 6563 7574 6f72 7202 0000 005a 1561 6932  ecutorr....Z.ai2
+00001d60: 5f6b 6974 2e63 6f72 652e 6172 7469 6661  _kit.core.artifa
+00001d70: 6374 7203 0000 005a 1061 6932 5f6b 6974  ctr....Z.ai2_kit
+00001d80: 2e63 6f72 652e 6c6f 6772 0400 0000 5a11  .core.logr....Z.
+00001d90: 6169 325f 6b69 742e 636f 7265 2e75 7469  ai2_kit.core.uti
+00001da0: 6c72 0500 0000 7206 0000 005a 1d61 6932  lr....r....Z.ai2
+00001db0: 5f6b 6974 2e63 6f72 652e 7265 736f 7572  _kit.core.resour
+00001dc0: 6365 5f6d 616e 6167 6572 7207 0000 00da  ce_managerr.....
+00001dd0: 1761 6932 5f6b 6974 2e63 6f72 652e 6368  .ai2_kit.core.ch
+00001de0: 6563 6b70 6f69 6e74 7208 0000 0072 0900  eckpointr....r..
+00001df0: 0000 5a0e 6169 325f 6b69 742e 646f 6d61  ..Z.ai2_kit.doma
+00001e00: 696e 720a 0000 0072 0b00 0000 720c 0000  inr....r....r...
+00001e10: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00001e20: 7210 0000 0072 1100 0000 7255 0000 0072  r....r....rU...r
+00001e30: 1200 0000 5a08 7079 6461 6e74 6963 7213  ....Z.pydanticr.
+00001e40: 0000 00da 0674 7970 696e 6772 1400 0000  .....typingr....
+00001e50: 7215 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00001e60: 0466 6972 6572 1800 0000 7241 0000 0072  .firer....rA...r
+00001e70: 4d00 0000 724b 0000 0072 5100 0000 721a  M...rK...rQ...r.
+00001e80: 0000 0072 4f00 0000 7219 0000 0072 2800  ...rO...r....r(.
+00001e90: 0000 7238 0000 0072 2d00 0000 7246 0000  ..r8...r-...rF..
+00001ea0: 0072 4300 0000 721e 0000 0072 1e00 0000  .rC...r....r....
+00001eb0: 721e 0000 0072 1f00 0000 da08 3c6d 6f64  r....r......<mod
+00001ec0: 756c 653e 0100 0000 7334 0000 000c 010c  ule>....s4......
+00001ed0: 010c 0110 010c 0110 012c 0c0c 0118 010c  .........,......
+00001ee0: 0208 0108 0108 0108 0208 0310 1410 1f10  ................
+00001ef0: 0702 0104 ff0a 010c ff0c 1914 7f00 1d0a  ................
+00001f00: 02                                       .
```

### Comparing `ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc` & `ai2_kit-0.5.0/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.4.0/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.5.0/ai2_kit/workflow/cll_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,20 +235,21 @@
 
         # select
         if workflow_config.select.model_devi:
             selector_input = selector.CllModelDeviSelectorInput(
                 config=workflow_config.select.model_devi,
                 model_devi_data=explore_output.get_model_devi_dataset(),
                 model_devi_out_filename=const.MODEL_DEVI_OUT,
+                type_map=type_map,
             )
             selector_context = selector.CllModelDevSelectorContext(
-                path_prefix=os.path.join(iter_path_prefix, 'selector-threshold'),
+                path_prefix=os.path.join(iter_path_prefix, 'selector-model-devi'),
                 resource_manager=resource_manager,
             )
-            selector_output = await apply_checkpoint(f'{cp_prefix}/selector-threshold')(selector.cll_model_devi_selector)(selector_input, selector_context)
+            selector_output = await apply_checkpoint(f'{cp_prefix}/selector-model-devi')(selector.cll_model_devi_selector)(selector_input, selector_context)
 
         else:
             raise ValueError('No select method is specified')
 
         # Update
         update_config = workflow_config.update.walkthrough
```

### Comparing `ai2_kit-0.4.0/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.5.0/ai2_kit/workflow/fep_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,25 +203,27 @@
         explore_output = await apply_checkpoint(f'{cp_prefix}/lammps')(lammps.cll_lammps)(lammps_input, lammps_context)
 
         # select
         red_selector_input = selector.CllModelDeviSelectorInput(
             config=workflow_config.red.threshold,
             model_devi_data=explore_output.get_model_devi_dataset(),
             model_devi_out_filename=const.MODEL_DEVI_RED_OUT,
+            type_map=type_map,
         )
         red_selector_context = selector.CllModelDevSelectorContext(
             path_prefix=os.path.join(
                 iter_path_prefix, 'red-selector-threshold'),
             resource_manager=resource_manager,
         )
 
         neu_selector_input = selector.CllModelDeviSelectorInput(
             config=workflow_config.neu.threshold,
             model_devi_data=explore_output.get_model_devi_dataset(),
             model_devi_out_filename=const.MODEL_DEVI_NEU_OUT,
+            type_map=type_map,
         )
         neu_selector_context = selector.CllModelDevSelectorContext(
             path_prefix=os.path.join(iter_path_prefix, 'neu-selector-threshold'),
             resource_manager=resource_manager,
         )
 
         red_selector_output, neu_selector_output = await asyncio.gather(
```

### Comparing `ai2_kit-0.4.0/pyproject.toml` & `ai2_kit-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.4.0/PKG-INFO` & `ai2_kit-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -64,15 +64,15 @@
 ```
 Note that instead of running global `ai2-kit` command, you should run `./ai2-kit` to run the command from source.
 
 ## Manuals
 
 ### Domain Specific Tools
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
-* [CLL MLP Training Workflow](doc/manual/cll-workflow.md)
+* CLL MLP Training Workflow: [English](doc/manual/cll-workflow.md), [中文](doc/manual/cll-workflow.zh.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ### Build-in Functionalities
 * [Checkpoint Mechanism](doc/manual/checkpoint.md)
 * [ASE Toolkit](doc/manual/ase.md)
 * [Tips](doc/manual/tips.md)
```

