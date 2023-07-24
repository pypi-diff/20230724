# Comparing `tmp/phylox-0.0.2.tar.gz` & `tmp/phylox-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylox-0.0.2.tar", last modified: Mon Jun 19 07:03:35 2023, max compression
+gzip compressed data, was "phylox-0.0.5.tar", last modified: Mon Jul 24 07:00:24 2023, max compression
```

## Comparing `phylox-0.0.2.tar` & `phylox-0.0.5.tar`

### file list

```diff
@@ -1,74 +1,82 @@
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/
--rw-rw-r--   0 remie     (1000) remie     (1000)     1069 2023-06-06 08:24:00.000000 phylox-0.0.2/LICENSE
--rw-rw-r--   0 remie     (1000) remie     (1000)     1243 2023-06-19 07:03:35.717074 phylox-0.0.2/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)      673 2023-06-19 07:03:23.000000 phylox-0.0.2/README.md
--rw-rw-r--   0 remie     (1000) remie     (1000)      809 2023-06-19 06:53:37.000000 phylox-0.0.2/pyproject.toml
--rw-rw-r--   0 remie     (1000) remie     (1000)       38 2023-06-19 07:03:35.717074 phylox-0.0.2/setup.cfg
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.709074 phylox-0.0.2/src/
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/
--rw-rw-r--   0 remie     (1000) remie     (1000)       57 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      469 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/cherrypicking/
--rw-rw-r--   0 remie     (1000) remie     (1000)    65903 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/CPH.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    10138 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     5145 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/NetworkContainment.py
--rw-rw-r--   0 remie     (1000) remie     (1000)       20 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     1903 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/classes/
--rw-rw-r--   0 remie     (1000) remie     (1000)      143 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/classes/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3226 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/classes/dinetwork.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      160 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/classes/networkclass.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3245 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/dinetwork.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/exceptions/
--rw-rw-r--   0 remie     (1000) remie     (1000)      130 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/exceptions/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      187 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/exceptions/invalidmovedefinitionexception.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      180 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/exceptions/invalidmoveexception.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/
--rw-rw-r--   0 remie     (1000) remie     (1000)       49 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/generators/__init__.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/betasplitting/
--rw-rw-r--   0 remie     (1000) remie     (1000)     4821 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingModelTree.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3278 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingNetwork_Main.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     6926 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingNetwork_Tools.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3416 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/MakeCatAndBalancedWithEdges.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3300 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/MakeNetworksBeta.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/heath/
--rw-rw-r--   0 remie     (1000) remie     (1000)    32262 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/heath/heath.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/lgt/
--rw-rw-r--   0 remie     (1000) remie     (1000)    13796 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/lgt/Generator.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/mcmc/
--rw-rw-r--   0 remie     (1000) remie     (1000)       20 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/mcmc/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     4562 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/mcmc/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/generators/randomTC/
--rw-rw-r--   0 remie     (1000) remie     (1000)    11203 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/randomTC/RandomNetworks.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/generators/zods/
--rw-rw-r--   0 remie     (1000) remie     (1000)     4739 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/zods/zods.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/isomorphism/
--rw-rw-r--   0 remie     (1000) remie     (1000)       53 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/isomorphism/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     4640 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/isomorphism/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/networkproperties/
--rw-rw-r--   0 remie     (1000) remie     (1000)     3283 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/networkproperties/properties.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     7804 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/parser.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/rearrangement/
--rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/__init__.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/rearrangement/exact_distance/
--rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/exact_distance/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     5317 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/exact_distance/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/rearrangement/heuristics/
--rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     7496 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/cli_main.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    26629 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/green_line_heuristic.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    12283 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/heuristic_tools.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    27078 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/red_line_heuristic.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     2431 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/invertsequence.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     4777 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/movability.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     8793 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/move.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      193 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/movetype.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      669 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/rearrangementproblem.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox.egg-info/
--rw-rw-r--   0 remie     (1000) remie     (1000)     1243 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)     2051 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/SOURCES.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)        1 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/dependency_links.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)       28 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/requires.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)        7 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/top_level.txt
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/tests/
--rw-rw-r--   0 remie     (1000) remie     (1000)     3530 2023-06-19 06:53:37.000000 phylox-0.0.2/tests/test_dinetwork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.606456 phylox-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 07:00:15.000000 phylox-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-24 07:00:24.606456 phylox-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-24 07:00:15.000000 phylox-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 07:00:15.000000 phylox-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:00:24.606456 phylox-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.598456 phylox-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.598456 phylox-0.0.5/src/phylox/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/cherrypicking/
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/cherrypicking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/cherrypicking/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/cherrypicking/best_subnetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27256 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/cherrypicking/combining_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/cherrypicking/tree_child_sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/classes/dinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/classes/networkclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/dinetwork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/exceptions/invalidmovedefinitionexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/exceptions/invalidmoveexception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/generators/heath/
+-rw-r--r--   0 runner    (1001) docker     (123)    24298 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/heath/heath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/heath/heath_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/generators/lgt/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/lgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/lgt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/generators/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/mcmc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/generators/randomTC/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/randomTC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/randomTC/random_tc_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/generators/trees/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/trees/add_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/trees/beta_splitting_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/trees/well_known.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/generators/zods/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/zods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/zods/zods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/generators/zods/zods_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/isomorphism/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/isomorphism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/isomorphism/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.602456 phylox-0.0.5/src/phylox/networkproperties/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/networkproperties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/networkproperties/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.606456 phylox-0.0.5/src/phylox/rearrangement/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.606456 phylox-0.0.5/src/phylox/rearrangement/exact_distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/exact_distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/exact_distance/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.606456 phylox-0.0.5/src/phylox/rearrangement/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/heuristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/heuristics/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26629 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/heuristics/green_line_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/heuristics/heuristic_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27078 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/heuristics/red_line_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/invertsequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/movability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/movetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-24 07:00:15.000000 phylox-0.0.5/src/phylox/rearrangement/rearrangementproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.598456 phylox-0.0.5/src/phylox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-24 07:00:24.000000 phylox-0.0.5/src/phylox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-24 07:00:24.000000 phylox-0.0.5/src/phylox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:00:24.000000 phylox-0.0.5/src/phylox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 07:00:24.000000 phylox-0.0.5/src/phylox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 07:00:24.000000 phylox-0.0.5/src/phylox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 07:00:24.000000 phylox-0.0.5/src/phylox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:00:24.606456 phylox-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-24 07:00:15.000000 phylox-0.0.5/tests/test_dinetwork.py
```

### Comparing `phylox-0.0.2/LICENSE` & `phylox-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/pyproject.toml` & `phylox-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phylox"
-version = "0.0.2"
+version = "0.0.5"
 authors = [
   { name="Remie Janssen", email="remiejanssen92@gmail.com" },
 ]
 description = "A package with tools for constructing, manipulating, and analyzing phylogenetic networks."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "networkx>=2.6",
