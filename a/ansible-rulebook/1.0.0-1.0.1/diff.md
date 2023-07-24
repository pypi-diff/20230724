# Comparing `tmp/ansible_rulebook-1.0.0.tar.gz` & `tmp/ansible_rulebook-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_rulebook-1.0.0.tar", last modified: Thu Jun 15 17:08:23 2023, max compression
+gzip compressed data, was "ansible_rulebook-1.0.1.tar", last modified: Mon Jul 24 18:07:57 2023, max compression
```

## Comparing `ansible_rulebook-1.0.0.tar` & `ansible_rulebook-1.0.1.tar`

### file list

```diff
@@ -1,402 +1,417 @@
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.819764 ansible_rulebook-1.0.0/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    11358 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/LICENSE
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      312 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/MANIFEST.in
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4111 2023-06-15 17:08:23.819847 ansible_rulebook-1.0.0/PKG-INFO
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3353 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/README.rst
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.772208 ansible_rulebook-1.0.0/ansible_rulebook/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      671 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/__init__.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      634 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/__main__.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     8413 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/app.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    26665 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/builtin.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     7948 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/cli.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4671 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/collection.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1075 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/common.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     8165 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/condition_parser.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2659 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/condition_types.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      796 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/conf.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     9754 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/engine.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.773332 ansible_rulebook-1.0.0/ansible_rulebook/event_filter/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/event_filter/__init__.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1346 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/event_filter/insert_meta_info.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2228 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/exception.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     6285 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/job_template_runner.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    11925 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/json_generator.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      827 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/messages.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3173 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rule_generator.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    17737 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rule_set_runner.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2418 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rule_types.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     6558 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/rules_parser.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.773465 ansible_rulebook-1.0.0/ansible_rulebook/schema/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    20517 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/schema/ruleset_schema.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     7223 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/util.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1428 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/validators.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4908 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/ansible_rulebook/websocket.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.773098 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4111 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/PKG-INFO
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    12566 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/SOURCES.txt
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        1 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/dependency_links.txt
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       63 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/entry_points.txt
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        1 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/not-zip-safe
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      104 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/requires.txt
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       17 2023-06-15 17:08:23.000000 ansible_rulebook-1.0.0/ansible_rulebook.egg-info/top_level.txt
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.776357 ansible_rulebook-1.0.0/docs/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      617 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/Makefile
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    11365 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/actions.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2647 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/collections.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    33663 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/conditions.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     5955 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/conf.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2033 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/contributing.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4272 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/decision_environment.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3560 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/development_environment.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2033 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/events_and_facts.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2700 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/filters.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     7006 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/getting_started.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      625 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/host_limit.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      495 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/index.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2437 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/installation.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     5447 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/introduction.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      778 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/make.bat
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2278 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/multi_events.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4137 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/rulebooks.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2397 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/rules.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       41 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/runner.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     5714 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/sources.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4380 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/usage.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4865 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/docs/variables.rst
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      277 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/pyproject.toml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1487 2023-06-15 17:08:23.820286 ansible_rulebook-1.0.0/setup.cfg
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.778280 ansible_rulebook-1.0.0/tests/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      634 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/__init__.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.785858 ansible_rulebook-1.0.0/tests/asts/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      516 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/01_noop.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      510 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/02_debug.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/03_print_event.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      888 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/04_set_fact.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      890 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/05_post_event.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1183 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/06_retract_fact.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      772 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/07_and.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      770 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/08_or.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/09_gt.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      516 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/10_lt.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      537 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/11_le.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      543 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/12_ge.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      662 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/13_add.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      670 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/14_sub.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      683 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/15_multiple_events_all.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      683 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/16_multiple_events_any.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      783 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/17_multiple_sources_any.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      787 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/18_multiple_sources_all.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1076 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/19_is_defined.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1100 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/20_is_not_defined.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      561 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/21_run_playbook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      565 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/23_nested_data.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      563 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/24_max_attributes.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      604 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/25_max_attributes_nested.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      643 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/26_print_events.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1066 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/27_var_root.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      769 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/28_right_side_condition_template.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      621 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/29_run_module.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      619 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/30_run_module_missing.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      626 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/31_run_module_missing_args.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      641 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/32_run_module_fail.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      649 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/33_run_playbook_retry.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      625 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/34_run_playbook_retries.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1521 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1537 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1090 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/37_hosts_facts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      534 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/38_shutdown.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2990 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      694 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_assignment.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      693 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_assignment2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      924 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      925 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1441 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions3.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1605 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_time.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2385 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_timestamp.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      916 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_with_vars.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      580 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/rules_without_assignment.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1638 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_filters.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1963 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_host_rules.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1955 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2022 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      530 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      530 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts3.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1338 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_set_facts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1552 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/asts/test_simple.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.786147 ansible_rulebook-1.0.0/tests/cassettes/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    28619 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/cassettes/test_job_template.yaml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    10489 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/cassettes/test_job_template_not_exist.yaml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2754 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/conftest.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.786819 ansible_rulebook-1.0.0/tests/data/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       37 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/bad_source.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      137 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/not_asyncio.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      727 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/rulebook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    47616 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/test.tar
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       68 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/data/test_vars.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.788152 ansible_rulebook-1.0.0/tests/e2e/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      878 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/README.md
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/__init__.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.788291 ansible_rulebook-1.0.0/tests/e2e/config/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      246 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/config/default.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      564 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/conftest.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.766501 ansible_rulebook-1.0.0/tests/e2e/files/
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.788913 ansible_rulebook-1.0.0/tests/e2e/files/extra_vars/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      826 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/extra_vars/operator_variables.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      162 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/extra_vars/test_variables_extra_vars.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.789258 ansible_rulebook-1.0.0/tests/e2e/files/inventories/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       35 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/inventories/default_inventory.ini
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       61 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/inventories/default_inventory.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.790032 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      404 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/long_running.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      344 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/print_event.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      240 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/print_rule_name.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/playbooks/run_playbook_test_playbook.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.790783 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.791409 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4727 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2451 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_run_playbook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1611 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1050 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      288 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/hello_events_with_var.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      253 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/malformed_rulebook.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.792607 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     6274 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_logical_operators.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     6060 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_membership_operators.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     6216 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_relational_operators.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3476 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_select_operator.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     7702 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2545 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_match.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2583 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2623 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_search_search.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1394 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_disabled_rules.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      270 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_process_sigint.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      955 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_process_source_end.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.792760 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/variables/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2070 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.792922 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/websockets/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      283 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/websockets/test_websocket_range.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      522 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/settings.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    10871 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_actions.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    20067 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_operators.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     5843 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_runtime.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2271 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_variables.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3595 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/test_websocket.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.766978 ansible_rulebook-1.0.0/tests/e2e/utils/
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.793811 ansible_rulebook-1.0.0/tests/e2e/utils/awx/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      164 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/ansible.cfg
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      602 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/create-cluster.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      637 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/install-awx.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      437 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/kind-config.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      855 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/readme.md
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       27 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/requirements.txt
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.767128 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.767376 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794029 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/defaults/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      226 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/defaults/main.yaml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794236 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/tasks/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1204 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794632 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      162 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/admin-password-secret.yml.j2
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      264 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/awx.yaml.j2
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.794816 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      464 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/kustomization.yaml.j2
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3917 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/e2e/utils.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.795509 ansible_rulebook-1.0.0/tests/event_filter/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1615 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/dashes_to_underscores.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1964 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/json_filter.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      691 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/noop.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1385 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/event_filter/test_insert_meta_info.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.806738 ansible_rulebook-1.0.0/tests/examples/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      182 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/01_noop.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      176 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/02_debug.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      188 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/03_print_event.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      324 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/04_set_fact.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      326 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/05_post_event.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      458 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/06_retract_fact.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      210 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/07_and.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      208 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/08_or.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      165 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/09_gt.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      162 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/10_lt.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      175 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/11_le.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      178 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/12_ge.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      203 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/13_add.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      208 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/14_sub.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      259 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/15_multiple_events_all.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      259 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/16_multiple_events_any.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      258 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/17_multiple_sources_any.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      262 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/18_multiple_sources_all.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      402 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/19_is_defined.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      431 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/20_is_not_defined.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      216 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/21_run_playbook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      249 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/22_run_playbook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      222 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/23_nested_data.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      220 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/24_max_attributes.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      261 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/25_max_attributes_nested.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      240 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/26_print_events.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      894 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/27_var_root.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      205 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/28_right_side_condition_template.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      270 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/29_run_module.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      268 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/30_run_module_missing.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      275 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/31_run_module_missing_args.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      278 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/32_run_module_fail.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      359 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/33_run_playbook_retry.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      339 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/34_run_playbook_retries.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      575 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      766 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      402 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/37_hosts_facts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      299 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/38_shutdown.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      206 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/39_is_defined.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      183 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/40_in.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      193 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/41_not_in.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      268 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/42_contains.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      276 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/43_not_contains.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      201 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/44_in_and.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      199 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/45_in_or.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      376 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/46_job_template.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      311 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/47_generic_plugin.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      206 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/48_echo.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      445 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/49_float.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      660 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/50_negation.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1375 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/51_vars_namespace.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      648 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/52_once_within.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      659 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/53_once_within_multiple_hosts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      542 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/54_time_window.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      622 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/55_not_all.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      798 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/56_once_after.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1890 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/57_once_after_multi.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1453 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/58_string_search.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      444 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/59_multiple_actions.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      713 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/60_json_filter.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      608 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/61_select_1.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      903 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/62_select_2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      938 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/63_selectattr_1.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      589 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/64_selectattr_2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      413 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/65_selectattr_3.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      881 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/66_sleepy_playbook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      835 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/67_shutdown_now.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      347 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/68_disabled_rule.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      729 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/69_enhanced_debug.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      724 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/70_null.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1101 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/72_set_fact_with_type.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      874 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/73_mix_and_match_list.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      231 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/74_self_referential.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      538 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/75_all_conditions.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      736 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/76_all_conditions.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      485 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/77_default_events_ttl.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      592 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/78_complete_retract_fact.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.768066 ansible_rulebook-1.0.0/tests/examples/replays/
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.808154 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/00.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/01.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/02.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/03.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/04.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/05.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/06.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/07.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/08.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       72 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/09.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      833 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/generate_data.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.808418 ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     5032 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/00.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      898 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/generate_data.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.808689 ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3791 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/00.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1107 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/generate_data.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.810142 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/00.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/01.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/02.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/03.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/04.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/05.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/06.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/07.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/08.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       73 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/09.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      833 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/generate_data.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1696 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/generate_asts.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.811576 ansible_rulebook-1.0.0/tests/playbooks/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      618 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/check_facts_playbook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      370 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/compare_value.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      829 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/fail_and_succeed.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      400 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/hello.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      309 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/hello_events.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      290 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/hello_world_set_fact.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      129 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/inventory.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      114 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/inventory1.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      260 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/sleeper.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      704 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/validate_args_playbook.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)       13 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/playbooks/vars.yml
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.816281 ansible_rulebook-1.0.0/tests/rules/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      300 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rule_names_with_substitution.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1410 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      252 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_assignment.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      251 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_assignment2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      307 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_multiple_conditions.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      308 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_multiple_conditions2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      475 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_multiple_conditions3.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      741 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_time.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1070 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_timestamp.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      281 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_with_vars.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      244 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/rules_without_assignment.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      203 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_blank_rule_name.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      171 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_blank_ruleset_name.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      282 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_combine_hosts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      329 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_combine_hosts_module.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      286 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_duplicate_rule_names.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      348 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_duplicate_ruleset_names.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      199 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_empty_rule_names.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      618 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_filters.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      754 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_host_rules.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1463 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_kafka.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      189 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_missing_rule_names.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      159 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_missing_ruleset_name.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      337 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_multiple_sources.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      746 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      461 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_expanded_conditions.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      813 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      195 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts2.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      195 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts3.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      244 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_rules_playbooks.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      728 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_set_facts.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      587 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_simple.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      985 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/test_states.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      944 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/rules/webserver_down.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      275 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/run_examples.sh
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.818607 ansible_rulebook-1.0.0/tests/sources/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/__init__.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2613 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/file.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4945 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/generic.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      963 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/hosts.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1613 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/infrange.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2841 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/log_scraper.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1258 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/nested.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1210 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/ping.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2195 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/process_check.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1245 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/range.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1014 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/range2.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1578 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replay.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.819318 ansible_rulebook-1.0.0/tests/sources/replays/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/01.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/02.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/03.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/04.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)        9 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/replays/05.json
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1224 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/template.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      891 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/tick.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1024 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/timestamp.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1908 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/sources/url_check.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1120 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_ansible_events.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     5887 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_app.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    18000 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_ast.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     2206 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_collection.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3038 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_controller.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    15993 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_engine.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)    66166 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_examples.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     8114 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_rules.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)      576 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_simple.yml
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     4931 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/test_websocket.py
-drwxr-xr-x   0 madhukanoor   (501) wheel        (0)        0 2023-06-15 17:08:23.819627 ansible_rulebook-1.0.0/tests/unit/
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     3055 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/unit/test_cli.py
--rw-r--r--   0 madhukanoor   (501) wheel        (0)     1147 2023-06-15 17:08:20.000000 ansible_rulebook-1.0.0/tests/unit/test_util.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.780255 ansible_rulebook-1.0.1/
+-rw-r--r--   0 alex      (1000) alex      (1000)    11358 2022-07-11 07:18:31.000000 ansible_rulebook-1.0.1/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      312 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     4061 2023-07-24 18:07:57.780255 ansible_rulebook-1.0.1/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     3353 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/README.rst
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.747255 ansible_rulebook-1.0.1/ansible_rulebook/
+-rw-r--r--   0 alex      (1000) alex      (1000)      671 2023-07-24 18:02:55.000000 ansible_rulebook-1.0.1/ansible_rulebook/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      634 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/ansible_rulebook/__main__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8637 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/ansible_rulebook/app.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    26654 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/ansible_rulebook/builtin.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7948 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/ansible_rulebook/cli.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4671 2023-05-29 08:08:23.000000 ansible_rulebook-1.0.1/ansible_rulebook/collection.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1136 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/ansible_rulebook/common.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8165 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/ansible_rulebook/condition_parser.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2659 2023-02-23 16:22:58.000000 ansible_rulebook-1.0.1/ansible_rulebook/condition_types.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      796 2023-06-01 12:57:54.000000 ansible_rulebook-1.0.1/ansible_rulebook/conf.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9754 2023-06-01 12:57:54.000000 ansible_rulebook-1.0.1/ansible_rulebook/engine.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.748255 ansible_rulebook-1.0.1/ansible_rulebook/event_filter/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.1/ansible_rulebook/event_filter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1346 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.1/ansible_rulebook/event_filter/insert_meta_info.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2228 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/ansible_rulebook/exception.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5096 2023-07-19 10:30:23.000000 ansible_rulebook-1.0.1/ansible_rulebook/job_template_runner.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11925 2023-04-27 08:47:19.000000 ansible_rulebook-1.0.1/ansible_rulebook/json_generator.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      827 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/ansible_rulebook/messages.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3173 2023-03-31 12:02:14.000000 ansible_rulebook-1.0.1/ansible_rulebook/rule_generator.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17771 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/ansible_rulebook/rule_set_runner.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2418 2023-06-01 12:57:54.000000 ansible_rulebook-1.0.1/ansible_rulebook/rule_types.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6558 2023-06-01 12:57:54.000000 ansible_rulebook-1.0.1/ansible_rulebook/rules_parser.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.748255 ansible_rulebook-1.0.1/ansible_rulebook/schema/
+-rw-r--r--   0 alex      (1000) alex      (1000)    20587 2023-06-27 07:08:54.000000 ansible_rulebook-1.0.1/ansible_rulebook/schema/ruleset_schema.json
+-rw-r--r--   0 alex      (1000) alex      (1000)     7223 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/ansible_rulebook/util.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1428 2023-05-11 09:41:59.000000 ansible_rulebook-1.0.1/ansible_rulebook/validators.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4908 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/ansible_rulebook/websocket.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.748255 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     4061 2023-07-24 18:07:57.000000 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)    12936 2023-07-24 18:07:57.000000 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-07-24 18:07:57.000000 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       63 2023-07-24 18:07:57.000000 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-07-24 18:07:57.000000 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/not-zip-safe
+-rw-r--r--   0 alex      (1000) alex      (1000)      104 2023-07-24 18:07:57.000000 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       17 2023-07-24 18:07:57.000000 ansible_rulebook-1.0.1/ansible_rulebook.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.750255 ansible_rulebook-1.0.1/docs/
+-rw-r--r--   0 alex      (1000) alex      (1000)      617 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/docs/Makefile
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.742255 ansible_rulebook-1.0.1/docs/_build/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.742255 ansible_rulebook-1.0.1/docs/_build/html/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.751255 ansible_rulebook-1.0.1/docs/_build/html/_static/
+-rw-r--r--   0 alex      (1000) alex      (1000)      286 2022-10-20 07:13:59.000000 ansible_rulebook-1.0.1/docs/_build/html/_static/file.png
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.751255 ansible_rulebook-1.0.1/docs/_build/html/_static/images/
+-rw-r--r--   0 alex      (1000) alex      (1000)     8664 2023-01-11 10:06:59.000000 ansible_rulebook-1.0.1/docs/_build/html/_static/images/Ansible-Mark-RGB_Black.png
+-rw-r--r--   0 alex      (1000) alex      (1000)     5173 2023-01-11 10:06:59.000000 ansible_rulebook-1.0.1/docs/_build/html/_static/images/Ansible-Mark-RGB_White.png
+-rw-r--r--   0 alex      (1000) alex      (1000)       90 2022-10-20 07:13:59.000000 ansible_rulebook-1.0.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 alex      (1000) alex      (1000)       90 2022-10-20 07:13:59.000000 ansible_rulebook-1.0.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 alex      (1000) alex      (1000)    11365 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/docs/actions.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2647 2023-06-05 18:56:04.000000 ansible_rulebook-1.0.1/docs/collections.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)    33660 2023-07-24 08:05:11.000000 ansible_rulebook-1.0.1/docs/conditions.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     5971 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/docs/conf.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2033 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/docs/contributing.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     3923 2023-07-18 19:35:09.000000 ansible_rulebook-1.0.1/docs/decision_environment.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     3560 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/docs/development_environment.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2033 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.1/docs/events_and_facts.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2700 2023-06-05 18:56:04.000000 ansible_rulebook-1.0.1/docs/filters.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     7006 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/docs/getting_started.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      625 2023-01-13 09:14:28.000000 ansible_rulebook-1.0.1/docs/host_limit.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      495 2023-06-05 18:56:04.000000 ansible_rulebook-1.0.1/docs/index.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2437 2023-06-27 14:11:13.000000 ansible_rulebook-1.0.1/docs/installation.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     5447 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/docs/introduction.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      778 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/docs/make.bat
+-rw-r--r--   0 alex      (1000) alex      (1000)     2278 2023-01-16 11:17:52.000000 ansible_rulebook-1.0.1/docs/multi_events.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     4137 2023-06-01 12:57:54.000000 ansible_rulebook-1.0.1/docs/rulebooks.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2391 2023-06-27 07:08:54.000000 ansible_rulebook-1.0.1/docs/rules.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)       41 2023-01-13 09:14:28.000000 ansible_rulebook-1.0.1/docs/runner.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     8083 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/docs/sources.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     4380 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/docs/usage.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     4865 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/docs/variables.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      269 2023-06-27 14:11:13.000000 ansible_rulebook-1.0.1/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1448 2023-07-24 18:07:57.781255 ansible_rulebook-1.0.1/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.752255 ansible_rulebook-1.0.1/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)      634 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.757255 ansible_rulebook-1.0.1/tests/asts/
+-rw-r--r--   0 alex      (1000) alex      (1000)      516 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/01_noop.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      510 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/02_debug.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      522 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/03_print_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      888 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/04_set_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      890 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/05_post_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1183 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/06_retract_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      772 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/07_and.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      770 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/08_or.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      522 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/09_gt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      516 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/10_lt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      537 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/11_le.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      543 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/12_ge.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      662 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/13_add.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      670 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/14_sub.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      683 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/15_multiple_events_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      683 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/16_multiple_events_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      783 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/17_multiple_sources_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      787 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/18_multiple_sources_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1076 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/asts/19_is_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1100 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/20_is_not_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      561 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/21_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      565 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/23_nested_data.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      563 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/24_max_attributes.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      604 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/25_max_attributes_nested.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      643 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/26_print_events.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1066 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/27_var_root.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      769 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/28_right_side_condition_template.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      621 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/29_run_module.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      619 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/30_run_module_missing.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      626 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/31_run_module_missing_args.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      641 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/32_run_module_fail.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      649 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/33_run_playbook_retry.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      625 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/34_run_playbook_retries.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1521 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1537 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1090 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/37_hosts_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      534 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.1/tests/asts/38_shutdown.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2990 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      694 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      693 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_assignment2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      924 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_multiple_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      925 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1441 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1605 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_time.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2385 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_timestamp.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      916 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules_with_vars.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      580 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/rules_without_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1638 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/test_filters.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1963 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/test_host_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1955 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/test_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2022 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/test_rules_multiple_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      530 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      530 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1338 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.1/tests/asts/test_set_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1552 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/asts/test_simple.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.757255 ansible_rulebook-1.0.1/tests/cassettes/
+-rw-r--r--   0 alex      (1000) alex      (1000)    28619 2023-05-16 08:13:11.000000 ansible_rulebook-1.0.1/tests/cassettes/test_job_template.yaml
+-rw-r--r--   0 alex      (1000) alex      (1000)    10489 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.1/tests/cassettes/test_job_template_not_exist.yaml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2754 2023-06-01 12:57:54.000000 ansible_rulebook-1.0.1/tests/conftest.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.758255 ansible_rulebook-1.0.1/tests/data/
+-rw-r--r--   0 alex      (1000) alex      (1000)       37 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.1/tests/data/bad_source.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      137 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.1/tests/data/not_asyncio.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      727 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/tests/data/rulebook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)    47616 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.1/tests/data/test.tar
+-rw-r--r--   0 alex      (1000) alex      (1000)       68 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/tests/data/test_vars.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.759255 ansible_rulebook-1.0.1/tests/e2e/
+-rw-r--r--   0 alex      (1000) alex      (1000)      878 2023-02-13 17:29:00.000000 ansible_rulebook-1.0.1/tests/e2e/README.md
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/e2e/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.759255 ansible_rulebook-1.0.1/tests/e2e/config/
+-rw-r--r--   0 alex      (1000) alex      (1000)      246 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/config/default.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      564 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.1/tests/e2e/conftest.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.743255 ansible_rulebook-1.0.1/tests/e2e/files/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.759255 ansible_rulebook-1.0.1/tests/e2e/files/extra_vars/
+-rw-r--r--   0 alex      (1000) alex      (1000)      826 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.1/tests/e2e/files/extra_vars/operator_variables.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      162 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/extra_vars/test_variables_extra_vars.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.760255 ansible_rulebook-1.0.1/tests/e2e/files/inventories/
+-rw-r--r--   0 alex      (1000) alex      (1000)       35 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/tests/e2e/files/inventories/default_inventory.ini
+-rw-r--r--   0 alex      (1000) alex      (1000)       61 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/e2e/files/inventories/default_inventory.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.760255 ansible_rulebook-1.0.1/tests/e2e/files/playbooks/
+-rw-r--r--   0 alex      (1000) alex      (1000)      404 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/playbooks/long_running.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      344 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/e2e/files/playbooks/print_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      240 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.1/tests/e2e/files/playbooks/print_rule_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1522 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.1/tests/e2e/files/playbooks/run_playbook_test_playbook.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.760255 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.761255 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/
+-rw-r--r--   0 alex      (1000) alex      (1000)     4727 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2451 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1611 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1050 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      288 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/hello_events_with_var.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      253 2023-01-12 10:03:30.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/malformed_rulebook.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.761255 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6274 2023-04-12 20:32:28.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_logical_operators.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     6060 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_membership_operators.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     6216 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_relational_operators.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     3476 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_select_operator.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     7702 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2545 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_string_match.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2583 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2623 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_string_search_search.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1394 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/test_disabled_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      270 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/test_process_sigint.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      955 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/test_process_source_end.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.762255 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/variables/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2070 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.762255 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/websockets/
+-rw-r--r--   0 alex      (1000) alex      (1000)      283 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/websockets/test_websocket_range.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      522 2023-02-13 17:29:00.000000 ansible_rulebook-1.0.1/tests/e2e/settings.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10871 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/tests/e2e/test_actions.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    20067 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.1/tests/e2e/test_operators.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5843 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/tests/e2e/test_runtime.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2271 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/e2e/test_variables.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3595 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.1/tests/e2e/test_websocket.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.743255 ansible_rulebook-1.0.1/tests/e2e/utils/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.762255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/
+-rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/ansible.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.743255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/artifacts/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.762255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/artifacts/localhost/
+-rw-r--r--   0 alex      (1000) alex      (1000)      219 2023-03-27 21:29:08.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/artifacts/localhost/awx.yaml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.762255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/artifacts/localhost/kustomization/
+-rw-r--r--   0 alex      (1000) alex      (1000)      406 2023-03-27 21:29:08.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/artifacts/localhost/kustomization/kustomization.yaml
+-rw-r--r--   0 alex      (1000) alex      (1000)      602 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/create-cluster.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      637 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/install-awx.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      437 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/kind-config.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      855 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/readme.md
+-rw-r--r--   0 alex      (1000) alex      (1000)       27 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/requirements.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.743255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.744255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.763255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/defaults/
+-rw-r--r--   0 alex      (1000) alex      (1000)      226 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/defaults/main.yaml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.763255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/tasks/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1204 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.763255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/templates/
+-rw-r--r--   0 alex      (1000) alex      (1000)      162 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/templates/admin-password-secret.yml.j2
+-rw-r--r--   0 alex      (1000) alex      (1000)      264 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/templates/awx.yaml.j2
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.763255 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/
+-rw-r--r--   0 alex      (1000) alex      (1000)      464 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/kustomization.yaml.j2
+-rw-r--r--   0 alex      (1000) alex      (1000)     3917 2023-05-24 15:20:29.000000 ansible_rulebook-1.0.1/tests/e2e/utils.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.763255 ansible_rulebook-1.0.1/tests/event_filter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1615 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.1/tests/event_filter/dashes_to_underscores.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1964 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.1/tests/event_filter/json_filter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      691 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.1/tests/event_filter/noop.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1385 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.1/tests/event_filter/test_insert_meta_info.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.771255 ansible_rulebook-1.0.1/tests/examples/
+-rw-r--r--   0 alex      (1000) alex      (1000)      182 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/01_noop.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      176 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/02_debug.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      188 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/03_print_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      324 2023-01-23 17:48:15.000000 ansible_rulebook-1.0.1/tests/examples/04_set_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      326 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/05_post_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      458 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/06_retract_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      210 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/07_and.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      208 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/08_or.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      165 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/09_gt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      162 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/10_lt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      175 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/11_le.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      178 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/12_ge.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      203 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/13_add.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      208 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/14_sub.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      259 2023-01-13 09:14:18.000000 ansible_rulebook-1.0.1/tests/examples/15_multiple_events_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      259 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/16_multiple_events_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      258 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/17_multiple_sources_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      262 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/18_multiple_sources_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      402 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/19_is_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      431 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/20_is_not_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      216 2022-11-29 16:59:01.000000 ansible_rulebook-1.0.1/tests/examples/21_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      249 2022-11-17 11:07:48.000000 ansible_rulebook-1.0.1/tests/examples/22_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      222 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/23_nested_data.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      220 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/24_max_attributes.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      261 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/25_max_attributes_nested.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      240 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/26_print_events.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      894 2023-05-24 15:20:29.000000 ansible_rulebook-1.0.1/tests/examples/27_var_root.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      205 2023-02-10 11:45:34.000000 ansible_rulebook-1.0.1/tests/examples/28_right_side_condition_template.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      270 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/29_run_module.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      268 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/30_run_module_missing.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      275 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/31_run_module_missing_args.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      278 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/32_run_module_fail.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      359 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.1/tests/examples/33_run_playbook_retry.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      339 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.1/tests/examples/34_run_playbook_retries.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      575 2022-11-08 11:23:52.000000 ansible_rulebook-1.0.1/tests/examples/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      766 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      402 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/examples/37_hosts_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      299 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/38_shutdown.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      206 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/39_is_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      183 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/40_in.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      193 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/41_not_in.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      268 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/42_contains.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      276 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/43_not_contains.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      201 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/examples/44_in_and.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      199 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/examples/45_in_or.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      376 2023-01-13 09:14:18.000000 ansible_rulebook-1.0.1/tests/examples/46_job_template.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      311 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/47_generic_plugin.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      206 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/48_echo.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      445 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.1/tests/examples/49_float.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      660 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/50_negation.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1375 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/51_vars_namespace.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      648 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/52_once_within.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      659 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/53_once_within_multiple_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      542 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/examples/54_time_window.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      622 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/55_not_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      798 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/56_once_after.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1890 2023-04-12 20:32:28.000000 ansible_rulebook-1.0.1/tests/examples/57_once_after_multi.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1453 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/58_string_search.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      444 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/examples/59_multiple_actions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      713 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/60_json_filter.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      608 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/61_select_1.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      903 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/62_select_2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      938 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/63_selectattr_1.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      589 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/64_selectattr_2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      413 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/65_selectattr_3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      881 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/66_sleepy_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      835 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/67_shutdown_now.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      347 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/68_disabled_rule.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      729 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/examples/69_enhanced_debug.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      724 2023-02-23 16:22:58.000000 ansible_rulebook-1.0.1/tests/examples/70_null.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1101 2023-03-01 22:34:32.000000 ansible_rulebook-1.0.1/tests/examples/72_set_fact_with_type.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      874 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.1/tests/examples/73_mix_and_match_list.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      231 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/examples/74_self_referential.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      538 2023-04-12 20:32:28.000000 ansible_rulebook-1.0.1/tests/examples/75_all_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      736 2023-04-12 20:32:28.000000 ansible_rulebook-1.0.1/tests/examples/76_all_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      485 2023-04-27 08:47:19.000000 ansible_rulebook-1.0.1/tests/examples/77_default_events_ttl.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      592 2023-05-30 21:59:52.000000 ansible_rulebook-1.0.1/tests/examples/78_complete_retract_fact.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.744255 ansible_rulebook-1.0.1/tests/examples/replays/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.772255 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/01.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/02.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/03.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/04.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/05.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/06.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/07.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/08.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       72 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/09.json
+-rw-r--r--   0 alex      (1000) alex      (1000)      833 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/generate_data.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.772255 ansible_rulebook-1.0.1/tests/examples/replays/24_max_attributes/
+-rw-r--r--   0 alex      (1000) alex      (1000)     5032 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/24_max_attributes/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)      898 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/24_max_attributes/generate_data.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.772255 ansible_rulebook-1.0.1/tests/examples/replays/25_max_attributes_nested/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3791 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.1/tests/examples/replays/25_max_attributes_nested/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)     1107 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/25_max_attributes_nested/generate_data.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.774255 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/01.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/02.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/03.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/04.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/05.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/06.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/07.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/08.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/09.json
+-rw-r--r--   0 alex      (1000) alex      (1000)      833 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/generate_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1696 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/generate_asts.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.775255 ansible_rulebook-1.0.1/tests/playbooks/
+-rw-r--r--   0 alex      (1000) alex      (1000)      618 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/playbooks/check_facts_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      370 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/playbooks/compare_value.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      829 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.1/tests/playbooks/fail_and_succeed.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      400 2023-02-10 21:49:17.000000 ansible_rulebook-1.0.1/tests/playbooks/hello.yaml
+-rw-r--r--   0 alex      (1000) alex      (1000)      400 2023-02-17 18:46:04.000000 ansible_rulebook-1.0.1/tests/playbooks/hello.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      309 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/playbooks/hello_events.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      290 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/playbooks/hello_world_set_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      129 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.1/tests/playbooks/inventory.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/playbooks/inventory1.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      260 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/playbooks/sleeper.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      704 2023-02-23 16:22:58.000000 ansible_rulebook-1.0.1/tests/playbooks/validate_args_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)       13 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/playbooks/vars.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.778255 ansible_rulebook-1.0.1/tests/rules/
+-rw-r--r--   0 alex      (1000) alex      (1000)      300 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.1/tests/rules/rule_names_with_substitution.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1410 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      252 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      251 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_assignment2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      307 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_multiple_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      308 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      475 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      741 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_time.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1070 2022-10-13 21:12:04.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_timestamp.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      281 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/rules_with_vars.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      244 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/rules_without_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      203 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/rules/test_blank_rule_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      171 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/rules/test_blank_ruleset_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      282 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/rules/test_combine_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      329 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/rules/test_combine_hosts_module.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      286 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_duplicate_rule_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      348 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/rules/test_duplicate_ruleset_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      199 2022-10-13 20:51:42.000000 ansible_rulebook-1.0.1/tests/rules/test_empty_rule_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      618 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_filters.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      754 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_host_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1463 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_kafka.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      189 2022-10-13 20:51:42.000000 ansible_rulebook-1.0.1/tests/rules/test_missing_rule_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      159 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.1/tests/rules/test_missing_ruleset_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      337 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/test_multiple_sources.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      746 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      461 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/test_rules_expanded_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      813 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_rules_multiple_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      195 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      195 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      244 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/test_rules_playbooks.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      728 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.1/tests/rules/test_set_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      587 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_simple.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      985 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.1/tests/rules/test_states.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      944 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/rules/webserver_down.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      275 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/run_examples.sh
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.780255 ansible_rulebook-1.0.1/tests/sources/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2022-11-17 11:54:27.000000 ansible_rulebook-1.0.1/tests/sources/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2613 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/file.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4945 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.1/tests/sources/generic.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      963 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/hosts.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1613 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/sources/infrange.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2841 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/log_scraper.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1258 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/sources/nested.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1210 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/ping.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/process_check.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1245 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.1/tests/sources/range.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1014 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/sources/range2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1578 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/sources/replay.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.780255 ansible_rulebook-1.0.1/tests/sources/replays/
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2022-07-19 14:11:31.000000 ansible_rulebook-1.0.1/tests/sources/replays/01.json
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2022-07-19 14:11:31.000000 ansible_rulebook-1.0.1/tests/sources/replays/02.json
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2022-07-19 14:11:31.000000 ansible_rulebook-1.0.1/tests/sources/replays/03.json
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2022-07-19 14:11:31.000000 ansible_rulebook-1.0.1/tests/sources/replays/04.json
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2022-07-19 14:11:31.000000 ansible_rulebook-1.0.1/tests/sources/replays/05.json
+-rw-r--r--   0 alex      (1000) alex      (1000)     1224 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/sources/template.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      891 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/tick.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1024 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/timestamp.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1908 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.1/tests/sources/url_check.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1120 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.1/tests/test_ansible_events.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5941 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/tests/test_app.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    18000 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/test_ast.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2206 2023-05-29 08:08:23.000000 ansible_rulebook-1.0.1/tests/test_collection.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3038 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/tests/test_controller.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    15993 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/tests/test_engine.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    66197 2023-07-19 14:32:50.000000 ansible_rulebook-1.0.1/tests/test_examples.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8114 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.1/tests/test_rules.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      576 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.1/tests/test_simple.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     4931 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.1/tests/test_websocket.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 18:07:57.780255 ansible_rulebook-1.0.1/tests/unit/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3055 2023-05-11 09:41:59.000000 ansible_rulebook-1.0.1/tests/unit/test_cli.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1147 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.1/tests/unit/test_util.py
```

### Comparing `ansible_rulebook-1.0.0/LICENSE` & `ansible_rulebook-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/PKG-INFO` & `ansible_rulebook-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ansible_rulebook
-Version: 1.0.0
+Version: 1.0.1
 Summary: Event driven automation for Ansible
 Home-page: https://github.com/ansible/ansible-rulebook
 License: Apache-2.0
 Keywords: ansible_rulebook
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 ================
 ansible-rulebook
 ================
