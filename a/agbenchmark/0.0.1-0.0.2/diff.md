# Comparing `tmp/agbenchmark-0.0.1.tar.gz` & `tmp/agbenchmark-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agbenchmark-0.0.1.tar", max compression
+gzip compressed data, was "agbenchmark-0.0.2.tar", max compression
```

## Comparing `agbenchmark-0.0.1.tar` & `agbenchmark-0.0.2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0     1069 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/LICENSE
--rw-r--r--   0        0        0     1753 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/README.md
--rw-r--r--   0        0        0     2780 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/README.md
--rw-r--r--   0        0        0     2336 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/ReportManager.py
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/__init__.py
--rw-r--r--   0        0        0     2530 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/agent_interface.py
--rw-r--r--   0        0        0     5140 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenge.py
--rw-r--r--   0        0        0     2581 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/README.md
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_in/__init__.py
--rw-r--r--   0        0        0      325 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_in/code.py
--rw-r--r--   0        0        0      893 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_in/test.py
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_out/__init__.py
--rw-r--r--   0        0        0      312 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_out/code.py
--rw-r--r--   0        0        0      893 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_out/test.py
--rw-r--r--   0        0        0      645 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/data.json
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_in/__init__.py
--rw-r--r--   0        0        0      325 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_in/code.py
--rw-r--r--   0        0        0      893 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_in/test.py
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_out/__init__.py
--rw-r--r--   0        0        0      312 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_out/code.py
--rw-r--r--   0        0        0      893 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_out/test.py
--rw-r--r--   0        0        0      612 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/data.json
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d3_two_sum/artifacts_out/__init__.py
--rw-r--r--   0        0        0      312 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d3_two_sum/artifacts_out/code.py
--rw-r--r--   0        0        0      893 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d3_two_sum/custom_python/test.py
--rw-r--r--   0        0        0      869 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d3_two_sum/data.json
--rw-r--r--   0        0        0     1171 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d4_web_server/custom_python/api_tests.py
--rw-r--r--   0        0        0      757 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d4_web_server/data.json
--rw-r--r--   0        0        0        0 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d5_three_sum/artifacts_out/__init__.py
--rw-r--r--   0        0        0      809 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d5_three_sum/artifacts_out/code.py
--rw-r--r--   0        0        0      921 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d5_three_sum/custom_python/test.py
--rw-r--r--   0        0        0      933 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/code/d5_three_sum/data.json
--rw-r--r--   0        0        0     2076 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/define_task_types.py
--rw-r--r--   0        0        0       13 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/interface/read_file/artifacts_in/file_to_check.txt
--rw-r--r--   0        0        0       27 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/interface/read_file/artifacts_out/file_to_check.txt
--rw-r--r--   0        0        0      517 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/interface/read_file/data.json
--rw-r--r--   0        0        0       38 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/interface/search/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      547 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/interface/search/data.json
--rw-r--r--   0        0        0       11 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/interface/write_file/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      519 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/interface/write_file/data.json
--rw-r--r--   0        0        0       60 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0       33 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0       33 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0       33 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0       63 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0        5 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/artifacts_out/result.txt
--rw-r--r--   0        0        0      598 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/data.json
--rw-r--r--   0        0        0       62 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0       62 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0       62 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0       62 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0       64 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0       20 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/artifacts_out/result.txt
--rw-r--r--   0        0        0      667 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/data.json
--rw-r--r--   0        0        0     1066 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0     1066 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0     1066 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0     1066 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0     1068 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0       20 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_out/result.txt
--rw-r--r--   0        0        0      774 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/data.json
--rw-r--r--   0        0        0     1127 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0     1124 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0     1117 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0     1126 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0     1072 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0      226 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_out/result.txt
--rw-r--r--   0        0        0     1234 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/data.json
--rw-r--r--   0        0        0        6 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r1_book_price/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      555 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r1_book_price/data.json
--rw-r--r--   0        0        0       16 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r2.1_specific/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      510 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r2.1_specific/data.json
--rw-r--r--   0        0        0       16 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r2.2_formatting/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      678 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r2.2_formatting/data.json
--rw-r--r--   0        0        0       16 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r2_tesla_revenue/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      473 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r2_tesla_revenue/data.json
--rw-r--r--   0        0        0      220 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r3/artifacts_out/random_file.txt
--rw-r--r--   0        0        0     1079 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r3/data.json
--rw-r--r--   0        0        0     2317 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/challenges/test_all.py
--rw-r--r--   0        0        0       61 2023-07-23 19:56:53.166825 agbenchmark-0.0.1/agbenchmark/config.json
--rw-r--r--   0        0        0     9449 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/conftest.py
--rw-r--r--   0        0        0      466 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/metrics.py
--rw-r--r--   0        0        0     1841 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/regression_tests.json
--rw-r--r--   0        0        0     2706 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/internal_info.json
--rw-r--r--   0        0        0      648 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/1.1_TestWriteFile.json
--rw-r--r--   0        0        0     1086 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/10.1_TestRememberMultipleWithNoise.json
--rw-r--r--   0        0        0     1200 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/10_TestRememberMultipleWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.1_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.2_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.3_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1377 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.4_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1446 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.5_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1059 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12.1_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0     1060 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12.2_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0     1066 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12.3_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0      980 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0      639 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/1_TestWriteFIle.json
--rw-r--r--   0        0        0      644 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/2.1_TestReadFile.json
--rw-r--r--   0        0        0      636 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/2_TestReadFile.json
--rw-r--r--   0        0        0      638 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/3.1_TestSearch.json
--rw-r--r--   0        0        0      630 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/3_TestSearch.json
--rw-r--r--   0        0        0      634 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/4.1_TestBasicRetrieval.json
--rw-r--r--   0        0        0      641 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/4_TestBasicRetrieval.json
--rw-r--r--   0        0        0      814 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/5.1_TestRetrieval2.0.json
--rw-r--r--   0        0        0      753 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/5_TestRetrieval2.0.json
--rw-r--r--   0        0        0      841 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.1_TestRetrieval2.1.json
--rw-r--r--   0        0        0      836 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.2_TestRetrieval2.1.json
--rw-r--r--   0        0        0      836 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.3_TestRetrieval2.1.json
--rw-r--r--   0        0        0      908 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.4_TestRetrieval2.1.json
--rw-r--r--   0        0        0      823 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6_TestRetrieval2.1.json
--rw-r--r--   0        0        0     1073 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/7.1_TestRetrieval2.2.json
--rw-r--r--   0        0        0      893 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/7_TestRetrieval2.2.json
--rw-r--r--   0        0        0      908 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/8.1_TestBasicMemory.json
--rw-r--r--   0        0        0     1041 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/8_TestBasicMemory.json
--rw-r--r--   0        0        0      982 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/9.1_TestRememberMultipleIds.json
--rw-r--r--   0        0        0     1110 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/reports/mini-agi/9_TestRememberMultipleIds.json
--rw-r--r--   0        0        0     3843 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/start_benchmark.py
--rw-r--r--   0        0        0     6977 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/agbenchmark/utils.py
--rw-r--r--   0        0        0     1646 2023-07-23 19:56:53.170825 agbenchmark-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 agbenchmark-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1753 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/README.md
+-rw-r--r--   0        0        0     2780 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/README.md
+-rw-r--r--   0        0        0     2336 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/ReportManager.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/__init__.py
+-rw-r--r--   0        0        0     2530 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/agent_interface.py
+-rw-r--r--   0        0        0     5140 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenge.py
+-rw-r--r--   0        0        0     2581 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_in/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_in/code.py
+-rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_in/test.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_out/__init__.py
+-rw-r--r--   0        0        0      312 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_out/code.py
+-rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_out/test.py
+-rw-r--r--   0        0        0      645 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/data.json
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_in/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_in/code.py
+-rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_in/test.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_out/__init__.py
+-rw-r--r--   0        0        0      312 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_out/code.py
+-rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_out/test.py
+-rw-r--r--   0        0        0      612 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/data.json
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/artifacts_out/__init__.py
+-rw-r--r--   0        0        0      312 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/artifacts_out/code.py
+-rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/custom_python/test.py
+-rw-r--r--   0        0        0      869 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/data.json
+-rw-r--r--   0        0        0     1171 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d4_web_server/custom_python/api_tests.py
+-rw-r--r--   0        0        0      757 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d4_web_server/data.json
+-rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/artifacts_out/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/artifacts_out/code.py
+-rw-r--r--   0        0        0      921 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/custom_python/test.py
+-rw-r--r--   0        0        0      933 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/data.json
+-rw-r--r--   0        0        0     2076 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/define_task_types.py
+-rw-r--r--   0        0        0       13 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/read_file/artifacts_in/file_to_check.txt
+-rw-r--r--   0        0        0       27 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/read_file/artifacts_out/file_to_check.txt
+-rw-r--r--   0        0        0      517 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/read_file/data.json
+-rw-r--r--   0        0        0       38 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/search/artifacts_out/random_file.txt
+-rw-r--r--   0        0        0      547 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/search/data.json
+-rw-r--r--   0        0        0       11 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/write_file/artifacts_out/random_file.txt
+-rw-r--r--   0        0        0      519 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/write_file/data.json
+-rw-r--r--   0        0        0       60 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_1.txt
+-rw-r--r--   0        0        0       33 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_2.txt
+-rw-r--r--   0        0        0       33 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_3.txt
+-rw-r--r--   0        0        0       33 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_4.txt
+-rw-r--r--   0        0        0       63 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_5.txt
+-rw-r--r--   0        0        0        5 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_out/result.txt
+-rw-r--r--   0        0        0      598 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/data.json
+-rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_1.txt
+-rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_2.txt
+-rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_3.txt
+-rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_4.txt
+-rw-r--r--   0        0        0       64 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_5.txt
+-rw-r--r--   0        0        0       20 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_out/result.txt
+-rw-r--r--   0        0        0      667 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/data.json
+-rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_1.txt
+-rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_2.txt
+-rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_3.txt
+-rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_4.txt
+-rw-r--r--   0        0        0     1068 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_5.txt
+-rw-r--r--   0        0        0       20 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_out/result.txt
+-rw-r--r--   0        0        0      774 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/data.json
+-rw-r--r--   0        0        0     1127 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_1.txt
+-rw-r--r--   0        0        0     1124 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_2.txt
+-rw-r--r--   0        0        0     1117 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_3.txt
+-rw-r--r--   0        0        0     1126 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_4.txt
+-rw-r--r--   0        0        0     1072 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_5.txt
+-rw-r--r--   0        0        0      226 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_out/result.txt
+-rw-r--r--   0        0        0     1234 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/data.json
+-rw-r--r--   0        0        0        6 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r1_book_price/artifacts_out/random_file.txt
+-rw-r--r--   0        0        0      555 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r1_book_price/data.json
+-rw-r--r--   0        0        0       16 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.1_specific/artifacts_out/random_file.txt
+-rw-r--r--   0        0        0      510 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.1_specific/data.json
+-rw-r--r--   0        0        0       16 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.2_formatting/artifacts_out/random_file.txt
+-rw-r--r--   0        0        0      678 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.2_formatting/data.json
+-rw-r--r--   0        0        0       16 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2_tesla_revenue/artifacts_out/random_file.txt
+-rw-r--r--   0        0        0      473 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2_tesla_revenue/data.json
+-rw-r--r--   0        0        0      220 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r3/artifacts_out/random_file.txt
+-rw-r--r--   0        0        0     1079 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r3/data.json
+-rw-r--r--   0        0        0     2317 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/test_all.py
+-rw-r--r--   0        0        0       61 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/config.json
+-rw-r--r--   0        0        0     9449 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/conftest.py
+-rw-r--r--   0        0        0      466 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/metrics.py
+-rw-r--r--   0        0        0     1841 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/regression_tests.json
+-rw-r--r--   0        0        0     2706 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/internal_info.json
+-rw-r--r--   0        0        0      648 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/1.1_TestWriteFile.json
+-rw-r--r--   0        0        0     1086 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/10.1_TestRememberMultipleWithNoise.json
+-rw-r--r--   0        0        0     1200 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/10_TestRememberMultipleWithNoise.json
+-rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.1_TestRememberMultiplePhrasesWithNoise.json
+-rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.2_TestRememberMultiplePhrasesWithNoise.json
+-rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.3_TestRememberMultiplePhrasesWithNoise.json
+-rw-r--r--   0        0        0     1377 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.4_TestRememberMultiplePhrasesWithNoise.json
+-rw-r--r--   0        0        0     1446 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.5_TestRememberMultiplePhrasesWithNoise.json
+-rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11_TestRememberMultiplePhrasesWithNoise.json
+-rw-r--r--   0        0        0     1059 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.1_TestDebugSimpleTypoWithGuidance.json
+-rw-r--r--   0        0        0     1060 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.2_TestDebugSimpleTypoWithGuidance.json
+-rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.3_TestDebugSimpleTypoWithGuidance.json
+-rw-r--r--   0        0        0      980 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12_TestDebugSimpleTypoWithGuidance.json
+-rw-r--r--   0        0        0      639 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/1_TestWriteFIle.json
+-rw-r--r--   0        0        0      644 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/2.1_TestReadFile.json
+-rw-r--r--   0        0        0      636 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/2_TestReadFile.json
+-rw-r--r--   0        0        0      638 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/3.1_TestSearch.json
+-rw-r--r--   0        0        0      630 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/3_TestSearch.json
+-rw-r--r--   0        0        0      634 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/4.1_TestBasicRetrieval.json
+-rw-r--r--   0        0        0      641 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/4_TestBasicRetrieval.json
+-rw-r--r--   0        0        0      814 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/5.1_TestRetrieval2.0.json
+-rw-r--r--   0        0        0      753 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/5_TestRetrieval2.0.json
+-rw-r--r--   0        0        0      841 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.1_TestRetrieval2.1.json
+-rw-r--r--   0        0        0      836 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.2_TestRetrieval2.1.json
+-rw-r--r--   0        0        0      836 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.3_TestRetrieval2.1.json
+-rw-r--r--   0        0        0      908 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.4_TestRetrieval2.1.json
+-rw-r--r--   0        0        0      823 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6_TestRetrieval2.1.json
+-rw-r--r--   0        0        0     1073 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/7.1_TestRetrieval2.2.json
+-rw-r--r--   0        0        0      893 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/7_TestRetrieval2.2.json
+-rw-r--r--   0        0        0      908 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/8.1_TestBasicMemory.json
+-rw-r--r--   0        0        0     1041 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/8_TestBasicMemory.json
+-rw-r--r--   0        0        0      982 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/9.1_TestRememberMultipleIds.json
+-rw-r--r--   0        0        0     1110 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/9_TestRememberMultipleIds.json
+-rw-r--r--   0        0        0     3843 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/start_benchmark.py
+-rw-r--r--   0        0        0     6977 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/utils.py
+-rw-r--r--   0        0        0     1646 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 agbenchmark-0.0.2/PKG-INFO
```

### Comparing `agbenchmark-0.0.1/LICENSE` & `agbenchmark-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/README.md` & `agbenchmark-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/README.md` & `agbenchmark-0.0.2/agbenchmark/README.md`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/ReportManager.py` & `agbenchmark-0.0.2/agbenchmark/ReportManager.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/agent_interface.py` & `agbenchmark-0.0.2/agbenchmark/agent_interface.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenge.py` & `agbenchmark-0.0.2/agbenchmark/challenge.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/README.md` & `agbenchmark-0.0.2/agbenchmark/challenges/README.md`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_in/test.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_in/test.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/artifacts_out/test.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_out/test.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d1_debug/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_in/test.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_in/test.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/artifacts_out/test.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_out/test.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d2_vague/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d3_two_sum/custom_python/test.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/custom_python/test.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d3_two_sum/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d4_web_server/custom_python/api_tests.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d4_web_server/custom_python/api_tests.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d4_web_server/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d4_web_server/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d5_three_sum/artifacts_out/code.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/artifacts_out/code.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d5_three_sum/custom_python/test.py` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/custom_python/test.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/code/d5_three_sum/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/define_task_types.py` & `agbenchmark-0.0.2/agbenchmark/challenges/define_task_types.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/interface/read_file/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/interface/read_file/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/interface/search/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/interface/search/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/interface/write_file/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/interface/write_file/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m1_id/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m2_multiple/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_1.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_1.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_2.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_2.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_3.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_3.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_4.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_4.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_5.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_5.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m3_noise/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_1.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_1.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_2.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_2.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_3.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_3.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_4.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_4.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_5.txt` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_5.txt`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/memory/m4_phrases/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r1_book_price/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r1_book_price/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r2.2_formatting/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.2_formatting/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/retrieval/r3/data.json` & `agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r3/data.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/challenges/test_all.py` & `agbenchmark-0.0.2/agbenchmark/challenges/test_all.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/conftest.py` & `agbenchmark-0.0.2/agbenchmark/conftest.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/regression_tests.json` & `agbenchmark-0.0.2/agbenchmark/regression_tests.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/internal_info.json` & `agbenchmark-0.0.2/agbenchmark/reports/internal_info.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/1.1_TestWriteFile.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/1.1_TestWriteFile.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/10.1_TestRememberMultipleWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/10.1_TestRememberMultipleWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/10_TestRememberMultipleWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/10_TestRememberMultipleWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.1_TestRememberMultiplePhrasesWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.1_TestRememberMultiplePhrasesWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.2_TestRememberMultiplePhrasesWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.2_TestRememberMultiplePhrasesWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.3_TestRememberMultiplePhrasesWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.3_TestRememberMultiplePhrasesWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.4_TestRememberMultiplePhrasesWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.4_TestRememberMultiplePhrasesWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11.5_TestRememberMultiplePhrasesWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.5_TestRememberMultiplePhrasesWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/11_TestRememberMultiplePhrasesWithNoise.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11_TestRememberMultiplePhrasesWithNoise.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12.1_TestDebugSimpleTypoWithGuidance.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.1_TestDebugSimpleTypoWithGuidance.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12.2_TestDebugSimpleTypoWithGuidance.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.2_TestDebugSimpleTypoWithGuidance.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12.3_TestDebugSimpleTypoWithGuidance.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.3_TestDebugSimpleTypoWithGuidance.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/12_TestDebugSimpleTypoWithGuidance.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12_TestDebugSimpleTypoWithGuidance.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/1_TestWriteFIle.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/1_TestWriteFIle.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/2.1_TestReadFile.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/2.1_TestReadFile.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/2_TestReadFile.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/2_TestReadFile.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/3.1_TestSearch.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/3.1_TestSearch.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/3_TestSearch.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/3_TestSearch.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/4.1_TestBasicRetrieval.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/4.1_TestBasicRetrieval.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/4_TestBasicRetrieval.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/4_TestBasicRetrieval.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/5.1_TestRetrieval2.0.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/5.1_TestRetrieval2.0.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/5_TestRetrieval2.0.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/5_TestRetrieval2.0.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.1_TestRetrieval2.1.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.1_TestRetrieval2.1.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.2_TestRetrieval2.1.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.2_TestRetrieval2.1.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.3_TestRetrieval2.1.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.3_TestRetrieval2.1.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6.4_TestRetrieval2.1.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.4_TestRetrieval2.1.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/6_TestRetrieval2.1.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6_TestRetrieval2.1.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/7.1_TestRetrieval2.2.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/7.1_TestRetrieval2.2.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/7_TestRetrieval2.2.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/7_TestRetrieval2.2.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/8.1_TestBasicMemory.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/8.1_TestBasicMemory.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/8_TestBasicMemory.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/8_TestBasicMemory.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/9.1_TestRememberMultipleIds.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/9.1_TestRememberMultipleIds.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/reports/mini-agi/9_TestRememberMultipleIds.json` & `agbenchmark-0.0.2/agbenchmark/reports/mini-agi/9_TestRememberMultipleIds.json`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/start_benchmark.py` & `agbenchmark-0.0.2/agbenchmark/start_benchmark.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/agbenchmark/utils.py` & `agbenchmark-0.0.2/agbenchmark/utils.py`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.1/pyproject.toml` & `agbenchmark-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agbenchmark"
-version = "0.0.1"
+version = "0.0.2"
 description = "Benchmarking the performance of agents far and wide, regardless of how they are set up and how they work"
 authors = ["Silen Naihin <silen.naihin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "agbenchmark"}]
 
 [tool.poetry.dependencies]
```

### Comparing `agbenchmark-0.0.1/PKG-INFO` & `agbenchmark-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agbenchmark
-Version: 0.0.1
+Version: 0.0.2
 Summary: Benchmarking the performance of agents far and wide, regardless of how they are set up and how they work
 License: MIT
 Author: Silen Naihin
 Author-email: silen.naihin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