-  "numpy>=1.21.6"
+  "numpy>=1.21.6",
+  "scipy>=1.7.3",
+  "matplotlib>=3.5",
 ]
 
 [tool.pytest.ini_options]
 pythonpath = [
   ".", "src",
 ]
-addopts = "--cov --cov-report term-missing"
+addopts = "--cov --cov-report term-missing --doctest-modules"
 
 [project.urls]
 "Homepage" = "https://github.com/RemieJanssen/PhyloX"
 "Bug Tracker" = "https://github.com/RemieJanssen/PhyloX/issues"
+
+[project.scripts]
+phylox-generator-heath = "phylox.generators.heath.heath_cli:main"
```

### Comparing `phylox-0.0.2/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py` & `phylox-0.0.5/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingNetwork_Tools.py` & `phylox-0.0.5/src/phylox/generators/trees/add_edges.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,181 +1,177 @@
-# ############################################
-# #
-# # Adapted from BetasplittingModel.py
-# # which contains the code for Beta-splitting model (Aldous1996)
-# # Written for python3
-# #
-# ############################################
-
-# import os
-# import sys
-# import math
-# import random
-# import numpy as np
-# import networkx as nx
-# from scipy.special import gamma, loggamma
-
-
-# ############################################
-# # Simulation functions
-# ############################################
-
-# # a_n is a normalizing constant defined in
-# # Equation (2) of Aldous1996 (so the sum of
-# # the values is equal to 1. It is not
-# # computed here to save time.
-# def a_n(beta):
-#     return 1
-
-# # Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
-# def computeProb(n,beta):
-#     q_n = []
-#     for i in range(1,n):
-#         q_i_n = np.exp((loggamma(beta+i+1)+loggamma(beta+n-i+1))-((a_n(beta)+loggamma(i+1)+loggamma(n-i+1))))
-#         q_n.append(q_i_n)
-#     return q_n
-
-# # n: number of tips
-# def simulateBetaSplitting(n, beta):
-#     # Initialize tree.
-#     tree = nx.DiGraph()
-#     tree.add_node(n+1)
-#     tree.node[n+1]['label'] = n
-#     last_internal_node       = n+1
-#     last_leaf_node           = 0
-#     queue                    = [n+1]
-#     # Insert one node at each iteration.
-#     while queue:
-#         node        = queue.pop()
-#         n_node      = tree.node[node].get('label')
-#         # Internal node. Splits again.
-#         if (n_node > 1):
-#             # Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
-#             q_n   = computeProb(n_node,beta)
-#             split = random.choices(population=list(range(1,n_node)), weights=q_n, k=1)[0]
-#             # Create children.
-#             for new_n in [split,n_node-split]:
-#                 if new_n == 1:
-#                     tree.add_edge(node,last_leaf_node+1)
-#                     last_leaf_node+=1
-#                 else:
-#                     tree.add_edge(node,last_internal_node+1)
-#                     tree.node[last_internal_node+1]['label']=new_n
-#                     queue.append(last_internal_node+1)
-#                     last_internal_node+=1
-#     # Return tree.
-#     return tree
-
-
-# def GenerateNetwork(tree,r,method):
-#     network = tree.copy()
-#     if method=="Horizontal":
-#         leaves = [x for x in tree.nodes() if tree.out_degree(x)==0]
-#     for i in range(r):
-#         if method==None:
-#             AddEdgeUniform(network)
-#         elif method=="Horizontal":
-#             AddEdgeHorizontal(network,leaves=leaves)
-#         else:
-#             AddEdgeLocal(network,stop_prob=method)
-#     return network
-
-
-# def AddEdgeBetween(network,edge1,edge2,new_nodes=None):
-#     #if we dont have new nodes yet, determine new nodes
-#     if new_nodes==None:
-#         max_node = max(network.nodes())
-#         new_nodes = (max_node+1,max_node+2)
-#     #make sure edge2 is not above edge1
-#     if nx.has_path(network,edge2[1],edge1[0]):
-#         edge1,edge2=edge2,edge1
-#     length1 = network[edge1[0]][edge1[1]].get('length')
-#     prob1 = network[edge1[0]][edge1[1]].get('prob')
-#     length2 = network[edge2[0]][edge2[1]].get('length')
-#     prob2 = network[edge2[0]][edge2[1]].get('prob')
-#     #add an edge from edge1 to edge2
-#     network.remove_edges_from([edge1,edge2])
-#     network.add_edges_from([(edge1[0],new_nodes[0]),(new_nodes[0],edge1[1]),(edge2[0],new_nodes[1]),(new_nodes[1],edge2[1]),(new_nodes[0],new_nodes[1])])
-
-#     #If the original network had lengths and probabilities, add these to the subdivided arcs as well.
-#     if length1!=None:
-#         l11 = random.random()*length1
-#         l12 = length1-l11
-#         network[edge1[0]][new_nodes[0]]['length']=l11
-#         network[new_nodes[0]][edge1[1]]['length']=l12
-#     if prob1!=None:
-#         network[new_nodes[0]][edge1[1]]['prob']=prob1
-#     if length2!=None:
-#         l21 = random.random()*length2
-#         l22 = length2-l21
-#         network[edge2[0]][new_nodes[1]]['length']=l21
-#         network[new_nodes[1]][edge2[1]]['length']=l22
-#     if prob2!=None:
-#         network[new_nodes[1]][edge2[1]]['prob']=prob2
-#     #TODO: add probabilities and length to the other new arcs as well?
-
-
-# #Pick two edges uniformly at random and add an edge between these
-# def AddEdgeHorizontal(network,leaves = None,new_nodes=None):
-#     if leaves==None:
-#         leaves = [x for x in network.nodes() if network.out_degree(x)==0]
-#     leaf_indices = np.random.choice(range(len(leaves)),2,replace=False)
-#     l0 = leaves[leaf_indices[0]]
-#     l1 = leaves[leaf_indices[1]]
-#     e0 = list(network.in_edges(l0))[0]
-#     e1 = list(network.in_edges(l1))[0]
-#     AddEdgeBetween(network,e0,e1,new_nodes=new_nodes)
-
-
-# #Pick two edges uniformly at random and add an edge between these
-# def AddEdgeUniform(network,new_nodes=None):
-#     edges = list(network.edges())
-#     edge_indices = np.random.choice(range(len(edges)),2,replace=False)
-#     AddEdgeBetween(network,edges[edge_indices[0]],edges[edge_indices[1]],new_nodes=new_nodes)
-
-
-# #Pick one edge, move a random number of edges through the network to find a second edge
-# #Add and edge between the two edges.
-# def AddEdgeLocal(network,new_nodes=None,stop_prob=0.2,max_steps=None,max_tries=None):
-#     try_number = 1
-#     while max_tries==None or try_number<=max_tries:
-#         #Pick a random edge
-#         edge1 = random.choice(list(network.edges()))
-#         edge2 = None
-#         #Initiate the random walk, by choosing an orientation
-#         previous_node = random.choice(edge1)
-#         current_node  = edge1[0]
-#         if current_node == previous_node:
-#             current_node = edge1[1]
-#         #Take a number of steps
-#         step_number =1
-#         while max_steps==None or step_number<=max_steps:
-#             previous_node,current_node = current_node,random.choice(list(network.successors(current_node))+list(network.predecessors(current_node)))
-#             if random.random()<stop_prob:
-#                 break
-#             step_number+=1
-#         #Set the new edge
-#         edge2 = (previous_node,current_node)
-#         if edge2 not in network.edges():
-#             edge2 = (current_node,previous_node)
-#         #Add an edge if possible, otherwise repeat the search
-#         if edge1!=edge2:
-#             break
-#         try_number+=1
-#     AddEdgeBetween(network,edge1,edge2,new_nodes=new_nodes)
-
-
-# def OutputNetwork(network,out_type):
-#     output = ""
-#     if out_type=="el":
-#         for i,e in enumerate(network.edges):
-#             if i!=0:
-#                 output+="\r\n"
-#             output += str(e[0])+" "+str(e[1])
-#     elif out_type=="pl":
-#         for i,v in enumerate(network.nodes):
-#             if i!=0:
-#                 output+="\r\n"
-#             output += str(v)
-#             for p in network.predecessors(v):
-#                 output+=" "+str(p)
-#     return output
+import random
+from enum import Enum
+
+import numpy as np
+
+from phylox.rearrangement.move import Move, apply_move
+from phylox.rearrangement.movetype import MoveType
+
+
+# Pick two edges uniformly at random and add an edge between these
+def random_vplu_move_at_bottom(network):
+    """
+    Returns a VPLU move that adds an edge between the incoming edges of two leaves.
+
+    :param network: the network to add an edge to.
+    :return: a VPLU move that adds an edge between the incoming edges of two leaves.
+
+    :example:
+    >>> from phylox import DiNetwork
+    >>> from phylox.rearrangement.movetype import MoveType
+    >>> from phylox.generators.trees.well_known import generate_balanced_tree
+    >>> from phylox.generators.trees.add_edges import random_vplu_move_at_bottom
+    >>> tree = generate_balanced_tree(8)
+    >>> move = random_vplu_move_at_bottom(tree)
+    >>> move.is_type(MoveType.VPLU)
+    True
+    """
+    leaves = list(network.leaves)
+    leaf_indices = np.random.choice(range(len(leaves)), 2, replace=False)
+    leaf1 = leaves[leaf_indices[0]]
+    parent1 = network.parent(leaf1)
+    leaf2 = leaves[leaf_indices[1]]
+    parent2 = network.parent(leaf2)
+    return Move(
+        move_type=MoveType.VPLU,
+        network=network,
+        start_edge=(parent1, leaf1),
+        end_edge=(parent2, leaf2),
+    )
+
+
+# Pick two edges uniformly at random and add an edge between these
+def random_vplu_move_uniform(network):
+    """
+    Returns a VPLU move that adds an edge between two edges in the network.
+    Two edges are chosen uniformly at random from the network.
+
+    :param network: the network to add an edge to.
+    :return: a VPLU move that adds an edge between two edges in the network.
+
+    :example:
+    >>> from phylox import DiNetwork
+    >>> from phylox.rearrangement.movetype import MoveType
+    >>> from phylox.generators.trees.well_known import generate_balanced_tree
+    >>> from phylox.generators.trees.add_edges import random_vplu_move_uniform
+    >>> tree = generate_balanced_tree(8)
+    >>> move = random_vplu_move_uniform(tree)
+    >>> move.is_type(MoveType.VPLU)
+    True
+    """
+    edges = list(network.edges())
+    edge_indices = np.random.choice(range(len(edges)), 2, replace=False)
+    return Move(
+        move_type=MoveType.VPLU,
+        network=network,
+        start_edge=edges[edge_indices[0]],
+        end_edge=edges[edge_indices[1]],
+    )
+
+
+def random_vplu_move_local(network, stop_prob=0.2, max_steps=None, max_tries=None):
+    """
+    Returns a VPLU move that adds an edge between two edges in the network.
+    Pick one edge, move a random number of edges through the network to find a second edge.
+
+    :param network: the network to add an edge to.
+    :param stop_prob: the probability to stop the random walk.
+    :param max_steps: the maximum number of steps to take in the random walk.
+    :param max_tries: the maximum number of tries to find a second edge.
+    :return: a VPLU move that adds an edge between two edges in the network.
+
+    :example:
+    >>> from phylox import DiNetwork
+    >>> from phylox.rearrangement.movetype import MoveType
+    >>> from phylox.generators.trees.well_known import generate_balanced_tree
+    >>> from phylox.generators.trees.add_edges import random_vplu_move_local
+    >>> tree = generate_balanced_tree(8)
+    >>> move = random_vplu_move_local(tree)
+    >>> move.is_type(MoveType.VPLU)
+    True
+    """
+    try_number = 1
+    while max_tries == None or try_number <= max_tries:
+        # Pick a random edge
+        edge1 = random.choice(list(network.edges()))
+        edge2 = None
+        # Initiate the random walk, by choosing an orientation
+        previous_node = random.choice(edge1)
+        current_node = edge1[0]
+        if current_node == previous_node:
+            current_node = edge1[1]
+        # Take a number of steps
+        step_number = 1
+        while max_steps == None or step_number <= max_steps:
+            previous_node, current_node = current_node, random.choice(
+                list(network.successors(current_node))
+                + list(network.predecessors(current_node))
+            )
+            if random.random() < stop_prob:
+                break
+            step_number += 1
+        # Set the new edge
+        edge2 = (previous_node, current_node)
+        if edge2 not in network.edges():
+            edge2 = (current_node, previous_node)
+        # Add an edge if possible, otherwise repeat the search
+        if edge1 != edge2:
+            break
+        try_number += 1
+    return Move(
+        move_type=MoveType.VPLU,
+        network=network,
+        start_edge=edge1,
+        end_edge=edge2,
+    )
+
+
+class AddEdgeMethod(Enum):
+    UNIFORM = 1
+    BOTTOM = 2
+    LOCAL = 3
+
+
+def network_from_tree(tree, reticulations, method):
+    """
+    Returns a network with the given number of reticulations added to the given tree.
+
+    :param tree: a phylogenetic network, i.e., a DAG with leaf labels stored as the node attribute LABEL_ATTR.
+    :param reticulations: the number of reticulations to add to the tree.
+    :param method: the method to use to add the reticulations.
+    :return: a network with the given number of reticulations added to the given tree.
+
+    :example:
+    >>> from phylox import DiNetwork
+    >>> from phylox.rearrangement.movetype import MoveType
+    >>> from phylox.generators.trees.well_known import generate_balanced_tree
+    >>> from phylox.generators.trees.add_edges import network_from_tree, AddEdgeMethod
+    >>> tree = generate_balanced_tree(8)
+    >>> network = network_from_tree(tree, 2, AddEdgeMethod.BOTTOM)
+    >>> len(network.leaves)
+    8
+    >>> network.reticulation_number
+    2
+    """
+
+    if method == AddEdgeMethod.BOTTOM:
+        leaves = tree.leaves
+
+    if method == AddEdgeMethod.UNIFORM:
+        add_edge_method = random_vplu_move_uniform
+    elif method == AddEdgeMethod.BOTTOM:
+        add_edge_method = random_vplu_move_at_bottom
+    elif method == AddEdgeMethod.LOCAL:
+        add_edge_method = random_vplu_move_local
+    else:
+        raise ValueError(f"Method {method} not implemented, use one of {AddEdgeMethod}")
+
+    network = tree.copy()
+    reticulations = int(reticulations)
+    while reticulations > 0:
+        try:
+            move = add_edge_method(network)
+            network = apply_move(network, move)
+            reticulations -= 1
+        except:
+            pass
+    return network
```

### Comparing `phylox-0.0.2/src/phylox/generators/zods/zods.py` & `phylox-0.0.5/src/phylox/generators/zods/zods_cli.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/src/phylox/rearrangement/exact_distance/base.py` & `phylox-0.0.5/src/phylox/rearrangement/exact_distance/base.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/src/phylox/rearrangement/heuristics/cli_main.py` & `phylox-0.0.5/src/phylox/rearrangement/heuristics/cli_main.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/src/phylox/rearrangement/heuristics/green_line_heuristic.py` & `phylox-0.0.5/src/phylox/rearrangement/heuristics/green_line_heuristic.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/src/phylox/rearrangement/heuristics/heuristic_tools.py` & `phylox-0.0.5/src/phylox/rearrangement/heuristics/heuristic_tools.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/src/phylox/rearrangement/heuristics/red_line_heuristic.py` & `phylox-0.0.5/src/phylox/rearrangement/heuristics/red_line_heuristic.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.2/src/phylox/rearrangement/invertsequence.py` & `phylox-0.0.5/src/phylox/rearrangement/invertsequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,23 @@
     """
     Finds the original location (from-edge) of the moving_endpoint of an edge if it is moved.
 
     :param network: a phylogenetic network.
     :param moving_edge: an edge of the network.
     :param moving_endpoint: a node of the network, which must be an endpoint of the edge.
     :return: a pair of nodes (p,c) where p and c are a parent and child of the moving_endpoint such that they are both not part of the moving_edge.
+
+    :example:
+    >>> from phylox import DiNetwork
+    >>> from phylox.rearrangement.invertsequence import from_edge
+    >>> network = DiNetwork(
+    ...     edges=[(0,1),(1,2),(1,3)],
+    ... )
+    >>> from_edge(network, (1,2), 1)
+    (0, 3)
     """
     other_parent = network.parent(moving_endpoint, exclude=moving_edge)
     other_child = network.child(moving_endpoint, exclude=moving_edge)
     return (other_parent, other_child)
 
 
 # def InvertMoveSequence(seq):