```

### Comparing `ansible_rulebook-1.0.0/README.rst` & `ansible_rulebook-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/__init__.py` & `ansible_rulebook-1.0.1/ansible_rulebook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Top-level package for Ansible Events."""
 
-__version__ = "__version__ = '1.0.0'"
+__version__ = "__version__ = '1.0.1'"
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/__main__.py` & `ansible_rulebook-1.0.1/ansible_rulebook/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/app.py` & `ansible_rulebook-1.0.1/ansible_rulebook/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,17 @@
             startup_args.inventory = load_inventory(parsed_args.inventory)
         startup_args.project_data_file = parsed_args.project_tarball
         startup_args.controller_url = parsed_args.controller_url
         startup_args.controller_token = parsed_args.controller_token
         startup_args.controller_ssl_verify = parsed_args.controller_ssl_verify
 
     validate_actions(startup_args)
-    await validate_controller_params(startup_args)
+
+    if startup_args.check_controller_connection:
+        await validate_controller_params(startup_args)
 
     if parsed_args.websocket_address:
         event_log = asyncio.Queue()
     else:
         event_log = NullQueue()
 
     logger.info("Starting sources")
@@ -135,14 +137,15 @@
             result, CancelledError
         ):
             logger.error(result)
             error_found = True
 
     logger.info("Main complete")
     await event_log.put(dict(type="Exit"))
+    await job_template_runner.close_session()
     if error_found:
         raise Exception("One of the source plugins failed")
 
 
 # TODO(cutwater): Maybe move to util.py
 def load_vars(parsed_args) -> Dict[str, str]:
     variables = dict()
@@ -221,14 +224,16 @@
     return tasks, ruleset_queues
 
 
 def validate_actions(startup_args: StartupArgs) -> None:
     for ruleset in startup_args.rulesets:
         for rule in ruleset.rules:
             for action in rule.actions:
+                if action.action == "run_job_template":
+                    startup_args.check_controller_connection = True
                 if (
                     action.action in INVENTORY_ACTIONS
                     and not startup_args.inventory
                 ):
                     raise InventoryNeededException(
                         f"Rule {rule.name} has an action {action.action} "
                         "which needs inventory to be defined"
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/builtin.py` & `ansible_rulebook-1.0.1/ansible_rulebook/builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -821,15 +821,15 @@
         status=controller_job["status"],
         run_at=controller_job["created"],
         url=_controller_job_url(controller_job),
         matching_events=_get_events(variables),
         rule_run_at=rule_run_at,
     )
     if "error" in controller_job:
-        a_log["reason"] = dict(error=controller_job["error"])
+        a_log["message"] = controller_job["error"]
     await event_log.put(a_log)
 
     if set_facts or post_events:
         logger.debug("set_facts")
         facts = controller_job["artifacts"]
         if facts:
             facts = _embellish_internal_event(facts, "run_job_template")
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/cli.py` & `ansible_rulebook-1.0.1/ansible_rulebook/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/collection.py` & `ansible_rulebook-1.0.1/ansible_rulebook/collection.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/common.py` & `ansible_rulebook-1.0.1/ansible_rulebook/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,7 +23,8 @@
     rulesets: List[RuleSet] = field(default_factory=list)
     variables: Dict = field(default_factory=dict)
     controller_url: str = field(default="")
     controller_token: str = field(default="")
     controller_ssl_verify: str = field(default="")
     project_data_file: str = field(default="")
     inventory: str = field(default="")
+    check_controller_connection: bool = field(default=False)
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/condition_parser.py` & `ansible_rulebook-1.0.1/ansible_rulebook/condition_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/condition_types.py` & `ansible_rulebook-1.0.1/ansible_rulebook/condition_types.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/conf.py` & `ansible_rulebook-1.0.1/ansible_rulebook/conf.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/engine.py` & `ansible_rulebook-1.0.1/ansible_rulebook/engine.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/event_filter/insert_meta_info.py` & `ansible_rulebook-1.0.1/ansible_rulebook/event_filter/insert_meta_info.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/exception.py` & `ansible_rulebook-1.0.1/ansible_rulebook/exception.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/job_template_runner.py` & `ansible_rulebook-1.0.1/ansible_rulebook/job_template_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,61 +31,56 @@
 
 logger = logging.getLogger(__name__)
 
 
 class JobTemplateRunner:
     JOB_TEMPLATE_SLUG = "/api/v2/job_templates"
     CONFIG_SLUG = "/api/v2/config"
-    VALID_POST_CODES = [200, 201, 202]
     JOB_COMPLETION_STATUSES = ["successful", "failed", "error", "canceled"]
 
     def __init__(
         self, host: str = "", token: str = "", verify_ssl: str = "yes"
     ):
         self.token = token
         self.host = host
         self.verify_ssl = verify_ssl
         self.refresh_delay = int(
             os.environ.get("EDA_JOB_TEMPLATE_REFRESH_DELAY", 10)
         )
+        self._session = None
 
-    async def _get_page(
-        self, session: aiohttp.ClientSession, href_slug: str, params: dict
-    ) -> dict:
-        url = urljoin(self.host, href_slug)
-        async with session.get(
-            url, params=params, ssl=self._sslcontext
-        ) as response:
-            response_text = dict(
-                status=response.status, body=await response.text()
-            )
-        if response_text["status"] != 200:
-            raise ControllerApiException(
-                "Failed to get from %s. Status: %s, Body: %s"
-                % (
-                    url,
-                    response_text["status"],
-                    response_text.get("body", "empty"),
-                )
+    async def close_session(self):
+        if self._session and not self._session.closed:
+            await self._session.close()
+
+    def _create_session(self):
+        if self._session is None:
+            limit = int(os.getenv("EDA_CONTROLLER_CONNECTION_LIMIT", "30"))
+            self._session = aiohttp.ClientSession(
+                connector=aiohttp.TCPConnector(limit=limit),
+                headers=self._auth_headers(),
+                raise_for_status=True,
             )
-        return response_text
 
-    async def get_config(self) -> dict:
+    async def _get_page(self, href_slug: str, params: dict) -> dict:
         try:
-            logger.info("Attempting to connect to Controller %s", self.host)
-            async with aiohttp.ClientSession(
-                raise_for_status=True, headers=self._auth_headers()
-            ) as session:
-                url = urljoin(self.host, self.CONFIG_SLUG)
-                async with session.get(url, ssl=self._sslcontext) as response:
-                    return json.loads(await response.text())
+            url = urljoin(self.host, href_slug)
+            self._create_session()
+            async with self._session.get(
+                url, params=params, ssl=self._sslcontext
+            ) as response:
+                return json.loads(await response.text())
         except aiohttp.ClientError as e:
             logger.error("Error connecting to controller %s", str(e))
             raise ControllerApiException(str(e))
 
+    async def get_config(self) -> dict:
+        logger.info("Attempting to connect to Controller %s", self.host)
+        return await self._get_page(self.CONFIG_SLUG, {})
+
     def _auth_headers(self) -> dict:
         return dict(Authorization=f"Bearer {self.token}")
 
     @cached_property
     def _sslcontext(self) -> Union[bool, ssl.SSLContext]:
         if self.host.startswith("https"):
             if self.verify_ssl.lower() == "yes":
@@ -94,34 +89,28 @@
                 return ssl.create_default_context(cafile=self.verify_ssl)
         return False
 
     async def _get_job_template_id(self, name: str, organization: str) -> int:
         slug = f"{self.JOB_TEMPLATE_SLUG}/"
         params = {"name": name}
 
-        async with aiohttp.ClientSession(
-            headers=self._auth_headers()
-        ) as session:
-            while True:
-                response = await self._get_page(session, slug, params)
-                json_body = json.loads(response["body"])
-                for jt in json_body["results"]:
-                    if (
-                        jt["name"] == name
-                        and dpath.get(
-                            jt, "summary_fields.organization.name", "."
-                        )
-                        == organization
-                    ):
-                        return jt["id"]
-
-                if json_body.get("next", None):
-                    params["page"] = params.get("page", 1) + 1
-                else:
-                    break
+        while True:
+            json_body = await self._get_page(slug, params)
+            for jt in json_body["results"]:
+                if (
+                    jt["name"] == name
+                    and dpath.get(jt, "summary_fields.organization.name", ".")
+                    == organization
+                ):
+                    return jt["id"]
+
+            if json_body.get("next", None):
+                params["page"] = params.get("page", 1) + 1
+            else:
+                break
 
         raise JobTemplateNotFoundException(
             (
                 f"Job template {name} in organization "
                 f"{organization} does not exist"
             )
         )
@@ -133,51 +122,33 @@
         job_params: dict,
     ) -> dict:
         job = await self.launch(name, organization, job_params)
 
         url = job["url"]
         params = {}
 
-        async with aiohttp.ClientSession(
-            headers=self._auth_headers()
-        ) as session:
-            while True:
-                # fetch and process job status
-                response = await self._get_page(session, url, params)
-                json_body = json.loads(response["body"])
-                job_status = json_body["status"]
-                if job_status in self.JOB_COMPLETION_STATUSES:
-                    return json_body
+        while True:
+            # fetch and process job status
+            json_body = await self._get_page(url, params)
+            job_status = json_body["status"]
+            if job_status in self.JOB_COMPLETION_STATUSES:
+                return json_body
 
-                await asyncio.sleep(self.refresh_delay)
+            await asyncio.sleep(self.refresh_delay)
 
     async def launch(
         self, name: str, organization: str, job_params: dict
     ) -> dict:
         jt_id = await self._get_job_template_id(name, organization)
         url = urljoin(self.host, f"{self.JOB_TEMPLATE_SLUG}/{jt_id}/launch/")
 
-        async with aiohttp.ClientSession(
-            headers=self._auth_headers()
-        ) as session:
-            async with session.post(
+        try:
+            async with self._session.post(
                 url, json=job_params, ssl=self._sslcontext
             ) as post_response:
-                response = dict(
-                    status=post_response.status,
-                    body=await post_response.text(),
-                )
-
-                if response["status"] not in self.VALID_POST_CODES:
-                    raise ControllerApiException(
-                        "Failed to post to %s. Status: %s, Body: %s"
-                        % (
-                            url,
-                            response["status"],
-                            response.get("body", "empty"),
-                        )
-                    )
-                json_body = json.loads(response["body"])
-        return json_body
+                return json.loads(await post_response.text())
+        except aiohttp.ClientError as e:
+            logger.error("Error connecting to controller %s", str(e))
+            raise ControllerApiException(str(e))
 
 
 job_template_runner = JobTemplateRunner()
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/json_generator.py` & `ansible_rulebook-1.0.1/ansible_rulebook/json_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/messages.py` & `ansible_rulebook-1.0.1/ansible_rulebook/messages.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/rule_generator.py` & `ansible_rulebook-1.0.1/ansible_rulebook/rule_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/rule_set_runner.py` & `ansible_rulebook-1.0.1/ansible_rulebook/rule_set_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,15 +447,16 @@
                     type="Action",
                     action=action,
                     action_uuid=str(uuid.uuid4()),
                     activation_id=settings.identifier,
                     playbook_name=action_args.get("name"),
                     status="failed",
                     run_at=run_at(),
-                    reason=dict(error=str(error)),
+                    rule_run_at=rule_run_at,
+                    message=str(error),
                     rule=rule,
                     ruleset=ruleset,
                     rule_uuid=rule_uuid,
                     ruleset_uuid=ruleset_uuid,
                 )
             )
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/rule_types.py` & `ansible_rulebook-1.0.1/ansible_rulebook/rule_types.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/rules_parser.py` & `ansible_rulebook-1.0.1/ansible_rulebook/rules_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/schema/ruleset_schema.json` & `ansible_rulebook-1.0.1/ansible_rulebook/schema/ruleset_schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999981352189999%*

 * *Differences: {"'$defs'": "{'ruleset': {'properties': {'execution_strategy': {'enum': {insert: [(1, "*

 * *            "'sequential')], delete: [0]}}}}}"}*

```diff
@@ -318,16 +318,16 @@
                 "default_events_ttl": {
                     "pattern": "^\\d+\\s(seconds?|minutes?|hours?|days?)$",
                     "type": "string"
                 },
                 "execution_strategy": {
                     "default": "sequential",
                     "enum": [
-                        "sequential",
-                        "parallel"
+                        "parallel",
+                        "sequential"
                     ],
                     "type": "string"
                 },
                 "gather_facts": {
                     "default": false,
                     "type": "boolean"
                 },
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/util.py` & `ansible_rulebook-1.0.1/ansible_rulebook/util.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/validators.py` & `ansible_rulebook-1.0.1/ansible_rulebook/validators.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook/websocket.py` & `ansible_rulebook-1.0.1/ansible_rulebook/websocket.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook.egg-info/PKG-INFO` & `ansible_rulebook-1.0.1/ansible_rulebook.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ansible-rulebook
-Version: 1.0.0
+Version: 1.0.1
 Summary: Event driven automation for Ansible
 Home-page: https://github.com/ansible/ansible-rulebook
 License: Apache-2.0
 Keywords: ansible_rulebook
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 ================
 ansible-rulebook
 ================
```

### Comparing `ansible_rulebook-1.0.0/ansible_rulebook.egg-info/SOURCES.txt` & `ansible_rulebook-1.0.1/ansible_rulebook.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,19 @@
 docs/multi_events.rst
 docs/rulebooks.rst
 docs/rules.rst
 docs/runner.rst
 docs/sources.rst
 docs/usage.rst
 docs/variables.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
+docs/_build/html/_static/images/Ansible-Mark-RGB_Black.png
+docs/_build/html/_static/images/Ansible-Mark-RGB_White.png
 tests/__init__.py
 tests/conftest.py
 tests/generate_asts.py
 tests/run_examples.sh
 tests/test_ansible_events.py
 tests/test_app.py
 tests/test_ast.py
@@ -174,14 +179,16 @@
 tests/e2e/files/rulebooks/websockets/test_websocket_range.yml
 tests/e2e/utils/awx/ansible.cfg
 tests/e2e/utils/awx/create-cluster.yml
 tests/e2e/utils/awx/install-awx.yml
 tests/e2e/utils/awx/kind-config.yml
 tests/e2e/utils/awx/readme.md
 tests/e2e/utils/awx/requirements.txt
+tests/e2e/utils/awx/artifacts/localhost/awx.yaml
+tests/e2e/utils/awx/artifacts/localhost/kustomization/kustomization.yaml
 tests/e2e/utils/awx/roles/install-awx/defaults/main.yaml
 tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml
 tests/e2e/utils/awx/roles/install-awx/templates/admin-password-secret.yml.j2
 tests/e2e/utils/awx/roles/install-awx/templates/awx.yaml.j2
 tests/e2e/utils/awx/roles/install-awx/templates/kustomization/kustomization.yaml.j2
 tests/event_filter/dashes_to_underscores.py
 tests/event_filter/json_filter.py
@@ -289,14 +296,15 @@
 tests/examples/replays/39_is_defined/07.json
 tests/examples/replays/39_is_defined/08.json
 tests/examples/replays/39_is_defined/09.json
 tests/examples/replays/39_is_defined/generate_data.py
 tests/playbooks/check_facts_playbook.yml
 tests/playbooks/compare_value.yml
 tests/playbooks/fail_and_succeed.yml
+tests/playbooks/hello.yaml
 tests/playbooks/hello.yml
 tests/playbooks/hello_events.yml
 tests/playbooks/hello_world_set_fact.yml
 tests/playbooks/inventory.yml
 tests/playbooks/inventory1.yml
 tests/playbooks/sleeper.yml
 tests/playbooks/validate_args_playbook.yml
```

### Comparing `ansible_rulebook-1.0.0/docs/Makefile` & `ansible_rulebook-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/actions.rst` & `ansible_rulebook-1.0.1/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/collections.rst` & `ansible_rulebook-1.0.1/docs/collections.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/conditions.rst` & `ansible_rulebook-1.0.1/docs/conditions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -250,16 +250,16 @@
                 - event.request.type == "Delete"
                 - event.friend_list.names contains events.m_0.request.friend_name
             action:
               print_event:
 
 | The above example uses the generic source plugin which allows for the event
 | payloads to be defined in the rule book for easy testing.
-| In this example the the first condition matches for the first 2 events
-| this leads to 2 partial matching rules, then the 3 and 4 the event arrive
+| In this example the first condition matches for the first 2 events
+| this leads to 2 partial matching rules, then the 3rd and 4th events arrive
 | with the friend_list payload and they match the 2nd condition. This will lead
 | to the rule being satisfied twice and the print_event will run twice with the
 | correct events.
 
 
 Multiple conditions where **any** one of them has to match
 ----------------------------------------------------------
```

### Comparing `ansible_rulebook-1.0.0/docs/conf.py` & `ansible_rulebook-1.0.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 import ansible_rulebook
 
 # -- General configuration ---------------------------------------------
```

### Comparing `ansible_rulebook-1.0.0/docs/contributing.rst` & `ansible_rulebook-1.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/decision_environment.rst` & `ansible_rulebook-1.0.1/docs/decision_environment.rst`

 * *Files 4% similar despite different names*

```diff
@@ -45,60 +45,54 @@
 
 .. code-block:: yaml
 
     ---
     version: 3
 
     images:
-    base_image:
-        name: 'minimal-decision-environment:latest'
+        base_image:
+            name: 'minimal-decision-environment:latest'
     dependencies:
         python:
             - pywinrm
         system:
             - iputils [platform:rpm]
         galaxy:
             collections:
                 - name: my_namespace.my_awesome_collection
                 - name: community.windows
                 - name: ansible.utils
-                version: 2.10.1
-    options:
-        container_init:
-            cmd: '["/opt/builder/bin/entrypoint","ansible-rulebook", "-r", "my_namespace.my_awesome_collection.my_rulebook", "-i", "/tmp/inventory"]'
+                  version: 2.10.1
 
 This shows an example where you may have your own Collection that contains rulebooks and playbooks but need to bring them together with some other collections
 and some python and system dependencies.
 
 You could also use Builder to add your own rulebooks and playbooks to the decision environment via `additional-build-steps <https://ansible-builder.readthedocs.io/en/latest/definition/#additional-build-steps>`_
 and then making use of Containerfile commands to ADD or COPY to get the files into the environment.
 
 .. code-block:: yaml
 
     ---
     version: 3
 
     images:
-    base_image:
-        name: 'minimal-decision-environment:latest'
+        base_image:
+            name: 'minimal-decision-environment:latest'
     dependencies:
         python:
             - pywinrm
         system:
             - iputils [platform:rpm]
         galaxy:
             collections:
                 - name: community.windows
                 - name: ansible.utils
-                version: 2.10.1
+                  version: 2.10.1
     additional_build_steps:
         prepend_builder:
             - 'RUN mkdir -p /opt/ansible/my_rulebooks'
             - 'COPY my_rulebook.yml /opt/ansible/my_rulebooks'
-    options:
-        container_init:
-            cmd: '["/opt/builder/bin/entrypoint","ansible-rulebook", "-r", "/opt/ansible/my_rulebooks/my_rulebook.yml", "-i", "/tmp/inventory"]'
 
 .. note::
 
     container_init.cmd is an optional override that can be used to override the default command that is run when the container is launched. This is useful if you want to
     run a playbook or rulebook without needing to supply the full command line arguments. It can still be overridden at runtime by passing a command to the container.
```

### Comparing `ansible_rulebook-1.0.0/docs/development_environment.rst` & `ansible_rulebook-1.0.1/docs/development_environment.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/events_and_facts.rst` & `ansible_rulebook-1.0.1/docs/events_and_facts.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/filters.rst` & `ansible_rulebook-1.0.1/docs/filters.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/getting_started.rst` & `ansible_rulebook-1.0.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/host_limit.rst` & `ansible_rulebook-1.0.1/docs/host_limit.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/installation.rst` & `ansible_rulebook-1.0.1/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 These instructions will guide you though installing the ansible-rulebook CLI on your local system.
 Please ensure you have installed all components listed in the **Requirements** section before starting the installation process.
 
 Requirements
 ------------
 
-* Python >= 3.8
+* Python >= 3.9
 * Python 3 pip
 
 * Java development kit >= 17
 
   * Fedora: java-17-openjdk
   * Ubuntu: openjdk-17-jdk
```

### Comparing `ansible_rulebook-1.0.0/docs/introduction.rst` & `ansible_rulebook-1.0.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/make.bat` & `ansible_rulebook-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/multi_events.rst` & `ansible_rulebook-1.0.1/docs/multi_events.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/rulebooks.rst` & `ansible_rulebook-1.0.1/docs/rulebooks.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/rules.rst` & `ansible_rulebook-1.0.1/docs/rules.rst`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
           - name: An automatic remediation rule
             condition: event.outage == true
             action:
               run_playbook:
                 name: remediate_outage.yml
 
           - name: Print event with linux
-            condition: event.target_os == "linux" or
+            condition: event.target_os == "linux"
             action:
               debug:
 
 Example: Multiple actions
 
     .. code-block:: yaml
 
@@ -77,13 +77,13 @@
             condition: event.outage == true
             enabled: false
             action:
               run_playbook:
                 name: remediate_outage.yml
 
           - name: Print event with linux
-            condition: event.target_os == "linux" or
+            condition: event.target_os == "linux"
             action:
               debug:
 
 | In the above example the first rule is disabled by setting enabled to false
 | This can be used when testing to temporarily disable a rule.
```

### Comparing `ansible_rulebook-1.0.0/docs/sources.rst` & `ansible_rulebook-1.0.1/docs/sources.rst`

 * *Files 23% similar despite different names*

```diff
@@ -42,22 +42,64 @@
     Mainly used for development and testing
 
 * range
     Generate events with an increasing index i within a range
     Mainly used for development and testing
 
 
+
 How to Develop a Custom Plugin
 ------------------------------
 You can build your own event source plugin in python. A plugin is a single
-python file. You can start with this example:
+python file but before we get to that lets take a look at some best practices and patterns:
+
+Best Practices and Patterns
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+There are 3 basic patterns that you'll be developing against when considering a new source plugin:
+
+#. Event Bus Plugins
+    These are plugins that listen to a stream of events from a source where the connection
+    is established by the plugin itself. Examples of this are the ``kafka`` and ``mqtt`` plugins.
+
+    This is the most ideal and reliable pattern to follow. Durability and Reliability of the data
+    is the responsibility of the event source and availability of the data can follow the patterns
+    of the event source and its own internal configuration.
+
+#. Scraper Plugins
+    These plugins connect to a source and scrape the data from the source usually after a given amount of time
+    has passed. Examples of this are the ``url_check`` and ``watchdog`` plugins.
+
+    These plugins can be reliable but may require extract logic for handling duplication. It's also possible
+    to miss data if the scraper is not running at the time the data is available.
+
+#. Callback Plugins
+    These plugins provide a callback endpoint that the event source can call when data is available.
+    Examples of this are the ``webhook`` and ``alertmanager`` plugins.
+
+    These plugins are the least reliable as they are dependent on the event source to call the callback
+    endpoint and are highly sensitive to data loss. If the event source is not available or the callback
+    endpoint is not available then there may not be another opportunity to receive the data.
+
+    These can also require other ingress policies and firewall rules to be available and configured properly
+    to operate.
+
+It's strongly recommended to adopt one of the first two patterns and only consider callback plugins in the absence
+of any other solution.
+
+When deciding whether to build a dedicated plugin you may consider configuring the data source to send data to a
+system where a more general plugin exists already. For example, if you have a system that can send data to a kafka
+topic then you can use the ``kafka`` plugin to receive the data. There are many connectors for tying systems to other
+message buses and this is a great way to leverage existing plugins.
 
 Plugin template
 ^^^^^^^^^^^^^^^
 
+Lets take a look at a very basic example that you could use in the form of a template for producing other plugins:
+
 .. code-block:: python
 
   """
   template.py
 
   An ansible-rulebook event source plugin template.