```

### Comparing `phylox-0.0.2/src/phylox/rearrangement/movability.py` & `phylox-0.0.5/src/phylox/rearrangement/movability.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,32 @@
 from phylox.rearrangement.movetype import MoveType
 
 
 def check_valid(network, move):
     """
     Checks whether a move is valid.
 
-    :param move: a move of type Move
+    :param move: a rearrangement move (see phylox.rearrangement.movetype.Move)
     :return: void
+    :exception: InvalidMoveException if the move is not valid
+
+    :example:
+    >>> from phylox import DiNetwork
+    >>> from phylox.rearrangement.move import Move
+    >>> from phylox.rearrangement.movability import check_valid
+    >>> network = DiNetwork(
+    ...     edges=[(0,1),(1,2),(1,3),(2,3),(2,4),(3,5)],
+    ... )
+    >>> move = Move(
+    ...     move_type=MoveType.HEAD,
+    ...     origin=(2, 5),
+    ...     moving_edge=(1, 3),
+    ...     target=(2, 4),
+    ... )
+    >>> check_valid(network, move)
     """
     if move.move_type == MoveType.NONE:
         return
     if move.is_type(MoveType.RSPR):
         if not network.has_edge(
             move.origin[0], move.moving_node
         ) or not network.has_edge(move.moving_node, move.origin[1]):
@@ -81,14 +97,27 @@
     """
     Checks whether an endpoint of an edge is movable in a network.
 
     :param network: a phylogenetic network, i.e., a DAG with labeled leaves.
     :param moving_edge: an edge in the network.
     :param moving_endpoint: a node, specifically, an endpoint of the moving_edge.
     :return: True if the endpoint of the edge is movable in the network, False otherwise.
+
+    :example:
+    >>> from phylox import DiNetwork
+    >>> from phylox.rearrangement.movability import check_movable
+    >>> network = DiNetwork(
+    ...     edges=[(0,1),(1,2),(1,3),(2,3),(2,4),(3,5)],
+    ... )
+    >>> check_movable(network, (1, 3), 3)
+    True
+    >>> check_movable(network, (1, 3), 1)
+    True
+    >>> check_movable(network, (3, 5), 3)
+    False
     """
     if moving_endpoint == moving_edge[0]:
         # Tail move
         if network.in_degree(moving_endpoint) in (0, 2):
             # cannot move the tail if it is a reticulation or root
             return False
     elif moving_endpoint == moving_edge[1]:
```

### Comparing `phylox-0.0.2/src/phylox.egg-info/SOURCES.txt` & `phylox-0.0.5/src/phylox.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 LICENSE
 README.md
 pyproject.toml
 src/phylox/__init__.py
 src/phylox/base.py