```

### Comparing `ansible_rulebook-1.0.0/docs/usage.rst` & `ansible_rulebook-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/docs/variables.rst` & `ansible_rulebook-1.0.1/docs/variables.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/setup.cfg` & `ansible_rulebook-1.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [metadata]
 name = ansible_rulebook
-version = 1.0.0
+version = 1.0.1
 description = Event driven automation for Ansible
 url = https://github.com/ansible/ansible-rulebook
 license = Apache-2.0
 keywords = ansible_rulebook
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.9
 install_requires = 
 	aiohttp
 	pyparsing >= 3.0
 	jsonschema
 	jinja2
 	dpath >= 2.1.4
 	janus
```

### Comparing `ansible_rulebook-1.0.0/tests/__init__.py` & `ansible_rulebook-1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/01_noop.yml` & `ansible_rulebook-1.0.1/tests/asts/01_noop.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/03_print_event.yml` & `ansible_rulebook-1.0.1/tests/asts/03_print_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/04_set_fact.yml` & `ansible_rulebook-1.0.1/tests/asts/04_set_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/05_post_event.yml` & `ansible_rulebook-1.0.1/tests/asts/05_post_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/06_retract_fact.yml` & `ansible_rulebook-1.0.1/tests/asts/06_retract_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/07_and.yml` & `ansible_rulebook-1.0.1/tests/asts/07_and.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/08_or.yml` & `ansible_rulebook-1.0.1/tests/asts/08_or.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/09_gt.yml` & `ansible_rulebook-1.0.1/tests/asts/09_gt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/10_lt.yml` & `ansible_rulebook-1.0.1/tests/asts/10_lt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/11_le.yml` & `ansible_rulebook-1.0.1/tests/asts/11_le.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/12_ge.yml` & `ansible_rulebook-1.0.1/tests/asts/12_ge.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/13_add.yml` & `ansible_rulebook-1.0.1/tests/asts/13_add.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/14_sub.yml` & `ansible_rulebook-1.0.1/tests/asts/14_sub.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/15_multiple_events_all.yml` & `ansible_rulebook-1.0.1/tests/asts/15_multiple_events_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/16_multiple_events_any.yml` & `ansible_rulebook-1.0.1/tests/asts/16_multiple_events_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/17_multiple_sources_any.yml` & `ansible_rulebook-1.0.1/tests/asts/17_multiple_sources_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/18_multiple_sources_all.yml` & `ansible_rulebook-1.0.1/tests/asts/18_multiple_sources_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/19_is_defined.yml` & `ansible_rulebook-1.0.1/tests/asts/19_is_defined.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/20_is_not_defined.yml` & `ansible_rulebook-1.0.1/tests/asts/20_is_not_defined.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/21_run_playbook.yml` & `ansible_rulebook-1.0.1/tests/asts/21_run_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/23_nested_data.yml` & `ansible_rulebook-1.0.1/tests/asts/23_nested_data.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/24_max_attributes.yml` & `ansible_rulebook-1.0.1/tests/asts/24_max_attributes.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/25_max_attributes_nested.yml` & `ansible_rulebook-1.0.1/tests/asts/25_max_attributes_nested.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/26_print_events.yml` & `ansible_rulebook-1.0.1/tests/asts/26_print_events.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/27_var_root.yml` & `ansible_rulebook-1.0.1/tests/asts/27_var_root.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/28_right_side_condition_template.yml` & `ansible_rulebook-1.0.1/tests/asts/28_right_side_condition_template.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/29_run_module.yml` & `ansible_rulebook-1.0.1/tests/asts/29_run_module.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/30_run_module_missing.yml` & `ansible_rulebook-1.0.1/tests/asts/30_run_module_missing.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/31_run_module_missing_args.yml` & `ansible_rulebook-1.0.1/tests/asts/31_run_module_missing_args.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/32_run_module_fail.yml` & `ansible_rulebook-1.0.1/tests/asts/32_run_module_fail.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/33_run_playbook_retry.yml` & `ansible_rulebook-1.0.1/tests/asts/33_run_playbook_retry.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/34_run_playbook_retries.yml` & `ansible_rulebook-1.0.1/tests/asts/34_run_playbook_retries.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-1.0.1/tests/asts/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/36_multiple_rulesets_both_fired.yml` & `ansible_rulebook-1.0.1/tests/asts/36_multiple_rulesets_both_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/37_hosts_facts.yml` & `ansible_rulebook-1.0.1/tests/asts/37_hosts_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/38_shutdown.yml` & `ansible_rulebook-1.0.1/tests/asts/38_shutdown.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules.yml` & `ansible_rulebook-1.0.1/tests/asts/rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_assignment.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_assignment.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_assignment2.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_assignment2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_multiple_conditions.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions2.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_multiple_conditions2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_multiple_conditions3.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_multiple_conditions3.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_time.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_time.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_timestamp.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_timestamp.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_with_vars.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_with_vars.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/rules_without_assignment.yml` & `ansible_rulebook-1.0.1/tests/asts/rules_without_assignment.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_filters.yml` & `ansible_rulebook-1.0.1/tests/asts/test_filters.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_host_rules.yml` & `ansible_rulebook-1.0.1/tests/asts/test_host_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_rules.yml` & `ansible_rulebook-1.0.1/tests/asts/test_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts.yml` & `ansible_rulebook-1.0.1/tests/asts/test_rules_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts2.yml` & `ansible_rulebook-1.0.1/tests/asts/test_rules_multiple_hosts2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_rules_multiple_hosts3.yml` & `ansible_rulebook-1.0.1/tests/asts/test_rules_multiple_hosts3.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_set_facts.yml` & `ansible_rulebook-1.0.1/tests/asts/test_set_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/asts/test_simple.yml` & `ansible_rulebook-1.0.1/tests/asts/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/cassettes/test_job_template.yaml` & `ansible_rulebook-1.0.1/tests/cassettes/test_job_template.yaml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/cassettes/test_job_template_not_exist.yaml` & `ansible_rulebook-1.0.1/tests/cassettes/test_job_template_not_exist.yaml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/conftest.py` & `ansible_rulebook-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/data/rulebook.yml` & `ansible_rulebook-1.0.1/tests/data/rulebook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/data/test.tar` & `ansible_rulebook-1.0.1/tests/data/test.tar`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/README.md` & `ansible_rulebook-1.0.1/tests/e2e/README.md`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/conftest.py` & `ansible_rulebook-1.0.1/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/extra_vars/operator_variables.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/extra_vars/operator_variables.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/playbooks/run_playbook_test_playbook.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/playbooks/run_playbook_test_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_run_playbook.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_run_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_logical_operators.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_logical_operators.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_membership_operators.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_membership_operators.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_relational_operators.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_relational_operators.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_select_operator.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_select_operator.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_match.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_string_match.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/operators/test_string_search_search.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/operators/test_string_search_search.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_disabled_rules.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/test_disabled_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/test_process_source_end.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/test_process_source_end.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml` & `ansible_rulebook-1.0.1/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/settings.py` & `ansible_rulebook-1.0.1/tests/e2e/settings.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/test_actions.py` & `ansible_rulebook-1.0.1/tests/e2e/test_actions.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/test_operators.py` & `ansible_rulebook-1.0.1/tests/e2e/test_operators.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/test_runtime.py` & `ansible_rulebook-1.0.1/tests/e2e/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/test_variables.py` & `ansible_rulebook-1.0.1/tests/e2e/test_variables.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/test_websocket.py` & `ansible_rulebook-1.0.1/tests/e2e/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/utils/awx/create-cluster.yml` & `ansible_rulebook-1.0.1/tests/e2e/utils/awx/create-cluster.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/utils/awx/install-awx.yml` & `ansible_rulebook-1.0.1/tests/e2e/utils/awx/install-awx.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/utils/awx/readme.md` & `ansible_rulebook-1.0.1/tests/e2e/utils/awx/readme.md`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml` & `ansible_rulebook-1.0.1/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/e2e/utils.py` & `ansible_rulebook-1.0.1/tests/e2e/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/event_filter/dashes_to_underscores.py` & `ansible_rulebook-1.0.1/tests/event_filter/dashes_to_underscores.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/event_filter/json_filter.py` & `ansible_rulebook-1.0.1/tests/event_filter/json_filter.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/event_filter/noop.py` & `ansible_rulebook-1.0.1/tests/event_filter/noop.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/event_filter/test_insert_meta_info.py` & `ansible_rulebook-1.0.1/tests/event_filter/test_insert_meta_info.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/27_var_root.yml` & `ansible_rulebook-1.0.1/tests/examples/27_var_root.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-1.0.1/tests/examples/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/36_multiple_rulesets_both_fired.yml` & `ansible_rulebook-1.0.1/tests/examples/36_multiple_rulesets_both_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/50_negation.yml` & `ansible_rulebook-1.0.1/tests/examples/50_negation.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/51_vars_namespace.yml` & `ansible_rulebook-1.0.1/tests/examples/51_vars_namespace.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/52_once_within.yml` & `ansible_rulebook-1.0.1/tests/examples/52_once_within.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/53_once_within_multiple_hosts.yml` & `ansible_rulebook-1.0.1/tests/examples/53_once_within_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/54_time_window.yml` & `ansible_rulebook-1.0.1/tests/examples/54_time_window.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/55_not_all.yml` & `ansible_rulebook-1.0.1/tests/examples/55_not_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/56_once_after.yml` & `ansible_rulebook-1.0.1/tests/examples/56_once_after.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/57_once_after_multi.yml` & `ansible_rulebook-1.0.1/tests/examples/57_once_after_multi.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/58_string_search.yml` & `ansible_rulebook-1.0.1/tests/examples/58_string_search.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/60_json_filter.yml` & `ansible_rulebook-1.0.1/tests/examples/60_json_filter.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/61_select_1.yml` & `ansible_rulebook-1.0.1/tests/examples/61_select_1.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/62_select_2.yml` & `ansible_rulebook-1.0.1/tests/examples/62_select_2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/63_selectattr_1.yml` & `ansible_rulebook-1.0.1/tests/examples/63_selectattr_1.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/64_selectattr_2.yml` & `ansible_rulebook-1.0.1/tests/examples/64_selectattr_2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/66_sleepy_playbook.yml` & `ansible_rulebook-1.0.1/tests/examples/66_sleepy_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/67_shutdown_now.yml` & `ansible_rulebook-1.0.1/tests/examples/67_shutdown_now.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/69_enhanced_debug.yml` & `ansible_rulebook-1.0.1/tests/examples/69_enhanced_debug.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/70_null.yml` & `ansible_rulebook-1.0.1/tests/examples/70_null.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/72_set_fact_with_type.yml` & `ansible_rulebook-1.0.1/tests/examples/72_set_fact_with_type.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/73_mix_and_match_list.yml` & `ansible_rulebook-1.0.1/tests/examples/73_mix_and_match_list.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/75_all_conditions.yml` & `ansible_rulebook-1.0.1/tests/examples/75_all_conditions.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/76_all_conditions.yml` & `ansible_rulebook-1.0.1/tests/examples/76_all_conditions.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/78_complete_retract_fact.yml` & `ansible_rulebook-1.0.1/tests/examples/78_complete_retract_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/replays/23_nested_data/generate_data.py` & `ansible_rulebook-1.0.1/tests/examples/replays/23_nested_data/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/00.json` & `ansible_rulebook-1.0.1/tests/examples/replays/24_max_attributes/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/replays/24_max_attributes/generate_data.py` & `ansible_rulebook-1.0.1/tests/examples/replays/24_max_attributes/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/00.json` & `ansible_rulebook-1.0.1/tests/examples/replays/25_max_attributes_nested/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/replays/25_max_attributes_nested/generate_data.py` & `ansible_rulebook-1.0.1/tests/examples/replays/25_max_attributes_nested/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/examples/replays/39_is_defined/generate_data.py` & `ansible_rulebook-1.0.1/tests/examples/replays/39_is_defined/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/generate_asts.py` & `ansible_rulebook-1.0.1/tests/generate_asts.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/playbooks/check_facts_playbook.yml` & `ansible_rulebook-1.0.1/tests/playbooks/check_facts_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/playbooks/fail_and_succeed.yml` & `ansible_rulebook-1.0.1/tests/playbooks/fail_and_succeed.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/playbooks/validate_args_playbook.yml` & `ansible_rulebook-1.0.1/tests/playbooks/validate_args_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/rules.yml` & `ansible_rulebook-1.0.1/tests/rules/rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/rules_with_time.yml` & `ansible_rulebook-1.0.1/tests/rules/rules_with_time.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/rules_with_timestamp.yml` & `ansible_rulebook-1.0.1/tests/rules/rules_with_timestamp.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_filters.yml` & `ansible_rulebook-1.0.1/tests/rules/test_filters.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_host_rules.yml` & `ansible_rulebook-1.0.1/tests/rules/test_host_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_kafka.yml` & `ansible_rulebook-1.0.1/tests/rules/test_kafka.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_rules.yml` & `ansible_rulebook-1.0.1/tests/rules/test_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_rules_multiple_hosts.yml` & `ansible_rulebook-1.0.1/tests/rules/test_rules_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_set_facts.yml` & `ansible_rulebook-1.0.1/tests/rules/test_set_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_simple.yml` & `ansible_rulebook-1.0.1/tests/rules/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/test_states.yml` & `ansible_rulebook-1.0.1/tests/rules/test_states.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/rules/webserver_down.yml` & `ansible_rulebook-1.0.1/tests/rules/webserver_down.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/file.py` & `ansible_rulebook-1.0.1/tests/sources/file.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/generic.py` & `ansible_rulebook-1.0.1/tests/sources/generic.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/hosts.py` & `ansible_rulebook-1.0.1/tests/sources/hosts.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/infrange.py` & `ansible_rulebook-1.0.1/tests/sources/infrange.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/log_scraper.py` & `ansible_rulebook-1.0.1/tests/sources/log_scraper.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/nested.py` & `ansible_rulebook-1.0.1/tests/sources/nested.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/ping.py` & `ansible_rulebook-1.0.1/tests/sources/ping.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/process_check.py` & `ansible_rulebook-1.0.1/tests/sources/process_check.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/range.py` & `ansible_rulebook-1.0.1/tests/sources/range.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/range2.py` & `ansible_rulebook-1.0.1/tests/sources/range2.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/replay.py` & `ansible_rulebook-1.0.1/tests/sources/replay.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/template.py` & `ansible_rulebook-1.0.1/tests/sources/template.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/tick.py` & `ansible_rulebook-1.0.1/tests/sources/tick.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/timestamp.py` & `ansible_rulebook-1.0.1/tests/sources/timestamp.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/sources/url_check.py` & `ansible_rulebook-1.0.1/tests/sources/url_check.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_ansible_events.py` & `ansible_rulebook-1.0.1/tests/test_ansible_events.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_app.py` & `ansible_rulebook-1.0.1/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
                 "ansible_rulebook.app.request_workload"
             ) as mock_request_workload:
                 mock_request_workload.return_value = StartupArgs(
                     rulesets=rulesets,
                     controller_url="abc",
                     controller_token="token",
                     controller_ssl_verify="no",
+                    check_controller_connection=True,
                 )
                 with patch(
                     "ansible_rulebook.app.job_template_runner.get_config",
                     return_value=dict(version="4.4.1"),
                 ):
                     await run(cmdline_args)
                     assert mock_start_source.call_count == 1
```