+src/phylox/constants.py
 src/phylox/dinetwork.py
 src/phylox/parser.py
 src/phylox.egg-info/PKG-INFO
 src/phylox.egg-info/SOURCES.txt
 src/phylox.egg-info/dependency_links.txt
+src/phylox.egg-info/entry_points.txt
 src/phylox.egg-info/requires.txt
 src/phylox.egg-info/top_level.txt
-src/phylox/cherrypicking/CPH.py
 src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
-src/phylox/cherrypicking/NetworkContainment.py
 src/phylox/cherrypicking/__init__.py
 src/phylox/cherrypicking/base.py
+src/phylox/cherrypicking/best_subnetwork.py
+src/phylox/cherrypicking/combining_networks.py
+src/phylox/cherrypicking/tree_child_sequences.py
 src/phylox/classes/__init__.py
 src/phylox/classes/dinetwork.py
 src/phylox/classes/networkclass.py
 src/phylox/exceptions/__init__.py
 src/phylox/exceptions/invalidmovedefinitionexception.py
 src/phylox/exceptions/invalidmoveexception.py
 src/phylox/generators/__init__.py
-src/phylox/generators/betasplitting/BetaSplittingModelTree.py
-src/phylox/generators/betasplitting/BetaSplittingNetwork_Main.py
-src/phylox/generators/betasplitting/BetaSplittingNetwork_Tools.py
-src/phylox/generators/betasplitting/MakeCatAndBalancedWithEdges.py
-src/phylox/generators/betasplitting/MakeNetworksBeta.py
 src/phylox/generators/heath/heath.py
-src/phylox/generators/lgt/Generator.py
+src/phylox/generators/heath/heath_cli.py
+src/phylox/generators/lgt/__init__.py
+src/phylox/generators/lgt/base.py
 src/phylox/generators/mcmc/__init__.py
 src/phylox/generators/mcmc/base.py
-src/phylox/generators/randomTC/RandomNetworks.py
+src/phylox/generators/randomTC/__init__.py
+src/phylox/generators/randomTC/random_tc_network.py
+src/phylox/generators/trees/__init__.py
+src/phylox/generators/trees/add_edges.py
+src/phylox/generators/trees/beta_splitting_tree.py
+src/phylox/generators/trees/well_known.py
+src/phylox/generators/zods/__init__.py
 src/phylox/generators/zods/zods.py
+src/phylox/generators/zods/zods_cli.py
 src/phylox/isomorphism/__init__.py
 src/phylox/isomorphism/base.py
+src/phylox/networkproperties/__init__.py
 src/phylox/networkproperties/properties.py
 src/phylox/rearrangement/__init__.py
 src/phylox/rearrangement/invertsequence.py
 src/phylox/rearrangement/movability.py
 src/phylox/rearrangement/move.py
 src/phylox/rearrangement/movetype.py
 src/phylox/rearrangement/rearrangementproblem.py
```

### Comparing `phylox-0.0.2/tests/test_dinetwork.py` & `phylox-0.0.5/tests/test_dinetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
-from phylox import LABEL_ATTR, DiNetwork
+from phylox import DiNetwork
+from phylox.constants import LABEL_ATTR
 
 
 class TestDiNetwork(unittest.TestCase):
     def test_init(self):
         network = DiNetwork()
         self.assertEqual(list(network.edges), [])
         self.assertEqual(list(network.nodes), [])
```