### Comparing `ansible_rulebook-1.0.0/tests/test_ast.py` & `ansible_rulebook-1.0.1/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_collection.py` & `ansible_rulebook-1.0.1/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_controller.py` & `ansible_rulebook-1.0.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_engine.py` & `ansible_rulebook-1.0.1/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_examples.py` & `ansible_rulebook-1.0.1/tests/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -2112,14 +2112,15 @@
             assert action["url"] == job_url
             assert action["action"] == "run_job_template"
 
 
 JOB_TEMPLATE_ERRORS = [
     ("api error", ControllerApiException("api error")),
     ("jt does not exist", JobTemplateNotFoundException("jt does not exist")),
+    ("Kaboom", RuntimeError("Kaboom")),
 ]
 
 
 @pytest.mark.parametrize("err_msg,err", JOB_TEMPLATE_ERRORS)
 @pytest.mark.asyncio
 async def test_46_job_template_exception(err_msg, err):
     ruleset_queues, event_log = load_rulebook("examples/46_job_template.yml")
@@ -2140,20 +2141,20 @@
 
             while not event_log.empty():
                 event = event_log.get_nowait()
                 if event["type"] == "Action":
                     action = event
 
             assert action["action"] == "run_job_template"
-            assert action["reason"] == {"error": err_msg}
+            assert action["message"] == err_msg
             required_keys = {
                 "action",
                 "action_uuid",
                 "activation_id",
-                "reason",
+                "message",
                 "rule_run_at",
                 "run_at",
                 "rule",
                 "ruleset",
                 "rule_uuid",
                 "ruleset_uuid",
                 "status",
```

### Comparing `ansible_rulebook-1.0.0/tests/test_rules.py` & `ansible_rulebook-1.0.1/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_simple.yml` & `ansible_rulebook-1.0.1/tests/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/test_websocket.py` & `ansible_rulebook-1.0.1/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/unit/test_cli.py` & `ansible_rulebook-1.0.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.0/tests/unit/test_util.py` & `ansible_rulebook-1.0.1/tests/unit/test_util.py`

 * *Files identical despite different names*

