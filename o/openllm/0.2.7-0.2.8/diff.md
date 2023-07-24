# Comparing `tmp/openllm-0.2.7.tar.gz` & `tmp/openllm-0.2.8.tar.gz`

## Comparing `openllm-0.2.7.tar` & `openllm-0.2.8.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.7/.gitattributes
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 openllm-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.7/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0    13282 2020-02-02 00:00:00.000000 openllm-0.2.7/CHANGELOG.md
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.7/CITATION.cff
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.7/DEVELOPMENT.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.7/nightly-requirements-gpu.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.7/nightly-requirements.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.7/package.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.7/pyoxidizer.bzl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.7/taplo.toml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/__about__.py
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/__main__.py
--rw-r--r--   0        0        0    90013 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_generation.py
--rw-r--r--   0        0        0    71077 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_llm.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_prompt.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_quantisation.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_schema.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_service.py
--rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_strategies.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/_types.py
--rw-r--r--   0        0        0   101935 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/cli.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/client.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/py.typed
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/testing.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/bundle/oci/Dockerfile-builder
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/bundle/oci/Dockerfile-vllm
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/bundle/oci/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/auto/modeling_vllm_auto.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/baichuan/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/baichuan/configuration_baichuan.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/baichuan/modeling_baichuan.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/gpt_neox/configuration_gpt_neox.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/gpt_neox/modeling_gpt_neox.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/llama/configuration_llama.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/llama/modeling_llama.py
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/llama/modeling_vllm_llama.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/mpt/__init__.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/mpt/configuration_mpt.py
--rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/mpt/modeling_mpt.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/playground/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/playground/_meta.yml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/playground/features.py
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/playground/opt_tuned.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/serialisation/ggml.py
--rw-r--r--   0        0        0    16004 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/serialisation/transformers.py
--rw-r--r--   0        0        0    17096 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    20013 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dummy_pt_and_triton_objects.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/dummy_vllm_objects.py
--rw-r--r--   0        0        0    20528 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm/utils/representation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.7/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/client_test.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/configuration_test.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/llm_test.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models_test.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/package_test.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/strategies_test.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/__init__.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/conftest.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/flan_t5_test.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/opt_test.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.7/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.7/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.7/LICENSE.md
--rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.7/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 openllm-0.2.7/hatch.toml
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 openllm-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    30097 2020-02-02 00:00:00.000000 openllm-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 openllm-0.2.8/.gitattributes
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 openllm-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.2.8/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 openllm-0.2.8/CHANGELOG.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 openllm-0.2.8/CITATION.cff
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 openllm-0.2.8/DEVELOPMENT.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 openllm-0.2.8/nightly-requirements-gpu.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 openllm-0.2.8/nightly-requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.2.8/package.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 openllm-0.2.8/pyoxidizer.bzl
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.2.8/taplo.toml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/__about__.py
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/__main__.py
+-rw-r--r--   0        0        0    90120 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_generation.py
+-rw-r--r--   0        0        0    69548 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_llm.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_schema.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_service.py
+-rw-r--r--   0        0        0    19111 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/_types.py
+-rw-r--r--   0        0        0    89468 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/cli.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/client.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/py.typed
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/testing.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/oci/Dockerfile-builder
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/oci/Dockerfile-vllm
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/bundle/oci/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/auto/modeling_vllm_auto.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/baichuan/__init__.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/baichuan/configuration_baichuan.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/baichuan/modeling_baichuan.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/gpt_neox/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/gpt_neox/modeling_gpt_neox.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/configuration_llama.py
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/modeling_llama.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/llama/modeling_vllm_llama.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/mpt/__init__.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/mpt/configuration_mpt.py
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/mpt/modeling_mpt.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/opt/modeling_vllm_opt.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/_meta.yml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/playground/opt_tuned.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/ggml.py
+-rw-r--r--   0        0        0    15916 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/serialisation/transformers.py
+-rw-r--r--   0        0        0    16946 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_and_triton_objects.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/dummy_vllm_objects.py
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm/utils/representation.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.2.8/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/client_test.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/configuration_test.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/conftest.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models_test.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/package_test.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/strategies_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__init__.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/conftest.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/flan_t5_test.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/opt_test.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[container].json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[local].json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 openllm-0.2.8/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.2.8/LICENSE.md
+-rw-r--r--   0        0        0    24680 2020-02-02 00:00:00.000000 openllm-0.2.8/README.md
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 openllm-0.2.8/hatch.toml
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 openllm-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    30106 2020-02-02 00:00:00.000000 openllm-0.2.8/PKG-INFO
```

### Comparing `openllm-0.2.7/.pre-commit-config.yaml` & `openllm-0.2.8/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -16,22 +16,18 @@
   autoupdate_schedule: weekly
   skip: [check-models-table-update, check-models-table-update, changelog-dry-run, pyright, mypy]
   autofix_commit_msg: "ci: auto fixes from pre-commit.ci\n\nFor more information, see https://pre-commit.ci"
   autoupdate_commit_msg: 'ci: pre-commit autoupdate [pre-commit.ci]'
 exclude: '.*\.(css|js|svg)$'
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.0.278'
+    rev: 'v0.0.280'
     hooks:
       - id: ruff
         args: [--exit-non-zero-on-fix, --show-fixes]
-  - repo: https://github.com/psf/black
-    rev: 23.7.0
-    hooks:
-      - id: black-jupyter
   - repo: https://github.com/econchick/interrogate
     rev: 1.5.0
     hooks:
       - id: interrogate
         types: [python]
         exclude: ^(docs|tools|tests)
         args: [--config=pyproject.toml]
@@ -46,18 +42,17 @@
         verbose: true
         exclude: |
           (?x)^(
               examples/.*|
               tools/.*|
               tests/.*|
               src/openllm/playground/.*|
-              src/openllm/models/.*|
               .github/.*
           )$
-        additional_dependencies: ["mypy==1.4.1", "types-tabulate", "types-Deprecated", "types-PyYAML", "types-decorator", "types-protobuf", "types-python-dateutil", "types-requests", "types-setuptools", "types-six", "types-ujson", "pandas-stubs", "types-Pillow", "types-Pygments", "types-appdirs", "types-colorama", "types-google-cloud-ndb", "types-jsonschema", "types-psutil", "types-pywin32", "types-tqdm", "types-openpyxl"]
+        additional_dependencies: ["mypy==1.4.1"]
       - id: pyright
         name: pyright
         entry: ./tools/pyright
         types: [python]
         language: node
         pass_filenames: false
         additional_dependencies: ['pyright@1.1.317']
```

### Comparing `openllm-0.2.7/ADDING_NEW_MODEL.md` & `openllm-0.2.8/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/CHANGELOG.md` & `openllm-0.2.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,35 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.2.8](https://github.com/bentoml/openllm/tree/v0.2.8)
+
+### Features
+
+- APIs for LLMService are now provisional based on the capabilities of the LLM.
+
+  The following APIs are considered provisional:
+
+  - `/v1/embeddings`: This will be available if the LLM supports embeddings (i.e: ``LLM.embeddings`` is implemented. Example model are ``llama``)
+  - `/hf/agent`: This will be available if LLM supports running HF agents (i.e: ``LLM.generate_one`` is implemented. Example model are ``starcoder``, ``falcon``.)
+  - `POST /v1/adapters` and `GET /v1/adapters`: This will be available if the server is running with LoRA weights
+
+  ``openllm.LLMRunner`` now include three additional boolean:
+  - `runner.supports_embeddings`: Whether this runner supports embeddings
+  - `runner.supports_hf_agent`: Whether this runner support HF agents
+  - `runner.has_adapters`: Whether this runner is loaded with LoRA adapters.
+
+  Optimized ``openllm.models``'s bytecode performance
+  [#133](https://github.com/bentoml/openllm/issues/133)
+
+
 ## [0.2.7](https://github.com/bentoml/openllm/tree/v0.2.7)
 No significant changes.
 
 
 ## [0.2.6](https://github.com/bentoml/openllm/tree/v0.2.6)
 
 ### Backwards-incompatible Changes
```

### Comparing `openllm-0.2.7/CITATION.cff` & `openllm-0.2.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/DEVELOPMENT.md` & `openllm-0.2.8/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/nightly-requirements.txt` & `openllm-0.2.8/nightly-requirements.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/package.json` & `openllm-0.2.8/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.2.8'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.2.7",
+    "version": "0.2.8",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.2.7/pyoxidizer.bzl` & `openllm-0.2.8/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/__about__.py` & `openllm-0.2.8/src/openllm/bundle/oci/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,8 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.2.7"
+"""OCI-related utilities for OpenLLM.
+
+## TODO
+- generate compatible Sagemaker container
+- build custom kernels and CUDA 11.8
+- compose vLLM for PagedAttention
+"""
```

### Comparing `openllm-0.2.7/src/openllm/__init__.py` & `openllm-0.2.8/src/openllm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,16 +56,18 @@
         ),
     )
 
 
 _import_structure: dict[str, list[str]] = {
     "_llm": ["LLM", "Runner", "LLMRunner", "LLMRunnable"],
     "_configuration": ["LLMConfig"],
+    "_schema": ["GenerationInput", "GenerationOutput", "MetadataOutput", "EmbeddingsOutput", "unmarshal_vllm_outputs"],
+    "_generation": ["StopSequenceCriteria", "StopOnTokens"],
+    "_quantisation": ["infer_quantisation_config"],
     "exceptions": [],
-    "_schema": ["GenerationInput", "GenerationOutput", "MetadataOutput", "EmbeddingsOutput"],
     "utils": ["infer_auto_class"],
     "models": [],
     "client": [],
     "bundle": [],
     "playground": [],
     "testing": [],
     "serialisation": ["ggml", "transformers"],
@@ -198,22 +200,26 @@
     from . import models as models
     from . import playground as playground
     from . import serialisation as serialisation
     from . import testing as testing
 
     # Specific types import
     from ._configuration import LLMConfig as LLMConfig
+    from ._generation import StopOnTokens as StopOnTokens
+    from ._generation import StopSequenceCriteria as StopSequenceCriteria
     from ._llm import LLM as LLM
     from ._llm import LLMRunnable as LLMRunnable
     from ._llm import LLMRunner as LLMRunner
     from ._llm import Runner as Runner
+    from ._quantisation import infer_quantisation_config as infer_quantisation_config
     from ._schema import EmbeddingsOutput as EmbeddingsOutput
     from ._schema import GenerationInput as GenerationInput
     from ._schema import GenerationOutput as GenerationOutput
     from ._schema import MetadataOutput as MetadataOutput
+    from ._schema import unmarshal_vllm_outputs as unmarshal_vllm_outputs
     from .cli import build as build
     from .cli import import_model as import_model
     from .cli import list_models as list_models
     from .cli import start as start
     from .cli import start_grpc as start_grpc
     from .models.auto import CONFIG_MAPPING as CONFIG_MAPPING
     from .models.auto import MODEL_FLAX_MAPPING_NAMES as MODEL_FLAX_MAPPING_NAMES
```

### Comparing `openllm-0.2.7/src/openllm/__main__.py` & `openllm-0.2.8/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/_configuration.py` & `openllm-0.2.8/src/openllm/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,27 +62,31 @@
 from cattr.gen import make_dict_structure_fn
 from cattr.gen import make_dict_unstructure_fn
 from cattr.gen import override
 from deepmerge.merger import Merger
 
 import openllm
 
+from ._strategies import LiteralResourceSpec
+from ._strategies import available_resource_spec
+from ._strategies import resource_spec
 from .exceptions import ForbiddenAttributeError
 from .utils import ENV_VARS_TRUE_VALUES
 from .utils import MYPY
 from .utils import LazyType
 from .utils import ReprMixin
 from .utils import bentoml_cattr
 from .utils import codegen
 from .utils import dantic
 from .utils import field_env_key
 from .utils import first_not_none
 from .utils import lenient_issubclass
 from .utils import non_intrusive_setattr
 from .utils import requires_dependencies
+from .utils.import_utils import BACKENDS_MAPPING
 
 
 # NOTE: We need to do check overload import
 # so that it can register
 # correct overloads to typing registry
 if sys.version_info[:2] >= (3, 11):
     from typing import NotRequired
@@ -145,47 +149,39 @@
     type_conflict_strategies=["override"],
 )
 
 
 # case insensitive, but rename to conform with type
 class _PeftEnumMeta(enum.EnumMeta):
     def __getitem__(self, __key: str | t.Any, /) -> t.Any:
-        if isinstance(__key, str):
-            __key = inflection.underscore(__key).upper()
+        if isinstance(__key, str): __key = inflection.underscore(__key).upper()
         return self._member_map_[__key]
 
 
-# vendorred from peft.utils.config.PeftType
-# since we don't hard depend on peft
-class PeftType(enum.Enum, metaclass=_PeftEnumMeta):
+# vendorred from peft.utils.config.PeftType since we don't have hard dependency on peft
+# see https://github.com/huggingface/peft/blob/main/src/peft/utils/config.py
+class PeftType(str, enum.Enum, metaclass=_PeftEnumMeta):
     PROMPT_TUNING = "PROMPT_TUNING"
     P_TUNING = "P_TUNING"
     PREFIX_TUNING = "PREFIX_TUNING"
     LORA = "LORA"
     ADALORA = "ADALORA"
     ADAPTION_PROMPT = "ADAPTION_PROMPT"
+    IA3 = "IA3"
 
     @classmethod
     def _missing_(cls, value: object) -> enum.Enum | None:
         if isinstance(value, str):
             normalized = inflection.underscore(value).upper()
-            if normalized in cls._member_map_:
-                return cls._member_map_[normalized]
-
+            if normalized in cls._member_map_: return cls._member_map_[normalized]
     @classmethod
-    def supported(cls) -> set[str]:
-        return {inflection.underscore(v.value) for v in cls}
-
-    def to_str(self) -> str:
-        return self.value
-
+    def supported(cls) -> set[str]: return {inflection.underscore(v.value) for v in cls}
+    def to_str(self) -> str: return self.value
     @staticmethod
-    def get(__key: str | t.Any, /) -> PeftType:
-        """type-safe getitem."""
-        return PeftType[__key]
+    def get(__key: str | t.Any, /) -> PeftType: return PeftType[__key]  # type-safe getitem.
 
 
 _PEFT_TASK_TYPE_TARGET_MAPPING = {"causal_lm": "CAUSAL_LM", "seq2seq_lm": "SEQ_2_SEQ_LM"}
 
 if t.TYPE_CHECKING:
     AdapterType = t.Literal["lora", "adalora", "adaption_prompt", "prefix_tuning", "p_tuning", "prompt_tuning"]
 else:
@@ -319,53 +315,39 @@
             self,
             adapter_type=adapter_type,
             inference_mode=inference_mode,
             adapter_config=config_merger.merge(self.adapter_config, attrs),
         )
 
     @classmethod
-    def make_adapter_config_class(
-        cls,
-        adapter_type: AdapterType,
-        llm_config_class: type[LLMConfig],
-        /,
-        *,
-        docs: str | None = None,
-        **attrs: t.Any,
-    ) -> type[FineTuneConfig]:
-        """A loose codegen to create default subclass for given adapter config type."""
-        _new_default = {
-            "adapter_type": PeftType[adapter_type],
-            "adapter_config": attrs,
-            "llm_config_class": llm_config_class,
-        }
+    def make_adapter_config_class(cls, adapter_type: AdapterType, llm_config_class: type[LLMConfig], /, *, docs: str | None = None, **attrs: t.Any) -> type[FineTuneConfig]:
+        """A loose codegen to create default subclass for given adapter config type.
 
+        This is used to make adapter subclass
+        """
+        _new_default = {"adapter_type": PeftType[adapter_type], "adapter_config": attrs, "llm_config_class": llm_config_class}
         def transformers(_: type[t.Any], fields: list[attr.Attribute[t.Any]]) -> list[attr.Attribute[t.Any]]:
             transformed: list[attr.Attribute[t.Any]] = []
             for f in fields:
-                if f.name in _new_default:
-                    transformed.append(f.evolve(default=_new_default[f.name]))
-                else:
-                    transformed.append(f)
+                if f.name in _new_default: transformed.append(f.evolve(default=_new_default[f.name]))
+                else: transformed.append(f)
             return transformed
 
         klass = attr.make_class(
             f"{inflection.camelize(adapter_type)}{llm_config_class.__name__}",
             [],
             bases=(cls,),
             slots=True,
             weakref_slot=True,
             frozen=True,
             repr=True,
             collect_by_mro=True,
             field_transformer=transformers,
         )
-
-        if docs is not None:
-            klass.__doc__ = docs
+        if docs is not None: klass.__doc__ = docs
 
         return klass
 
 
 @attr.frozen(slots=True, repr=False, init=False)
 class GenerationConfig(ReprMixin):
     """GenerationConfig is the attrs-compatible version of ``transformers.GenerationConfig``, with some additional validation and environment constructor.
@@ -595,34 +577,24 @@
     decoder_start_token_id: int = dantic.Field(
         description="""If an encoder-decoder model starts decoding with a
         different token than *bos*, the id of that token.
         """,
     )
 
     if t.TYPE_CHECKING and not MYPY:
-
-        def __attrs_init__(self, *args: t.Any, **attrs: t.Any) -> None:
-            ...
-
+        # stubs this for pyright as mypy already has a attr plugin builtin
+        def __attrs_init__(self, *args: t.Any, **attrs: t.Any) -> None: ...
     def __init__(self, *, _internal: bool = False, **attrs: t.Any):
-        if not _internal:
-            raise RuntimeError(
-                "GenerationConfig is not meant to be used directly, "
-                "but you can access this via a LLMConfig.generation_config"
-            )
+        if not _internal: raise RuntimeError("GenerationConfig is not meant to be used directly, but you can access this via a LLMConfig.generation_config")
         self.__attrs_init__(**attrs)
-
     def __getitem__(self, item: str) -> t.Any:
-        if hasattr(self, item):
-            return getattr(self, item)
+        if hasattr(self, item): return getattr(self, item)
         raise KeyError(f"'{self.__class__.__name__}' has no attribute {item}.")
-
     @property
-    def __repr_keys__(self) -> set[str]:
-        return {i.name for i in attr.fields(self.__class__)}
+    def __repr_keys__(self) -> set[str]: return {i.name for i in attr.fields(self.__class__)}
 
 
 bentoml_cattr.register_unstructure_hook_factory(
     lambda cls: attr.has(cls) and lenient_issubclass(cls, GenerationConfig),
     lambda cls: make_dict_unstructure_fn(
         cls,
         bentoml_cattr,
@@ -699,72 +671,41 @@
         top_k: int
         top_p: float
 
         def __attrs_init__(self, *args: t.Any, **attrs: t.Any) -> None:
             ...
 
     def __init__(self, *, _internal: bool = False, **attrs: t.Any):
-        if not _internal:
-            raise RuntimeError(
-                "SamplingParams is not meant to be used directly, "
-                "but you can access this via a LLMConfig.sampling_config or create one with 'SamplingParams.from_generation_config'"
-            )
+        if not _internal: raise RuntimeError("SamplingParams is not meant to be used directly, but you can access this via a LLMConfig.sampling_config or create one with 'SamplingParams.from_generation_config'")
         _object_setattr(self, "max_tokens", attrs.pop("max_tokens", 16))
         _object_setattr(self, "temperature", attrs.pop("temperature", 1.0))
         _object_setattr(self, "top_k", attrs.pop("top_k", -1))
         _object_setattr(self, "top_p", attrs.pop("top_p", 1.0))
         self.__attrs_init__(**attrs)
-
     def __getitem__(self, item: str) -> t.Any:
-        if hasattr(self, item):
-            return getattr(self, item)
+        if hasattr(self, item): return getattr(self, item)
         raise KeyError(f"'{self.__class__.__name__}' has no attribute {item}.")
-
     @property
-    def __repr_keys__(self) -> set[str]:
-        return {i.name for i in attr.fields(self.__class__)}
-
+    def __repr_keys__(self) -> set[str]: return {i.name for i in attr.fields(self.__class__)}
     @classmethod
     def from_generation_config(cls, generation_config: GenerationConfig, **attrs: t.Any) -> t.Self:
         """The main entrypoint for creating a SamplingParams from ``openllm.LLMConfig``."""
         stop = attrs.pop("stop", None)
-        if stop is not None and isinstance(stop, str):
-            stop = [stop]
+        if stop is not None and isinstance(stop, str): stop = [stop]
         attrs["stop"] = stop
 
-        if "max_tokens" in attrs and "max_new_tokens" in attrs:
-            raise ValueError("Both 'max_tokens' and 'max_new_tokens' are passed. Make sure to only use one of them.")
-
+        if "max_tokens" in attrs and "max_new_tokens" in attrs: raise ValueError("Both 'max_tokens' and 'max_new_tokens' are passed. Make sure to only use one of them.")
         temperature = first_not_none(attrs.pop("temperature", None), default=generation_config["temperature"])
         top_k = first_not_none(attrs.pop("top_k", None), default=generation_config["top_k"])
         top_p = first_not_none(attrs.pop("top_p", None), default=generation_config["top_p"])
-        max_tokens = first_not_none(
-            attrs.pop("max_tokens", None),
-            attrs.pop("max_new_tokens", None),
-            default=generation_config["max_new_tokens"],
-        )
-
-        return cls(
-            _internal=True,
-            temperature=temperature,
-            top_k=top_k,
-            top_p=top_p,
-            max_tokens=max_tokens,
-            **attrs,
-        )
+        max_tokens = first_not_none(attrs.pop("max_tokens", None), attrs.pop("max_new_tokens", None), default=generation_config["max_new_tokens"])
 
+        return cls(_internal=True, temperature=temperature, top_k=top_k, top_p=top_p, max_tokens=max_tokens, **attrs)
     @requires_dependencies("vllm", extra="vllm")
-    def to_vllm(self) -> vllm.SamplingParams:
-        return vllm.SamplingParams(
-            max_tokens=self.max_tokens,
-            temperature=self.temperature,
-            top_k=self.top_k,
-            top_p=self.top_p,
-            **bentoml_cattr.unstructure(self),
-        )
+    def to_vllm(self) -> vllm.SamplingParams: return vllm.SamplingParams(max_tokens=self.max_tokens, temperature=self.temperature, top_k=self.top_k, top_p=self.top_p, **bentoml_cattr.unstructure(self))
 
 
 bentoml_cattr.register_unstructure_hook_factory(
     lambda cls: attr.has(cls) and lenient_issubclass(cls, SamplingParams),
     lambda cls: make_dict_unstructure_fn(
         cls,
         bentoml_cattr,
@@ -796,15 +737,15 @@
 
     # NOTE: These required fields should be at the top, as it will be kw_only
     default_id: Required[str]
     model_ids: Required[ListStr]
     architecture: Required[str]
 
     # default OpenLLM runtime imlementation
-    default_implementation: NotRequired[LiteralRuntime]
+    default_implementation: NotRequired[t.Dict[LiteralResourceSpec, LiteralRuntime]]
 
     # meta
     url: str
     requires_gpu: bool
     trust_remote_code: bool
     service_name: NotRequired[str]
     requirements: t.Optional[ListStr]
@@ -829,15 +770,15 @@
 
     # tokenizer_class is the custom tokenizer class for this given LLM
     tokenizer_class: t.Optional[str]
 
 
 _transformed_type: DictStrAny = {
     "fine_tune_strategies": t.Dict[AdapterType, FineTuneConfig],
-    "default_implementation": LiteralRuntime,
+    "default_implementation": t.Dict[LiteralResourceSpec, LiteralRuntime],
 }
 
 
 @attr.define(
     slots=True,
     field_transformer=lambda _, __: [
         attr.Attribute.from_counting_attr(
@@ -868,39 +809,37 @@
         return cls(
             **t.cast(
                 DictStrAny,
                 ModelSettings(
                     default_id="__default__",
                     model_ids=["__default__"],
                     architecture="PreTrainedModel",
-                    default_implementation="pt",
+                    default_implementation={"cpu":"pt", "nvidia.com/gpu": "pt"},
                     name_type="dasherize",
                     requires_gpu=False,
                     url="",
                     model_type="causal_lm",
                     trust_remote_code=False,
                     requirements=None,
                     tokenizer_class=None,
                     timeout=int(36e6),
                     service_name="",
-                    workers_per_resource=1,
+                    workers_per_resource=1.,
                     runtime="transformers",
                 ),
             )
         )
 
     # NOTE: The below are dynamically generated by the field_transformer
     if t.TYPE_CHECKING:
-        # fmt: off
-
         # update-config-stubs.py: attrs start
         default_id: str
         model_ids: ListStr
         architecture: str
-        default_implementation: t.Literal["pt", "tf", "flax", "vllm"]
+        default_implementation: t.Dict[LiteralResourceSpec, LiteralRuntime]
         url: str
         requires_gpu: bool
         trust_remote_code: bool
         service_name: str
         requirements: t.Optional[ListStr]
         bettertransformer: bool
         model_type: t.Literal["causal_lm", "seq2seq_lm"]
@@ -911,78 +850,69 @@
         env: openllm.utils.EnvVarMixin
         timeout: int
         workers_per_resource: t.Union[int, float]
         fine_tune_strategies: t.Dict[AdapterType, FineTuneConfig]
         tokenizer_class: t.Optional[str]
         # update-config-stubs.py: attrs stop
 
-        # fmt: on
-
+# a heuristic cascading implementation resolver based on available resources
+def get_default_implementation(default_implementation_mapping: dict[LiteralResourceSpec, LiteralRuntime]) -> LiteralRuntime:
+    available_spec = available_resource_spec()
+    if resource_spec("tpu") in available_spec: return default_implementation_mapping.get(resource_spec("tpu"), "pt")
+    elif resource_spec("amd") in available_spec: return default_implementation_mapping.get(resource_spec("amd"), "pt")
+    elif resource_spec("nvidia") in available_spec: return default_implementation_mapping.get(resource_spec("nvidia"), "pt")
+    else: return default_implementation_mapping.get(resource_spec("cpu"), "pt")
 
 def structure_settings(cl_: type[LLMConfig], cls: type[_ModelSettingsAttr]) -> _ModelSettingsAttr:
-    if "generation_class" in cl_.__config__:
-        raise ValueError(
-            "'generation_class' shouldn't be defined in '__config__', rather defining "
-            f"all required attributes under '{cl_}.GenerationConfig' instead."
-        )
+    if "generation_class" in cl_.__config__: raise ValueError(f"'generation_class' shouldn't be defined in '__config__', rather defining all required attributes under '{cl_}.GenerationConfig' instead.")
 
     required_fields = {k for k, ann in t.get_type_hints(ModelSettings).items() if t.get_origin(ann) is Required}
-    if any(i not in cl_.__config__ for i in required_fields):
-        raise ValueError(f"Missing required fields {required_fields} '__config__'.")
+    if any(i not in cl_.__config__ for i in required_fields): raise ValueError(f"Missing required fields {required_fields} '__config__'.")
 
     _cl_name = cl_.__name__.replace("Config", "")
     _settings_attr = cls.default()
     has_custom_name = all(i in cl_.__config__ for i in {"model_name", "start_name"})
 
-    _settings_attr = attr.evolve(_settings_attr, **t.cast(DictStrAny, cl_.__config__))
-
+    _settings_attr = attr.evolve(_settings_attr, **cl_.__config__)
     _final_value_dct: DictStrAny = {}
 
     if not has_custom_name:
-        _final_value_dct["model_name"] = (
-            inflection.underscore(_cl_name) if _settings_attr["name_type"] == "dasherize" else _cl_name.lower()
-        )
-        _final_value_dct["start_name"] = (
-            inflection.dasherize(_final_value_dct["model_name"])
-            if _settings_attr["name_type"] == "dasherize"
-            else _final_value_dct["model_name"]
-        )
+        _final_value_dct["model_name"] = inflection.underscore(_cl_name) if _settings_attr["name_type"] == "dasherize" else _cl_name.lower()
+        _final_value_dct["start_name"] = inflection.dasherize(_final_value_dct["model_name"]) if _settings_attr["name_type"] == "dasherize" else _final_value_dct["model_name"]
+
     model_name = _final_value_dct["model_name"] if "model_name" in _final_value_dct else _settings_attr.model_name
+    # if the default implementation dependencies doesn't exist, then always fallback to 'pt'
+    default_implementation = _settings_attr.default_implementation
+    for rs, runtime in default_implementation.items():
+        library_stub = "torch" if runtime == "pt" else runtime
+        if not BACKENDS_MAPPING[library_stub][0](): default_implementation[rs] = "pt"
+    _final_value_dct["default_implementation"] = default_implementation
 
-    env = openllm.utils.EnvVarMixin(model_name)
+    env = openllm.utils.EnvVarMixin(model_name, get_default_implementation(default_implementation), model_id=_settings_attr.default_id,bettertransformer=_settings_attr.bettertransformer)
     _final_value_dct["env"] = env
 
     # bettertransformer support
-    if _settings_attr["bettertransformer"] is None:
-        _final_value_dct["bettertransformer"] = str(env.bettertransformer_value).upper() in ENV_VARS_TRUE_VALUES
-    if _settings_attr["requires_gpu"]:
-        # if requires_gpu is True, then disable BetterTransformer for quantization.
-        _final_value_dct["bettertransformer"] = False
-
+    if _settings_attr["bettertransformer"] is None: _final_value_dct["bettertransformer"] = str(env.bettertransformer_value).upper() in ENV_VARS_TRUE_VALUES
+    # if requires_gpu is True, then disable BetterTransformer for quantization.
+    if _settings_attr["requires_gpu"]: _final_value_dct["bettertransformer"] = False
     _final_value_dct["service_name"] = f"generated_{model_name}_service.py"
 
     # NOTE: The key for fine-tune strategies is 'fine_tune_strategies'
     _fine_tune_strategies: tuple[dict[str, t.Any], ...] | None = getattr(_settings_attr, "fine_tune_strategies", None)
     _converted: dict[AdapterType, FineTuneConfig] = {}
     if _fine_tune_strategies is not None:
         # the given value is a tuple[dict[str, t.Any] ,...]
         for _possible_ft_config in _fine_tune_strategies:
             _adapter_type: AdapterType | None = _possible_ft_config.pop("adapter_type", None)
-            if _adapter_type is None:
-                raise RuntimeError("'adapter_type' is required under config definition (currently missing)'.")
+            if _adapter_type is None: raise RuntimeError("'adapter_type' is required under config definition (currently missing)'.")
             _llm_config_class = _possible_ft_config.pop("llm_config_class", cl_)
-            _doc = _possible_ft_config.pop(
-                "docs",
-                f"Default {inflection.camelize(_adapter_type)}Config for {model_name}",
-            )
+            _doc = _possible_ft_config.pop("docs", f"Default {inflection.camelize(_adapter_type)}Config for {model_name}")
             _converted[_adapter_type] = codegen.add_method_dunders(
                 cl_,
-                FineTuneConfig.make_adapter_config_class(
-                    _adapter_type, _llm_config_class, docs=_doc, **_possible_ft_config
-                ),
+                FineTuneConfig.make_adapter_config_class(_adapter_type, _llm_config_class, docs=_doc, **_possible_ft_config),
             )()
     _final_value_dct["fine_tune_strategies"] = _converted
 
     return attr.evolve(_settings_attr, **_final_value_dct)
 
 
 bentoml_cattr.register_structure_hook(_ModelSettingsAttr, structure_settings)
@@ -997,17 +927,15 @@
     If add_dunder to True, the generated globs should include a __add_dunder
     value that will be used to add the dunder methods to the class for given
     value_var
     """
     return f"setattr(cls, '{attr_name}', {value_var})"
 
 
-def _make_assignment_script(
-    cls: type[LLMConfig], attributes: attr.AttrsInstance, _prefix: t.LiteralString = "openllm"
-) -> t.Callable[..., None]:
+def _make_assignment_script(cls: type[LLMConfig], attributes: attr.AttrsInstance, _prefix: t.LiteralString = "openllm") -> t.Callable[..., None]:
     """Generate the assignment script with prefix attributes __openllm_<value>__."""
     args: ListStr = []
     globs: DictStrAny = {
         "cls": cls,
         "_cached_attribute": attributes,
         "_cached_getattribute_get": _object_getattribute.__get__,
     }
@@ -1111,16 +1039,14 @@
         def __attrs_init__(self, *args: t.Any, **attrs: t.Any) -> None:
             """Generated __attrs_init__ for LLMConfig subclass that follows the attrs contract."""
 
         # NOTE: The following will be populated from __config__ and also
         # considered to be public API. Users can also access these via self[key]
         # To update the docstring for these field, update it through tools/update-config-stubs.py
 
-        # fmt: off
-
         # update-config-stubs.py: special start
         __openllm_default_id__: str = Field(None)
         """Return the default model to use when using 'openllm start <model_id>'.
         This could be one of the keys in 'self.model_ids' or custom users model.
 
         This field is required when defining under '__config__'.
         """
@@ -1130,48 +1056,48 @@
         For example:
             For FLAN-T5 impl, this would be ["google/flan-t5-small", "google/flan-t5-base",
                                              "google/flan-t5-large", "google/flan-t5-xl", "google/flan-t5-xxl"]
 
         This field is required when defining under '__config__'.
         """
         __openllm_architecture__: str = Field(None)
-        """The model architecture that is supported by this LLM. Note that any model weights within this architecture generation can
-    always be run and supported by this LLM.
+        """The model architecture that is supported by this LLM.
+
+        Note that any model weights within this architecture generation can always be run and supported by this LLM.
 
         For example:
             For GPT-NeoX implementation, it is based on GptNeoXForCausalLM, which supports dolly-v2, stablelm:
 
             ```bash
             openllm start gpt-neox --model-id stabilityai/stablelm-tuned-alpha-3b
             ```"""
-        __openllm_default_implementation__: t.Literal["pt", "tf", "flax", "vllm"] = Field(None)
-        """The default runtime to run this LLM. By default, it will be PyTorch (pt) for most models. For some models, such as LlaMA, it will use `vllm` or `flax`."""
+        __openllm_default_implementation__: t.Dict[LiteralResourceSpec, LiteralRuntime] = Field(None)
+        """The default runtime to run this LLM. By default, it will be PyTorch (pt) for most models. For some models, such as LlaMA, it will use `vllm` or `flax`.
+
+    It is a dictionary of key as the accelerator spec in k8s ('cpu', 'nvidia.com/gpu', 'amd.com/gpu', 'cloud-tpus.google.com/v2', ...) and the values as supported OpenLLM Runtime ('flax', 'tf', 'pt', 'vllm')
+    """
         __openllm_url__: str = Field(None)
         """The resolved url for this LLMConfig."""
         __openllm_requires_gpu__: bool = Field(None)
         """Determines if this model is only available on GPU. By default it supports GPU and fallback to CPU."""
         __openllm_trust_remote_code__: bool = Field(None)
         """Whether to always trust remote code"""
         __openllm_service_name__: str = Field(None)
         """Generated service name for this LLMConfig. By default, it is 'generated_{model_name}_service.py'"""
         __openllm_requirements__: t.Optional[ListStr] = Field(None)
         """The default PyPI requirements needed to run this given LLM. By default, we will depend on
         bentoml, torch, transformers."""
         __openllm_bettertransformer__: bool = Field(None)
-        """Whether to use BetterTransformer for this given LLM. This depends per model
-        architecture. By default, we will use BetterTransformer for T5 and StableLM models,
-        and set to False for every other models.
-        """
+        """Whether to use BetterTransformer for this given LLM. This depends per model architecture. By default, we will use BetterTransformer for T5 and StableLM models, and set to False for every other models."""
         __openllm_model_type__: t.Literal["causal_lm", "seq2seq_lm"] = Field(None)
         """The model type for this given LLM. By default, it should be causal language modeling.
         Currently supported 'causal_lm' or 'seq2seq_lm'
         """
         __openllm_runtime__: t.Literal["transformers", "ggml"] = Field(None)
-        """The runtime to use for this model. Possible values are `transformers` or `ggml`. See
-        LlaMA for more information."""
+        """The runtime to use for this model. Possible values are `transformers` or `ggml`. See LlaMA for more information."""
         __openllm_name_type__: t.Optional[t.Literal["dasherize", "lowercase"]] = Field(None)
         """The default name typed for this model. "dasherize" will convert the name to lowercase and
         replace spaces with dashes. "lowercase" will convert the name to lowercase. If this is not set, then both
         `model_name` and `start_name` must be specified."""
         __openllm_model_name__: str = Field(None)
         """The normalized version of __openllm_start_name__, determined by __openllm_name_type__"""
         __openllm_start_name__: str = Field(None)
@@ -1192,16 +1118,14 @@
         """
         __openllm_fine_tune_strategies__: t.Dict[AdapterType, FineTuneConfig] = Field(None)
         """The fine-tune strategies for this given LLM."""
         __openllm_tokenizer_class__: t.Optional[str] = Field(None)
         """Optional tokenizer class for this given LLM. See LlaMA for example."""
         # update-config-stubs.py: special stop
 
-        # fmt: on
-
 
 class _ConfigBuilder:
     """A modified version of attrs internal _ClassBuilder, and should only be called within __init_subclass__ of LLMConfig.
 
     Where:
     - has_custom_setattr=True
     - getstate_setstate=None (config class will always be a slotted class.)
@@ -1210,86 +1134,48 @@
     - cache_hash=False (We don't need to cache the hash code of this object for now.)
     - collect_by_mro=True (The correct behaviour to resolve inheritance)
     - field_transformer=codegen.make_env_transformer (We need to transform the field to have env variable)
 
     It takes `these` arguments as a fully parsed attr.Attribute[t.Any] from __init_subclass__
     """
 
-    __slots__ = (
-        "_cls",
-        "_cls_dict",
-        "_attr_names",
-        "_attrs",
-        "_model_name",
-        "_base_attr_map",
-        "_base_names",
-        "_has_pre_init",
-        "_has_post_init",
-    )
-
-    def __init__(
-        self,
-        cls: type[LLMConfig],
-        these: dict[str, _CountingAttr[t.Any]],
-        auto_attribs: bool = False,
-        kw_only: bool = False,
-        collect_by_mro: bool = True,
-    ):
-        attrs, base_attrs, base_attr_map = _transform_attrs(
-            cls,
-            these,
-            auto_attribs,
-            kw_only,
-            collect_by_mro,
-            field_transformer=codegen.make_env_transformer(cls, cls.__openllm_model_name__),
-        )
-
+    __slots__ = ("_cls", "_cls_dict", "_attr_names", "_attrs", "_model_name", "_base_attr_map", "_base_names", "_has_pre_init", "_has_post_init")
+    def __init__(self, cls: type[LLMConfig], these: dict[str, _CountingAttr[t.Any]], auto_attribs: bool = False, kw_only: bool = False, collect_by_mro: bool = True):
+        attrs, base_attrs, base_attr_map = _transform_attrs(cls, these, auto_attribs, kw_only, collect_by_mro, field_transformer=codegen.make_env_transformer(cls, cls.__openllm_model_name__))
         self._cls = cls
         self._model_name = cls.__openllm_model_name__
         self._cls_dict = dict(cls.__dict__)
         self._attrs = attrs
         self._base_names = {a.name for a in base_attrs}
         self._base_attr_map = base_attr_map
         self._attr_names = tuple(a.name for a in attrs)
         self._has_pre_init = bool(getattr(cls, "__attrs_pre_init__", False))
         self._has_post_init = bool(getattr(cls, "__attrs_post_init__", False))
-
         self._cls_dict["__attrs_attrs__"] = self._attrs
-
     def build_class(self) -> type[LLMConfig]:
         """Finalize class based on the accumulated configuration.
 
         Builder cannot be used after calling this method.
 
         > A difference between this and attrs._ClassBuilder is that we don't
         > create a new class after constructing all __dict__. This has to do
         > with recursive called within __init_subclass__
         """
-        cd = {
-            k: v for k, v in self._cls_dict.items() if k not in (*tuple(self._attr_names), "__dict__", "__weakref__")
-        }
+        cd = {k: v for k, v in self._cls_dict.items() if k not in (*tuple(self._attr_names), "__dict__", "__weakref__")}
         # Traverse the MRO to collect existing slots
         # and check for an existing __weakref__.
-        existing_slots: DictStrAny = {}
         weakref_inherited = False
+        existing_slots: DictStrAny = {}
         for base_cls in self._cls.__mro__[1:-1]:
-            if base_cls.__dict__.get("__weakref__", None) is not None:
-                weakref_inherited = True
-            existing_slots.update(
-                {name: getattr(base_cls, name, codegen._sentinel) for name in getattr(base_cls, "__slots__", [])}
-            )
+            if base_cls.__dict__.get("__weakref__", None) is not None: weakref_inherited = True
+            existing_slots.update({name: getattr(base_cls, name, codegen._sentinel) for name in getattr(base_cls, "__slots__", [])})
 
-        base_names = set(self._base_names)
         names = self._attr_names
-        if (
-            "__weakref__" not in getattr(self._cls, "__slots__", ())
-            and "__weakref__" not in names
-            and not weakref_inherited
-        ):
-            names += ("__weakref__",)
+        base_names = set(self._base_names)
+        if "__weakref__" not in getattr(self._cls, "__slots__", ()) and "__weakref__" not in names and not weakref_inherited: names += ("__weakref__",)
 
         # We only add the names of attributes that aren't inherited.
         # Setting __slots__ to inherited attributes wastes memory.
         slot_names = [name for name in names if name not in base_names]
         # There are slots for attributes from current class
         # that are defined in parent classes.
         # As their descriptors may be overridden by a child class,
@@ -1499,19 +1385,16 @@
                 else field_default,
                 globs=globs,
             ),
         )
 
         # For pickling to work, the __module__ variable needs to be set to the
         # frame where the class is created. This respect the module that is created from cls
-        try:
-            klass.__module__ = cls.__module__
-        except (AttributeError, ValueError):
-            pass
-
+        try: klass.__module__ = cls.__module__
+        except (AttributeError, ValueError): pass
         return t.cast("type[At]", klass)
 
     def __init_subclass__(cls: type[LLMConfig]):
         """The purpose of this ``__init_subclass__`` is to offer pydantic UX while adhering to attrs contract.
 
         This means we will construct all fields and metadata and hack into
         how attrs use some of the 'magic' construction to generate the fields.
@@ -1519,66 +1402,51 @@
         It also does a few more extra features: It also generate all __openllm_*__ config from
         ModelSettings (derived from __config__) to the class.
         """
         if not cls.__name__.endswith("Config"):
             logger.warning("LLMConfig subclass should end with 'Config'. Updating to %sConfig", cls.__name__)
             cls.__name__ = f"{cls.__name__}Config"
 
-        if not hasattr(cls, "__config__"):
-            raise RuntimeError("Given LLMConfig must have '__config__' that is not None defined.")
+        if not hasattr(cls, "__config__"): raise RuntimeError("Given LLMConfig must have '__config__' that is not None defined.")
 
         # auto assignment attributes generated from __config__ after create the new slot class.
         _make_assignment_script(cls, bentoml_cattr.structure(cls, _ModelSettingsAttr))(cls)
-
-        cls.__openllm_generation_class__ = cls._make_subclass(
-            "GenerationConfig", GenerationConfig, suffix_env="generation"
-        )
-        cls.__openllm_sampling_class__ = cls._make_subclass("SamplingParams", SamplingParams, suffix_env="sampling")
+        cls.__openllm_generation_class__ = cls._make_subclass("GenerationConfig", openllm._configuration.GenerationConfig, suffix_env="generation")
+        cls.__openllm_sampling_class__ = cls._make_subclass("SamplingParams", openllm._configuration.SamplingParams, suffix_env="sampling")
 
         # process a fields under cls.__dict__ and auto convert them with dantic.Field
         # this is similar logic to attr._make._transform_attrs
         cd = cls.__dict__
         anns = codegen.get_annotations(cls)
         # _CountingAttr is the underlying representation of attr.field
         ca_names = {name for name, attr in cd.items() if isinstance(attr, _CountingAttr)}
         these: dict[str, _CountingAttr[t.Any]] = {}
         annotated_names: set[str] = set()
         for attr_name, typ in anns.items():
-            if codegen.is_class_var(typ):
-                continue
+            if codegen.is_class_var(typ): continue
             annotated_names.add(attr_name)
             val = cd.get(attr_name, attr.NOTHING)
             if not LazyType["_CountingAttr[t.Any]"](_CountingAttr).isinstance(val):
-                if val is attr.NOTHING:
-                    val = cls.Field(env=field_env_key(cls.__openllm_model_name__, attr_name))
-                else:
-                    val = cls.Field(default=val, env=field_env_key(cls.__openllm_model_name__, attr_name))
+                if val is attr.NOTHING: val = cls.Field(env=field_env_key(cls.__openllm_model_name__, attr_name))
+                else: val = cls.Field(default=val, env=field_env_key(cls.__openllm_model_name__, attr_name))
             these[attr_name] = val
         unannotated = ca_names - annotated_names
         if len(unannotated) > 0:
             missing_annotated = sorted(unannotated, key=lambda n: t.cast("_CountingAttr[t.Any]", cd.get(n)).counter)
-            raise openllm.exceptions.MissingAnnotationAttributeError(
-                f"The following field doesn't have a type annotation: {missing_annotated}"
-            )
+            raise openllm.exceptions.MissingAnnotationAttributeError(f"The following field doesn't have a type annotation: {missing_annotated}")
         # We need to set the accepted key before generation_config
         # as generation_config is a special field that users shouldn't pass.
-        cls.__openllm_accepted_keys__ = (
-            set(these.keys())
-            | {a.name for a in attr.fields(cls.__openllm_generation_class__)}
-            | {a.name for a in attr.fields(cls.__openllm_sampling_class__)}
-        )
-
+        cls.__openllm_accepted_keys__ = set(these.keys()) | {a.name for a in attr.fields(cls.__openllm_generation_class__)} | {a.name for a in attr.fields(cls.__openllm_sampling_class__)}
         cls = _ConfigBuilder(cls, these).add_attrs_init().add_repr().build_class()
 
         # Finally, resolve the types
         if getattr(cls, "__attrs_types_resolved__", None) != cls:
             # NOTE: We will try to resolve type here, and cached it for faster use
             globs: DictStrAny = {"t": t, "typing": t, "Constraint": Constraint}
-            if cls.__module__ in sys.modules:
-                globs.update(sys.modules[cls.__module__].__dict__)
+            if cls.__module__ in sys.modules: globs.update(sys.modules[cls.__module__].__dict__)
             attr.resolve_types(cls.__openllm_generation_class__, globalns=globs)
             attr.resolve_types(cls.__openllm_sampling_class__, globalns=globs)
             cls = attr.resolve_types(cls, globalns=globs)
         # the hint cache for easier access
         cls.__openllm_hints__ = {
             f.name: f.type
             for ite in [
@@ -1589,78 +1457,53 @@
             for f in ite
         }
 
         # For pickling to work, the __module__ variable needs to be set to the
         # frame where the class is created.  Bypass this step in environments where
         # sys._getframe is not defined (Jython for example) or sys._getframe is not
         # defined for arguments greater than 0 (IronPython).
-        try:
-            cls.__module__ = sys._getframe(1).f_globals.get("__name__", "__main__")
-        except (AttributeError, ValueError):
-            pass
+        try: cls.__module__ = sys._getframe(1).f_globals.get("__name__", "__main__")
+        except (AttributeError, ValueError): pass
 
     def __setattr__(self, attr: str, value: t.Any) -> None:
-        if attr in _reserved_namespace:
-            raise ForbiddenAttributeError(
-                f"{attr} should not be set during runtime "
-                f"as these value will be reflected during runtime. "
-                f"Instead, you can create a custom LLM subclass {self.__class__.__name__}."
-            )
-
+        if attr in _reserved_namespace: raise ForbiddenAttributeError(f"{attr} should not be set during runtime as these value will be reflected during runtime. Instead, you can create a custom LLM subclass {self.__class__.__name__}.")
         super().__setattr__(attr, value)
 
-    def __init__(
-        self,
-        *,
-        generation_config: DictStrAny | None = None,
-        __openllm_extras__: DictStrAny | None = None,
-        **attrs: t.Any,
-    ):
+    def __init__(self, *, generation_config: DictStrAny | None = None, __openllm_extras__: DictStrAny | None = None, **attrs: t.Any):
         # create a copy of the keys as cache
         _cached_keys = tuple(attrs.keys())
 
         _generation_cl_dict = attr.fields_dict(self.__openllm_generation_class__)
-        if generation_config is None:
-            generation_config = {k: v for k, v in attrs.items() if k in _generation_cl_dict}
-        else:
-            generation_config = config_merger.merge(
-                generation_config, {k: v for k, v in attrs.items() if k in _generation_cl_dict}
-            )
+        if generation_config is None: generation_config = {k: v for k, v in attrs.items() if k in _generation_cl_dict}
+        else: generation_config = config_merger.merge(generation_config, {k: v for k, v in attrs.items() if k in _generation_cl_dict})
 
         sampling_config = {k: v for k, v in attrs.items() if k in attr.fields_dict(self.__openllm_sampling_class__)}
 
         for k in _cached_keys:
-            if k in generation_config or k in sampling_config or attrs[k] is None:
-                del attrs[k]
-
-        self.__openllm_extras__ = config_merger.merge(
-            first_not_none(__openllm_extras__, default={}),
-            {k: v for k, v in attrs.items() if k not in self.__openllm_accepted_keys__},
-        )
+            if k in generation_config or k in sampling_config or attrs[k] is None: del attrs[k]
 
+        self.__openllm_extras__ = config_merger.merge(first_not_none(__openllm_extras__, default={}), {k: v for k, v in attrs.items() if k not in self.__openllm_accepted_keys__})
         self.generation_config = self["generation_class"](_internal=True, **generation_config)
         self.sampling_config = self["sampling_class"].from_generation_config(self.generation_config, **sampling_config)
 
         # The rest of attrs should only be the attributes to be passed to __attrs_init__
         self.__attrs_init__(**attrs)
 
     # NOTE: These required fields should be at the top, as it will be kw_only
 
-    # fmt: off
-
     # update-config-stubs.py: start
     # NOTE: ModelSettings arguments
     @overload
     def __getitem__(self, item: t.Literal["default_id"]) -> str: ...
     @overload
     def __getitem__(self, item: t.Literal["model_ids"]) -> ListStr: ...
     @overload
     def __getitem__(self, item: t.Literal["architecture"]) -> str: ...
     @overload
-    def __getitem__(self, item: t.Literal["default_implementation"]) -> t.Literal["pt", "tf", "flax", "vllm"]: ...
+    def __getitem__(self, item: t.Literal["default_implementation"]) -> t.Dict[LiteralResourceSpec, LiteralRuntime]: ...
     @overload
     def __getitem__(self, item: t.Literal["url"]) -> str: ...
     @overload
     def __getitem__(self, item: t.Literal["requires_gpu"]) -> bool: ...
     @overload
     def __getitem__(self, item: t.Literal["trust_remote_code"]) -> bool: ...
     @overload
@@ -1803,18 +1646,18 @@
     def __getitem__(self, item: t.Literal["prefix_tuning"]) -> dict[str, t.Any]: ...
     @overload
     def __getitem__(self, item: t.Literal["lora"]) -> dict[str, t.Any]: ...
     @overload
     def __getitem__(self, item: t.Literal["adalora"]) -> dict[str, t.Any]: ...
     @overload
     def __getitem__(self, item: t.Literal["adaption_prompt"]) -> dict[str, t.Any]: ...
+    @overload
+    def __getitem__(self, item: t.Literal["ia3"]) -> dict[str, t.Any]: ...
     # update-config-stubs.py: stop
 
-    # fmt: on
-
     def __getitem__(self, item: t.LiteralString | t.Any) -> t.Any:
         """Allowing access LLMConfig as a dictionary. The order will always evaluate as.
 
         __openllm_*__ > self.key > self.generation_config > self['fine_tune_strategies'] > __openllm_extras__
 
         This method is purely for convenience, and should not be used for performance critical code.
         """
@@ -1838,53 +1681,40 @@
             return self.__class__.__openllm_fine_tune_strategies__[item]
         elif item in self.__openllm_extras__:
             return self.__openllm_extras__[item]
         else:
             raise KeyError(item)
 
     def __getattribute__(self, item: str) -> t.Any:
-        if item in _reserved_namespace:
-            raise ForbiddenAttributeError(
-                f"'{item}' belongs to a private namespace for {self.__class__} and should not be access nor modified."
-            )
+        if item in _reserved_namespace: raise ForbiddenAttributeError(f"'{item}' belongs to a private namespace for {self.__class__} and should not be access nor modified.")
         return _object_getattribute.__get__(self)(item)
 
-    def __len__(self) -> int:
-        return len(self.__openllm_accepted_keys__) + len(self.__openllm_extras__)
-
-    def keys(self) -> list[str]:
-        return list(self.__openllm_accepted_keys__) + list(self.__openllm_extras__)
-
+    def __len__(self) -> int: return len(self.__openllm_accepted_keys__) + len(self.__openllm_extras__)
+    def keys(self) -> list[str]: return list(self.__openllm_accepted_keys__) + list(self.__openllm_extras__)
     def values(self) -> list[t.Any]:
         return (
             [getattr(self, k.name) for k in attr.fields(self.__class__)]
             + [getattr(self.generation_config, k.name) for k in attr.fields(self.__openllm_generation_class__)]
             + [getattr(self.sampling_config, k.name) for k in attr.fields(self.__openllm_sampling_class__)]
             + list(self.__openllm_extras__.values())
         )
-
     def items(self) -> list[tuple[str, t.Any]]:
         return (
             [(k.name, getattr(self, k.name)) for k in attr.fields(self.__class__)]
             + [
                 (k.name, getattr(self.generation_config, k.name))
                 for k in attr.fields(self.__openllm_generation_class__)
             ]
             + [(k.name, getattr(self.sampling_config, k.name)) for k in attr.fields(self.__openllm_sampling_class__)]
             + list(self.__openllm_extras__.items())
         )
-
-    def __iter__(self) -> t.Iterable[str]:
-        return iter(self.keys())
-
+    def __iter__(self) -> t.Iterable[str]: return iter(self.keys())
     def __contains__(self, item: t.Any) -> bool:
-        if item in self.__openllm_extras__:
-            return True
+        if item in self.__openllm_extras__: return True
         return item in self.__openllm_accepted_keys__
-
     @classmethod
     def model_derivate(cls, name: str | None = None, **attrs: t.Any) -> LLMConfig:
         """A helper class to generate a new LLMConfig class with additional attributes.
 
         This is useful to modify builtin __config__ value attributes.
 
         ```python
@@ -1915,76 +1745,58 @@
             ),
         )
 
         # For pickling to work, the __module__ variable needs to be set to the
         # frame where the class is created.  Bypass this step in environments where
         # sys._getframe is not defined (Jython for example) or sys._getframe is not
         # defined for arguments greater than 0 (IronPython).
-        try:
-            new_cls.__module__ = sys._getframe(1).f_globals.get("__name__", "__main__")
-        except (AttributeError, ValueError):
-            pass
-
+        try: new_cls.__module__ = sys._getframe(1).f_globals.get("__name__", "__main__")
+        except (AttributeError, ValueError): pass
         return new_cls(**attrs)
-
     def model_dump(self, flatten: bool = False, **_: t.Any) -> DictStrAny:
         dumped = bentoml_cattr.unstructure(self)
         generation_config = bentoml_cattr.unstructure(self.generation_config)
         sampling_config = bentoml_cattr.unstructure(self.sampling_config)
-        if flatten:
-            dumped.update(generation_config)
-        else:
-            dumped["generation_config"] = generation_config
+        if flatten: dumped.update(generation_config)
+        else: dumped["generation_config"] = generation_config
         dumped.update(sampling_config)
         return dumped
-
-    def model_dump_json(self, **kwargs: t.Any) -> bytes:
-        return orjson.dumps(self.model_dump(**kwargs))
-
+    def model_dump_json(self, **kwargs: t.Any) -> bytes: return orjson.dumps(self.model_dump(**kwargs))
     @classmethod
     def model_construct_json(cls, json_str: str | bytes) -> t.Self:
         try:
             attrs = orjson.loads(json_str)
         except orjson.JSONDecodeError as err:
             raise openllm.exceptions.ValidationError(f"Failed to load JSON: {err}") from None
         return bentoml_cattr.structure(attrs, cls)
-
     @classmethod
     def model_construct_env(cls, **attrs: t.Any) -> t.Self:
         """A helpers that respect configuration values environment variables."""
         attrs = {k: v for k, v in attrs.items() if v is not None}
 
         model_config = cls.__openllm_env__.config
 
         env_json_string = os.environ.get(model_config, None)
 
         config_from_env: DictStrAny = {}
         if env_json_string is not None:
-            try:
-                config_from_env = orjson.loads(env_json_string)
-            except orjson.JSONDecodeError as e:
-                raise RuntimeError(f"Failed to parse '{model_config}' as valid JSON string.") from e
+            try: config_from_env = orjson.loads(env_json_string)
+            except orjson.JSONDecodeError as e: raise RuntimeError(f"Failed to parse '{model_config}' as valid JSON string.") from e
 
         if "generation_config" in attrs:
             generation_config = attrs.pop("generation_config")
-            if not LazyType(DictStrAny).isinstance(generation_config):
-                raise RuntimeError(f"Expected a dictionary, but got {type(generation_config)}")
-        else:
-            generation_config = {
-                k: v for k, v in attrs.items() if k in attr.fields_dict(cls.__openllm_generation_class__)
-            }
+            if not LazyType(DictStrAny).isinstance(generation_config): raise RuntimeError(f"Expected a dictionary, but got {type(generation_config)}")
+        else: generation_config = {k: v for k, v in attrs.items() if k in attr.fields_dict(cls.__openllm_generation_class__)}
 
         for k in tuple(attrs.keys()):
-            if k in generation_config:
-                del attrs[k]
+            if k in generation_config: del attrs[k]
 
         config_from_env.update(attrs)
         config_from_env["generation_config"] = generation_config
         return bentoml_cattr.structure(config_from_env, cls)
-
     def model_validate_click(self, **attrs: t.Any) -> tuple[LLMConfig, DictStrAny]:
         """Parse given click attributes into a LLMConfig and return the remaining click attributes."""
         llm_config_attrs: DictStrAny = {"generation_config": {}}
         key_to_remove: ListStr = []
 
         for k, v in attrs.items():
             if k.startswith(f"{self['model_name']}_generation_"):
@@ -1994,79 +1806,65 @@
                 llm_config_attrs[k[len(self["model_name"] + "_sampling_") :]] = v
                 key_to_remove.append(k)
             elif k.startswith(f"{self['model_name']}_"):
                 llm_config_attrs[k[len(self["model_name"] + "_") :]] = v
                 key_to_remove.append(k)
 
         return self.model_construct_env(**llm_config_attrs), {k: v for k, v in attrs.items() if k not in key_to_remove}
-
     @overload
-    def to_generation_config(self, return_as_dict: t.Literal[False] = False) -> transformers.GenerationConfig:
-        ...
-
+    def to_generation_config(self, return_as_dict: t.Literal[False] = False) -> transformers.GenerationConfig: ...
     @overload
-    def to_generation_config(self, return_as_dict: t.Literal[True] = ...) -> DictStrAny:
-        ...
-
+    def to_generation_config(self, return_as_dict: t.Literal[True] = ...) -> DictStrAny: ...
     def to_generation_config(self, return_as_dict: bool = False) -> transformers.GenerationConfig | DictStrAny:
         config = transformers.GenerationConfig(**bentoml_cattr.unstructure(self.generation_config))
         return config.to_dict() if return_as_dict else config
-
     @requires_dependencies("vllm", extra="vllm")
-    def to_sampling_config(self) -> vllm.SamplingParams:
-        return self.sampling_config.to_vllm()
-
+    def to_sampling_config(self) -> vllm.SamplingParams: return self.sampling_config.to_vllm()
     @classmethod
     def to_click_options(cls, f: AnyCallable) -> click.Command:
         """Convert current configuration to click options.
 
         This can be used as a decorator for click commands.
 
         > **Note**: that the identifier for all LLMConfig will be prefixed with '<model_name>_*', and the generation config
         will be prefixed with '<model_name>_generation_*'.
         """
         for name, field in attr.fields_dict(cls.__openllm_generation_class__).items():
             ty = cls.__openllm_hints__.get(name)
-            if t.get_origin(ty) is t.Union:
-                # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
-                continue
+            # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
+            if t.get_origin(ty) is t.Union: continue
             f = dantic.attrs_to_options(name, field, cls.__openllm_model_name__, typ=ty, suffix_generation=True)(f)
         f = cog.optgroup.group(f"{cls.__openllm_generation_class__.__name__} generation options")(f)
 
         for name, field in attr.fields_dict(cls.__openllm_sampling_class__).items():
             ty = cls.__openllm_hints__.get(name)
-            if t.get_origin(ty) is t.Union:
-                # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
-                continue
+            # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
+            if t.get_origin(ty) is t.Union: continue
             f = dantic.attrs_to_options(name, field, cls.__openllm_model_name__, typ=ty, suffix_sampling=True)(f)
         f = cog.optgroup.group(f"{cls.__openllm_sampling_class__.__name__} sampling options")(f)
 
-        total_keys = set(attr.fields_dict(cls.__openllm_generation_class__)) | set(
-            attr.fields_dict(cls.__openllm_sampling_class__)
-        )
+        total_keys = set(attr.fields_dict(cls.__openllm_generation_class__)) | set(attr.fields_dict(cls.__openllm_sampling_class__))
 
-        if len(cls.__openllm_accepted_keys__.difference(total_keys)) == 0:
-            return f
+        if len(cls.__openllm_accepted_keys__.difference(total_keys)) == 0: return f
 
-        # We pop out 'generation_config' as it is a attribute that we don't
-        # need to expose to CLI.
+        # We pop out 'generation_config' as it is a attribute that we don't need to expose to CLI.
         for name, field in attr.fields_dict(cls).items():
             ty = cls.__openllm_hints__.get(name)
-            if t.get_origin(ty) is t.Union or name == "generation_config" or name == "sampling_config":
-                # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
-                continue
+            # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
+            if t.get_origin(ty) is t.Union or name == "generation_config" or name == "sampling_config": continue
             f = dantic.attrs_to_options(name, field, cls.__openllm_model_name__, typ=ty)(f)
 
         return cog.optgroup.group(f"{cls.__name__} options")(f)
-
-    # All fine-tune related starts here
+    # holds a mapping from self.__openllm_model_type__ to peft.TaskType
+    @classmethod
+    def peft_task_type(cls) -> str: return _PEFT_TASK_TYPE_TARGET_MAPPING[cls.__openllm_model_type__]
     @classmethod
-    def peft_task_type(cls) -> str:
-        # holds a mapping from self.__openllm_model_type__ to peft.TaskType
-        return _PEFT_TASK_TYPE_TARGET_MAPPING[cls.__openllm_model_type__]
+    def default_implementation(cls) -> LiteralRuntime:
+        env_implementation = cls.__openllm_env__["framework_value"]
+        return env_implementation if env_implementation is not None else get_default_implementation(cls.__openllm_default_implementation__)
 
 
 bentoml_cattr.register_unstructure_hook_factory(
     lambda cls: lenient_issubclass(cls, LLMConfig),
     lambda cls: make_dict_unstructure_fn(
         cls,
         bentoml_cattr,
```

### Comparing `openllm-0.2.7/src/openllm/_generation.py` & `openllm-0.2.8/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/_llm.py` & `openllm-0.2.8/src/openllm/_llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,32 +19,35 @@
 import inspect
 import logging
 import os
 import re
 import sys
 import types
 import typing as t
+import uuid
 from abc import ABC
 from abc import abstractmethod
 from pathlib import Path
 
 import attr
+import inflection
 import orjson
 from huggingface_hub import hf_hub_download
 
 import bentoml
 import openllm
+from bentoml._internal.configuration.containers import BentoMLContainer
 from bentoml._internal.models import ModelStore
+from bentoml._internal.models.model import CUSTOM_OBJECTS_FILENAME
 from bentoml._internal.models.model import ModelSignature
 
 from ._configuration import AdapterType
 from ._configuration import FineTuneConfig
 from ._configuration import _object_getattribute
 from ._configuration import _setattr_class
-from ._quantisation import infer_quantisation_config
 from .exceptions import ForbiddenAttributeError
 from .exceptions import GpuNotAvailableError
 from .utils import DEBUG
 from .utils import ENV_VARS_TRUE_VALUES
 from .utils import MYPY
 from .utils import EnvVarMixin
 from .utils import LazyLoader
@@ -78,14 +81,15 @@
     import vllm
 
     import transformers
 
     from ._configuration import PeftType
     from ._types import AdaptersMapping
     from ._types import AdaptersTuple
+    from ._types import AnyCallable
     from ._types import DictStrAny
     from ._types import ListStr
     from ._types import LiteralRuntime
     from ._types import LLMEmbeddings
     from ._types import LLMRunnable
     from ._types import LLMRunner
     from ._types import ModelSignatureDict as _ModelSignatureDict
@@ -115,98 +119,28 @@
 class ModelSignatureDict(t.TypedDict, total=False):
     batchable: bool
     batch_dim: t.Union[t.Tuple[int, int], int]
     input_spec: NotRequired[t.Union[t.Any, t.Tuple[t.Any]]]
     output_spec: NotRequired[t.Any]
 
 
-def normalise_model_name(name: str) -> str:
-    return os.path.basename(resolve_filepath(name)) if validate_is_path(name) else re.sub("[^a-zA-Z0-9]+", "-", name)
-
-
-def make_tag(
-    model_id: str,
-    model_version: str | None = None,
-    trust_remote_code: bool = False,
-    implementation: LiteralRuntime = "pt",
-    quiet: bool = False,
-) -> bentoml.Tag:
-    """Generate a ``bentoml.Tag`` from a given transformers model name.
-
-    Note that this depends on your model to have a config class available.
-
-    Args:
-        model_id: The transformers model name or path to load the model from.
-        model_version: Optional model version to be saved with this tag. Default to None.
-                       If model_id is a custom path, then the version would be the hash of the last modified
-                       time from given ``model_id``.
-        trust_remote_code: Whether to trust the remote code. Defaults to False.
-        model_version: Optional model version to be saved with this tag.
-        implementation: Given implementation for said LLM. One of t.Literal['pt', 'tf', 'flax']
-        quiet: Whether to show warning logs. Default to 'False'
-
-    Returns:
-        A tuple of ``bentoml.Tag`` and a dict of unused kwargs.
-    """
-    model_name = normalise_model_name(model_id)
-    if os.getenv("OPENLLM_USE_LOCAL_LATEST", str(False)).upper() in ENV_VARS_TRUE_VALUES:
-        return bentoml.models.get(f"{implementation}-{model_name}").tag
-
-    if validate_is_path(model_id):
-        model_id = resolve_filepath(model_id)
-        # special cases, if it is the model store, then we return the tags
-        # this will happens within the container, where we use the relative path
-        if in_docker() and os.getenv("BENTO_PATH") is not None:
-            _store = ModelStore(Path(model_id).parent.parent)
-            tag = _store.list()[0].tag
-            model_version = tag.version
-            model_name = tag.name
-        else:
-            if model_version is None:  # noqa: PLR5501
-                if not quiet:
-                    logger.warning(
-                        "Given 'model_id=%s' is a path, and 'model_version' is not passed. OpenLLM will generate the version based on the last modified time of this given directory.",
-                        model_id,
-                    )
-                model_version = generate_hash_from_file(model_id)
-    else:
-        config = t.cast(
-            "transformers.PretrainedConfig",
-            transformers.AutoConfig.from_pretrained(
-                model_id,
-                trust_remote_code=trust_remote_code,
-                revision=first_not_none(model_version, default="main"),
-            ),
-        )
-
-        model_version = getattr(config, "_commit_hash", None)
-        if model_version is None:
-            raise ValueError(
-                f"Internal errors when parsing config for pretrained {model_id} ('commit_hash' not found)"
-            )
-
-    return bentoml.Tag.from_taglike(
-        f"{model_name if in_docker() and os.getenv('BENTO_PATH') is not None else implementation + '-' + model_name}:{model_version}".strip().lower()
-    )
-
+def normalise_model_name(name: str) -> str: return os.path.basename(resolve_filepath(name)) if validate_is_path(name) else re.sub("[^a-zA-Z0-9]+", "-", name)
 
 @functools.lru_cache(maxsize=128)
 def generate_hash_from_file(f: str, algorithm: t.Literal["md5", "sha1"] = "sha1") -> str:
     """Generate a hash from given file's modification time.
 
     Args:
         f: The file to generate the hash from.
         algorithm: The hashing algorithm to use. Defaults to 'sha1' (similar to how Git generate its commit hash.)
 
     Returns:
         The generated hash.
     """
-    modification_time = str(os.path.getmtime(resolve_filepath(f)))
-    hashed = getattr(hashlib, algorithm)(modification_time.encode())
-    return hashed.hexdigest()
+    return getattr(hashlib, algorithm)(str(os.path.getmtime(resolve_filepath(f))).encode()).hexdigest()
 
 
 # the below is similar to peft.utils.other.CONFIG_NAME
 PEFT_CONFIG_NAME = "adapter_config.json"
 
 
 def resolve_peft_config_type(adapter_map: dict[str, str | None]) -> AdaptersMapping:
@@ -216,42 +150,38 @@
 
     Args:
         adapter_map: The given mapping from either SDK or CLI. See CLI docs for more information.
     """
     resolved: AdaptersMapping = {}
     _has_set_default = False
     for path_or_adapter_id, name in adapter_map.items():
-        if _has_set_default:
-            raise ValueError("Only one adapter can be set as default.")
         resolve_name = name
         if resolve_name is None:
+            if _has_set_default: raise ValueError("Only one adapter can be set as default.")
             resolve_name = "default"
             _has_set_default = True
         if os.path.isfile(os.path.join(path_or_adapter_id, PEFT_CONFIG_NAME)):
             config_file = os.path.join(path_or_adapter_id, PEFT_CONFIG_NAME)
         else:
-            try:
-                config_file = hf_hub_download(path_or_adapter_id, PEFT_CONFIG_NAME)
-            except Exception as err:
-                raise ValueError(f"Can't find '{PEFT_CONFIG_NAME}' at '{path_or_adapter_id}'") from err
+            try: config_file = hf_hub_download(path_or_adapter_id, PEFT_CONFIG_NAME)
+            except Exception as err: raise ValueError(f"Can't find '{PEFT_CONFIG_NAME}' at '{path_or_adapter_id}'") from err
         with open(config_file, "r") as file:
             resolved_config = orjson.loads(file.read())
         # all peft_type should be available in PEFT_CONFIG_NAME
         _peft_type: AdapterType = resolved_config["peft_type"].lower()
-        if _peft_type not in resolved:
-            resolved[_peft_type] = ()
+        if _peft_type not in resolved: resolved[_peft_type] = ()
         resolved[_peft_type] += (_AdaptersTuple((path_or_adapter_id, resolve_name, resolved_config)),)
     return resolved
 
 
 _reserved_namespace = {"config_class", "model", "tokenizer", "import_kwargs"}
 
 M = t.TypeVar(
     "M",
-    bound="t.Union[transformers.PreTrainedModel, transformers.Pipeline, transformers.TFPreTrainedModel, transformers.FlaxPreTrainedModel, vllm.LLM, peft.PeftModel, autogptq.modeling.BaseGPTQForCausalLM]",
+    bound="t.Union[transformers.PreTrainedModel, transformers.Pipeline, transformers.TFPreTrainedModel, transformers.FlaxPreTrainedModel, vllm.LLMEngine, vllm.AsyncLLMEngine, peft.PeftModel, autogptq.modeling.BaseGPTQForCausalLM]",
 )
 T = t.TypeVar(
     "T",
     bound="t.Union[transformers.PreTrainedTokenizerFast, transformers.PreTrainedTokenizer, transformers.PreTrainedTokenizerBase]",
 )
 
 
@@ -373,28 +303,27 @@
         This is useful during fine tuning.
         """
         raise NotImplementedError
 
     # NOTE: All fields below are attributes that can be accessed by users.
     config_class: type[openllm.LLMConfig]
     """The config class to use for this LLM. If you are creating a custom LLM, you must specify this class."""
-
     bettertransformer: bool
     """Whether to load this LLM with FasterTransformer enabled. The order of loading is:
 
     - If pass within `for_model`, `from_pretrained` or `__init__`.
     - If `self.bettertransformer` is set within `llm_post_init`.
     - Finally, if none of the above, default to self.config['bettertransformer']
 
     > **Note** that if LoRA is enabled, bettertransformer will be disabled.
     """
-
-    device: torch.device
+    device: "torch.device"
     """The device to be used for this LLM. If the implementation is 'pt', then it will be torch.device, else string."""
-
+    tokenizer_id: t.LiteralString | t.Literal["local"]
+    """optional tokenizer_id for loading with vLLM if the model supports vLLM."""
     # NOTE: The following will be populated by __init_subclass__, note that these should be immutable.
     __llm_trust_remote_code__: bool
     """This is used to determine during 'import_model' whether to trust remote code or not.
 
     This works synonymous with `trust_remote_code` kwarg in transformers Auto classes. If not passed,
     then by default fallback to config_class['trust_remote_code']
     """
@@ -413,14 +342,22 @@
     """A reference to the actual model. Instead of access this directly, you should use `model` property instead."""
     __llm_tokenizer__: T | None
     """A reference to the actual tokenizer. Instead of access this directly, you should use `tokenizer` property instead."""
     __llm_bentomodel__: bentoml.Model | None
     """A reference to the bentomodel used for this LLM. Instead of access this directly, you should use `_bentomodel` property instead."""
     __llm_adapter_map__: dict[AdapterType, dict[str | t.Literal["default"], tuple[peft.PeftConfig, str]]] | None
     """A reference to the the cached LoRA adapter mapping."""
+    __llm_supports_embeddings__: bool
+    """A boolean to determine whether models does implement ``LLM.embeddings``."""
+    __llm_supports_generate__: bool
+    """A boolean to determine whether models does implement ``LLM.generate``."""
+    __llm_supports_generate_one__: bool
+    """A boolean to determine whether models does implement ``LLM.generate_one``."""
+    __llm_supports_generate_iterator__: bool
+    """A boolean to determine whether models does implement ``LLM.generate_iterator``."""
 
     if t.TYPE_CHECKING and not MYPY:
 
         def __attrs_init__(
             self,
             config: openllm.LLMConfig,
             quantization_config: transformers.BitsAndBytesConfig | autogptq.BaseQuantizeConfig | None,
@@ -475,24 +412,33 @@
         decls = (*model_decls, *decls)
         attrs = {**model_attrs, **attrs}
         return f(self, *decls, trust_remote_code=trust_remote_code, **attrs)
 
     return wrapper
 
 
+_DEFAULT_TOKENIZER = "hf-internal-testing/llama-tokenizer"
+
+
+@requires_dependencies("vllm", extra="vllm")
+def get_engine_args(llm: openllm.LLM[M, T], tokenizer: str = _DEFAULT_TOKENIZER) -> vllm.EngineArgs: return vllm.EngineArgs(model=llm._bentomodel.path, tokenizer=tokenizer, tokenizer_mode="auto", tensor_parallel_size=1, dtype="auto", worker_use_ray=False)
 def _wrapped_load_model(f: _load_model_wrapper[M, T]):
     @functools.wraps(f)
-    def wrapper(self: LLM[M, T], *decls: t.Any, **attrs: t.Any) -> M:
-        # wrapped around custom init to provide some meta compression
-        # for all decls and attrs
-        (model_decls, model_attrs), _ = self.llm_parameters
-        decls = (*model_decls, *decls)
-        attrs = {**model_attrs, **attrs}
-        return f(self, *decls, **attrs)
-
+    def wrapper(self: LLM[M, T], *decls: t.Any, **attrs: t.Any) -> M | vllm.LLMEngine:
+        # wrapped around custom init to provide some meta compression for all decls and attrs
+        # and add general vllm.LLMEngine for any vllm implementation.
+        if self.__llm_implementation__ == "vllm":
+            # TODO: Do some more processing with token_id once we support token streaming
+            tokenizer_id = self._bentomodel.path if self.tokenizer_id == "local" else self.tokenizer_id
+            engine = vllm.LLMEngine.from_engine_args(get_engine_args(self, tokenizer=tokenizer_id))
+            if self._bentomodel._fs.isfile(CUSTOM_OBJECTS_FILENAME): engine.tokenizer = self.tokenizer
+            return engine
+        else:
+            (model_decls, model_attrs), _ = self.llm_parameters
+            return f(self, *(*model_decls, *decls), **{**model_attrs, **attrs})
     return wrapper
 
 
 def _wrapped_load_tokenizer(f: _load_tokenizer_wrapper[M, T]):
     @functools.wraps(f)
     def wrapper(self: LLM[M, T], **tokenizer_attrs: t.Any) -> T:
         _, model_tokenizer_attrs = self.llm_parameters
@@ -510,40 +456,53 @@
 
     return wrapper
 
 
 def _wrapped_save_pretrained(f: _save_pretrained_wrapper[M, T]):
     @functools.wraps(f)
     def wrapper(self: LLM[M, T], save_directory: str | Path, **attrs: t.Any) -> None:
-        if isinstance(save_directory, Path):
-            save_directory = str(save_directory)
+        if isinstance(save_directory, Path): save_directory = str(save_directory)
         if self.__llm_model__ is not None and self.bettertransformer and self.__llm_implementation__ == "pt":
             from optimum.bettertransformer import BetterTransformer
-
-            self.__llm_model__ = t.cast(
-                M,
-                BetterTransformer.reverse(t.cast("transformers.PreTrainedModel", self.__llm_model__)),
-            )
+            self.__llm_model__ = t.cast(M, BetterTransformer.reverse(t.cast("transformers.PreTrainedModel", self.__llm_model__)))
         f(self, save_directory, **attrs)
-
     return wrapper
 
 
+def _update_docstring(cls: LLM[M, T], fn: str) -> AnyCallable:
+    # update docstring for given entrypoint
+    original_fn = getattr(cls, fn, getattr(LLMInterface, fn))
+    original_fn.__doc__ = (
+        original_fn.__doc__
+        or f"""\
+    {cls.__name__}'s implementation for {fn}.
+
+    Note that if LoRA is enabled (via either SDK or CLI), `self.model` will become a `peft.PeftModel`
+    The original model can then be accessed with 'self.model.get_base_model()'.
+    """
+    )
+    setattr(cls, fn, original_fn)
+
+
 def _make_assignment_script(cls: type[LLM[M, T]]) -> t.Callable[[type[LLM[M, T]]], None]:
     attributes = {
         "import_model": _wrapped_import_model,
         "load_model": _wrapped_load_model,
         "load_tokenizer": _wrapped_load_tokenizer,
         "llm_post_init": _wrapped_llm_post_init,
         "save_pretrained": _wrapped_save_pretrained,
     }
     args: ListStr = []
     anns: DictStrAny = {}
     lines: ListStr = []
-    globs: DictStrAny = {"cls": cls, "_cached_LLMInterface_get": _object_getattribute.__get__(LLMInterface)}
+    globs: DictStrAny = {
+        "cls": cls,
+        "_cached_LLMInterface_get": _object_getattribute.__get__(LLMInterface),
+        "__gen_docstring": _update_docstring,
+    }
     # function initialisation
     for func, impl in attributes.items():
         impl_name = f"__wrapped_{func}"
         globs.update({f"__serialisation_{func}": getattr(openllm.serialisation, func, None), impl_name: impl})
         cached_func_name = f"_cached_{cls.__name__}_func"
         if func == "llm_post_init":
             func_call = f"_impl_{cls.__name__}_{func}={cached_func_name}"
@@ -557,123 +516,116 @@
             ]
         )
 
     # cached attribute initialisation
     interface_anns = codegen.get_annotations(LLMInterface)
     for v in {"bentomodel", "model", "tokenizer", "adapter_map"}:
         lines.append(_setattr_class(f"__llm_{v}__", None))
-        anns[f"__llm_{v}__"] = interface_anns.get("__llm_{v}__")
+        anns[f"__llm_{v}__"] = interface_anns.get(f"__llm_{v}__")
+
+    # boolean to determine whether LLM has defined an implementation for a function
+    for fn in {"generate", "generate_one", "generate_iterator", "embeddings"}:
+        key = f"__llm_supports_{fn}__"
+        lines.extend(
+            [
+                _setattr_class(key, f"cls.{fn} is not _cached_LLMInterface_get('{fn}')"),
+                f"__gen_docstring(cls, '{fn}')",
+            ]
+        )
+        anns[key] = interface_anns.get(key)
 
-    return codegen.generate_function(cls, "__assign_attr", lines, args=("cls", *args), globs=globs, annotations=anns)
+    return codegen.generate_function(
+        cls, "__assign_llm_attr", lines, args=("cls", *args), globs=globs, annotations=anns
+    )
 
 
 _AdaptersTuple: type[AdaptersTuple] = codegen.make_attr_tuple_class("AdaptersTuple", ["adapter_id", "name", "config"])
 
 
 @attr.define(slots=True, repr=False, init=False)
 class LLM(LLMInterface[M, T], ReprMixin):
     config: openllm.LLMConfig
     """The config instance to use for this LLM. This will be created based on config_class and available
     when initialising the LLM."""
-
     quantization_config: transformers.BitsAndBytesConfig | autogptq.BaseQuantizeConfig | None
     """Quantisation config for quantised model on the fly."""
-
     _model_id: str
     _runtime: t.Literal["ggml", "transformers"]
     _model_decls: TupleAny
     _model_attrs: DictStrAny
     _tokenizer_attrs: DictStrAny
     _tag: bentoml.Tag
     _adapters_mapping: AdaptersMapping | None
     _model_version: str
     _quantize_method: t.Literal["int8", "int4", "gptq"] | None
     _serialisation_format: t.Literal["safetensors", "legacy"]
-
-    tokenizer_cls: t.ClassVar[str | None] = None
-
     @staticmethod
     def _infer_implementation_from_name(name: str) -> tuple[LiteralRuntime, str]:
-        if name.startswith("Flax"):
-            return "flax", name[4:]
-        elif name.startswith("TF"):
-            return "tf", name[2:]
-        elif name.startswith("VLLM"):
-            return "vllm", name[4:]
-        else:
-            return "pt", name
-
+        if name.startswith("Flax"): return "flax", name[4:]
+        elif name.startswith("TF"): return "tf", name[2:]
+        elif name.startswith("VLLM"): return "vllm", name[4:]
+        else: return "pt", name
     def __init_subclass__(cls: type[openllm.LLM[M, T]]) -> None:
         cd = cls.__dict__
         implementation, config_class_name = cls._infer_implementation_from_name(cls.__name__)
         cls.__llm_implementation__ = implementation
         config_class = openllm.AutoConfig.infer_class_from_name(config_class_name)
-
         if "__openllm_internal__" in cd:
-            if "config_class" not in cd:
-                cls.config_class = config_class
-        elif "config_class" not in cd:
-            raise RuntimeError("Missing required key 'config_class'. Make sure to define it within the LLM subclass.")
-
+            if "config_class" not in cd: cls.config_class = config_class
+        elif "config_class" not in cd: raise RuntimeError("Missing required key 'config_class'. Make sure to define it within the LLM subclass.")
         _make_assignment_script(cls)(cls)
+        if "tokenizer_id" not in cd and cls.__llm_implementation__ == "vllm": cls.tokenizer_id = _DEFAULT_TOKENIZER
 
-        # update docstring for given entrypoint
-        for fn in {"generate", "generate_one", "generate_iterator"}:
-            original_fn = getattr(cls, fn, getattr(LLMInterface, fn))
-            original_fn.__doc__ = (
-                original_fn.__doc__
-                or f"""\
-            '{fn}' implementation {cls.__name__}.
-
-            Note that if LoRA is enabled (via either SDK or CLI), `self.model` will become a `peft.PeftModel`
-            The original can then be accessed with 'self.model.get_base_model()'.
-            """
-            )
-            setattr(cls, fn, original_fn)
+        if implementation == "vllm":
+            def vllm_postprocess_generate(self: LLM["vllm.LLMEngine", T], prompt: str, generation_result: list[dict[str, t.Any]], **_: t.Any) -> str: return generation_result[0]["outputs"][0]["text"]
+            def vllm_generate(self: LLM["vllm.LLMEngine", T], prompt: str, **attrs: t.Any) -> list[dict[str, t.Any]]:
+                outputs: list[vllm.RequestOutput] = []
+                # TODO: support prompt_token_ids
+                self.model.add_request(request_id=str(uuid.uuid4().hex), prompt=prompt, sampling_params=self.config.model_construct_env(**attrs).to_sampling_config())
+                while self.model.has_unfinished_requests(): outputs.extend([r for r in self.model.step() if r.finished])
+                return [openllm.unmarshal_vllm_outputs(i) for i in outputs]
+            cls.postprocess_generate = vllm_postprocess_generate
+            cls.generate = vllm_generate
 
-    @classmethod
+    # fmt: off
     @overload
-    def from_pretrained(
-        cls,
-        model_id: str | None = ...,
-        model_version: str | None = ...,
-        llm_config: openllm.LLMConfig | None = ...,
-        *args: t.Any,
-        runtime: t.Literal["ggml", "transformers"] | None = ...,
-        quantize: t.Literal["int8", "int4"] = ...,
-        bettertransformer: str | bool | None = ...,
-        adapter_id: str | None = ...,
-        adapter_name: str | None = ...,
-        adapter_map: dict[str, str | None] | None = ...,
-        quantization_config: transformers.BitsAndBytesConfig | None = ...,
-        serialisation: t.Literal["safetensors", "legacy"] = ...,
-        **attrs: t.Any,
-    ) -> LLM[M, T]:
-        ...
+    def __getitem__(self, item: t.Literal["trust_remote_code"]) -> bool: ...
+    @overload
+    def __getitem__(self, item: t.Literal["implementation"]) -> LiteralRuntime: ...
+    @overload
+    def __getitem__(self, item: t.Literal["model"]) -> M | None: ...
+    @overload
+    def __getitem__(self, item: t.Literal["tokenizer"]) -> T | None: ...
+    @overload
+    def __getitem__(self, item: t.Literal["bentomodel"]) -> bentoml.Model | None: ...
+    @overload
+    def __getitem__(self, item: t.Literal["adapter_map"]) -> dict[AdapterType, dict[str | t.Literal["default"], tuple[peft.PeftConfig, str]]] | None: ...
+    @overload
+    def __getitem__(self, item: t.Literal["supports_embeddings"]) -> bool: ...
+    @overload
+    def __getitem__(self, item: t.Literal["supports_generate"]) -> bool: ...
+    @overload
+    def __getitem__(self, item: t.Literal["supports_generate_one"]) -> bool: ...
+    @overload
+    def __getitem__(self, item: t.Literal["supports_generate_iterator"]) -> bool: ...
+    # fmt: on
+    def __getitem__(self, item: t.LiteralString | t.Any) -> t.Any:
+        if item is None: raise TypeError(f"{self} doesn't understand how to index None.")
+        item = inflection.underscore(item)
+        internal_attributes = f"__llm_{item}__"
+        if hasattr(self, internal_attributes): return getattr(self, internal_attributes)
+        elif hasattr(self, item): return getattr(self, item)
+        else: raise KeyError(item)
 
     @classmethod
     @overload
-    def from_pretrained(
-        cls,
-        model_id: str | None = ...,
-        model_version: str | None = ...,
-        llm_config: openllm.LLMConfig | None = ...,
-        *args: t.Any,
-        runtime: t.Literal["ggml", "transformers"] | None = ...,
-        quantize: t.Literal["gptq"] = ...,
-        bettertransformer: str | bool | None = ...,
-        adapter_id: str | None = ...,
-        adapter_name: str | None = ...,
-        adapter_map: dict[str, str | None] | None = ...,
-        quantization_config: autogptq.BaseQuantizeConfig | None = ...,
-        serialisation: t.Literal["safetensors", "legacy"] = ...,
-        **attrs: t.Any,
-    ) -> LLM[M, T]:
-        ...
-
+    def from_pretrained(cls, model_id: str | None = ..., model_version: str | None = ..., llm_config: openllm.LLMConfig | None = ..., *args: t.Any, runtime: t.Literal["ggml", "transformers"] | None = ..., quantize: t.Literal["int8", "int4"] = ..., bettertransformer: str | bool | None = ..., adapter_id: str | None = ..., adapter_name: str | None = ..., adapter_map: dict[str, str | None] | None = ..., quantization_config: transformers.BitsAndBytesConfig | None = ..., serialisation: t.Literal["safetensors", "legacy"] = ..., **attrs: t.Any) -> LLM[M, T]: ...
+    @classmethod
+    @overload
+    def from_pretrained(cls, model_id: str | None = ..., model_version: str | None = ..., llm_config: openllm.LLMConfig | None = ..., *args: t.Any, runtime: t.Literal["ggml", "transformers"] | None = ..., quantize: t.Literal["gptq"] = ..., bettertransformer: str | bool | None = ..., adapter_id: str | None = ..., adapter_name: str | None = ..., adapter_map: dict[str, str | None] | None = ..., quantization_config: autogptq.BaseQuantizeConfig | None = ..., serialisation: t.Literal["safetensors", "legacy"] = ..., **attrs: t.Any) -> LLM[M, T]: ...
     @classmethod
     def from_pretrained(
         cls,
         model_id: str | None = None,
         model_version: str | None = None,
         llm_config: openllm.LLMConfig | None = None,
         *args: t.Any,
@@ -740,66 +692,41 @@
             adapter_id: The [LoRA](https://arxiv.org/pdf/2106.09685.pdf) pretrained id or local path to use for this LLM. Defaults to None.
             adapter_name: The adapter name to use for this LLM. Defaults to None.
             adapter_map: The adapter map to use for this LLM. Defaults to None. Note that this is mutually exclusive with adapter_id/adapter_name arguments.
             *args: The args to be passed to the model.
             **attrs: The kwargs to be passed to the model.
         """
         cfg_cls = cls.config_class
-        model_id = first_not_none(
-            model_id, cfg_cls.__openllm_env__["model_id_value"], default=cfg_cls.__openllm_default_id__
-        )
+        model_id = t.cast("t.LiteralString", first_not_none(model_id, cfg_cls.__openllm_env__["model_id_value"], default=cfg_cls.__openllm_default_id__))
+        if validate_is_path(model_id): model_id = resolve_filepath(model_id)
         runtime = first_not_none(runtime, default=cfg_cls.__openllm_runtime__)
-
-        model_id, *maybe_revision = model_id.rsplit(":")
-        if len(maybe_revision) > 0:
-            if model_version is not None:
-                logger.warning(
-                    "revision is specified within 'model_id' (%s), which will override the 'model_version=%s'",
-                    maybe_revision[0],
-                    model_version,
-                )
-            model_version = maybe_revision[0]
+        quantize = first_not_none(quantize, cfg_cls.__openllm_env__["quantize_value"], default=None)
+        bettertransformer = first_not_none(bettertransformer, cfg_cls.__openllm_env__["bettertransformer_value"], default=None)
 
         # quantization setup
-        if quantization_config and quantize:
-            raise ValueError(
-                """'quantization_config' and 'quantize' are mutually exclusive. Either customise
-            your quantization_config or use the 'quantize' argument."""
-            )
-        if quantization_config is None and quantize is not None:
-            quantization_config, attrs = infer_quantisation_config(cls, quantize, **attrs)
-
-        if quantize == "gptq":
-            # We will use safetensors for gptq
-            serialisation = "safetensors"
+        if quantization_config and quantize: raise ValueError("'quantization_config' and 'quantize' are mutually exclusive. Either customise your quantization_config or use the 'quantize' argument.")
+        if quantization_config is None and quantize is not None: quantization_config, attrs = openllm.infer_quantisation_config(cls, quantize, **attrs)
+        # We will use safetensors for gptq
+        if quantize == "gptq": serialisation = "safetensors"
+        # We will use legacy format for vllm
+        elif cls.__llm_implementation__ == "vllm": serialisation = "legacy"
 
         # NOTE: LoRA adapter setup
-        if adapter_map and adapter_id:
-            raise ValueError(
-                """'adapter_map' and 'adapter_id' are mutually exclusive. Either provide a
-                'adapter_map' ({adapter_id: adapter_name | None, ...}) or use
-                the combination of adapter_id/adapter_name arguments.
-                """
-            )
-        if adapter_map is None and adapter_id is not None:
-            adapter_map = {adapter_id: adapter_name}
-
-        if adapter_map is not None and not is_peft_available():
-            raise RuntimeError(
-                "LoRA adapter requires 'peft' to be installed. Make sure to install OpenLLM with 'pip install \"openllm[fine-tune]\"'"
-            )
+        if adapter_map and adapter_id: raise ValueError("'adapter_map' and 'adapter_id' are mutually exclusive. Either provide a 'adapter_map' ({adapter_id: adapter_name | None, ...}) or use the combination of adapter_id/adapter_name arguments. ")
+        if adapter_map is None and adapter_id is not None: adapter_map = {adapter_id: adapter_name}
+        if adapter_map is not None and not is_peft_available(): raise RuntimeError("LoRA adapter requires 'peft' to be installed. Make sure to install OpenLLM with 'pip install \"openllm[fine-tune]\"'")
+        if adapter_map: logger.debug("OpenLLM will apply the following adapters layers: %s", list(adapter_map))
 
         if llm_config is None:
             llm_config = cls.config_class.model_construct_env(**attrs)
             # The rests of the kwargs that is not used by the config class should be stored into __openllm_extras__.
             attrs = llm_config["extras"]
 
-        _tag = cls._infer_tag_from_model_id(model_id, model_version)
-        if _tag.version is None:
-            raise RuntimeError("Failed to resolve model version.")
+        _tag = cls.generate_tag(model_id, model_version)
+        if _tag.version is None: raise RuntimeError("Failed to resolve model version.")
 
         return cls(
             *args,
             model_id=model_id,
             llm_config=llm_config,
             bettertransformer=str(bettertransformer).upper() in ENV_VARS_TRUE_VALUES,
             quantization_config=quantization_config,
@@ -809,30 +736,36 @@
             _model_version=_tag.version,
             _tag=_tag,
             _serialisation_format=serialisation,
             **attrs,
         )
 
     @classmethod
-    def _infer_tag_from_model_id(cls, model_id: str, model_version: str | None) -> bentoml.Tag:
-        # XXX: Fix me later, if the model is a valid tag, then we return it directly
-        # instead of creating a new tag from the model_id. this branch will be hit during `openllm build`
-        try:
-            return bentoml.models.get(model_id.lower()).tag
-        except (ValueError, bentoml.exceptions.BentoMLException):
-            try:
-                return bentoml.Tag.from_taglike(model_id.lower())
-            except (ValueError, bentoml.exceptions.BentoMLException):
-                return make_tag(
-                    model_id,
-                    model_version=model_version,
-                    trust_remote_code=cls.config_class.__openllm_trust_remote_code__,
-                    implementation=cls.__llm_implementation__,
-                    quiet=True,
-                )
+    @functools.lru_cache
+    def generate_tag(cls, model_id: str, model_version: str | None) -> bentoml.Tag:
+        """Generate a compliant bentoml tag from model_id.
+
+        If model_id is a pretrained_id from HF, then it will have the following format: <framework>-<normalise_model_id>:revision
+        If model_id contains the revision itself, then it will be <framework>-<normalise_model_id>:revision
+        If model_id is a path, then it will be <framework>-<basename_of_path>-<generated_sha1>
+        """
+        model_name = normalise_model_name(model_id)
+        model_id, *maybe_revision = model_id.rsplit(":")
+        if len(maybe_revision) > 0:
+            if model_version is not None: logger.warning("revision is specified within 'model_id' (%s), and 'model_version=%s' will be ignored.", maybe_revision[0], model_version)
+            return bentoml.Tag.from_taglike(f"{cls.__llm_implementation__}-{model_name}:{maybe_revision[0]}")
+
+        tag_name = f"{cls.__llm_implementation__}-{model_name}".lower().strip()
+        if os.getenv("OPENLLM_USE_LOCAL_LATEST", str(False)).upper() in ENV_VARS_TRUE_VALUES: return bentoml.models.get(f"{tag_name}{':'+model_version if model_version is not None else ''}").tag
+
+        if validate_is_path(model_id): model_id, model_version = resolve_filepath(model_id), first_not_none(model_version, default=generate_hash_from_file(model_id))
+        else:
+            model_version = getattr(transformers.AutoConfig.from_pretrained(model_id, trust_remote_code=cls.config_class.__openllm_trust_remote_code__, revision=first_not_none(model_version, default="main")), "_commit_hash", None)
+            if model_version is None: raise ValueError(f"Internal errors when parsing config for pretrained {model_id} ('commit_hash' not found)")
+        return bentoml.Tag.from_taglike(f"{tag_name}:{model_version}")
 
     def __init__(
         self,
         *args: t.Any,
         model_id: str,
         llm_config: openllm.LLMConfig,
         bettertransformer: bool | None,
@@ -931,361 +864,181 @@
         # low_cpu_mem_usage is only available for model
         # this is helpful on system with low memory to avoid OOM
         low_cpu_mem_usage = attrs.pop("low_cpu_mem_usage", True)
 
         if self.__llm_implementation__ == "pt":
             attrs.update({"low_cpu_mem_usage": low_cpu_mem_usage, "quantization_config": quantization_config})
 
-        model_kwds: DictStrAny = {}
-        tokenizer_kwds: DictStrAny = {}
-        if self.import_kwargs is not None:
-            model_kwds, tokenizer_kwds = self.import_kwargs
-
+        model_kwds, tokenizer_kwds = {}, {}
+        if self.import_kwargs is not None: model_kwds, tokenizer_kwds = self.import_kwargs
         # parsing tokenizer and model kwargs, as the hierachy is param pass > default
         normalized_model_kwds, normalized_tokenizer_kwds = normalize_attrs_to_model_tokenizer_pair(**attrs)
         # NOTE: Save the args and kwargs for latter load
 
-        self.__attrs_init__(
-            llm_config,
-            quantization_config,
-            model_id,
-            _runtime,
-            args,
-            {**model_kwds, **normalized_model_kwds},
-            {**tokenizer_kwds, **normalized_tokenizer_kwds},
-            _tag,
-            _adapters_mapping,
-            _model_version,
-            _quantize_method,
-            _serialisation_format,
-        )
+        # specific branch for running in docker, this is very hacky, needs change upstream
+        if in_docker() and os.getenv("BENTO_PATH") is not None:
+            BentoMLContainer.model_store.set(ModelStore("/home/bentoml/bento/models"))
+            os.environ["OPENLLM_USE_LOCAL_LATEST"] = str(True)
+            _tag = self.generate_tag(model_id, _model_version)
+
+        self.__attrs_init__(llm_config, quantization_config, model_id, _runtime, args, {**model_kwds, **normalized_model_kwds}, {**tokenizer_kwds, **normalized_tokenizer_kwds}, _tag, _adapters_mapping, _model_version, _quantize_method, _serialisation_format)
         # handle trust_remote_code
         self.__llm_trust_remote_code__ = self._model_attrs.pop("trust_remote_code", self.config["trust_remote_code"])
 
         self.llm_post_init()
-
         # we set it here so that we allow subclass to overwrite bettertransformer in llm_post_init
-        if bettertransformer is True:
-            logger.debug("Using %r with BetterTransformer", self)
-            self.bettertransformer = bettertransformer
-        else:
-            non_intrusive_setattr(self, "bettertransformer", self.config["bettertransformer"])
+        if bettertransformer is True: self.bettertransformer = bettertransformer
+        else: non_intrusive_setattr(self, "bettertransformer", self.config["bettertransformer"])
         # If lora is passed, the disable bettertransformer
-        if _adapters_mapping and self.bettertransformer is True:
-            logger.debug("LoRA is visible for %s, disabling BetterTransformer", self)
-            self.bettertransformer = False
+        if _adapters_mapping and self.bettertransformer is True: self.bettertransformer = False
 
     def __setattr__(self, attr: str, value: t.Any) -> None:
-        if attr in _reserved_namespace:
-            raise ForbiddenAttributeError(
-                f"{attr} should not be set during runtime "
-                f"as these value will be reflected during runtime. "
-                f"Instead, you can create a custom LLM subclass {self.__class__.__name__}."
-            )
-
+        if attr in _reserved_namespace: raise ForbiddenAttributeError(f"{attr} should not be set during runtime as these value will be reflected during runtime. Instead, you can create a custom LLM subclass {self.__class__.__name__}.")
         super().__setattr__(attr, value)
 
     @property
-    def adapters_mapping(self) -> AdaptersMapping | None:
-        return self._adapters_mapping
-
+    def adapters_mapping(self) -> AdaptersMapping | None: return self._adapters_mapping
     @adapters_mapping.setter
-    def adapters_mapping(self, value: AdaptersMapping) -> None:
-        self._adapters_mapping = value
-
+    def adapters_mapping(self, value: AdaptersMapping) -> None: self._adapters_mapping = value
     @property
-    def __repr_keys__(self) -> set[str]:
-        return {"model_id", "runner_name", "config", "adapters_mapping", "runtime", "tag"}
-
+    def __repr_keys__(self) -> set[str]: return {"model_id", "runner_name", "config", "adapters_mapping", "runtime", "tag"}
     def __repr_args__(self) -> ReprArgs:
         for k in self.__repr_keys__:
-            if k == "config":
-                yield k, self.config.model_dump(flatten=True)
-            else:
-                yield k, getattr(self, k)
-
+            if k == "config": yield k, self.config.model_dump(flatten=True)
+            else: yield k, getattr(self, k)
     @property
-    def model_id(self) -> str:
-        return self._model_id
-
+    def model_id(self) -> str: return self._model_id
     @property
-    def runtime(self) -> t.Literal["ggml", "transformers"]:
-        return self._runtime
-
+    def runtime(self) -> t.Literal["ggml", "transformers"]: return self._runtime
     @property
-    def runner_name(self) -> str:
-        return f"llm-{self.config['start_name']}-runner"
-
+    def runner_name(self) -> str: return f"llm-{self.config['start_name']}-runner"
     # NOTE: The section below defines a loose contract with langchain's LLM interface.
     @property
-    def llm_type(self) -> str:
-        return normalise_model_name(self._model_id)
-
+    def llm_type(self) -> str: return normalise_model_name(self._model_id)
     @property
-    def identifying_params(self) -> DictStrAny:
-        return {
-            "configuration": self.config.model_dump_json().decode(),
-            "model_ids": orjson.dumps(self.config["model_ids"]).decode(),
-        }
-
+    def identifying_params(self) -> DictStrAny: return {"configuration": self.config.model_dump_json().decode(), "model_ids": orjson.dumps(self.config["model_ids"]).decode()}
+    # llm_parameters are used to store args and attrs for model and tokenizer, as it returns a tuple[tuple[model_args, model_kwargs], tokenizer_kwargs]
     @property
-    def llm_parameters(self) -> tuple[tuple[tuple[t.Any, ...], DictStrAny], DictStrAny]:
-        """Returning the processed model and tokenizer parameters.
-
-        These can then be used with 'import_model' or any other place that requires loading model and tokenizer.
-
-        See 'openllm.cli.download_models' for example usage.
-
-        Returns:
-            ``tuple``: It returns a tuple of (model_args, model_kwargs) & tokenizer_kwargs
-        """
-        return (self._model_decls, self._model_attrs), self._tokenizer_attrs
-
+    def llm_parameters(self) -> tuple[tuple[tuple[t.Any, ...], DictStrAny], DictStrAny]: return (self._model_decls, self._model_attrs), self._tokenizer_attrs
     @property
-    def tag(self) -> bentoml.Tag:
-        return self._tag
-
-    def ensure_model_id_exists(self) -> bentoml.Model:
-        """This utility function will download the model if it doesn't exist yet.
-
-        Make sure to call this function if 'ensure_available' is not set during
-        Auto LLM initialisation.
-
-        The equivalent for ``openllm.Runner`` is ``openllm.Runner.download_model``.
-        """
-        return openllm.import_model(
-            self.config["start_name"],
-            model_id=self.model_id,
-            model_version=self._model_version,
-            runtime=self.runtime,
-            implementation=self.__llm_implementation__,
-            quantize=self._quantize_method,
-            serialisation_format=self._serialisation_format,
-        )
-
+    def tag(self) -> bentoml.Tag: return self._tag
+    # ensure_model_id_exists can be called to save the model to local store
+    def ensure_model_id_exists(self) -> bentoml.Model: return openllm.import_model(self.config["start_name"], model_id=self.model_id, model_version=self._model_version, runtime=self.runtime, implementation=self.__llm_implementation__, quantize=self._quantize_method, serialisation_format=self._serialisation_format)
     @property
     def _bentomodel(self) -> bentoml.Model:
-        if self.__llm_bentomodel__ is None:
-            self.__llm_bentomodel__ = openllm.serialisation.get(self)
+        if self.__llm_bentomodel__ is None: self.__llm_bentomodel__ = openllm.serialisation.get(self)
         return self.__llm_bentomodel__
-
     @property
     def model(self) -> M:
-        """The model to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         # Run check for GPU
-        if self.config["requires_gpu"] and openllm.utils.device_count() < 1:
-            raise GpuNotAvailableError(f"{self} only supports running with GPU (None available).") from None
-
-        if self.__llm_model__ is None:
-            # NOTE: the signature of load_model here is the wrapper under _wrapped_load_model
-            self.__llm_model__ = self.load_model(*self._model_decls, **self._model_attrs)
+        if self.config["requires_gpu"] and openllm.utils.device_count() < 1: raise GpuNotAvailableError(f"{self} only supports running with GPU (None available).") from None
+        # NOTE: the signature of load_model here is the wrapper under _wrapped_load_model
+        if self.__llm_model__ is None: self.__llm_model__ = self.load_model(*self._model_decls, **self._model_attrs)
         return self.__llm_model__
-
     @property
     def tokenizer(self) -> T:
-        """The tokenizer to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
-        if self.__llm_tokenizer__ is None:
-            # NOTE: the signature of load_tokenizer here is the wrapper under _wrapped_load_tokenizer
-            self.__llm_tokenizer__ = self.load_tokenizer(**self._tokenizer_attrs)
+        # NOTE: the signature of load_tokenizer here is the wrapper under _wrapped_load_tokenizer
+        if self.__llm_tokenizer__ is None: self.__llm_tokenizer__ = self.load_tokenizer(**self._tokenizer_attrs)
         return self.__llm_tokenizer__
 
     def _default_ft_config(self, _adapter_type: AdapterType, inference_mode: bool) -> FineTuneConfig:
-        strategy = first_not_none(
-            self.config["fine_tune_strategies"].get(_adapter_type),
-            default=FineTuneConfig(adapter_type=t.cast("PeftType", _adapter_type), llm_config_class=self.config_class),
-        )
+        strategy = first_not_none(self.config["fine_tune_strategies"].get(_adapter_type), default=FineTuneConfig(adapter_type=t.cast("PeftType", _adapter_type), llm_config_class=self.config_class))
         return strategy.eval() if inference_mode else strategy.train()
 
-    def _transpose_adapter_mapping(
-        self,
-        inference_mode: bool = True,
-        use_cache: bool = True,
-    ) -> ResolvedAdaptersMapping:
-        if self._adapters_mapping is None:
-            raise ValueError("LoRA mapping is not set up correctly.")
-
-        if use_cache and self.__llm_adapter_map__ is not None:
-            # early out if we already serialized everything.
-            return self.__llm_adapter_map__
-
-        if not use_cache:
-            logger.debug("Adapter mapping resolution will not be cached. This should only be used during training.")
-
+    def _transpose_adapter_mapping( self, inference_mode: bool = True, use_cache: bool = True) -> ResolvedAdaptersMapping:
+        if self._adapters_mapping is None: raise ValueError("LoRA mapping is not set up correctly.")
+        # early out if we already serialized everything.
+        if use_cache and self.__llm_adapter_map__ is not None: return self.__llm_adapter_map__
+        if not use_cache: logger.debug("Adapter mapping resolution will not be cached. This should only be used during training.")
         adapter_map: ResolvedAdaptersMapping = {k: {} for k in self._adapters_mapping}
         # this is a temporary check to accept the first option name as 'default'
         # then we will raise Error when the optional_name is set to None in next iteration.
         _converted_first_none = False
         for _adapter_type, _adapters_tuples in self._adapters_mapping.items():
             default_config = self._default_ft_config(_adapter_type, inference_mode)
             for adapter in _adapters_tuples:
-                if not adapter.name and _converted_first_none:
-                    raise ValueError(
-                        f"{self.__class__.__name__} doesn't know how to resolve adapter_name None mapping: {adapter.adapter_id, adapter.config}"
-                    )
+                if not adapter.name and _converted_first_none: raise ValueError(f"{self.__class__.__name__} doesn't know how to resolve adapter_name None mapping: {adapter.adapter_id, adapter.config}")
                 name = adapter.name
                 if name is None:
                     _converted_first_none = True
                     name = "default"
-                peft_config = (
-                    default_config.with_config(**adapter.config).to_peft_config()
-                    if name == "default"
-                    else FineTuneConfig(
-                        adapter_type=t.cast("PeftType", _adapter_type),
-                        adapter_config=adapter.config,
-                        inference_mode=inference_mode,
-                        llm_config_class=self.config_class,
-                    ).to_peft_config()
-                )
+                peft_config = default_config.with_config(**adapter.config).to_peft_config() if name == "default" else FineTuneConfig(adapter_type=t.cast("PeftType", _adapter_type), adapter_config=adapter.config, inference_mode=inference_mode, llm_config_class=self.config_class).to_peft_config()
                 adapter_map[_adapter_type][name] = (peft_config, adapter.adapter_id)
 
-        if self.__llm_adapter_map__ is None and use_cache:
-            self.__llm_adapter_map__ = adapter_map
+        if self.__llm_adapter_map__ is None and use_cache: self.__llm_adapter_map__ = adapter_map
         return adapter_map
 
     @requires_dependencies("peft", extra="fine-tune")
-    def prepare_for_training(
-        self,
-        adapter_type: AdapterType = "lora",
-        use_gradient_checkpointing: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[peft.PeftModel, T]:
+    def prepare_for_training(self, adapter_type: AdapterType = "lora", use_gradient_checkpointing: bool = True, **attrs: t.Any) -> tuple[peft.PeftModel, T]:
         from peft import prepare_model_for_kbit_training
-
-        peft_config = (
-            self.config["fine_tune_strategies"]
-            .get(
-                adapter_type,
-                FineTuneConfig(
-                    adapter_type=t.cast("PeftType", adapter_type),
-                    llm_config_class=self.config_class,
-                ),
-            )
-            .train()
-            .with_config(**attrs)
-            .to_peft_config()
-        )
-        wrapped_peft = peft.get_peft_model(
-            prepare_model_for_kbit_training(
-                self.model,
-                use_gradient_checkpointing=use_gradient_checkpointing,
-            ),
-            peft_config,
-        )
-        if DEBUG:
-            wrapped_peft.print_trainable_parameters()
+        peft_config = self.config["fine_tune_strategies"].get(adapter_type, FineTuneConfig(adapter_type=t.cast("PeftType", adapter_type), llm_config_class=self.config_class)).train().with_config(**attrs).to_peft_config()
+        wrapped_peft = peft.get_peft_model(prepare_model_for_kbit_training(self.model, use_gradient_checkpointing=use_gradient_checkpointing), peft_config)
+        if DEBUG: wrapped_peft.print_trainable_parameters()
         return wrapped_peft, self.tokenizer
 
     @requires_dependencies("peft", extra="fine-tune")
-    def apply_adapter(
-        self,
-        inference_mode: bool = True,
-        adapter_type: AdapterType = "lora",
-        load_adapters: t.Literal["all"] | list[str] | None = None,
-        use_cache: bool = True,
-    ) -> peft.PeftModel | M:
+    def apply_adapter(self, inference_mode: bool = True, adapter_type: AdapterType = "lora", load_adapters: t.Literal["all"] | list[str] | None = None, use_cache: bool = True) -> peft.PeftModel | M:
         """Apply given LoRA mapping to the model.
 
         Note that the base model can still be accessed via self.model.get_base_model().
         """
         assert self.__llm_model__ is not None  # noqa: S101
 
         # early out if _adapters_mapping is empty or it is already wrapped with peft.
-        if not self._adapters_mapping:
-            logger.debug("No adapter mapping is found. Skip applying adapter.")
-            return self.__llm_model__
-        if isinstance(self.__llm_model__, peft.PeftModel):
-            logger.debug("Model is already wrapped with peft. Skip applying adapter.")
-            return self.__llm_model__
+        if not self._adapters_mapping: return self.__llm_model__
+        if isinstance(self.__llm_model__, peft.PeftModel): return self.__llm_model__
 
         _mapping = self._transpose_adapter_mapping(inference_mode=inference_mode, use_cache=use_cache)
-        if adapter_type not in _mapping:
-            raise ValueError(
-                f"Given adapter type {adapter_type} is not supported. Please choose from {list(_mapping.keys())}"
-            )
+        if adapter_type not in _mapping: raise ValueError(f"Given adapter type {adapter_type} is not supported. Please choose from {list(_mapping.keys())}")
         adapter_mapping = _mapping[adapter_type]
 
         self.__llm_model__ = self._wrap_default_peft_model(adapter_mapping, inference_mode=inference_mode)
 
-        if not isinstance(self.__llm_model__, peft.PeftModel):
-            # We hit this branch during inference
-            # TODO: load multiple adapters
-            return self.__llm_model__
-
         # now we loop through the rest with add_adapter
         if len(adapter_mapping) > 0:
-            for adapter_name, (_peft_config, _) in adapter_mapping.items():
-                self.__llm_model__.add_adapter(adapter_name, _peft_config)
+            for adapter_name, (_peft_config, _) in adapter_mapping.items(): self.__llm_model__.add_adapter(adapter_name, _peft_config)
 
             # optionally load adapters. In case of multiple adapters, or on Runner,
             # we will need to set load_adapters='all'
             if load_adapters is not None:
                 adapters_to_load = adapter_mapping.keys() if load_adapters == "all" else load_adapters
                 for adapter_name in adapters_to_load:
                     _peft_config, _peft_model_id = adapter_mapping[adapter_name]
-                    self.__llm_model__.load_adapter(
-                        _peft_model_id,
-                        adapter_name=adapter_name,
-                        is_trainable=not inference_mode,
-                        **dict(_peft_config.to_dict()),
-                    )
+                    self.__llm_model__.load_adapter(_peft_model_id, adapter_name=adapter_name, is_trainable=not inference_mode, **dict(_peft_config.to_dict()))
 
         return self.__llm_model__
 
-    # XXX: Until peft publish py.typed PR, we will need to set the wrapper to t.Any (not ideal since we ducking the actual Peft class here.)
-    def _wrap_default_peft_model(
-        self, adapter_mapping: dict[str, tuple[peft.PeftConfig, str]], inference_mode: bool
-    ) -> t.Any:
+    def _wrap_default_peft_model(self, adapter_mapping: dict[str, tuple[peft.PeftConfig, str]], inference_mode: bool):
         assert self.__llm_model__ is not None, "Error: Model is not loaded correctly"  # noqa: S101
-        if isinstance(self.__llm_model__, peft.PeftModel):
-            logger.warning("Model is already wrapped with peft. Skip wrapping with default peft model.")
-            return self.__llm_model__
-
-        if "default" not in adapter_mapping:
-            raise ValueError(
-                "There is no 'default' mapping. Please check the adapter mapping and report this bug to the OpenLLM team."
-            )
+        if isinstance(self.__llm_model__, peft.PeftModel): return self.__llm_model__
 
+        if "default" not in adapter_mapping: raise ValueError("There is no 'default' mapping. Please check the adapter mapping and report this bug to the OpenLLM team.")
         default_config, peft_model_id = adapter_mapping.pop("default")
 
         # the below shared similar logics with `get_peft_model`
         # TODO: Support PromptLearningConfig
-        if default_config.task_type not in peft.MODEL_TYPE_TO_PEFT_MODEL_MAPPING.keys() and not isinstance(
-            default_config, peft.PromptLearningConfig
-        ):
-            logger.debug(
-                "Given task type '%s' is not supported by peft. Make sure the adapter is loaded manually before running inference.",
-                default_config.task_type,
-            )
+        if default_config.task_type not in peft.MODEL_TYPE_TO_PEFT_MODEL_MAPPING.keys() and not isinstance(default_config, peft.PromptLearningConfig):
+            logger.debug("Given task type '%s' is not supported by peft. Make sure the adapter is loaded manually before running inference.", default_config.task_type)
             model = peft.PeftModel(self.__llm_model__, default_config)
         else:
             # XXX: this is not ideal to serialize like this, maybe for fine-tune we will only support 0.4.0
             # onwards. For now, keep this logic here.
             peft_class = peft.MODEL_TYPE_TO_PEFT_MODEL_MAPPING[default_config.task_type]
             if default_config.base_model_name_or_path:
                 kwargs: DictStrAny = {"is_trainable": not inference_mode}
-                if "config" in inspect.signature(peft_class.from_pretrained).parameters:
-                    kwargs["config"] = default_config
-                else:
-                    kwargs.update(dict(default_config.to_dict().items()))
+                if "config" in inspect.signature(peft_class.from_pretrained).parameters: kwargs["config"] = default_config
+                else: kwargs.update(dict(default_config.to_dict().items()))
                 # BUG: This hits during inference, need fixing
                 model = peft_class.from_pretrained(self.__llm_model__, peft_model_id, **kwargs)
-            else:
-                # in this case, the given base_model_name_or_path is None. This will be hit during training
-                model = peft_class(self.__llm_model__, default_config)
+            else: model = peft_class(self.__llm_model__, default_config)  # in this case, the given base_model_name_or_path is None. This will be hit during training
         return model
 
     # order of these fields matter here, make sure to sync it with
     # openllm.models.auto.factory.BaseAutoLLMClass.for_model
-    def to_runner(
-        self,
-        models: list[bentoml.Model] | None = None,
-        max_batch_size: int | None = None,
-        max_latency_ms: int | None = None,
-        scheduling_strategy: type[bentoml.Strategy] | None = None,
-    ) -> LLMRunner:
+    def to_runner(self, models: list[bentoml.Model] | None = None, max_batch_size: int | None = None, max_latency_ms: int | None = None, scheduling_strategy: type[bentoml.Strategy] | None = None) -> LLMRunner[M, T]:
         """Convert this LLM into a Runner.
 
         Args:
             models: Any additional ``bentoml.Model`` to be included in this given models.
                     By default, this will be determined from the model_name.
             max_batch_size: The maximum batch size for the runner.
             max_latency_ms: The maximum latency for the runner.
@@ -1300,47 +1053,34 @@
         - 'name': will be generated by OpenLLM, hence users don't shouldn't worry about this.
             The generated name will be 'llm-<model-start-name>-runner' (ex: llm-dolly-v2-runner, llm-chatglm-runner)
         - 'embedded': Will be disabled by default. There is no reason to run LLM in embedded mode.
         - 'method_configs': The method configs for the runner will be managed internally by OpenLLM.
         """
         models = models if models is not None else []
 
-        try:
-            models.append(self._bentomodel)
-        except bentoml.exceptions.NotFound:
-            models.append(openllm.serialisation.get(self, auto_import=True))
+        try: models.append(self._bentomodel)
+        except bentoml.exceptions.NotFound: models.append(openllm.serialisation.get(self, auto_import=True))
 
         if scheduling_strategy is None:
             from ._strategies import CascadingResourceStrategy
-
             scheduling_strategy = CascadingResourceStrategy
 
         generate_sig = ModelSignature.from_dict(t.cast("_ModelSignatureDict", ModelSignatureDict(batchable=False)))
         embeddings_sig = ModelSignature.from_dict(t.cast("_ModelSignatureDict", ModelSignatureDict(batchable=False)))
-        generate_iterator_sig = ModelSignature.from_dict(
-            t.cast("_ModelSignatureDict", ModelSignatureDict(batchable=True))
-        )
+        generate_iterator_sig = ModelSignature.from_dict(t.cast("_ModelSignatureDict", ModelSignatureDict(batchable=True)))
 
         # NOTE: returning the two langchain API's to the runner
         return llm_runner_class(self)(
             llm_runnable_class(self, embeddings_sig, generate_sig, generate_iterator_sig),
             name=self.runner_name,
             embedded=False,
             models=models,
             max_batch_size=max_batch_size,
             max_latency_ms=max_latency_ms,
-            method_configs=bentoml_cattr.unstructure(
-                {
-                    "embeddings": embeddings_sig,
-                    "__call__": generate_sig,
-                    "generate": generate_sig,
-                    "generate_one": generate_sig,
-                    "generate_iterator": generate_iterator_sig,
-                }
-            ),
+            method_configs=bentoml_cattr.unstructure({"embeddings": embeddings_sig, "__call__": generate_sig, "generate": generate_sig, "generate_one": generate_sig, "generate_iterator": generate_iterator_sig}),
             scheduling_strategy=scheduling_strategy,
         )
 
     def predict(self, prompt: str, **attrs: t.Any) -> t.Any:
         """The scikit-compatible API for self(...)."""
         return self.__call__(prompt, **attrs)
 
@@ -1355,88 +1095,26 @@
 
         ```python
         llm = openllm.AutoLLM.for_model("dolly-v2")
         llm("What is the meaning of life?")
         ```
         """
         prompt, generate_kwargs, postprocess_kwargs = self.sanitize_parameters(prompt, **attrs)
-        generated_result = self.generate(prompt, **generate_kwargs)
-        return self.postprocess_generate(prompt, generated_result, **postprocess_kwargs)
+        return self.postprocess_generate(prompt, self.generate(prompt, **generate_kwargs), **postprocess_kwargs)
 
 
 @overload
-def Runner(
-    model_name: str,
-    *,
-    model_id: str | None = None,
-    model_version: str | None = ...,
-    init_local: t.Literal[False, True] = ...,
-    **attrs: t.Any,
-) -> LLMRunner:
-    ...
-
-
+def Runner(model_name: str, *, model_id: str | None = None, model_version: str | None = ..., init_local: t.Literal[False, True] = ..., **attrs: t.Any) -> LLMRunner[t.Any, t.Any]: ...
 @overload
-def Runner(
-    model_name: str,
-    *,
-    model_id: str = ...,
-    model_version: str | None = ...,
-    models: list[bentoml.Model] | None = ...,
-    max_batch_size: int | None = ...,
-    max_latency_ms: int | None = ...,
-    method_configs: dict[str, ModelSignatureDict | ModelSignature] | None = ...,
-    embedded: t.Literal[True, False] = ...,
-    scheduling_strategy: type[bentoml.Strategy] | None = ...,
-    **attrs: t.Any,
-) -> LLMRunner:
-    ...
-
-
+def Runner(model_name: str, *, model_id: str = ..., model_version: str | None = ..., models: list[bentoml.Model] | None = ..., max_batch_size: int | None = ..., max_latency_ms: int | None = ..., method_configs: dict[str, ModelSignatureDict | ModelSignature] | None = ..., embedded: t.Literal[True, False] = ..., scheduling_strategy: type[bentoml.Strategy] | None = ..., **attrs: t.Any) -> LLMRunner[t.Any, t.Any]: ...
 @overload
-def Runner(
-    model_name: str,
-    *,
-    ensure_available: bool | None = None,
-    init_local: bool = ...,
-    implementation: LiteralRuntime | None = None,
-    llm_config: openllm.LLMConfig | None = None,
-    **attrs: t.Any,
-) -> LLMRunner:
-    ...
-
-
+def Runner(model_name: str, *, ensure_available: bool | None = None, init_local: bool = ..., implementation: LiteralRuntime | None = None, llm_config: openllm.LLMConfig | None = None, **attrs: t.Any) -> LLMRunner[t.Any, t.Any]: ...
 @overload
-def Runner(
-    model_name: str,
-    *args: t.Any,
-    model_id: str | None = ...,
-    model_version: str | None = ...,
-    llm_config: openllm.LLMConfig | None = ...,
-    runtime: t.Literal["ggml", "transformers"] | None = ...,
-    quantize: t.Literal["int8", "int4", "gptq"] | None = ...,
-    bettertransformer: str | bool | None = ...,
-    adapter_id: str | None = ...,
-    adapter_name: str | None = ...,
-    adapter_map: dict[str, str | None] | None = ...,
-    quantization_config: transformers.BitsAndBytesConfig | autogptq.BaseQuantizeConfig | None = None,
-    serialisation: t.Literal["safetensors", "legacy"] = ...,
-    **attrs: t.Any,
-) -> LLMRunner:
-    ...
-
-
-def Runner(
-    model_name: str,
-    ensure_available: bool | None = None,
-    init_local: bool = False,
-    implementation: LiteralRuntime | None = None,
-    llm_config: openllm.LLMConfig | None = None,
-    **attrs: t.Any,
-) -> LLMRunner:
+def Runner(model_name: str, *, model_id: str | None = ..., model_version: str | None = ..., llm_config: openllm.LLMConfig | None = ..., runtime: t.Literal["ggml", "transformers"] | None = ..., quantize: t.Literal["int8", "int4", "gptq"] | None = ..., bettertransformer: str | bool | None = ..., adapter_id: str | None = ..., adapter_name: str | None = ..., adapter_map: dict[str, str | None] | None = ..., quantization_config: transformers.BitsAndBytesConfig | autogptq.BaseQuantizeConfig | None = None, serialisation: t.Literal["safetensors", "legacy"] = ..., **attrs: t.Any) -> LLMRunner[t.Any, t.Any]: ...
+def Runner(model_name: str, ensure_available: bool | None = None, init_local: bool = False, implementation: LiteralRuntime | None = None, llm_config: openllm.LLMConfig | None = None, **attrs: t.Any) -> LLMRunner[t.Any, t.Any]:
     """Create a Runner for given LLM. For a list of currently supported LLM, check out 'openllm models'.
 
     The behaviour of ensure_available that is synonymous to `AutoLLM.for_model` depends on `init_local`.
     By default, `ensure_available` is synonymous to `init_local`, meaning on the service when creating
     runner, it won't download the model. So before running your BentoML Service, you should create a `on_startup`
     hook to check download if you don't want to do it manually:
 
@@ -1463,57 +1141,38 @@
                     run the model locally. (Symmetrical to bentoml.Runner.init_local())
         **attrs: The rest of kwargs will then be passed to the LLM. Refer to the LLM documentation for the kwargs
                 behaviour
     """
     if llm_config is not None:
         attrs.update(
             {
+                "model_id": llm_config["env"]["model_id_value"],
                 "bettertransformer": llm_config["env"]["bettertransformer_value"],
                 "quantize": llm_config["env"]["quantize_value"],
                 "runtime": llm_config["env"]["runtime_value"],
-                "serialisation": first_not_none(
-                    os.getenv("OPENLLM_SERIALIZATION"), attrs.get("serialisation"), default="safetensors"
-                ),
+                "serialisation": first_not_none(os.getenv("OPENLLM_SERIALIZATION"), attrs.get("serialisation"), default="safetensors"),
             }
         )
 
-    default_implementation = llm_config["default_implementation"] if llm_config is not None else "pt"
-
-    implementation = first_not_none(
-        implementation, default=EnvVarMixin(model_name, default_implementation)["framework_value"]
-    )
-
-    runner = openllm.infer_auto_class(implementation).create_runner(
-        model_name,
-        llm_config=llm_config,
-        ensure_available=ensure_available if ensure_available is not None else init_local,
-        **attrs,
-    )
-
-    if init_local:
-        runner.init_local(quiet=True)
-
+    default_implementation = llm_config.default_implementation() if llm_config is not None else "pt"
+    implementation = first_not_none(implementation, default=EnvVarMixin(model_name, default_implementation)["framework_value"])
+    runner = openllm.infer_auto_class(implementation).create_runner(model_name, llm_config=llm_config, ensure_available=ensure_available if ensure_available is not None else init_local, **attrs)
+    if init_local: runner.init_local(quiet=True)
     return runner
 
 
-def method_signature(sig: ModelSignature) -> ModelSignatureDict:
-    return bentoml_cattr.unstructure(sig)
+def method_signature(sig: ModelSignature) -> ModelSignatureDict: return bentoml_cattr.unstructure(sig)
 
 
 class SetAdapterOutput(t.TypedDict):
     success: bool
     message: str
 
 
-def llm_runnable_class(
-    self: openllm.LLM[M, T],
-    embeddings_sig: ModelSignature,
-    generate_sig: ModelSignature,
-    generate_iterator_sig: ModelSignature,
-) -> type[LLMRunnable]:
+def llm_runnable_class(self: openllm.LLM[M, T], embeddings_sig: ModelSignature, generate_sig: ModelSignature, generate_iterator_sig: ModelSignature) -> type[LLMRunnable[M, T]]:
     class _Runnable(bentoml.Runnable):
         SUPPORTED_RESOURCES = ("nvidia.com/gpu", "amd.com/gpu", "cpu")
         SUPPORTS_CPU_MULTI_THREADING = True
 
         def __init__(__self: _Runnable):
             # NOTE: The side effect of this line
             # is that it will load the imported model during
@@ -1523,51 +1182,40 @@
                 logger.info("Applying LoRA to %s...", self.runner_name)
                 self.apply_adapter(inference_mode=True, load_adapters="all")
 
         @bentoml.Runnable.method(batchable=False)
         def set_adapter(__self: _Runnable, adapter_name: str) -> SetAdapterOutput:
             success = False
             message = None
-            if not is_peft_available():
-                message = "peft is not available. Make sure to install: 'pip install \"openllm[fine-tune]\"'"
-            elif self.__llm_adapter_map__ is None:
-                message = "No adapters available for current running server."
-            elif not isinstance(__self.model, peft.PeftModel):
-                message = "Model is not a PeftModel"
-            if message is not None:
-                return SetAdapterOutput(success=success, message=message)
-
+            if not is_peft_available(): message = "peft is not available. Make sure to install: 'pip install \"openllm[fine-tune]\"'"
+            elif self.__llm_adapter_map__ is None: message = "No adapters available for current running server."
+            elif not isinstance(__self.model, peft.PeftModel): message = "Model is not a PeftModel"
+            if message is not None: return SetAdapterOutput(success=success, message=message)
             try:
                 t.cast("peft.PeftModel", __self.model).set_adapter(adapter_name)
                 return SetAdapterOutput(success=True, message=f"Successfully set current adapter to {adapter_name}")
             except ValueError:
                 logger.info("Adapter %s not found", adapter_name)
-                return SetAdapterOutput(
-                    success=success,
-                    message=f"Adapter {adapter_name} not found. Available adapters: {list(t.cast('peft.PeftModel', __self.model).peft_config)}",
-                )
+                return SetAdapterOutput(success=success, message=f"Adapter {adapter_name} not found. Available adapters: {list(t.cast('peft.PeftModel', __self.model).peft_config)}")
 
         @bentoml.Runnable.method(**method_signature(embeddings_sig))
         def embeddings(__self: _Runnable, prompt: str | list[str]) -> LLMEmbeddings:
-            if isinstance(prompt, str):
-                prompt = [prompt]
+            if isinstance(prompt, str): prompt = [prompt]
             return self.embeddings(prompt)
 
         @bentoml.Runnable.method(**method_signature(generate_sig))
         def __call__(__self: _Runnable, prompt: str, **attrs: t.Any) -> list[t.Any]:
             return self.generate(prompt, **attrs)
 
         @bentoml.Runnable.method(**method_signature(generate_sig))
         def generate(__self: _Runnable, prompt: str, **attrs: t.Any) -> list[t.Any]:
             return self.generate(prompt, **attrs)
 
         @bentoml.Runnable.method(**method_signature(generate_sig))
-        def generate_one(
-            __self: _Runnable, prompt: str, stop: list[str], **attrs: t.Any
-        ) -> t.Sequence[dict[t.Literal["generated_text"], str]]:
+        def generate_one(__self: _Runnable, prompt: str, stop: list[str], **attrs: t.Any) -> t.Sequence[dict[t.Literal["generated_text"], str]]:
             return self.generate_one(prompt, stop, **attrs)
 
         @bentoml.Runnable.method(**method_signature(generate_iterator_sig))
         def generate_iterator(__self: _Runnable, prompt: str, **attrs: t.Any) -> t.Generator[t.Any, None, None]:
             yield self.generate_iterator(prompt, **attrs)
 
     return types.new_class(
@@ -1582,71 +1230,51 @@
                 "__module__": self.__module__,
                 "__doc__": self.config["env"].start_docstring,
             }
         ),
     )
 
 
-def llm_runner_class(self: openllm.LLM[M, T]) -> type[LLMRunner]:
-    def available_adapters(__self: LLMRunner) -> PeftAdapterOutput:
-        if not is_peft_available():
-            return {
-                "success": False,
-                "result": {},
-                "error_msg": "peft is not available. Make sure to install: 'pip install \"openllm[fine-tune]\"'",
-            }
-        if self.__llm_adapter_map__ is None:
-            return {
-                "success": False,
-                "result": {},
-                "error_msg": "No adapters available for current running server.",
-            }
-        if not isinstance(__self.model, peft.PeftModel):
-            return {"success": False, "result": {}, "error_msg": "Model is not a PeftModel"}
+def llm_runner_class(self: openllm.LLM[M, T]) -> type[LLMRunner[M, T]]:
+    def available_adapters(__self: LLMRunner[M, T]) -> PeftAdapterOutput:
+        if not is_peft_available(): return {"success": False, "result": {}, "error_msg": "peft is not available. Make sure to install: 'pip install \"openllm[fine-tune]\"'"}
+        if self.__llm_adapter_map__ is None: return {"success": False, "result": {}, "error_msg": "No adapters available for current running server."}
+        if not isinstance(__self.model, peft.PeftModel): return {"success": False, "result": {}, "error_msg": "Model is not a PeftModel"}
         return {"success": True, "result": __self.model.peft_config, "error_msg": ""}
 
-    def _wrapped_generate_run(__self: LLMRunner, prompt: str, **kwargs: t.Any) -> t.Any:
+    def _wrapped_generate_run(__self: LLMRunner[M, T], prompt: str, **kwargs: t.Any) -> t.Any:
         """Wrapper for runner.generate.run() to handle the prompt and postprocessing.
 
         This will be used for LangChain API.
 
         Usage:
         ```python
         runner = openllm.Runner("dolly-v2", init_local=True)
         runner("What is the meaning of life?")
         ```
         """
         prompt, generate_kwargs, postprocess_kwargs = self.sanitize_parameters(prompt, **kwargs)
-        generated_result = __self.generate.run(prompt, **generate_kwargs)
-        return self.postprocess_generate(prompt, generated_result, **postprocess_kwargs)
+        return self.postprocess_generate(prompt, __self.generate.run(prompt, **generate_kwargs), **postprocess_kwargs)
 
-    def _wrapped_embeddings_run(__self: LLMRunner, prompt: str | list[str]) -> LLMEmbeddings:
+    def _wrapped_embeddings_run(__self: LLMRunner[M, T], prompt: str | list[str]) -> LLMEmbeddings:
         """``llm.embed`` is a light wrapper around runner.embeedings.run().
 
         Usage:
         ```python
         runner = openllm.Runner('llama', implementation='pt')
         runner.embed("What is the meaning of life?")
         ```
         """
-        if isinstance(prompt, str):
-            prompt = [prompt]
+        if isinstance(prompt, str): prompt = [prompt]
         return __self.embeddings.run(prompt)
 
-    def _wrapped_repr_keys(_: LLMRunner) -> set[str]:
-        return {"config", "llm_type", "runner_methods", "runtime", "llm_tag"}
+    def _wrapped_repr_keys(_: LLMRunner[M, T]) -> set[str]: return {"config", "llm_type", "runner_methods", "runtime", "llm_tag"}
 
-    def _wrapped_repr_args(__self: LLMRunner) -> ReprArgs:
-        yield "runner_methods", {
-            method.name: {
-                "batchable": method.config.batchable,
-                "batch_dim": method.config.batch_dim if method.config.batchable else None,
-            }
-            for method in __self.runner_methods
-        }
+    def _wrapped_repr_args(__self: LLMRunner[M, T]) -> ReprArgs:
+        yield "runner_methods", {method.name: {"batchable": method.config.batchable, "batch_dim": method.config.batch_dim if method.config.batchable else None} for method in __self.runner_methods}
         yield "config", self.config.model_dump(flatten=True)
         yield "llm_type", __self.llm_type
         yield "runtime", self.runtime
         yield "llm_tag", self.tag
 
     return types.new_class(
         self.__class__.__name__ + "Runner",
@@ -1654,19 +1282,23 @@
         exec_body=lambda ns: ns.update(
             {
                 "llm_type": self.llm_type,
                 "identifying_params": self.identifying_params,
                 "llm_tag": self.tag,
                 "llm": self,  # NOTE: self reference to LLM
                 "config": self.config,
+                "implementation": self.__llm_implementation__,
                 "peft_adapters": property(fget=available_adapters),
                 "download_model": self.ensure_model_id_exists,
                 "__call__": _wrapped_generate_run,
                 "embed": _wrapped_embeddings_run,
                 "__module__": self.__module__,
                 "__doc__": self.config["env"].start_docstring,
                 "__repr__": ReprMixin.__repr__,
                 "__repr_keys__": property(_wrapped_repr_keys),
                 "__repr_args__": _wrapped_repr_args,
+                "supports_embeddings": self["supports_embeddings"],
+                "supports_hf_agent": self["supports_generate_one"],
+                "has_adapters": self._adapters_mapping is not None,
             }
         ),
     )
```

### Comparing `openllm-0.2.7/src/openllm/_prompt.py` & `openllm-0.2.8/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/_quantisation.py` & `openllm-0.2.8/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/_schema.py` & `openllm-0.2.8/src/openllm/_schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,49 +15,55 @@
 from __future__ import annotations
 import functools
 import typing as t
 
 import attr
 import inflection
 
-import openllm
-from openllm._configuration import GenerationConfig
-from openllm.utils import bentoml_cattr
+from ._configuration import GenerationConfig
+from ._configuration import LLMConfig
+from .utils import LazyLoader
+from .utils import LazyType
+from .utils import bentoml_cattr
+from .utils import requires_dependencies
 
 
 if t.TYPE_CHECKING:
+    import vllm
+
     from ._types import DictStrAny
 else:
     DictStrAny = dict
+    vllm = LazyLoader("vllm", globals(), "vllm")
 
 
 @attr.frozen(slots=True)
 class GenerationInput:
     prompt: str
     """The prompt to be sent to system."""
 
-    llm_config: openllm.LLMConfig
+    llm_config: LLMConfig
     """A mapping of given LLM configuration values for given system."""
 
     @staticmethod
-    def convert_llm_config(
-        data: dict[str, t.Any] | openllm.LLMConfig, cls: type[openllm.LLMConfig] | None = None
-    ) -> openllm.LLMConfig:
-        if isinstance(data, openllm.LLMConfig):
+    def convert_llm_config(data: dict[str, t.Any] | LLMConfig, cls: type[LLMConfig] | None = None) -> LLMConfig:
+        if isinstance(data, LLMConfig):
             return data
-        elif openllm.utils.LazyType(DictStrAny).isinstance(data):
+        elif LazyType(DictStrAny).isinstance(data):
             if cls is None:
                 raise ValueError("'cls' must pass if given data is a dictionary.")
             return cls(**data)
         else:
             raise RuntimeError(f"Type {type(data)} is not yet supported.")
 
     @classmethod
     def for_model(cls, model_name: str, **attrs: t.Any) -> type[GenerationInput]:
-        llm_config = openllm.AutoConfig.for_model(model_name, **attrs)
+        from .models.auto import AutoConfig
+
+        llm_config = AutoConfig.for_model(model_name, **attrs)
         return attr.make_class(
             inflection.camelize(llm_config["model_name"]) + "GenerationInput",
             attrs={
                 "prompt": attr.field(type=str),
                 "llm_config": attr.field(
                     type=llm_config.__class__,
                     default=llm_config,
@@ -90,13 +96,36 @@
 @attr.frozen(slots=True)
 class MetadataOutput:
     model_id: str
     timeout: int
     model_name: str
     framework: str
     configuration: str
+    supports_embeddings: bool
+    supports_hf_agent: bool
 
 
 @attr.frozen(slots=True)
 class EmbeddingsOutput:
     embeddings: t.List[float]
     num_tokens: int
+
+
+@requires_dependencies("vllm", extra="vllm")
+def unmarshal_vllm_outputs(request_output: vllm.RequestOutput) -> DictStrAny:
+    return dict(
+        request_id=request_output.request_id,
+        prompt=request_output.prompt,
+        finished=request_output.finished,
+        prompt_token_ids=request_output.prompt_token_ids,
+        outputs=[
+            dict(
+                index=it.index,
+                text=it.text,
+                token_ids=it.token_ids,
+                cumulative_logprob=it.cumulative_logprob,
+                logprobs=it.logprobs,
+                finish_reason=it.finish_reason,
+            )
+            for it in request_output.outputs
+        ],
+    )
```

### Comparing `openllm-0.2.7/src/openllm/_service.py` & `openllm-0.2.8/src/openllm/_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,196 +7,73 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """The service definition for running any LLMService.
 
 Note that the line `model = ...` is a special line and should not be modified. This will be handled by openllm
 internally to generate the correct model service when bundling the LLM to a Bento.
 This will ensure that 'bentoml serve llm-bento' will work accordingly.
 
 The generation code lives under utils/codegen.py
 """
 from __future__ import annotations
-import os
-import typing as t
-import warnings
-
-import attr
-import orjson
+import os, typing as t, warnings, attr, orjson, bentoml, openllm
 from starlette.applications import Starlette
 from starlette.responses import JSONResponse
 from starlette.routing import Route
-
-import bentoml
-import openllm
-
-
 if t.TYPE_CHECKING:
     from starlette.requests import Request
     from starlette.responses import Response
-
-# The following warnings from bitsandbytes, and probably not that important
-# for users to see
-warnings.filterwarnings(
-    "ignore",
-    message="MatMul8bitLt: inputs will be cast from torch.float32 to float16 during quantization",
-)
-warnings.filterwarnings(
-    "ignore",
-    message="MatMul8bitLt: inputs will be cast from torch.bfloat16 to float16 during quantization",
-)
-warnings.filterwarnings(
-    "ignore",
-    message=(
-        "The installed version of bitsandbytes was compiled without GPU support. 8-bit optimizers and GPU quantization"
-        " are unavailable."
-    ),
-)
-
+# The following warnings from bitsandbytes, and probably not that important for users to see
+warnings.filterwarnings("ignore", message="MatMul8bitLt: inputs will be cast from torch.float32 to float16 during quantization")
+warnings.filterwarnings("ignore", message="MatMul8bitLt: inputs will be cast from torch.bfloat16 to float16 during quantization")
+warnings.filterwarnings("ignore", message="The installed version of bitsandbytes was compiled without GPU support. 8-bit optimizers and GPU quantization are unavailable.")
 model = os.environ.get("OPENLLM_MODEL", "{__model_name__}")  # openllm: model name
-# NOTE: The default value is used when running inside the container
-# OPENLLM_MODEL_ID must be set when running this service from `bentoml serve`
-# See `openllm start {__bento_name__} -h` for more information
-model_id = os.environ.get("OPENLLM_MODEL_ID", "{__model_id__}")  # openllm: model id
 adapter_map = os.environ.get("OPENLLM_ADAPTER_MAP", """{__model_adapter_map__}""")  # openllm: model adapter map
-
 llm_config = openllm.AutoConfig.for_model(model)
-
-runner = openllm.Runner(
-    model,
-    model_id=model_id,
-    llm_config=llm_config,
-    ensure_available=False,
-    adapter_map=orjson.loads(adapter_map),
-)
-
+runner = openllm.Runner(model, llm_config=llm_config, ensure_available=False, adapter_map=orjson.loads(adapter_map))
 svc = bentoml.Service(name=f"llm-{llm_config['start_name']}-service", runners=[runner])
-
-
-@svc.api(
-    input=bentoml.io.JSON.from_sample(sample={"prompt": "", "llm_config": llm_config.model_dump(flatten=True)}),
-    output=bentoml.io.JSON.from_sample(sample={"responses": [], "configuration": llm_config.model_dump(flatten=True)}),
-    route="/v1/generate",
-)
+@svc.api(input=bentoml.io.JSON.from_sample(sample={"prompt": "", "llm_config": llm_config.model_dump(flatten=True)}), output=bentoml.io.JSON.from_sample(sample={"responses": [], "configuration": llm_config.model_dump(flatten=True)}), route="/v1/generate")
 async def generate_v1(input_dict: dict[str, t.Any]) -> openllm.GenerationOutput:
     qa_inputs = openllm.GenerationInput.for_model(model)(**input_dict)
     config = qa_inputs.llm_config.model_dump()
     responses = await runner.generate.async_run(qa_inputs.prompt, **config)
     return openllm.GenerationOutput(responses=responses, configuration=config)
-
-
-@svc.api(
-    input=bentoml.io.JSON.from_sample(sample=["Hey Jude, welcome to the jumgle!", "What is the meaning of life?"]),
-    output=bentoml.io.JSON.from_sample(
-        sample={
-            "embeddings": [
-                0.007917795330286026,
-                -0.014421648345887661,
-                0.00481307040899992,
-                0.007331526838243008,
-                -0.0066398633643984795,
-                0.00945580005645752,
-                0.0087016262114048,
-                -0.010709521360695362,
-                0.012635177001357079,
-                0.010541186667978764,
-                -0.00730888033285737,
-                -0.001783102168701589,
-                0.02339819073677063,
-                -0.010825827717781067,
-                -0.015888236463069916,
-                0.01876218430697918,
-                0.0076906150206923485,
-                0.0009032754460349679,
-                -0.010024012066423893,
-                0.01090280432254076,
-                -0.008668390102684498,
-                0.02070549875497818,
-                0.0014594447566196322,
-                -0.018775740638375282,
-                -0.014814382418990135,
-                0.01796768605709076,
-            ],
-            "num_tokens": 20,
-        }
-    ),
-    route="/v1/embeddings",
-)
-async def embeddings_v1(phrases: list[str]) -> openllm.EmbeddingsOutput:
-    responses = await runner.embeddings.async_run(phrases)
-    return openllm.EmbeddingsOutput(embeddings=responses["embeddings"].tolist()[0], num_tokens=responses["num_tokens"])
-
-
-@svc.api(
-    input=bentoml.io.Text(),
-    output=bentoml.io.JSON.from_sample(
-        sample={
-            "model_id": model_id,
-            "timeout": 3600,
-            "model_name": llm_config["model_name"],
-            "framework": "pt",
-            "configuration": "",
-        }
-    ),
-    route="/v1/metadata",
-)
-def metadata_v1(_: str) -> openllm.MetadataOutput:
-    return openllm.MetadataOutput(
-        model_id=model_id,
-        timeout=llm_config["timeout"],
-        model_name=llm_config["model_name"],
-        framework=llm_config["env"]["framework_value"],
-        configuration=llm_config.model_dump_json().decode(),
-    )
-
-
-@svc.api(
-    input=bentoml.io.Text.from_sample(sample="default"),
-    output=bentoml.io.JSON.from_sample(sample={"success": True, "error_msg": "some error message"}),
-    route="/v1/adapters",
-)
-async def adapters_v1(adapter_name: str) -> dict[str, bool | str]:
-    return await runner.set_adapter.async_run(adapter_name)
-
-
-@attr.define
-class HfAgentInput:
-    inputs: str
-    parameters: t.Dict[str, t.Any]
-
-
-async def hf_agent(request: Request) -> Response:
-    json_str = await request.body()
-    try:
-        input_data = openllm.utils.bentoml_cattr.structure(orjson.loads(json_str), HfAgentInput)
-    except orjson.JSONDecodeError as err:
-        raise openllm.exceptions.OpenLLMException(f"Invalid JSON input received: {err}") from None
-
-    stop = input_data.parameters.pop("stop", ["\n"])
-    try:
-        resp = await runner.generate_one.async_run(input_data.inputs, stop, **input_data.parameters)
-        return JSONResponse(resp, status_code=200)
-    except NotImplementedError:
-        return JSONResponse(f"'{model}' is currently not supported with HuggingFace agents.", status_code=500)
-
-
-hf_app = Starlette(debug=True, routes=[Route("/agent", hf_agent, methods=["POST"])])
-
-svc.mount_asgi_app(hf_app, path="/hf")
-
-
+@svc.api(input=bentoml.io.Text(), output=bentoml.io.JSON.from_sample(sample={"model_id": runner.llm.model_id, "timeout": 3600, "model_name": llm_config["model_name"], "framework": "pt", "configuration": "", "supports_embeddings": runner.supports_embeddings, "supports_hf_agent": runner.supports_hf_agent}), route="/v1/metadata")
+def metadata_v1(_: str) -> openllm.MetadataOutput: return openllm.MetadataOutput(model_id=runner.llm.model_id, timeout=llm_config["timeout"], model_name=llm_config["model_name"], framework=llm_config["env"]["framework_value"], configuration=llm_config.model_dump_json().decode(), supports_embeddings=runner.supports_embeddings, supports_hf_agent=runner.supports_hf_agent,)
+if runner.supports_embeddings:
+    @svc.api(input=bentoml.io.JSON.from_sample(sample=["Hey Jude, welcome to the jumgle!", "What is the meaning of life?"]), output=bentoml.io.JSON.from_sample(sample={"embeddings": [0.007917795330286026, -0.014421648345887661, 0.00481307040899992, 0.007331526838243008, -0.0066398633643984795, 0.00945580005645752, 0.0087016262114048, -0.010709521360695362, 0.012635177001357079, 0.010541186667978764, -0.00730888033285737, -0.001783102168701589, 0.02339819073677063, -0.010825827717781067, -0.015888236463069916, 0.01876218430697918, 0.0076906150206923485, 0.0009032754460349679, -0.010024012066423893, 0.01090280432254076, -0.008668390102684498, 0.02070549875497818, 0.0014594447566196322, -0.018775740638375282, -0.014814382418990135, 0.01796768605709076], "num_tokens": 20}), route="/v1/embeddings")
+    async def embeddings_v1(phrases: list[str]) -> openllm.EmbeddingsOutput:
+        responses = await runner.embeddings.async_run(phrases)
+        return openllm.EmbeddingsOutput(embeddings=responses["embeddings"].tolist()[0], num_tokens=responses["num_tokens"])
+if runner.supports_hf_agent and openllm.utils.is_transformers_supports_agent():
+    @attr.define
+    class HfAgentInput:
+        inputs: str
+        parameters: t.Dict[str, t.Any]
+    async def hf_agent(request: Request) -> Response:
+        json_str = await request.body()
+        try: input_data = openllm.utils.bentoml_cattr.structure(orjson.loads(json_str), HfAgentInput)
+        except orjson.JSONDecodeError as err: raise openllm.exceptions.OpenLLMException(f"Invalid JSON input received: {err}") from None
+        stop = input_data.parameters.pop("stop", ["\n"])
+        try: return JSONResponse(await runner.generate_one.async_run(input_data.inputs, stop, **input_data.parameters), status_code=200)
+        except NotImplementedError: return JSONResponse(f"'{model}' is currently not supported with HuggingFace agents.", status_code=500)
+    hf_app = Starlette(debug=True, routes=[Route("/agent", hf_agent, methods=["POST"])])
+    svc.mount_asgi_app(hf_app, path="/hf")
+if runner.has_adapters:
+    @svc.api(input=bentoml.io.Text.from_sample(sample="default"), output=bentoml.io.JSON.from_sample(sample={"success": True, "error_msg": "some error message"}), route="/v1/adapters")
+    async def adapters_v1(adapter_name: str) -> dict[str, bool | str]: return await runner.set_adapter.async_run(adapter_name)
+else:
+    async def adapters_v1(_: Request) -> Response: return JSONResponse({"success": False, "message": "No available adapters for current running server"})
 async def list_adapter_v1(_: Request) -> Response:
     res: dict[str, t.Any] = {}
-    if runner.peft_adapters["success"] is True:
-        res["result"] = {k: v.to_dict() for k, v in runner.peft_adapters["result"].items()}
-    res["success"] = runner.peft_adapters["success"]
-    res["error_msg"] = runner.peft_adapters["error_msg"]
+    if runner.peft_adapters["success"] is True: res["result"] = {k: v.to_dict() for k, v in runner.peft_adapters["result"].items()}
+    res.update({"success": runner.peft_adapters["success"], "error_msg": runner.peft_adapters["error_msg"]})
     return JSONResponse(res, status_code=200)
-
-
-metadata_app = Starlette(debug=True, routes=[Route("/adapters", list_adapter_v1, methods=["GET"])])
-svc.mount_asgi_app(metadata_app, path="/v1")
+adapters_routes_v1 = [Route("/adapters", list_adapter_v1, methods=["GET"])]
+if not runner.has_adapters: adapters_routes_v1.append(Route("/adapters", adapters_v1, methods=["POST"]))
+adapters_app_v1 = Starlette(debug=True, routes=adapters_routes_v1)
+svc.mount_asgi_app(adapters_app_v1, path="/v1")
```

### Comparing `openllm-0.2.7/src/openllm/_strategies.py` & `openllm-0.2.8/src/openllm/_strategies.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
+import functools
 import inspect
 import logging
 import math
 import os
 import sys
 import types
 import typing as t
@@ -31,15 +32,14 @@
 
 from .utils import LazyType
 from .utils import ReprMixin
 
 
 if t.TYPE_CHECKING:
     ListIntStr = list[int | str]
-
     class DynResource(bentoml.Resource[t.List[str]], resource_id=""):
         resource_id: t.ClassVar[str]
 
 else:
     DynResource = bentoml.Resource[t.List[str]]
     ListIntStr = list
 
@@ -48,82 +48,64 @@
 if sys.version_info[:2] >= (3, 11):
     from typing import overload
 else:
     from typing_extensions import overload
 
 logger = logging.getLogger(__name__)
 
-
 def _strtoul(s: str) -> int:
     """Return -1 or positive integer sequence string starts with,."""
-    if not s:
-        return -1
+    if not s: return -1
     idx = 0
     for idx, c in enumerate(s):
-        if not (c.isdigit() or (idx == 0 and c in "+-")):
-            break
-        if idx + 1 == len(s):
-            idx += 1  # noqa: PLW2901
+        if not (c.isdigit() or (idx == 0 and c in "+-")): break
+        if idx + 1 == len(s): idx += 1  # noqa: PLW2901
     # NOTE: idx will be set via enumerate
     return int(s[:idx]) if idx > 0 else -1
 
 
 def _parse_list_with_prefix(lst: str, prefix: str) -> list[str]:
     rcs: list[str] = []
     for elem in lst.split(","):
         # Repeated id results in empty set
-        if elem in rcs:
-            return []
+        if elem in rcs: return []
         # Anything other but prefix is ignored
-        if not elem.startswith(prefix):
-            break
+        if not elem.startswith(prefix): break
         rcs.append(elem)
     return rcs
 
 
 _STACK_LEVEL = 3
 
-
 @overload
-def _parse_visible_devices(default_var: str | None = ..., respect_env: t.Literal[True] = True) -> list[str] | None:
-    ...
-
-
+def _parse_visible_devices(default_var: str | None = ..., respect_env: t.Literal[True] = True) -> list[str] | None: ...
 @overload
-def _parse_visible_devices(default_var: str = ..., respect_env: t.Literal[False] = False) -> list[str]:
-    ...
-
-
+def _parse_visible_devices(default_var: str = ..., respect_env: t.Literal[False] = False) -> list[str]: ...
 def _parse_visible_devices(default_var: str | None = None, respect_env: bool = True) -> list[str] | None:
     """CUDA_VISIBLE_DEVICES aware with default var for parsing spec."""
     if respect_env:
         spec = os.getenv("CUDA_VISIBLE_DEVICES", default_var)
-        if not spec:
-            return
+        if not spec: return
     else:
         assert default_var is not None, "spec is required to be not None when parsing spec."  # noqa: S101
         spec = default_var
 
-    if spec.startswith("GPU-"):
-        return _parse_list_with_prefix(spec, "GPU-")
-    if spec.startswith("MIG-"):
-        return _parse_list_with_prefix(spec, "MIG-")
+    if spec.startswith("GPU-"): return _parse_list_with_prefix(spec, "GPU-")
+    if spec.startswith("MIG-"): return _parse_list_with_prefix(spec, "MIG-")
 
     # XXX: We to somehow handle cases such as '100m'
     # CUDA_VISIBLE_DEVICES uses something like strtoul
     # which makes `1gpu2,2ampere` is equivalent to `1,2`
     rc: list[int] = []
     for el in spec.split(","):
         x = _strtoul(el.strip())
         # Repeated ordinal results in empty set
-        if x in rc:
-            return []
+        if x in rc: return []
         # Negative value aborts the sequence
-        if x < 0:
-            break
+        if x < 0: break
         rc.append(x)
     return [str(i) for i in rc]
 
 
 def _from_system(cls: type[DynResource]) -> list[str]:
     """Shared mixin implementation for OpenLLM's NVIDIA and AMD resource implementation.
 
@@ -146,88 +128,65 @@
 
                 # refers to https://github.com/RadeonOpenCompute/rocm_smi_lib/blob/master/python_smi_tools/rsmiBindings.py
                 from rsmiBindings import rocmsmi
                 from rsmiBindings import rsmi_status_t
 
                 device_count = c_uint32(0)
                 ret = rocmsmi.rsmi_num_monitor_devices(byref(device_count))
-                if ret == rsmi_status_t.RSMI_STATUS_SUCCESS:
-                    return [str(i) for i in range(device_count.value)]
-                return []
-            except (ModuleNotFoundError, ImportError):
-                # In this case the binary is not found, returning empty list
+                if ret == rsmi_status_t.RSMI_STATUS_SUCCESS: return [str(i) for i in range(device_count.value)]
                 return []
-            finally:
-                sys.path.remove("/opt/rocm/libexec/rocm_smi")
+            # In this case the binary is not found, returning empty list
+            except (ModuleNotFoundError, ImportError): return []
+            finally: sys.path.remove("/opt/rocm/libexec/rocm_smi")
         else:
             try:
                 from cuda import cuda
-
                 err, *_ = cuda.cuInit(0)
                 if err != cuda.CUresult.CUDA_SUCCESS:
                     logger.warning("Failed to initialise CUDA", stacklevel=_STACK_LEVEL)
                     return []
                 _, dev = cuda.cuDeviceGetCount()
                 return [str(i) for i in range(dev)]
-            except (ImportError, RuntimeError):
-                return []
+            except (ImportError, RuntimeError): return []
     return visible_devices
 
 
 @overload
-def _from_spec(cls: type[DynResource], spec: int) -> list[str]:
-    ...
-
-
+def _from_spec(cls: type[DynResource], spec: int) -> list[str]: ...
 @overload
-def _from_spec(cls: type[DynResource], spec: ListIntStr) -> list[str]:
-    ...
-
-
+def _from_spec(cls: type[DynResource], spec: ListIntStr) -> list[str]: ...
 @overload
-def _from_spec(cls: type[DynResource], spec: str) -> list[str]:
-    ...
-
-
+def _from_spec(cls: type[DynResource], spec: str) -> list[str]: ...
 def _from_spec(cls: type[DynResource], spec: t.Any) -> list[str]:
     """Shared mixin implementation for OpenLLM's NVIDIA and AMD resource implementation.
 
     The parser behaves similar to how PyTorch handles CUDA_VISIBLE_DEVICES. This means within
     BentoML's resource configuration, its behaviour is similar to CUDA_VISIBLE_DEVICES.
     """
     if isinstance(spec, int):
-        if spec in (-1, 0):
-            return []
-        if spec < -1:
-            raise ValueError("Spec cannot be < -1.")
+        if spec in (-1, 0): return []
+        if spec < -1: raise ValueError("Spec cannot be < -1.")
         return [str(i) for i in range(spec)]
     elif isinstance(spec, str):
-        if not spec:
-            return []
-        if spec.isdigit():
-            spec = ",".join([str(i) for i in range(_strtoul(spec))])
+        if not spec: return []
+        if spec.isdigit(): spec = ",".join([str(i) for i in range(_strtoul(spec))])
         return _parse_visible_devices(spec, respect_env=False)
-    elif LazyType(ListIntStr).isinstance(spec):
-        return [str(x) for x in spec]
-    else:
-        raise TypeError(
-            f"'{cls.__name__}.from_spec' only supports parsing spec of type int, str, or list, got '{type(spec)}' instead."
-        )
+    elif LazyType(ListIntStr).isinstance(spec): return [str(x) for x in spec]
+    else: raise TypeError(f"'{cls.__name__}.from_spec' only supports parsing spec of type int, str, or list, got '{type(spec)}' instead.")
 
 
 def _raw_device_uuid_nvml() -> list[str] | None:
     """Return list of device UUID as reported by NVML or None if NVML discovery/initialization failed."""
     from ctypes import CDLL
     from ctypes import byref
     from ctypes import c_int
     from ctypes import c_void_p
     from ctypes import create_string_buffer
 
-    try:
-        nvml_h = CDLL("libnvidia-ml.so.1")
+    try: nvml_h = CDLL("libnvidia-ml.so.1")
     except Exception:
         warnings.warn("Failed to find nvidia binding", stacklevel=_STACK_LEVEL)
         return
 
     rc = nvml_h.nvmlInit()
     if rc != 0:
         warnings.warn("Can't initialize NVML", stacklevel=_STACK_LEVEL)
@@ -253,44 +212,34 @@
         uuids.append(buf.raw.decode("ascii").strip("\0"))
     del nvml_h
     return uuids
 
 
 def _validate(cls: type[DynResource], val: list[t.Any]):
     if cls.resource_id == "amd.com/gpu":
-        raise RuntimeError(
-            "AMD GPU validation is not yet supported. Make sure to call 'get_resource(..., validate=False)'"
-        )
-    if not all(isinstance(i, str) for i in val):
-        raise ValueError("Input list should be all string type.")
+        raise RuntimeError("AMD GPU validation is not yet supported. Make sure to call 'get_resource(..., validate=False)'")
+    if not all(isinstance(i, str) for i in val): raise ValueError("Input list should be all string type.")
 
     try:
         from cuda import cuda
 
         err, *_ = cuda.cuInit(0)
         if err != cuda.CUresult.CUDA_SUCCESS:
             raise RuntimeError("Failed to initialise CUDA runtime binding.")
+        # correctly parse handle
+        for el in val:
+            if el.startswith("GPU-") or el.startswith("MIG-"):
+                uuids = _raw_device_uuid_nvml()
+                if uuids is None: raise ValueError("Failed to parse available GPUs UUID")
+                if el not in uuids: raise ValueError(f"Given UUID {el} is not found with available UUID (available: {uuids})")
+            elif el.isdigit():
+                err, _ = cuda.cuDeviceGet(int(el))
+                if err != cuda.CUresult.CUDA_SUCCESS: raise ValueError(f"Failed to get device {el}")
     except (ImportError, RuntimeError):
-        if sys.platform == "darwin":
-            raise RuntimeError("GPU is not available on Darwin system.") from None
-        raise RuntimeError(
-            "Failed to initialise CUDA runtime binding. Make sure that 'cuda-python' is setup correctly."
-        ) from None
-    # correctly parse handle
-    for el in val:
-        if el.startswith("GPU-") or el.startswith("MIG-"):
-            uuids = _raw_device_uuid_nvml()
-            if uuids is None:
-                raise ValueError("Failed to parse available GPUs UUID")
-            if el not in uuids:
-                raise ValueError(f"Given UUID {el} is not found with available UUID (available: {uuids})")
-        elif el.isdigit():
-            err, _ = cuda.cuDeviceGet(int(el))
-            if err != cuda.CUresult.CUDA_SUCCESS:
-                raise ValueError(f"Failed to get device {el}")
+        pass
 
 
 def _make_resource_class(name: str, resource_kind: str, docstring: str) -> type[DynResource]:
     return types.new_class(
         name,
         (DynResource, ReprMixin),
         {"resource_id": resource_kind},
@@ -303,32 +252,59 @@
                 "__repr_keys__": property(lambda _: {"resource_id"}),
                 "__doc__": inspect.cleandoc(docstring),
                 "__module__": "openllm._strategies",
             }
         ),
     )
 
+_TPU_RESOURCE = "cloud-tpus.google.com/v2"
+_AMD_GPU_RESOURCE = "amd.com/gpu"
+_NVIDIA_GPU_RESOURCE = "nvidia.com/gpu"
+_CPU_RESOURCE = "cpu"
 
 NvidiaGpuResource = _make_resource_class(
     "NvidiaGpuResource",
-    "nvidia.com/gpu",
+    _NVIDIA_GPU_RESOURCE,
     """NVIDIA GPU resource.
 
     This is a modified version of internal's BentoML's NvidiaGpuResource
     where it respects and parse CUDA_VISIBLE_DEVICES correctly.""",
 )
 AmdGpuResource = _make_resource_class(
     "AmdGpuResource",
-    "amd.com/gpu",
+    _AMD_GPU_RESOURCE,
     """AMD GPU resource.
 
     Since ROCm will respect CUDA_VISIBLE_DEVICES, the behaviour of from_spec, from_system are similar to
     ``NvidiaGpuResource``. Currently ``validate`` is not yet supported.""",
 )
 
+LiteralResourceSpec = t.Literal["cloud-tpus.google.com/v2", "amd.com/gpu", "nvidia.com/gpu", "cpu"]
+
+# convenient mapping
+def resource_spec(name: t.Literal["tpu", "amd", "nvidia", "cpu"]) ->  LiteralResourceSpec:
+    if name == "tpu": return _TPU_RESOURCE
+    elif name == "amd": return _AMD_GPU_RESOURCE
+    elif name == "nvidia": return _NVIDIA_GPU_RESOURCE
+    elif name == "cpu": return _CPU_RESOURCE
+    else: raise ValueError("Unknown alias. Accepted: ['tpu', 'amd', 'nvidia', 'cpu']")
+@functools.lru_cache
+def available_resource_spec() -> tuple[LiteralResourceSpec, ...]:
+    """This is a utility function helps to determine the available resources from given running system.
+
+    It will first check for TPUs -> AMD GPUS -> NVIDIA GPUS -> CPUs.
+
+    TODO: Supports TPUs
+    """
+    available = ()
+    if len(AmdGpuResource.from_system()) > 0: available += (_AMD_GPU_RESOURCE,)
+    if len(NvidiaGpuResource.from_system()) > 0: available += (_NVIDIA_GPU_RESOURCE,)
+    available += (_CPU_RESOURCE,)
+    return t.cast(t.Tuple[LiteralResourceSpec, ...], available)
+
 
 class CascadingResourceStrategy(bentoml.Strategy, ReprMixin):
     """This is extends the default BentoML strategy where we check for NVIDIA GPU resource -> AMD GPU resource -> CPU resource.
 
     It also respect CUDA_VISIBLE_DEVICES for both AMD and NVIDIA GPU.
     See https://rocm.docs.amd.com/en/develop/understand/gpu_isolation.html#cuda-visible-devices
     for ROCm's support for CUDA_VISIBLE_DEVICES.
```

### Comparing `openllm-0.2.7/src/openllm/_types.py` & `openllm-0.2.8/src/openllm/_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 if t.TYPE_CHECKING:
     import click
     import peft
     import torch
 
     import openllm
+    from openllm._llm import M as _M
+    from openllm._llm import T as _T
     from bentoml._internal.runner.runnable import RunnableMethod
     from bentoml._internal.runner.runner import RunnerMethod
     from bentoml._internal.runner.strategy import Strategy
 
 
 AnyCallable = t.Callable[..., t.Any]
 DictStrAny = dict[str, t.Any]
@@ -69,38 +71,14 @@
     __name__: str
     __click_params__: list[click.Option]
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> O_co:
         ...
 
 
-_MT = t.TypeVar("_MT", covariant=True)
-
-
-class _StubsMixin(t.Generic[_MT], t.Protocol):
-    def save_pretrained(self, save_directory: str, **kwargs: t.Any) -> t.Any:
-        ...
-
-    @classmethod
-    def from_pretrained(cls, pretrained_model_name_or_path: str, *args: t.Any, **kwargs: t.Any) -> _MT:
-        ...
-
-
-class ModelProtocol(_StubsMixin[_MT], t.Protocol):
-    @property
-    def framework(self) -> str:
-        ...
-
-
-class TokenizerProtocol(_StubsMixin[_MT], t.Protocol):
-    @t.override
-    def save_pretrained(self, save_directory: str, **kwargs: t.Any) -> tuple[str]:
-        ...
-
-
 class PeftAdapterOutput(t.TypedDict):
     success: bool
     result: dict[str, peft.PeftConfig]
     error_msg: str
 
 
 class LLMEmbeddings(t.TypedDict):
@@ -113,72 +91,57 @@
     name: str | None
     config: DictStrAny
 
 
 AdaptersMapping = dict[AdapterType, tuple[AdaptersTuple, ...]]
 
 
-class LLMRunnable(bentoml.Runnable):
+class LLMRunnable(bentoml.Runnable, t.Generic[_M, _T]):
     SUPPORTED_RESOURCES = ("amd.com/gpu", "nvidia.com/gpu", "cpu")
     SUPPORTS_CPU_MULTI_THREADING = True
+    model: t.Any
+    __call__: RunnableMethod[LLMRunnable[_M, _T], [str], list[t.Any]]
+    set_adapter: RunnableMethod[LLMRunnable[_M, _T], [str], dict[t.Literal["success", "error_msg"], bool | str]]
+    embeddings: RunnableMethod[LLMRunnable[_M, _T], [list[str]], LLMEmbeddings]
+    generate: RunnableMethod[LLMRunnable[_M, _T], [str], list[t.Any]]
+    generate_one: RunnableMethod[LLMRunnable[_M, _T], [str, list[str]], t.Sequence[dict[t.Literal["generated_text"], str]]]
+    generate_iterator: RunnableMethod[LLMRunnable[_M, _T], [str], t.Generator[t.Any, None, None]]
 
-    model: ModelProtocol[t.Any]
-
-    set_adapter: RunnableMethod[LLMRunnable, [str], dict[t.Literal["success", "error_msg"], bool | str]]
-    __call__: RunnableMethod[LLMRunnable, [str], list[t.Any]]
-    embeddings: RunnableMethod[LLMRunnable, [list[str]], LLMEmbeddings]
-    generate: RunnableMethod[LLMRunnable, [str], list[t.Any]]
-    generate_one: RunnableMethod[LLMRunnable, [str, list[str]], t.Sequence[dict[t.Literal["generated_text"], str]]]
-    generate_iterator: RunnableMethod[LLMRunnable, [str], t.Generator[t.Any, None, None]]
 
-
-class LLMRunner(bentoml.Runner):
+class LLMRunner(bentoml.Runner, t.Generic[_M, _T]):
     __doc__: str
     __module__: str
     llm_type: str
     identifying_params: dict[str, t.Any]
-    llm: openllm.LLM[t.Any, t.Any]
-    model: ModelProtocol[t.Any]
+    llm: openllm.LLM[_M, _T]
+    model: _M
     config: openllm.LLMConfig
-
-    embeddings: RunnerMethod[LLMRunnable, [list[str]], LLMEmbeddings]
-    generate: RunnerMethod[LLMRunnable, [str], list[t.Any]]
-    generate_one: RunnerMethod[LLMRunnable, [str, list[str]], t.Sequence[dict[t.Literal["generated_text"], str]]]
-    generate_iterator: RunnerMethod[LLMRunnable, [str], t.Generator[t.Any, None, None]]
-
+    implementation: LiteralRuntime
+    supports_embeddings: bool
+    supports_hf_agent: bool
+    has_adapters: bool
+    embeddings: RunnerMethod[LLMRunnable[_M, _T], [list[str]], LLMEmbeddings]
+    generate: RunnerMethod[LLMRunnable[_M, _T], [str], list[t.Any]]
+    generate_one: RunnerMethod[LLMRunnable[_M, _T], [str, list[str]], t.Sequence[dict[t.Literal["generated_text"], str]]]
+    generate_iterator: RunnerMethod[LLMRunnable[_M, _T], [str], t.Generator[t.Any, None, None]]
     def __init__(
         self,
-        runnable_class: type[LLMRunnable],
+        runnable_class: type[LLMRunnable[_M, _T]],
         *,
         runnable_init_params: dict[str, t.Any] | None = ...,
         name: str | None = ...,
         scheduling_strategy: type[Strategy] = ...,
         models: list[bentoml.Model] | None = ...,
         max_batch_size: int | None = ...,
         max_latency_ms: int | None = ...,
         method_configs: dict[str, dict[str, int]] | None = ...,
         embedded: bool = False,
-    ) -> None:
-        ...
-
-    def __call__(self, prompt: str, **attrs: t.Any) -> t.Any:
-        ...
-
-    def embed(self, prompt: str | list[str]) -> LLMEmbeddings:
-        ...
-
-    def run(self, prompt: str, **attrs: t.Any) -> t.Any:
-        ...
-
-    async def async_run(self, prompt: str, **attrs: t.Any) -> t.Any:
-        ...
-
-    def download_model(self) -> bentoml.Model:
-        ...
-
+    ) -> None: ...
+    def __call__(self, prompt: str, **attrs: t.Any) -> t.Any: ...
+    def embed(self, prompt: str | list[str]) -> LLMEmbeddings: ...
+    def run(self, prompt: str, **attrs: t.Any) -> t.Any: ...
+    async def async_run(self, prompt: str, **attrs: t.Any) -> t.Any: ...
+    def download_model(self) -> bentoml.Model: ...
     @property
-    def peft_adapters(self) -> PeftAdapterOutput:
-        ...
-
+    def peft_adapters(self) -> PeftAdapterOutput: ...
     @property
-    def __repr_keys__(self) -> set[str]:
-        ...
+    def __repr_keys__(self) -> set[str]: ...
```

### Comparing `openllm-0.2.7/src/openllm/cli.py` & `openllm-0.2.8/src/openllm/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 Import any LLM into local store
 ```python
 bentomodel = openllm.import_model("falcon", model_id='tiiuae/falcon-7b-instruct')
 ```
 """
 from __future__ import annotations
 import functools
+import http.client
 import importlib.machinery
 import importlib.util
 import inspect
 import itertools
 import logging
 import os
 import pkgutil
@@ -49,14 +50,15 @@
 import traceback
 import typing as t
 
 import attr
 import click
 import click_option_group as cog
 import fs
+import fs.copy
 import fs.errors
 import inflection
 import orjson
 import yaml
 from bentoml_cli.utils import BentoMLCommandGroup
 from bentoml_cli.utils import opt_callback
 from simple_di import Provide
@@ -174,15 +176,15 @@
     call = click.echo
     if _with_style:
         attrs["fg"] = fg if not get_debug_mode() else None
         call = click.secho
     call(text, **attrs)
 
 
-def output_option(f: t.Callable[[FC], FC], *, factory: t.Any = click) -> t.Callable[[FC], FC]:
+def output_option(f: _AnyCallable, *, factory: t.Any = click) -> t.Callable[[FC], FC]:
     return factory.option(
         "-o",
         "--output",
         "output",
         type=click.Choice(["json", "pretty", "porcelain"]),
         default="pretty",
         help="Showing output type.",
@@ -215,14 +217,23 @@
         "--model-version",
         type=click.STRING,
         default=None,
         help="Optional model version to save for this model. It will be inferred automatically from model-id.",
     )
 
 
+def workers_per_resource_callback(ctx: click.Context, param: click.Parameter, value: str | None) -> str | None:
+    if value is None: return value
+    value = inflection.underscore(value)
+    if value in {"round_robin", "conserved"}: return value
+    else:
+        try: float(value)  # type: ignore[arg-type]
+        except ValueError: ctx.fail(f"'workers_per_resource' only accept '{_wpr_strategies}' as possible strategies, otherwise pass in float.")
+        else: return value
+
 def workers_per_resource_option(factory: t.Any, build: bool = False) -> t.Callable[[FC], FC]:
     help_str = """Number of workers per resource assigned.
     See https://docs.bentoml.org/en/latest/guides/scheduling.html#resource-scheduling-strategy
     for more information. By default, this is set to 1.
 
     **Note**: ``--workers-per-resource`` will also accept the following strategies:
 
@@ -231,30 +242,25 @@
     - ``conserved``: This will determine the number of available GPU resources, and only assign one worker for the LLMRunner. For example, if ther are 4 GPUs available, then ``conserved`` is equivalent to ``--workers-per-resource 0.25``.
     """
     if build:
         help_str += """\n
     **Note**: The workers value passed into 'build' will determine how the LLM can
     be provisioned in Kubernetes as well as in standalone container. This will
     ensure it has the same effect with 'openllm start --workers ...'"""
-    return factory.option("--workers-per-resource", default=None, help=help_str, type=str, required=False)
+    return factory.option("--workers-per-resource", default=None, help=help_str, callback=workers_per_resource_callback, type=str, required=False)
 
 
 def quantize_option(factory: t.Any, build: bool = False, model_env: EnvVarMixin | None = None) -> t.Callable[[FC], FC]:
     envvar = None
     if model_env is not None:
         envvar = model_env.quantize
     help_str = (
         "Running this model in quantized mode." if not build else "Set quantization mode for serving in deployment."
     )
-    help_str += """\n
-
-    GPTQ is currently working in progress and will be available soon.
-
-    NOTE: Quantization is only available for PyTorch models.
-    """
+    help_str += "\nNOTE: Quantization is only available for PyTorch models. "
     return factory.option(
         "--quantise",
         "--quantize",
         "quantize",
         type=click.Choice(["int8", "int4", "gptq"]),
         default=None,
         help=help_str,
@@ -292,16 +298,14 @@
         show_default=True,
         show_envvar=True,
         envvar="OPENLLM_SERIALIZATION",
     )
 
 
 _adapter_mapping_key = "adapter_map"
-
-
 def _id_callback(ctx: click.Context, _: click.Parameter, value: tuple[str, ...] | None) -> None:
     if not value:
         return None
     if _adapter_mapping_key not in ctx.params:
         ctx.params[_adapter_mapping_key] = {}
     for v in value:
         adapter_id, *adapter_name = v.rsplit(":", maxsplit=1)
@@ -314,95 +318,61 @@
         ctx.params[_adapter_mapping_key][adapter_id] = adapter_name[0] if len(adapter_name) > 0 else None
     return None
 
 
 @attr.define
 class CliContext:
     cloud_context: str | None = attr.field(default=None, converter=attr.converters.default_if_none("default"))
-
-    def with_options(self, **attrs: t.Any) -> t.Self:
-        return attr.evolve(self, **attrs)
+    def with_options(self, **attrs: t.Any) -> t.Self: return attr.evolve(self, **attrs)
 
 
 class OpenLLMCommandGroup(BentoMLCommandGroup):
     NUMBER_OF_COMMON_PARAMS = 5  # parameters in common_params + 1 faked group option header
-
     @staticmethod
     def common_params(f: FC) -> t.Callable[[FC], FC]:
         """This is not supposed to be used with unprocessed click function.
 
         This should be used a the last currying from common_params -> usage_tracking -> exception_handling.
         """
         # The following logics is similar to one of BentoMLCommandGroup
 
         from bentoml._internal.configuration import DEBUG_ENV_VAR
         from bentoml._internal.configuration import QUIET_ENV_VAR
 
         @cog.optgroup.group("Global options")
-        @cog.optgroup.option(
-            "-q", "--quiet", envvar=QUIET_ENV_VAR, is_flag=True, default=False, help="Suppress all output."
-        )
-        @cog.optgroup.option(
-            "--debug",
-            "--verbose",
-            "debug",
-            envvar=DEBUG_ENV_VAR,
-            is_flag=True,
-            default=False,
-            help="Print out debug logs.",
-        )
-        @cog.optgroup.option(
-            "--do-not-track",
-            is_flag=True,
-            default=False,
-            envvar=analytics.OPENLLM_DO_NOT_TRACK,
-            help="Do not send usage info",
-        )
-        @cog.optgroup.option(
-            "--context",
-            "cloud_context",
-            type=click.STRING,
-            default=None,
-            help="BentoCloud context name.",
-        )
+        @cog.optgroup.option("-q", "--quiet", envvar=QUIET_ENV_VAR, is_flag=True, default=False, help="Suppress all output.")
+        @cog.optgroup.option( "--debug", "--verbose", "debug", envvar=DEBUG_ENV_VAR, is_flag=True, default=False, help="Print out debug logs.")
+        @cog.optgroup.option("--do-not-track", is_flag=True, default=False, envvar=analytics.OPENLLM_DO_NOT_TRACK, help="Do not send usage info")
+        @cog.optgroup.option( "--context", "cloud_context", type=click.STRING, default=None, help="BentoCloud context name.")
         @click.pass_context
         @functools.wraps(f)
-        def wrapper(
-            ctx: click.Context, quiet: bool, debug: bool, cloud_context: str | None, *args: P.args, **attrs: P.kwargs
-        ) -> t.Any:
+        def wrapper(ctx: click.Context, quiet: bool, debug: bool, cloud_context: str | None, *args: P.args, **attrs: P.kwargs) -> t.Any:
             ctx.obj = CliContext(cloud_context=cloud_context)
             if quiet:
                 set_quiet_mode(True)
-                if debug:
-                    logger.warning("'--quiet' passed; ignoring '--verbose/--debug'")
-            elif debug:
-                set_debug_mode(True)
-
+                if debug: logger.warning("'--quiet' passed; ignoring '--verbose/--debug'")
+            elif debug: set_debug_mode(True)
             configure_logging()
-
             return f(*args, **attrs)
-
         return wrapper
 
     @staticmethod
     def usage_tracking(func: _AnyCallable, group: click.Group, **attrs: t.Any) -> _AnyCallable:
         """This is not supposed to be used with unprocessed click function.
 
         This should be used a the last currying from common_params -> usage_tracking -> exception_handling.
         """
         command_name = attrs.get("name", func.__name__)
 
         @functools.wraps(func)
         def wrapper(do_not_track: bool, *args: P.args, **attrs: P.kwargs) -> t.Any:
             if do_not_track:
-                with analytics.set_bentoml_tracking():
-                    return func(*args, **attrs)
+                with analytics.set_bentoml_tracking(): return func(*args, **attrs)
 
             start_time = time.time_ns()
-
             with analytics.set_bentoml_tracking():
                 assert group.name is not None, "group.name should not be None"
                 event = analytics.OpenllmCliEvent(cmd_group=group.name, cmd_name=command_name)
                 try:
                     return_value = func(*args, **attrs)
                     duration_in_ms = (time.time_ns() - start_time) / 1e6
                     event.duration_in_ms = duration_in_ms
@@ -424,102 +394,69 @@
 
         This should be used a the last currying from common_params -> usage_tracking -> exception_handling.
         """
         command_name = attrs.get("name", func.__name__)
 
         @functools.wraps(func)
         def wrapper(*args: P.args, **attrs: P.kwargs) -> t.Any:
-            try:
-                return func(*args, **attrs)
+            try: return func(*args, **attrs)
             except OpenLLMException as err:
-                raise click.ClickException(
-                    click.style(f"[{group.name}] '{command_name}' failed: " + err.message, fg="red")
-                ) from err
-            except KeyboardInterrupt:  # NOTE: silience KeyboardInterrupt
-                pass
-
+                raise click.ClickException(click.style(f"[{group.name}] '{command_name}' failed: " + err.message, fg="red")) from err
+            except KeyboardInterrupt: pass
         return t.cast("ClickFunctionWrapper[..., t.Any]", wrapper)
 
     def get_command(self, ctx: click.Context, cmd_name: str) -> click.Command | None:
         cmd_name = self.resolve_alias(cmd_name)
-        if ctx.command.name == "start":
-            try:
-                return _cached_http[cmd_name]
+        _mapping = {"start": _cached_http, "start-grpc": _cached_grpc}
+        if ctx.command.name in _mapping:
+            try: return _mapping[ctx.command.name][cmd_name]
             except KeyError:
-                # support start from a bento
+                # TODO: support start from a bento
                 try:
-                    return start_command_factory(bentoml.get(cmd_name), _context_settings=_CONTEXT_SETTINGS)
-                except bentoml.exceptions.NotFound:
-                    pass
-                raise click.BadArgumentUsage(
-                    f"{cmd_name} is not a valid model identifier supported by OpenLLM."
-                ) from None
-        elif ctx.command.name == "start-grpc":
-            try:
-                return _cached_grpc[cmd_name]
-            except KeyError:
-                # support start from a bento
-                try:
-                    return start_command_factory(
-                        bentoml.get(cmd_name), _context_settings=_CONTEXT_SETTINGS, _serve_grpc=True
-                    )
-                except bentoml.exceptions.NotFound:
-                    pass
-                raise click.BadArgumentUsage(
-                    f"{cmd_name} is not a valid model identifier supported by OpenLLM."
-                ) from None
+                    bentoml.get(cmd_name)
+                    raise click.ClickException(f"'openllm start {cmd_name}' is currently disabled for the time being. Please let us know if you need this feature by opening an issue on GitHub.")
+                except bentoml.exceptions.NotFound: pass
+                raise click.BadArgumentUsage(f"{cmd_name} is not a valid model identifier supported by OpenLLM.") from None
         return super().get_command(ctx, cmd_name)
 
     def list_commands(self, ctx: click.Context) -> list[str]:
-        if ctx.command.name == "start" or ctx.command.name == "start-grpc":
-            return list(openllm.CONFIG_MAPPING.keys())
-
+        if ctx.command.name in {"start", "start-grpc"}: return list(openllm.CONFIG_MAPPING.keys())
         return super().list_commands(ctx)
 
     @override
     def command(self, *args: t.Any, **attrs: t.Any):
         """Override the default 'cli.command' with supports for aliases for given command, and it wraps the implementation with common parameters."""
-        if "context_settings" not in attrs:
-            attrs["context_settings"] = {}
-        if "max_content_width" not in attrs["context_settings"]:
-            attrs["context_settings"]["max_content_width"] = 120
+        if "context_settings" not in attrs: attrs["context_settings"] = {}
+        if "max_content_width" not in attrs["context_settings"]: attrs["context_settings"]["max_content_width"] = 120
         aliases = attrs.pop("aliases", None)
 
         def wrapper(f: _AnyCallable) -> click.Command:
             name = f.__name__.lower()
-            if name.endswith("_command"):
-                name = name[:-8]
+            if name.endswith("_command"): name = name[:-8]
             name = name.replace("_", "-")
             attrs.setdefault("help", inspect.getdoc(f))
             attrs.setdefault("name", name)
 
             # Wrap implementation withc common parameters
             wrapped = self.common_params(f)
             # Wrap into OpenLLM tracking
             wrapped = self.usage_tracking(wrapped, self, **attrs)
             # Wrap into exception handling
             wrapped = self.exception_handling(wrapped, self, **attrs)
 
             # move common parameters to end of the parameters list
-            wrapped.__click_params__ = (
-                wrapped.__click_params__[-self.NUMBER_OF_COMMON_PARAMS :]
-                + wrapped.__click_params__[: -self.NUMBER_OF_COMMON_PARAMS]
-            )
-
-            # NOTE: we need to call super of super to avoid conflict with BentoMLCommandGroup command
-            # setup
+            wrapped.__click_params__ = wrapped.__click_params__[-self.NUMBER_OF_COMMON_PARAMS:] + wrapped.__click_params__[:-self.NUMBER_OF_COMMON_PARAMS]
+            # NOTE: we need to call super of super to avoid conflict with BentoMLCommandGroup command setup
             cmd = super(BentoMLCommandGroup, self).command(*args, **attrs)(wrapped)
             # NOTE: add aliases to a given commands if it is specified.
             if aliases is not None:
                 assert cmd.name
                 self._commands[cmd.name] = aliases
                 self._aliases.update({alias: cmd.name for alias in aliases})
-
             return cmd
-
         return wrapper
 
 
 @click.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="openllm")
 @click.version_option(__version__, "--version", "-v")
 def cli() -> None:
     """\b
@@ -570,65 +507,47 @@
 
     command = "serve" if not serve_grpc else "serve-grpc"
     group = cog.optgroup.group(
         f"Start a {'HTTP' if not serve_grpc else 'gRPC'} server options",
         help=f"Related to serving the model [synonymous to `bentoml {'serve-http' if not serve_grpc else command }`]",
     )
 
-    def decorator(f: t.Callable[t.Concatenate[int, str | None, P], openllm.LLMConfig]):
+    def decorator(f: t.Callable[t.Concatenate[int, str | None, P], openllm.LLMConfig]) -> t.Callable[[FC], FC]:
         serve_command = cli.commands[command]
         # The first variable is the argument bento
         # The last five is from BentoMLCommandGroup.NUMBER_OF_COMMON_PARAMS
-        serve_options = [
-            p
-            for p in serve_command.params[1 : -BentoMLCommandGroup.NUMBER_OF_COMMON_PARAMS]
-            if p.name not in _IGNORED_OPTIONS
-        ]
+        serve_options = [p for p in serve_command.params[1 :-BentoMLCommandGroup.NUMBER_OF_COMMON_PARAMS] if p.name not in _IGNORED_OPTIONS]
         for options in reversed(serve_options):
             attrs = options.to_info_dict()
             # we don't need param_type_name, since it should all be options
             attrs.pop("param_type_name")
             # name is not a valid args
             attrs.pop("name")
             # type can be determine from default value
             attrs.pop("type")
             param_decls = (*attrs.pop("opts"), *attrs.pop("secondary_opts"))
             f = cog.optgroup.option(*param_decls, **attrs)(f)
-
         return group(f)
-
     return decorator
 
 
 _http_server_args = parse_serve_args(False)
 _grpc_server_args = parse_serve_args(True)
 
 
-def start_decorator(
-    llm_config: openllm.LLMConfig, serve_grpc: bool = False
-) -> t.Callable[[_AnyCallable], t.Callable[[FC], FC]]:
+def start_decorator(llm_config: openllm.LLMConfig, serve_grpc: bool = False) -> t.Callable[[_AnyCallable], t.Callable[[FC], FC]]:
     opts = [
         llm_config.to_click_options,
         _http_server_args if not serve_grpc else _grpc_server_args,
         cog.optgroup.group("General LLM Options", help="The following options are related to running the LLM Server."),
-        cog.optgroup.option(
-            "--server-timeout",
-            type=int,
-            default=None,
-            help="Server timeout in seconds",
-        ),
-        workers_per_resource_option(cog.optgroup),
         model_id_option(cog.optgroup, model_env=llm_config["env"]),
         model_version_option(cog.optgroup),
-        cog.optgroup.option(
-            "--fast",
-            is_flag=True,
-            default=False,
-            help="Bypass auto model checks and setup. This option is ahead-of-serving time.",
-        ),
+        cog.optgroup.option("--server-timeout", type=int, default=None, help="Server timeout in seconds"),
+        workers_per_resource_option(cog.optgroup),
+        cog.optgroup.option("--fast", is_flag=True, default=False, help="Bypass auto model checks and setup. This option is ahead-of-serving time."),
         cog.optgroup.group(
             "LLM Optimization Options",
             help="""\
     These options are related for dynamic optimization on the fly. Current supported strategies:
 
     - int8: Quantize the model with 8bit (bitsandbytes required)
 
@@ -646,29 +565,16 @@
 
     The following are currently being worked on:
 
     - DeepSpeed Inference: [link](https://www.deepspeed.ai/inference/)
 
       """,
         ),
-        cog.optgroup.option(
-            "--device",
-            type=dantic.CUDA,
-            multiple=True,
-            envvar="CUDA_VISIBLE_DEVICES",
-            callback=parse_device_callback,
-            help=f"Assign GPU devices (if available) for {llm_config['model_name']}.",
-            show_envvar=True,
-        ),
-        cog.optgroup.option(
-            "--runtime",
-            type=click.Choice(["ggml", "transformers"]),
-            default="transformers",
-            help="The runtime to use for the given model. Default is transformers.",
-        ),
+        cog.optgroup.option("--device", type=dantic.CUDA, multiple=True, envvar="CUDA_VISIBLE_DEVICES", callback=parse_device_callback, help=f"Assign GPU devices (if available) for {llm_config['model_name']}.", show_envvar=True),
+        cog.optgroup.option("--runtime", type=click.Choice(["ggml", "transformers"]), default="transformers", help="The runtime to use for the given model. Default is transformers."),
         quantize_option(cog.optgroup, model_env=llm_config["env"]),
         bettertransformer_option(cog.optgroup, model_env=llm_config["env"]),
         serialisation_option(cog.optgroup),
         cog.optgroup.group(
             "Fine-tuning related options",
             help="""\
     Note that the argument `--adapter-id` can accept the following format:
@@ -682,22 +588,15 @@
     ```bash
 
     $ openllm start opt --adapter-id /path/to/adapter_dir --adapter-id remote/adapter:eng_lora
 
     ```
     """,
         ),
-        cog.optgroup.option(
-            "--adapter-id",
-            default=None,
-            help="Optional name or path for given LoRA adapter" + f" to wrap '{llm_config['model_name']}'",
-            multiple=True,
-            callback=_id_callback,
-            metavar="[PATH | [remote/][adapter_name:]adapter_id][, ...]",
-        ),
+        cog.optgroup.option("--adapter-id", default=None, help="Optional name or path for given LoRA adapter" + f" to wrap '{llm_config['model_name']}'", multiple=True, callback=_id_callback, metavar="[PATH | [remote/][adapter_name:]adapter_id][, ...]"),
         click.option("--return-process", is_flag=True, default=False, help="Internal use only.", hidden=True),
     ]
 
     def decorator(f: _AnyCallable) -> _AnyCallable:
         for opt in reversed(opts):
             f = opt(f)
         return f
@@ -709,77 +608,46 @@
     config: openllm.LLMConfig,
     server_timeout: int,
     workers_per_resource: float,
     device: tuple[str, ...] | None,
     environ: DictStrAny,
 ) -> DictStrAny:
     _bentoml_config_options_env = environ.pop("BENTOML_CONFIG_OPTIONS", "")
-    _bentoml_config_options_opts = [
-        "tracing.sample_rate=1.0",
-        f"api_server.traffic.timeout={server_timeout}",
-        f'runners."llm-{config["start_name"]}-runner".traffic.timeout={config["timeout"]}',
-        f'runners."llm-{config["start_name"]}-runner".workers_per_resource={workers_per_resource}',
-    ]
+    _bentoml_config_options_opts = ["tracing.sample_rate=1.0", f"api_server.traffic.timeout={server_timeout}", f'runners."llm-{config["start_name"]}-runner".traffic.timeout={config["timeout"]}', f'runners."llm-{config["start_name"]}-runner".workers_per_resource={workers_per_resource}']
     if device:
-        if len(device) > 1:
-            for idx, dev in enumerate(device):
-                _bentoml_config_options_opts.append(
-                    f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"[{idx}]={dev}'
-                )
-        else:
-            _bentoml_config_options_opts.append(
-                f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"=[{device[0]}]'
-            )
-
+        if len(device) > 1: _bentoml_config_options_opts.extend([f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"[{idx}]={dev}' for idx, dev in enumerate(device)])
+        else: _bentoml_config_options_opts.append(f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"=[{device[0]}]')
     _bentoml_config_options_env += " " if _bentoml_config_options_env else "" + " ".join(_bentoml_config_options_opts)
     environ["BENTOML_CONFIG_OPTIONS"] = _bentoml_config_options_env
     return environ
 
 
-def start_command_factory(
-    model_name_or_bento: str | bentoml.Bento,
-    _context_settings: DictStrAny | None = None,
-    _serve_grpc: bool = False,
-) -> click.Command:
+_wpr_strategies = {"round_robin", "conserved"}
+
+def start_command_factory(model: str, _context_settings: DictStrAny | None = None, _serve_grpc: bool = False) -> click.Command:
     """Generate a 'click.Command' for any given LLM.
 
     Args:
-        model_name_or_bento: The name of the model or the ``bentoml.Bento`` instance.
+        model: The name of the model or the ``bentoml.Bento`` instance.
 
     Returns:
         The click.Command for starting the model server
 
     Note that the internal commands will return the llm_config and a boolean determine
     whether the server is run with GPU or not.
     """
     group = start_command if not _serve_grpc else start_grpc_command
+    llm_config = openllm.AutoConfig.for_model(model)
 
-    if isinstance(model_name_or_bento, bentoml.Bento):
-        if "start_name" not in model_name_or_bento.info.labels:
-            raise click.BadOptionUsage(
-                "model_name",
-                f"'{model_name_or_bento.tag}' is built with older version of OpenLLM and not supported with 'openllm start'. Please use 'bentoml {'serve-http' if not _serve_grpc else 'serve-grpc'} {model_name_or_bento.tag!s}' instead.",
-            )
-        llm_config = openllm.AutoConfig.infer_class_from_name(
-            model_name_or_bento.info.labels["start_name"]
-        ).model_construct_json(model_name_or_bento.info.labels["configuration"])
-        return start_bento(group, model_name_or_bento, llm_config, _serve_grpc, context_settings=_CONTEXT_SETTINGS)
-    else:
-        llm_config = openllm.AutoConfig.for_model(model_name_or_bento)
-
-        return start_model(
-            group,
-            model_name_or_bento,
-            llm_config,
-            _serve_grpc,
-            name=llm_config["model_name"],
-            context_settings=_context_settings or {},
-            short_help=f"Start a LLMServer for '{model_name_or_bento}'",
-            aliases=[llm_config["start_name"]] if llm_config["name_type"] == "dasherize" else None,
-            help=f"""\
+    command_attrs: DictStrAny = dict(
+        name=llm_config["model_name"],
+        context_settings=_context_settings or {},
+        short_help=f"Start a LLMServer for '{model}'",
+        aliases=[llm_config["start_name"]] if llm_config["name_type"] == "dasherize" else None,
+        help=f"""\
 {llm_config['env'].start_docstring}
 
 \b
 Note: ``{llm_config['start_name']}`` can also be run with any other models available on HuggingFace
 or fine-tuned variants as long as it belongs to the architecture generation ``{llm_config['architecture']}`` (trust_remote_code={llm_config['trust_remote_code']}).
 
 \b
@@ -790,440 +658,182 @@
 
 \b
 Available official model_id(s): [default: {llm_config['default_id']}]
 
 \b
 {orjson.dumps(llm_config['model_ids'], option=orjson.OPT_INDENT_2).decode()}
 """,
-        )
-
-
-def start_bento_docstring(bento: bentoml.Bento, llm_config: openllm.LLMConfig, serve_grpc: bool) -> str:
-    environ = parse_config_options(llm_config, llm_config["timeout"], llm_config["workers_per_resource"], None, {})
-
-    serve_cmd_envvar = {
-        "OPENLLM_MODEL_ID": f"$(bentoml models get {bento.info.labels['_framework']}-{bento.info.labels['_type']} -o path)",
-        "BENTOML_DEBUG": get_debug_mode(),
-        "BENTOML_CONFIG_OPTIONS": environ["BENTOML_CONFIG_OPTIONS"],
-    }
-
-    return f"""\
-Start {bento!r} with OpenLLM.
-
-\b
-This is a lightwrapper around 'bentoml serve' to provide nicer interaction with LLM Bentos.
-
-\b
-The equivalent 'bentoml {'serve' if not serve_grpc else 'serve-grpc'}' command:
-
-\b
-```bash
-$ {' '.join([f'{k}={v}' for k, v in serve_cmd_envvar.items()])} bentoml {'serve-http' if not serve_grpc else 'serve-grpc'} {bento.tag!s}
-```
-
-\b
-> Note that if you want to enable GPU with 'bentoml serve', add the following to BENTOML_CONFIG_OPTIONS:
-
-\b
-If you have more than 1 GPU:
-
-\b
-```bash
-BENTOML_CONFIG_OPTIONS += ' runners."llm-{llm_config['start_name']}-runner".resources."nvidia.com/gpu"[<gpu_idx>]=<gpu_device_id>'
-```
-
-Make sure to adjust `workers_per_resource` in BENTOML_CONFIG_OPTIONS accordingly. See https://docs.bentoml.com/en/latest/guides/scheduling.html
-for more information.
-
-\b
-If you only have 1 GPU:
-
-\b
-```bash
-BENTOML_CONFIG_OPTIONS += ' runners."llm-{llm_config['start_name']}-runner".resources."nvidia.com/gpu"=[<gpu_device_id>]'
-```
-"""
-
-
-def noop_command(
-    group: click.Group, llm_config: openllm.LLMConfig, reason: str, **command_attrs: t.Any
-) -> click.Command:
-    context_settings = command_attrs.pop("context_settings", {})
-    context_settings["ignore_unknown_options"] = True
-    context_settings["allow_extra_args"] = True
-    command_attrs["context_settings"] = context_settings
-
-    # NOTE: The model requires GPU, therefore we will return a dummy command
-    @group.command(**command_attrs)
-    def noop(**_: t.Any) -> openllm.LLMConfig:
-        _echo(reason, fg="red")
-        analytics.track_start_init(llm_config)
-        return llm_config
-
-    return noop
-
-
-def prerequisite_check(
-    ctx: click.Context,
-    llm_config: openllm.LLMConfig,
-    quantize: t.LiteralString | None,
-    adapter_map: dict[str, str | None] | None,
-    num_workers: int,
-) -> None:
-    if quantize:
-        if device_count() < 1:
-            _echo("Quantization requires at least 1 GPU (got None)", fg="red")
-            ctx.exit(1)
-
-    if adapter_map and not is_peft_available():
-        _echo(
-            "Using adapter requires 'peft' to be available. Make sure to install with 'pip install \"openllm[fine-tune]\"'",
-            fg="red",
-        )
-        ctx.exit(1)
-
-    requirements = llm_config["requirements"]
-    if requirements is not None and len(requirements) > 0:
-        missing_requirements = [i for i in requirements if importlib.util.find_spec(i) is None]
-        if len(missing_requirements) > 0:
-            _echo(
-                f"Make sure to have the following dependencies available: {missing_requirements}",
-                fg="yellow",
-            )
-
-    if num_workers > 1 and device_count() < num_workers:
-        raise click.BadOptionUsage(
-            "workers_per_resource",
-            f"# of workers is infered to {num_workers} GPUs per runner worker, while there are only"
-            f"'{device_count()}' for inference. (Tip: Try again using '--workers-per-resource={1/device_count()}')",
-            ctx=ctx,
-        )
-
-
-_wpr_strategies = {"round_robin", "conserved"}
-
-
-def start_bento(
-    group: click.Group,
-    bento: bentoml.Bento,
-    llm_config: openllm.LLMConfig,
-    serve_grpc: bool,
-    **command_attrs: t.Any,
-) -> click.Command:
-    if llm_config["requires_gpu"] and device_count() < 1:
-        return noop_command(
-            group, llm_config, f"No GPU available, while {bento!r} requires GPU to run.", **command_attrs
-        )
-
-    command_attrs["help"] = start_bento_docstring(bento, llm_config, serve_grpc)
-
-    # Now we have to format the model_id accordingly based on the model_fs
-    model_type = bento.info.labels["_type"]
-    model_framework = bento.info.labels["_framework"]
-    # the models should have the type
-    try:
-        model_store = ModelStore(bento._fs.opendir("models"))
-        model = model_store.get(f"{model_framework}-{model_type}")
-    except fs.errors.ResourceNotFound:
-        # new behaviour with BentoML models
-        _model_store = BentoMLContainer.model_store.get()
-        model = _model_store.get(f"{model_framework}-{model_type}")
-    except bentoml.exceptions.NotFound:
-        raise OpenLLMException(f"Failed to find models for {llm_config['start_name']}") from None
-
-    @group.command(**command_attrs)
-    @start_decorator(llm_config, serve_grpc=serve_grpc)
-    @click.pass_context
-    def start_cmd(
-        ctx: click.Context,
-        server_timeout: int,
-        model_id: str | None,
-        model_version: str | None,
-        workers_per_resource: t.LiteralString | float,
-        device: tuple[str, ...],
-        quantize: t.Literal["int8", "int4", "gptq"] | None,
-        bettertransformer: bool | None,
-        runtime: t.Literal["ggml", "transformers"],
-        fast: bool,
-        adapter_id: str | None,
-        return_process: bool,
-        serialisation_format: t.Literal["safetensors", "legacy"],
-        **attrs: t.Any,
-    ) -> openllm.LLMConfig | subprocess.Popen[bytes]:
-        if model_id is not None:
-            _echo("'model_id' has no effect when starting a BentoLLM", fg="yellow")
-
-        adapter_map: dict[str, str | None] | None = attrs.pop(_adapter_mapping_key, None)
-
-        config, server_attrs = llm_config.model_validate_click(**attrs)
-        server_timeout = first_not_none(server_timeout, default=config["timeout"])
-
-        server_attrs.update({"working_dir": os.path.dirname(__file__), "timeout": server_timeout})
-        if serve_grpc:
-            server_attrs["grpc_protocol_version"] = "v1"
-        # NOTE: currently, theres no development args in bentoml.Server. To be fixed upstream.
-        development = server_attrs.pop("development")
-        server_attrs.setdefault("production", not development)
-
-        workers_per_resource = first_not_none(workers_per_resource, default=config["workers_per_resource"])
-
-        if isinstance(workers_per_resource, str):
-            if workers_per_resource == "round_robin":
-                workers_per_resource = 1.0
-            elif workers_per_resource == "conserved":
-                available_gpu = device if device else available_devices()
-                workers_per_resource = 1.0 if len(available_gpu) == 0 else float(1 / len(available_gpu))
-            else:
-                try:
-                    workers_per_resource = float(workers_per_resource)
-                except ValueError:
-                    ctx.fail(f"'workers_per_resource' only accept '{_wpr_strategies}' as possible strategies.")
-
-        num_workers = int(1 / workers_per_resource)
-
-        # Create a new model env to work with the envvar during CLI invocation
-        env = EnvVarMixin(
-            config["model_name"],
-            config["default_implementation"],
-            bettertransformer=bettertransformer,
-            quantize=quantize,
-            runtime=runtime,
-        )
-
-        prerequisite_check(ctx, config, quantize, adapter_map, num_workers)
-
-        # NOTE: This is to set current configuration
-        start_env = os.environ.copy()
-        start_env = parse_config_options(config, server_timeout, workers_per_resource, device, start_env)
-
-        if fast:
-            _echo(f"Fast mode has no effects when 'start' {bento.tag!s}", fg="yellow")
-
-        start_env.update(
-            {
-                env.framework: env.framework_value,
-                env.config: config.model_dump_json().decode(),
-                env.runtime: env.runtime_value,
-                "BENTOML_DEBUG": str(not get_quiet_mode()),
-                "BENTOML_HOME": os.environ.get("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
-                "OPENLLM_MODEL_ID": model.path,
-                "OPENLLM_SERIALIZATION": serialisation_format,
-            }
-        )
-
-        if adapter_map:
-            _echo(f"OpenLLM will convert '{bento.tag!s}' to use provided adapters layers: {list(adapter_map)}")
-        start_env["OPENLLM_ADAPTER_MAP"] = orjson.dumps(adapter_map).decode()
-
-        if bettertransformer is not None:
-            start_env[env.bettertransformer] = str(bettertransformer)
-        if quantize is not None:
-            start_env[env.quantize] = quantize
-
-        if serve_grpc:
-            server = bentoml.GrpcServer(bento, **server_attrs)
-        else:
-            server = bentoml.HTTPServer(bento, **server_attrs)
-        analytics.track_start_init(config)
-
-        if return_process:
-            server.start(env=start_env, text=True)
-            process = server.process
-            if process is None:
-                raise click.ClickException("Failed to start the server.")
-            return process
-        else:
-            try:
-                server.start(env=start_env, text=True, blocking=True)
-            except Exception as err:
-                _echo(f"Error caught while running LLM Server:\n{err}", fg="red")
-
-        # NOTE: Return the configuration for telemetry purposes.
-        return config
-
-    return start_cmd
-
+    )
 
-def start_model(
-    group: click.Group,
-    model_name: str,
-    llm_config: openllm.LLMConfig,
-    serve_grpc: bool,
-    **command_attrs: t.Any,
-) -> click.Command:
     if llm_config["requires_gpu"] and device_count() < 1:
         # NOTE: The model requires GPU, therefore we will return a dummy command
-        command_attrs.update(
-            {
-                "short_help": "(Disabled because there is no GPU available)",
-                "help": f"""{model_name} is currently not available to run on your
-                local machine because it requires GPU for inference.""",
-            }
-        )
-        return noop_command(group, llm_config, "No GPU available, therefore this command is disabled", **command_attrs)
+        command_attrs.update({"short_help": "(Disabled because there is no GPU available)", "help": f"""{model} is currently not available to run on your local machine because it requires GPU for inference."""})
+        return noop_command(llm_config, _serve_grpc, **command_attrs)
+
 
     @group.command(**command_attrs)
-    @start_decorator(llm_config, serve_grpc=serve_grpc)
+    @start_decorator(llm_config, serve_grpc=_serve_grpc)
     @click.pass_context
     def start_cmd(
         ctx: click.Context,
         server_timeout: int,
         model_id: str | None,
         model_version: str | None,
-        workers_per_resource: t.LiteralString | float,
+        workers_per_resource: t.Literal["conserved", "round_robin"] | t.LiteralString,
         device: tuple[str, ...],
         quantize: t.Literal["int8", "int4", "gptq"] | None,
         bettertransformer: bool | None,
         runtime: t.Literal["ggml", "transformers"],
         fast: bool,
         serialisation_format: t.Literal["safetensors", "legacy"],
         adapter_id: str | None,
         return_process: bool,
         **attrs: t.Any,
     ) -> openllm.LLMConfig | subprocess.Popen[bytes]:
         if serialisation_format == "safetensors" and quantize is not None:
             if os.getenv("OPENLLM_SERIALIZATION_WARNING", str(True)).upper() in ENV_VARS_TRUE_VALUES:
                 _echo(
-                    f"'--quantize={quantize}' might not work with 'safetensors' serialisation format. Use with caution!. To silence this warning, set \"OPENLLM_SERIALIZATION_WARNING=True\"\nNote: You can always fallback to '--serialisation legacy' when running quantisation.",
+                    f"'--quantize={quantize}' might not work with 'safetensors' serialisation format. Use with caution!. To silence this warning, set \"OPENLLM_SERIALIZATION_WARNING=False\"\nNote: You can always fallback to '--serialisation legacy' when running quantisation.",
                     fg="yellow",
                 )
         adapter_map: dict[str, str | None] | None = attrs.pop(_adapter_mapping_key, None)
-
         config, server_attrs = llm_config.model_validate_click(**attrs)
         server_timeout = first_not_none(server_timeout, default=config["timeout"])
 
         server_attrs.update({"working_dir": os.path.dirname(__file__), "timeout": server_timeout})
-        if serve_grpc:
-            server_attrs["grpc_protocol_version"] = "v1"
+        if _serve_grpc: server_attrs["grpc_protocol_version"] = "v1"
         # NOTE: currently, theres no development args in bentoml.Server. To be fixed upstream.
         development = server_attrs.pop("development")
         server_attrs.setdefault("production", not development)
+        wpr: t.Any = first_not_none(workers_per_resource, default=config["workers_per_resource"])
 
-        workers_per_resource = first_not_none(workers_per_resource, default=config["workers_per_resource"])
-
-        if isinstance(workers_per_resource, str):
-            if workers_per_resource == "round_robin":
-                workers_per_resource = 1.0
-            elif workers_per_resource == "conserved":
+        if isinstance(wpr, str):
+            if wpr == "round_robin": wpr = 1.0
+            elif wpr == "conserved":
                 available_gpu = device if device else available_devices()
-                workers_per_resource = 1.0 if len(available_gpu) == 0 else float(1 / len(available_gpu))
-            else:
-                try:
-                    workers_per_resource = float(workers_per_resource)
-                except ValueError:
-                    ctx.fail(f"'workers_per_resource' only accept '{_wpr_strategies}' as possible strategies.")
-
-        num_workers = int(1 / workers_per_resource)
+                wpr = 1.0 if len(available_gpu) == 0 else float(1 / len(available_gpu))
+            else: wpr = float(wpr)
 
         # Create a new model env to work with the envvar during CLI invocation
-        env = EnvVarMixin(
-            config["model_name"],
-            config["default_implementation"],
-            bettertransformer=bettertransformer,
-            quantize=quantize,
-            runtime=runtime,
-        )
-
-        prerequisite_check(ctx, config, quantize, adapter_map, num_workers)
+        env = EnvVarMixin(config["model_name"], config.default_implementation(), model_id=model_id, bettertransformer=bettertransformer, quantize=quantize, runtime=runtime)
+        prerequisite_check(ctx, config, quantize, adapter_map, int(1 / wpr))
 
         # NOTE: This is to set current configuration
         start_env = os.environ.copy()
-        start_env = parse_config_options(config, server_timeout, workers_per_resource, device, start_env)
-
-        if fast and not get_quiet_mode():
-            _echo(
-                f"Fast mode is enabled. Make sure the model is available in local store before 'start': 'openllm import {model_name}{'--model-id ' + model_id if model_id else ''}'",
-                fg="yellow",
-            )
+        start_env = parse_config_options(config, server_timeout, wpr, device, start_env)
+        if fast and not get_quiet_mode(): _echo(f"Fast mode is enabled. Make sure the model is available in local store before 'start': 'openllm import {model}{'--model-id ' + model_id if model_id else ''}'", fg="yellow")
 
         start_env.update(
             {
-                env.framework: env.framework_value,
+                "OPENLLM_MODEL": model,
                 "BENTOML_DEBUG": str(not get_quiet_mode()),
-                "BENTOML_HOME": os.environ.get("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
+                "BENTOML_HOME": os.getenv("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
+                "OPENLLM_ADAPTER_MAP": orjson.dumps(adapter_map).decode(),
                 "OPENLLM_SERIALIZATION": serialisation_format,
+                env.model_id: env.model_id_value,
+                env.runtime: env.runtime_value,
+                env.framework: env.framework_value,
             }
         )
 
-        if adapter_map:
-            _echo(f"OpenLLM will convert '{model_name}' to use provided adapters layers: {list(adapter_map)}")
-
         llm = openllm.infer_auto_class(env.framework_value).for_model(
-            model_name,
-            model_id=model_id,
+            model,
+            model_id=env.model_id_value,
             model_version=model_version,
             llm_config=config,
             ensure_available=not fast,
             return_runner_kwargs=False,
-            quantize=quantize,
-            bettertransformer=bettertransformer,
+            quantize=env.quantize_value,
+            bettertransformer=env.bettertransformer_value,
             adapter_map=adapter_map,
-            runtime=runtime,
+            runtime=env.runtime_value,
             serialisation=serialisation_format,
         )
+        start_env.update({env.config: llm.config.model_dump_json().decode(), env.model_id: llm.model_id})
+        # NOTE: quantize and bettertransformer value is already assigned within env
+        if bettertransformer is not None: start_env[env.bettertransformer] = str(env.bettertransformer_value)
+        if quantize is not None: start_env[env.quantize] = str(env.quantize_value)
 
-        start_env.update(
-            {
-                env.config: llm.config.model_dump_json().decode(),
-                env.runtime: env.runtime_value,
-                "OPENLLM_MODEL": model_name,
-                "OPENLLM_MODEL_ID": llm.model_id,
-                "OPENLLM_ADAPTER_MAP": orjson.dumps(adapter_map).decode(),
-            }
-        )
-
-        if bettertransformer is not None:
-            start_env[env.bettertransformer] = str(bettertransformer)
-        if quantize is not None:
-            start_env[env.quantize] = quantize
-
-        if serve_grpc:
-            server = bentoml.GrpcServer("_service.py:svc", **server_attrs)
-        else:
-            server = bentoml.HTTPServer("_service.py:svc", **server_attrs)
+        if _serve_grpc: server = bentoml.GrpcServer("_service.py:svc", **server_attrs)
+        else: server = bentoml.HTTPServer("_service.py:svc", **server_attrs)
         analytics.track_start_init(llm.config)
 
-        def next_step(model_name: str, adapter_map: DictStrAny | None):
+        def next_step(model_name: str, adapter_map: DictStrAny | None) -> None:
             cmd_name = f"openllm build {model_name}"
-            if adapter_map is not None:
-                cmd_name += " " + " ".join(
-                    [
-                        f"--adapter-id {s}"
-                        for s in [
-                            f"{p}:{name}" if name not in (None, "default") else p for p, name in adapter_map.items()
-                        ]
-                    ]
-                )
-            _echo(
-                f"\n🚀 Next step: run '{cmd_name}' to create a Bento for {model_name}",
-                fg="blue",
-            )
+            if adapter_map is not None: cmd_name += " " + " ".join([f"--adapter-id {s}" for s in [f"{p}:{name}" if name not in (None, "default") else p for p, name in adapter_map.items()]])
+            _echo(f"\n🚀 Next step: run '{cmd_name}' to create a Bento for {model_name}", fg="blue")
 
         if return_process:
             server.start(env=start_env, text=True)
-            process = server.process
-            if process is None:
-                raise click.ClickException("Failed to start the server.")
-            return process
+            if server.process is None: raise click.ClickException("Failed to start the server.")
+            return server.process
         else:
-            try:
-                server.start(env=start_env, text=True, blocking=True)
-            except KeyboardInterrupt:
-                next_step(model_name, adapter_map)
-            except Exception as err:
-                _echo(f"Error caught while running LLM Server:\n{err}", fg="red")
-            else:
-                next_step(model_name, adapter_map)
+            try: server.start(env=start_env, text=True, blocking=True)
+            except KeyboardInterrupt: next_step(model, adapter_map)
+            except Exception as err: _echo(f"Error caught while running LLM Server:\n{err}", fg="red")
+            else: next_step(model, adapter_map)
 
         # NOTE: Return the configuration for telemetry purposes.
         return config
 
     return start_cmd
 
 
+def noop_command(llm_config: openllm.LLMConfig, _serve_grpc: bool, **command_attrs: t.Any) -> click.Command:
+    context_settings = command_attrs.pop("context_settings", {})
+    context_settings.update({"ignore_unknown_options": True, "allow_extra_args": True})
+    command_attrs["context_settings"] = context_settings
+    group = start_command if not _serve_grpc else start_grpc_command
+    # NOTE: The model requires GPU, therefore we will return a dummy command
+    @group.command(**command_attrs)
+    def noop(**_: t.Any) -> openllm.LLMConfig:
+        _echo("No GPU available, therefore this command is disabled", fg="red")
+        analytics.track_start_init(llm_config)
+        return llm_config
+
+    return noop
+
+
+def prerequisite_check(
+    ctx: click.Context,
+    llm_config: openllm.LLMConfig,
+    quantize: t.LiteralString | None,
+    adapter_map: dict[str, str | None] | None,
+    num_workers: int,
+) -> None:
+    if quantize:
+        if device_count() < 1:
+            _echo("Quantization requires at least 1 GPU (got None)", fg="red")
+            ctx.exit(1)
+
+    if adapter_map and not is_peft_available():
+        _echo(
+            "Using adapter requires 'peft' to be available. Make sure to install with 'pip install \"openllm[fine-tune]\"'",
+            fg="red",
+        )
+        ctx.exit(1)
+
+    requirements = llm_config["requirements"]
+    if requirements is not None and len(requirements) > 0:
+        missing_requirements = [i for i in requirements if importlib.util.find_spec(inflection.underscore(i)) is None]
+        if len(missing_requirements) > 0:
+            _echo(
+                f"Make sure to have the following dependencies available: {missing_requirements}",
+                fg="yellow",
+            )
+
+    if num_workers > 1 and device_count() < num_workers:
+        raise click.BadOptionUsage(
+            "workers_per_resource",
+            f"# of workers is infered to {num_workers} GPUs per runner worker, while there are only"
+            f"'{device_count()}' for inference. (Tip: Try again using '--workers-per-resource={1/device_count()}')",
+            ctx=ctx,
+        )
+
+
 @cli.command(name="import", aliases=["download"])
 @click.argument(
     "model",
     type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]),
 )
 @click.argument(
     "model_id",
@@ -1239,15 +849,20 @@
     type=click.Choice(["ggml", "transformers"]),
     default="transformers",
     help="The runtime to use for the given model. Default is transformers.",
 )
 @output_option
 @quantize_option(click)
 @machine_option(click)
-@click.option("--implementation", type=click.Choice(["pt", "tf", "flax", "vllm"]), default=None, hidden=True)
+@click.option(
+    "--implementation",
+    type=click.Choice(["pt", "tf", "flax", "vllm"]),
+    default=None,
+    help="The implementation for saving this LLM.",
+)
 @serialisation_option(click)
 def download_models_command(
     model: str,
     model_id: str | None,
     converter: str | None,
     model_version: str | None,
     output: OutputLiteral,
@@ -1306,81 +921,57 @@
     ```bash
     $ CONVERTER=llama2-hf openllm import llama /path/to/llama-2
     ```
 
     > **Note**: This behaviour will override ``--runtime``. Therefore make sure that the LLM contains correct conversion strategies to both GGML and HF.
     """
     llm_config = openllm.AutoConfig.for_model(model)
-    impl: LiteralRuntime = first_not_none(
-        implementation, default=EnvVarMixin(model, llm_config["default_implementation"]).framework_value
-    )
+    env = EnvVarMixin(model, llm_config.default_implementation(), model_id=model_id, runtime=runtime, quantize=quantize)
+    impl: LiteralRuntime = first_not_none(implementation, default=env.framework_value)
     llm = openllm.infer_auto_class(impl).for_model(
         model,
         llm_config=llm_config,
-        model_id=model_id,
+        model_id=env.model_id_value,
         model_version=model_version,
-        runtime=runtime,
+        runtime=env.runtime_value,
+        quantize=env.quantize_value,
         return_runner_kwargs=False,
-        quantize=quantize,
         ensure_available=False,
         serialisation=serialisation_format,
     )
-
     _previously_saved = False
     try:
-        _ref = bentoml.models.get(llm.tag)
+        _ref = openllm.serialisation.get(llm)
         _previously_saved = True
     except bentoml.exceptions.NotFound:
         if not machine and output == "pretty":
             msg = f"'{model}' does not exists in local store. Saving..."
-            if model_id is not None:
-                msg = f"'{model}' with 'model_id={model_id}' does not exists in local store. Saving..."
+            if model_id is not None: msg = f"'{model}' with 'model_id={model_id}' does not exists in local store. Saving..."
             _echo(msg, fg="yellow", nl=True)
-
-        _ref = llm.import_model(trust_remote_code=llm.__llm_trust_remote_code__)
-
-        if impl == "pt" and is_torch_available() and torch.cuda.is_available():
-            torch.cuda.empty_cache()
-
+        _ref = openllm.serialisation.get(llm, auto_import=True)
+        if impl == "pt" and is_torch_available() and torch.cuda.is_available(): torch.cuda.empty_cache()
     if machine:
         # NOTE: We will prefix the tag with __tag__ and we can use regex to correctly
         # get the tag from 'bentoml.bentos.build|build_bentofile'
         _echo(f"__tag__:{_ref.tag}", fg="white")
     elif output == "pretty":
-        if _previously_saved:
-            _echo(
-                f"{model} with 'model_id={model_id}' is already setup for framework '{impl}': {_ref.tag!s}",
-                nl=True,
-                fg="yellow",
-            )
-        else:
-            _echo(f"Saved model: {_ref.tag}")
-    elif output == "json":
-        _echo(
-            orjson.dumps(
-                {"previously_setup": _previously_saved, "framework": impl, "tag": str(_ref.tag)},
-                option=orjson.OPT_INDENT_2,
-            ).decode()
-        )
-    else:
-        _echo(_ref.tag)
-
+        if _previously_saved: _echo(f"{model} with 'model_id={model_id}' is already setup for framework '{impl}': {_ref.tag!s}", nl=True, fg="yellow")
+        else: _echo(f"Saved model: {_ref.tag}")
+    elif output == "json": _echo(orjson.dumps({"previously_setup": _previously_saved, "framework": impl, "tag": str(_ref.tag)}, option=orjson.OPT_INDENT_2).decode())
+    else: _echo(_ref.tag)
     return _ref
 
 
 _cached_http = {key: start_command_factory(key, _context_settings=_CONTEXT_SETTINGS) for key in openllm.CONFIG_MAPPING}
-_cached_grpc = {
-    key: start_command_factory(key, _context_settings=_CONTEXT_SETTINGS, _serve_grpc=True)
-    for key in openllm.CONFIG_MAPPING
-}
+_cached_grpc = {key: start_command_factory(key, _context_settings=_CONTEXT_SETTINGS, _serve_grpc=True) for key in openllm.CONFIG_MAPPING}
 
 
 @overload
 def _start(
-    model_name: str | bentoml.Bento,
+    model_name: str,
     /,
     model_id: str | None = ...,
     timeout: int = ...,
     workers_per_resource: t.Literal["conserved", "round_robin"] | float | None = ...,
     device: tuple[str, ...] | t.Literal["all"] | None = ...,
     quantize: t.Literal["int8", "int4", "gptq"] | None = ...,
     bettertransformer: bool | None = ...,
@@ -1393,15 +984,15 @@
     __test__: t.Literal[False] = False,
 ) -> openllm.LLMConfig:
     ...
 
 
 @overload
 def _start(
-    model_name: str | bentoml.Bento,
+    model_name: str,
     /,
     model_id: str | None = ...,
     timeout: int = ...,
     workers_per_resource: t.Literal["conserved", "round_robin"] | float | None = ...,
     device: tuple[str, ...] | t.Literal["all"] | None = ...,
     quantize: t.Literal["int8", "int4", "gptq"] | None = ...,
     bettertransformer: bool | None = ...,
@@ -1413,15 +1004,15 @@
     _serve_grpc: bool = ...,
     __test__: t.Literal[True] = True,
 ) -> subprocess.Popen[bytes]:
     ...
 
 
 def _start(
-    model_name: str | bentoml.Bento,
+    model_name: str,
     /,
     model_id: str | None = None,
     timeout: int = 30,
     workers_per_resource: t.Literal["conserved", "round_robin"] | float | None = None,
     device: tuple[str, ...] | t.Literal["all"] | None = None,
     quantize: t.Literal["int8", "int4", "gptq"] | None = None,
     bettertransformer: bool | None = None,
@@ -1470,75 +1061,43 @@
         bettertransformer: Convert given model to FastTransformer with PyTorch.
         runtime: The runtime to use for this LLM. By default, this is set to ``transformers``. In the future, this will include supports for GGML.
         fast: Enable fast mode. This will skip downloading models, and will raise errors if given model_id does not exists under local store.
         adapter_map: The adapter mapping of LoRA to use for this LLM. It accepts a dictionary of ``{adapter_id: adapter_name}``.
         framework: The framework to use for this LLM. By default, this is set to ``pt``.
         additional_args: Additional arguments to pass to ``openllm start``.
     """
-    if isinstance(model_name, str):
-        llm_config = openllm.AutoConfig.for_model(model_name)
-        _ModelEnv = EnvVarMixin(model_name, llm_config["default_implementation"])
-        if framework is None:
-            framework = _ModelEnv.framework_value
-        os.environ[_ModelEnv.framework] = framework
+    llm_config = openllm.AutoConfig.for_model(model_name)
+    _ModelEnv = EnvVarMixin(model_name, first_not_none(framework, default=llm_config.default_implementation()), model_id=model_id, bettertransformer=bettertransformer, quantize=quantize, runtime=runtime)
+    os.environ[_ModelEnv.framework] = _ModelEnv.framework_value
 
     args: ListStr = ["--runtime", runtime]
-    if model_id:
-        if isinstance(model_id, bentoml.Bento):
-            logger.warning("'model_id' has no effect if since %s is already a Bento.", model_name)
-        else:
-            args.extend(["--model-id", model_id])
-    if timeout:
-        args.extend(["--server-timeout", str(timeout)])
-    if workers_per_resource:
-        args.extend(
-            [
-                "--workers-per-resource",
-                str(workers_per_resource) if not isinstance(workers_per_resource, str) else workers_per_resource,
-            ]
-        )
-    if device and not os.getenv("CUDA_VISIBLE_DEVICES"):
-        args.extend(["--device", ",".join(device)])
-
-    if quantize and bettertransformer:
-        raise OpenLLMException("'quantize' and 'bettertransformer' are currently mutually exclusive.")
-
-    if quantize:
-        args.extend(["--quantize", str(quantize)])
-    if bettertransformer:
-        args.append("--bettertransformer")
-    if fast:
-        args.append("--fast")
-    if adapter_map:
-        args.extend(
-            list(
-                itertools.chain.from_iterable(
-                    [["--adapter-id", f"{k}{':'+v if v else ''}"] for k, v in adapter_map.items()]
-                )
-            )
-        )
-    if additional_args:
-        args.extend(additional_args)
+    if model_id: args.extend(["--model-id", model_id])
+    if timeout: args.extend(["--server-timeout", str(timeout)])
+    if workers_per_resource: args.extend(["--workers-per-resource", str(workers_per_resource) if not isinstance(workers_per_resource, str) else workers_per_resource])
+    if device and not os.getenv("CUDA_VISIBLE_DEVICES"): args.extend(["--device", ",".join(device)])
+
+    if quantize and bettertransformer: raise OpenLLMException("'quantize' and 'bettertransformer' are currently mutually exclusive.")
+
+    if quantize: args.extend(["--quantize", str(quantize)])
+    elif bettertransformer: args.append("--bettertransformer")
+
+    if fast: args.append("--fast")
+    if adapter_map: args.extend(list(itertools.chain.from_iterable([["--adapter-id", f"{k}{':'+v if v else ''}"] for k, v in adapter_map.items()])))
+    if additional_args: args.extend(additional_args)
+    if __test__: args.append("--return-process")
 
-    if __test__:
-        args.append("--return-process")
-
-    return start_command_factory(model_name, _context_settings=_CONTEXT_SETTINGS, _serve_grpc=_serve_grpc).main(
-        args=args if len(args) > 0 else None,
-        standalone_mode=False,
-    )
+    return start_command_factory(model_name, _context_settings=_CONTEXT_SETTINGS, _serve_grpc=_serve_grpc).main( args=args if len(args) > 0 else None, standalone_mode=False)
 
 
 def _tag_parsing(output: bytes) -> str:
     # NOTE: This usually only concern BentoML devs.
     pattern = r"^__tag__:[^:\n]+:[^:\n]+"
     matched = re.search(pattern, output.decode("utf-8").strip(), re.MULTILINE)
     assert matched is not None, f"Failed to find tag from output: {output!s}"
-    _, _, tag = matched.group(0).partition(":")
-    return tag
+    return matched.group(0).partition(":")[-1]
 
 
 @inject
 def _build(
     model_name: str,
     /,
     *,
@@ -1772,48 +1331,31 @@
 @click.option(
     "--adapter-id",
     default=None,
     help="Optional adapters id to be included within the Bento. Note that if you are using relative path, '--build-ctx' must be passed.",
     multiple=True,
     metavar="[PATH | [remote/][adapter_name:]adapter_id][, ...]",
 )
-@click.option("--build-ctx", default=".", help="Build context. This is required if --adapter-id uses relative path")
+@click.option("--build-ctx", help="Build context. This is required if --adapter-id uses relative path", default=".")
 @model_version_option(click)
-@click.option(
-    "--dockerfile-template",
-    default=None,
-    type=click.File(),
-    help="Optional custom dockerfile template to be used with this BentoLLM.",
-)
+@click.option("--dockerfile-template", default=None, type=click.File(), help="Optional custom dockerfile template to be used with this BentoLLM.")
 @serialisation_option(click)
 @cog.optgroup.group(cls=cog.MutuallyExclusiveOptionGroup, name="Utilities options")
-@cog.optgroup.option(
-    "--containerize",
-    default=False,
-    is_flag=True,
-    type=click.BOOL,
-    help="Whether to containerize the Bento after building. '--containerize' is the shortcut of 'openllm build && bentoml containerize'.",
-)
-@cog.optgroup.option(
-    "--push",
-    default=False,
-    is_flag=True,
-    type=click.BOOL,
-    help="Whether to push the result bento to BentoCloud. Make sure to login with 'bentoml cloud login' first.",
-)
+@cog.optgroup.option("--containerize", default=False, is_flag=True, type=click.BOOL, help="Whether to containerize the Bento after building. '--containerize' is the shortcut of 'openllm build && bentoml containerize'.")
+@cog.optgroup.option("--push", default=False, is_flag=True, type=click.BOOL, help="Whether to push the result bento to BentoCloud. Make sure to login with 'bentoml cloud login' first.")
 @click.pass_context
 def build_command(
     ctx: click.Context,
     model_name: str,
     model_id: str | None,
     overwrite: bool,
     output: OutputLiteral,
     runtime: t.Literal["ggml", "transformers"],
     quantize: t.Literal["int8", "int4", "gptq"] | None,
-    enable_features: tuple[str] | None,
+    enable_features: tuple[str, ...] | None,
     bettertransformer: bool | None,
     workers_per_resource: float | None,
     adapter_id: tuple[str, ...],
     build_ctx: str | None,
     machine: bool,
     model_version: str | None,
     dockerfile_template: t.TextIO | None,
@@ -1829,84 +1371,82 @@
     $ openllm build flan-t5 --model-id google/flan-t5-large
     ```
 
     \b
     > NOTE: To run a container built from this Bento with GPU support, make sure
     > to have https://github.com/NVIDIA/nvidia-container-toolkit install locally.
     """
-    adapter_map: dict[str, str | None] | None = None
-
-    if adapter_id:
-        if not build_ctx:
-            _echo("'build_ctx' must not be None when '--adapter-id' is passsed.", fg="red")
-            ctx.exit(1)
-
-        adapter_map = {}
-        for v in adapter_id:
-            _adapter_id, *adapter_name = v.rsplit(":", maxsplit=1)
-            # We don't resolve full path here, leave it to build
-            # we are just doing the parsing here.
-            adapter_map[_adapter_id] = adapter_name[0] if len(adapter_name) > 0 else None
-
-    if machine:
-        output = "porcelain"
-
-    if enable_features:
-        enable_features = tuple(itertools.chain.from_iterable((s.split(",") for s in enable_features)))
+    if machine: output = "porcelain"
+    if enable_features: enable_features = tuple(itertools.chain.from_iterable((s.split(",") for s in enable_features)))
 
     _previously_built = False
-    current_model_envvar = os.environ.pop("OPENLLM_MODEL", None)
-    current_model_id_envvar = os.environ.pop("OPENLLM_MODEL_ID", None)
-    current_adapter_map_envvar = os.environ.pop("OPENLLM_ADAPTER_MAP", None)
-    current_serialisation_envvar = os.environ.pop("OPENLLM_SERIALIZATION", None)
 
     llm_config = openllm.AutoConfig.for_model(model_name)
+    env = EnvVarMixin(model_name, llm_config.default_implementation(), model_id=model_id, quantize=quantize, bettertransformer=bettertransformer, runtime=runtime)
 
     # NOTE: We set this environment variable so that our service.py logic won't raise RuntimeError
     # during build. This is a current limitation of bentoml build where we actually import the service.py into sys.path
     try:
-        os.environ[llm_config["env"].runtime] = runtime
         os.environ["OPENLLM_MODEL"] = inflection.underscore(model_name)
-        os.environ["OPENLLM_ADAPTER_MAP"] = orjson.dumps(adapter_map).decode()
+        os.environ[env.runtime] = env.runtime_value
         os.environ["OPENLLM_SERIALIZATION"] = serialisation_format
 
-        framework_envvar = llm_config["env"].framework_value
-        llm = openllm.infer_auto_class(framework_envvar).for_model(
+        llm = openllm.infer_auto_class(env.framework_value).for_model(
             model_name,
-            model_id=model_id,
+            model_id=env.model_id_value,
             llm_config=llm_config,
-            quantize=quantize,
-            adapter_map=adapter_map,
-            bettertransformer=bettertransformer,
+            quantize=env.quantize_value,
+            bettertransformer=env.bettertransformer_value,
             return_runner_kwargs=False,
             ensure_available=True,
             model_version=model_version,
-            runtime=runtime,
+            runtime=env.runtime_value,
             serialisation=serialisation_format,
             **attrs,
         )
-        os.environ["OPENLLM_MODEL_ID"] = str(llm.tag)
+        os.environ[env.model_id] = str(llm.tag)
 
         labels = dict(llm.identifying_params)
-        labels.update({"_type": llm.llm_type, "_framework": framework_envvar})
+        labels.update({"_type": llm.llm_type, "_framework": env.framework_value})
         workers_per_resource = first_not_none(workers_per_resource, default=llm_config["workers_per_resource"])
 
         with fs.open_fs(f"temp://llm_{llm_config['model_name']}") as llm_fs:
             dockerfile_template_path = None
             if dockerfile_template:
-                with dockerfile_template:
-                    llm_fs.writetext("Dockerfile.template", dockerfile_template.read())
+                with dockerfile_template: llm_fs.writetext("Dockerfile.template", dockerfile_template.read())
                 dockerfile_template_path = llm_fs.getsyspath("/Dockerfile.template")
 
-            bento_tag = bentoml.Tag.from_taglike(f"{llm.llm_type}-service:{llm.tag.version}")
+            adapter_map: dict[str, str | None] | None = None
+            if adapter_id:
+                if not build_ctx:
+                    _echo("'build_ctx' is required when '--adapter-id' is passsed.", fg="red")
+                    ctx.exit(1)
+                adapter_map = {}
+                for v in adapter_id:
+                    _adapter_id, *adapter_name = v.rsplit(":", maxsplit=1)
+                    name = adapter_name[0] if len(adapter_name) > 0 else None
+                    try:
+                        resolve_user_filepath(_adapter_id, build_ctx)
+                        src_folder_name = os.path.basename(_adapter_id)
+                        src_fs = fs.open_fs(build_ctx)
+                        llm_fs.makedir(src_folder_name, recreate=True)
+                        fs.copy.copy_dir(src_fs, _adapter_id, llm_fs, src_folder_name)
+                        adapter_map[src_folder_name] = name
+                    except FileNotFoundError:
+                        # this is the remote adapter, then just added back
+                        # note that there is a drawback here. If the path of the local adapter
+                        # path have the same name as the remote, then we currently don't support
+                        # that edge case.
+                        adapter_map[_adapter_id] = name
+                os.environ["OPENLLM_ADAPTER_MAP"] = orjson.dumps(adapter_map).decode()
+            bento_tag = bentoml.Tag.from_taglike(f"{llm.llm_type}-service:{llm.tag.version}".lower().strip())
             try:
                 bento = bentoml.get(bento_tag)
                 if overwrite:
-                    if output == "pretty":
-                        _echo(f"Overwriting existing Bento {bento_tag}", fg="yellow")
+                    if output == "pretty": _echo(f"Overwriting existing Bento {bento_tag}", fg="yellow")
                     bentoml.delete(bento_tag)
                     bento = openllm.bundle.create_bento(
                         bento_tag,
                         llm_fs,
                         llm,
                         workers_per_resource=workers_per_resource,
                         adapter_map=adapter_map,
@@ -1928,181 +1468,105 @@
                     quantize=quantize,
                     bettertransformer=bettertransformer,
                     extra_dependencies=enable_features,
                     build_ctx=build_ctx,
                     dockerfile_template=dockerfile_template_path,
                     runtime=runtime,
                 )
-    except Exception as e:
-        logger.error("\nException caught during building LLM %s: \n", model_name, exc_info=e)
+    except Exception:
         raise
-    else:
-        os.environ.pop("OPENLLM_MODEL", None)
-        os.environ.pop("OPENLLM_MODEL_ID", None)
-        os.environ.pop("OPENLLM_ADAPTER_MAP", None)
-        os.environ.pop("OPENLLM_SERIALIZATION", None)
-        # restore original OPENLLM_MODEL envvar if set.
-        if current_model_envvar is not None:
-            os.environ["OPENLLM_MODEL"] = current_model_envvar
-        if current_model_id_envvar is not None:
-            os.environ["OPENLLM_MODEL_ID"] = current_model_id_envvar
-        if current_adapter_map_envvar is not None:
-            os.environ["OPENLLM_ADAPTER_MAP"] = current_adapter_map_envvar
-        if current_serialisation_envvar is not None:
-            os.environ["OPENLLM_SERIALIZATION"] = current_serialisation_envvar
 
-    if machine:
-        # NOTE: We will prefix the tag with __tag__ and we can use regex to correctly
-        # get the tag from 'bentoml.bentos.build|build_bentofile'
-        _echo(f"__tag__:{bento.tag}", fg="white")
+    if machine: _echo(f"__tag__:{bento.tag}", fg="white")
     elif output == "pretty":
         if not get_quiet_mode():
             _echo("\n" + OPENLLM_FIGLET, fg="white")
-            if not _previously_built:
-                _echo(f"Successfully built {bento}.", fg="green")
-            elif not overwrite:
-                _echo(
-                    f"'{model_name}' already has a Bento built [{bento}]. To overwrite it pass '--overwrite'.",
-                    fg="yellow",
-                )
-
+            if not _previously_built: _echo(f"Successfully built {bento}.", fg="green")
+            elif not overwrite: _echo(f"'{model_name}' already has a Bento built [{bento}]. To overwrite it pass '--overwrite'.", fg="yellow")
             _echo(
                 "📖 Next steps:\n\n"
                 + "* Serving BentoLLM locally with 'openllm start':\n"
                 + f"    $ openllm start {bento.tag}\n\n"
                 + "* Push to BentoCloud with 'bentoml push':\n"
                 + f"    $ bentoml push {bento.tag}\n\n"
                 + "* Containerize your Bento with 'bentoml containerize':\n"
                 + f"    $ bentoml containerize {bento.tag} --opt progress=plain"
                 + "\n\n"
                 + "    Tip: To enable additional BentoML features for 'containerize', "
                 + "use '--enable-features=FEATURE[,FEATURE]' "
                 + "[see 'bentoml containerize -h' for more advanced usage]\n",
                 fg="blue",
             )
-    elif output == "json":
-        _echo(orjson.dumps(bento.info.to_dict(), option=orjson.OPT_INDENT_2).decode())
-    else:
-        _echo(bento.tag)
+    elif output == "json": _echo(orjson.dumps(bento.info.to_dict(), option=orjson.OPT_INDENT_2).decode())
+    else: _echo(bento.tag)
 
-    if push:
-        client = BentoMLContainer.bentocloud_client.get()
-        client.push_bento(bento, context=t.cast(CliContext, ctx.obj).cloud_context)
+    if push: BentoMLContainer.bentocloud_client.get().push_bento(bento, context=t.cast(CliContext, ctx.obj).cloud_context)
     elif containerize:
         backend = t.cast("DefaultBuilder", os.getenv("BENTOML_CONTAINERIZE_BACKEND", "docker"))
         _echo(f"Building {bento} into a LLMContainer using backend '{backend}'", fg="magenta")
-        try:
-            bentoml.container.health(backend)
-        except subprocess.CalledProcessError:
-            raise OpenLLMException(f"Failed to use backend {backend}") from None
-
+        try: bentoml.container.health(backend)
+        except subprocess.CalledProcessError: raise OpenLLMException(f"Failed to use backend {backend}") from None
         bentoml.container.build(bento.tag, backend=backend, features=("grpc",))
-
     return bento
 
 
 @overload
-def models_command(
-    ctx: click.Context, output: OutputLiteral, show_available: bool, machine: t.Literal[True] = True
-) -> DictStrAny:
-    ...
-
-
+def models_command(ctx: click.Context, output: OutputLiteral, show_available: bool, machine: t.Literal[True] = True) -> DictStrAny: ...
 @overload
-def models_command(
-    ctx: click.Context, output: OutputLiteral, show_available: bool, machine: t.Literal[False] = ...
-) -> None:
-    ...
-
-
+def models_command(ctx: click.Context, output: OutputLiteral, show_available: bool, machine: t.Literal[False] = ...) -> None: ...
 @cli.command()
 @output_option
-@click.option(
-    "--show-available",
-    is_flag=True,
-    default=False,
-    help="Show available models in local store (mutually exclusive with '-o porcelain').",
-)
+@click.option("--show-available", is_flag=True, default=False, help="Show available models in local store (mutually exclusive with '-o porcelain').")
 @machine_option(click)
 @click.pass_context
-def models_command(
-    ctx: click.Context, output: OutputLiteral, show_available: bool, machine: bool
-) -> DictStrAny | None:
+def models_command(ctx: click.Context, output: OutputLiteral, show_available: bool, machine: bool) -> DictStrAny | None:
     """List all supported models.
 
     \b
     > NOTE: '--show-available' and '-o porcelain' are mutually exclusive.
 
     \b
     ```bash
     openllm models --show-available
     ```
     """
     from ._llm import normalise_model_name
 
     models = tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())
     if output == "porcelain":
-        if show_available:
-            raise click.BadOptionUsage(
-                "--show-available", "Cannot use '--show-available' with '-o porcelain' (mutually exclusive)."
-            )
+        if show_available: raise click.BadOptionUsage("--show-available", "Cannot use '--show-available' with '-o porcelain' (mutually exclusive).")
         _echo("\n".join(models), fg="white")
     else:
         failed_initialized: list[tuple[str, Exception]] = []
 
-        json_data: dict[
-            str,
-            dict[t.Literal["architecture", "model_id", "url", "installation", "cpu", "gpu", "runtime_impl"], t.Any]
-            | t.Any,
-        ] = {}
-
+        json_data: dict[str, dict[t.Literal["architecture", "model_id", "url", "installation", "cpu", "gpu", "runtime_impl"], t.Any] | t.Any] = {}
         converted: list[str] = []
         for m in models:
             config = openllm.AutoConfig.for_model(m)
             runtime_impl: tuple[str, ...] = ()
-            if config["model_name"] in openllm.MODEL_MAPPING_NAMES:
-                runtime_impl += ("pt",)
-            if config["model_name"] in openllm.MODEL_FLAX_MAPPING_NAMES:
-                runtime_impl += ("flax",)
-            if config["model_name"] in openllm.MODEL_TF_MAPPING_NAMES:
-                runtime_impl += ("tf",)
-            if config["model_name"] in openllm.MODEL_VLLM_MAPPING_NAMES:
-                runtime_impl += ("vllm",)
+            if config["model_name"] in openllm.MODEL_MAPPING_NAMES: runtime_impl += ("pt",)
+            if config["model_name"] in openllm.MODEL_FLAX_MAPPING_NAMES: runtime_impl += ("flax",)
+            if config["model_name"] in openllm.MODEL_TF_MAPPING_NAMES: runtime_impl += ("tf",)
+            if config["model_name"] in openllm.MODEL_VLLM_MAPPING_NAMES: runtime_impl += ("vllm",)
             json_data[m] = {
                 "architecture": config["architecture"],
                 "model_id": config["model_ids"],
-                "url": config["url"],
                 "cpu": not config["requires_gpu"],
                 "gpu": True,
                 "runtime_impl": runtime_impl,
-                "installation": f'pip install "openllm[{m}]"'
-                if m in openllm.utils.OPTIONAL_DEPENDENCIES or config["requirements"]
-                else "pip install openllm",
+                "installation": f'"openllm[{m}]"' if m in openllm.utils.OPTIONAL_DEPENDENCIES or config["requirements"] else "openllm",
             }
             converted.extend([normalise_model_name(i) for i in config["model_ids"]])
             if DEBUG:
-                try:
-                    openllm.AutoLLM.for_model(m, llm_config=config)
-                except Exception as e:
-                    failed_initialized.append((m, e))
+                try: openllm.AutoLLM.for_model(m, llm_config=config)
+                except Exception as e: failed_initialized.append((m, e))
 
         ids_in_local_store: DictStrAny | None = None
         local_models: DictStrAny | None = None
         if show_available:
-            ids_in_local_store = {
-                k: [
-                    i
-                    for i in bentoml.models.list()
-                    if "framework" in i.info.labels
-                    and i.info.labels["framework"] == "openllm"
-                    and "model_name" in i.info.labels
-                    and i.info.labels["model_name"] == k
-                ]
-                for k in json_data.keys()
-            }
+            ids_in_local_store = {k: [i for i in bentoml.models.list() if "framework" in i.info.labels and i.info.labels["framework"] == "openllm" and "model_name" in i.info.labels and i.info.labels["model_name"] == k] for k in json_data.keys()}
             ids_in_local_store = {k: v for k, v in ids_in_local_store.items() if v}
             local_models = {k: [str(i.tag) for i in val] for k, val in ids_in_local_store.items()}
 
         if machine:
             if show_available:
                 assert ids_in_local_store
                 assert local_models
@@ -2110,73 +1574,53 @@
             return json_data
         elif output == "pretty":
             import tabulate
 
             tabulate.PRESERVE_WHITESPACE = True
 
             # llm, architecture, url, model_id, installation, cpu, gpu, runtime_impl
-            data: list[
-                str
-                | tuple[
-                    str,
-                    str,
-                    str,
-                    list[str],
-                    str,
-                    t.LiteralString,
-                    t.LiteralString,
-                    tuple[LiteralRuntime, ...],
-                ]
-            ] = []
+            data: list[str | tuple[str, str, list[str], str, t.LiteralString, t.LiteralString, tuple[LiteralRuntime, ...]] ] = []
             for m, v in json_data.items():
                 data.extend(
                     [
                         (
                             m,
                             v["architecture"],
-                            v["url"],
                             v["model_id"],
                             v["installation"],
                             "❌" if not v["cpu"] else "✅",
                             "✅",
                             v["runtime_impl"],
                         )
                     ]
                 )
             column_widths = [
                 int(COLUMNS / 12),
                 int(COLUMNS / 6),
-                int(COLUMNS / 6),
-                int(COLUMNS / 6),
-                int(COLUMNS / 6),
+                int(COLUMNS / 4),
                 int(COLUMNS / 12),
                 int(COLUMNS / 12),
                 int(COLUMNS / 12),
+                int(COLUMNS / 4),
             ]
 
             if len(data) == 0 and len(failed_initialized) > 0:
                 _echo("Exception found while parsing models:\n", fg="yellow")
                 for m, err in failed_initialized:
                     _echo(f"- {m}: ", fg="yellow", nl=False)
                     _echo(traceback.print_exception(err, limit=3), fg="red")
                 sys.exit(1)
 
             table = tabulate.tabulate(
                 data,
                 tablefmt="fancy_grid",
-                headers=["LLM", "Architecture", "URL", "Models Id", "Installation", "CPU", "GPU", "Runtime"],
+                headers=["LLM", "Architecture", "Models Id", "pip install", "CPU", "GPU", "Runtime"],
                 maxcolwidths=column_widths,
             )
-
-            formatted_table = ""
-            for line in table.split("\n"):
-                formatted_table += (
-                    "".join(f"{cell:{width}}" for cell, width in zip(line.split("\t"), column_widths)) + "\n"
-                )
-            _echo(formatted_table, fg="white")
+            _echo(table, fg="white")
 
             if DEBUG and len(failed_initialized) > 0:
                 _echo("\nThe following models are supported but failed to initialize:\n")
                 for m, err in failed_initialized:
                     _echo(f"- {m}: ", fg="blue", nl=False)
                     _echo(err, fg="red")
 
@@ -2184,77 +1628,47 @@
                 assert ids_in_local_store is not None
                 assert local_models
                 if len(ids_in_local_store) == 0:
                     _echo("No models available locally.")
                     ctx.exit(0)
 
                 _echo("The following are available in local store:", fg="magenta")
-                _echo(
-                    orjson.dumps(
-                        local_models,
-                        option=orjson.OPT_INDENT_2,
-                    ).decode(),
-                    fg="white",
-                )
+                _echo(orjson.dumps(local_models, option=orjson.OPT_INDENT_2).decode(), fg="white")
         else:
             if show_available:
                 assert ids_in_local_store
                 assert local_models
                 json_data["local"] = local_models
-            _echo(
-                orjson.dumps(
-                    json_data,
-                    option=orjson.OPT_INDENT_2,
-                ).decode(),
-                fg="white",
-            )
+            _echo(orjson.dumps(json_data, option=orjson.OPT_INDENT_2,).decode(), fg="white")
     ctx.exit(0)
 
 
 @cli.command()
-@click.argument(
-    "model_name",
-    type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]),
-    required=False,
-)
-@click.option(
-    "-y",
-    "--yes",
-    "--assume-yes",
-    is_flag=True,
-    help="Skip confirmation when deleting a specific model",
-)
+@click.argument("model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]), required=False)
+@click.option("-y", "--yes", "--assume-yes", is_flag=True, help="Skip confirmation when deleting a specific model")
+@click.option("--include-bentos/--no-include-bentos", is_flag=True, default=False, help="Whether to also include pruning bentos.")
 @inject
-def prune_command(
-    model_name: str | None, yes: bool, model_store: ModelStore = Provide[BentoMLContainer.model_store]
-) -> None:
-    """Remove all saved models locally.
+def prune_command(model_name: str | None, yes: bool, include_bentos: bool, model_store: ModelStore = Provide[BentoMLContainer.model_store], bento_store: BentoStore = Provide[BentoMLContainer.bento_store]) -> None:
+    """Remove all saved models, (and optionally bentos) built with OpenLLM locally.
 
     \b
     If a model type is passed, then only prune models for that given model type.
     """
-    available = [
-        m for m in bentoml.models.list() if "framework" in m.info.labels and m.info.labels["framework"] == "openllm"
-    ]
-    if model_name is not None:
-        available = [
-            m
-            for m in available
-            if "model_name" in m.info.labels and m.info.labels["model_name"] == inflection.underscore(model_name)
-        ]
-
-    for model in available:
-        if yes:
-            delete_confirmed = True
-        else:
-            delete_confirmed = click.confirm(f"delete model {model.tag}?")
-
+    available: list[tuple[bentoml.Model | bentoml.Bento, ModelStore | BentoStore]]= [(m, model_store) for m in bentoml.models.list() if "framework" in m.info.labels and m.info.labels["framework"] == "openllm"]
+    if model_name is not None: available = [(m, store) for m, store in available if "model_name" in m.info.labels and m.info.labels["model_name"] == inflection.underscore(model_name)]
+    if include_bentos:
+        if model_name is not None: available += [(b, bento_store) for b in bentoml.bentos.list() if "start_name" in b.info.labels and b.info.labels["start_name"] == inflection.underscore(model_name)]
+        else: available += [(b, bento_store) for b in bentoml.bentos.list() if "_type" in b.info.labels and "_framework" in b.info.labels]
+
+    for store_item, store in available:
+        if yes: delete_confirmed = True
+        else: delete_confirmed = click.confirm(f"delete {'model' if isinstance(store, ModelStore) else 'bento'} {store_item.tag}?")
         if delete_confirmed:
-            model_store.delete(model.tag)
-            click.echo(f"{model} deleted.")
+            store.delete(store_item.tag)
+            _echo(f"{store_item} deleted from {'model' if isinstance(store, ModelStore) else 'bento'} store.", fg="yellow")
 
 
 def parsing_instruction_callback(
     ctx: click.Context, param: click.Parameter, value: list[str] | str | None
 ) -> tuple[str, bool | str] | list[str] | str | None:
     if value is None:
         return value
@@ -2271,15 +1685,15 @@
         return key, True
     elif len(values) == 1:
         return key, values[0]
     else:
         raise click.BadParameter(f"Invalid option format: {value}")
 
 
-def shared_client_options(f: t.Callable[[FC], FC]) -> t.Callable[[FC], FC]:
+def shared_client_options(f: _AnyCallable) -> t.Callable[[FC], FC]:
     options = [
         click.option(
             "--endpoint",
             type=click.STRING,
             help="OpenLLM Server endpoint, i.e: http://localhost:3000",
             envvar="OPENLLM_ENDPOINT",
             default="http://localhost:3000",
@@ -2291,250 +1705,152 @@
         f = opt(f)
     return f
 
 
 @cli.command()
 @click.argument("task", type=click.STRING, metavar="TASK")
 @shared_client_options
-@click.option(
-    "--agent",
-    type=click.Choice(["hf"]),
-    default="hf",
-    help="Whether to interact with Agents from given Server endpoint.",
-    show_default=True,
-)
-@click.option(
-    "--remote",
-    is_flag=True,
-    default=False,
-    help="Whether or not to use remote tools (inference endpoints) instead of local ones.",
-    show_default=True,
-)
-@click.option(
-    "--opt",
-    help="Define prompt options. "
-    "(format: ``--opt text='I love this' --opt audio:./path/to/audio  --opt image:/path/to/file``)",
-    required=False,
-    multiple=True,
-    callback=opt_callback,
-    metavar="ARG=VALUE[,ARG=VALUE]",
-)
-def instruct(
-    endpoint: str,
-    timeout: int,
-    agent: t.LiteralString,
-    output: OutputLiteral,
-    remote: bool,
-    task: str,
-    _memoized: DictStrAny,
-    **attrs: t.Any,
-) -> str:
+@click.option("--agent", type=click.Choice(["hf"]), default="hf", help="Whether to interact with Agents from given Server endpoint.", show_default=True)
+@click.option("--remote", is_flag=True, default=False, help="Whether or not to use remote tools (inference endpoints) instead of local ones.", show_default=True)
+@click.option("--opt", help="Define prompt options. " "(format: ``--opt text='I love this' --opt audio:./path/to/audio  --opt image:/path/to/file``)", required=False, multiple=True, callback=opt_callback, metavar="ARG=VALUE[,ARG=VALUE]")
+def instruct(endpoint: str, timeout: int, agent: t.LiteralString, output: OutputLiteral, remote: bool, task: str, _memoized: DictStrAny, **attrs: t.Any) -> str:
     """Instruct agents interactively for given tasks, from a terminal.
 
     \b
     ```bash
     $ openllm instruct --endpoint http://12.323.2.1:3000 \\
         "Is the following `text` (in Spanish) positive or negative?" \\
         --text "¡Este es un API muy agradable!"
     ```
     """
     client = openllm.client.HTTPClient(endpoint, timeout=timeout)
 
+    try: client.call("metadata")
+    except http.client.BadStatusLine: raise click.ClickException(f"{endpoint} is neither a HTTP server nor reachable.") from None
     if agent == "hf":
-        if not is_transformers_supports_agent():
-            raise click.UsageError(
-                "Transformers version should be at least 4.29 to support HfAgent. "
-                "Upgrade with 'pip install -U transformers'"
-            )
-
+        if not is_transformers_supports_agent(): raise click.UsageError("Transformers version should be at least 4.29 to support HfAgent. Upgrade with 'pip install -U transformers'")
         _memoized = {k: v[0] for k, v in _memoized.items() if v}
-
         client._hf_agent.set_stream(logger.info)
-        if output != "porcelain":
-            _echo(f"Sending the following prompt ('{task}') with the following vars: {_memoized}", fg="magenta")
-
+        if output != "porcelain": _echo(f"Sending the following prompt ('{task}') with the following vars: {_memoized}", fg="magenta")
         result = client.ask_agent(task, agent_type=agent, return_code=False, remote=remote, **_memoized)
-        if output == "json":
-            _echo(orjson.dumps(result, option=orjson.OPT_INDENT_2).decode(), fg="white")
-        else:
-            _echo(result, fg="white")
+        if output == "json": _echo(orjson.dumps(result, option=orjson.OPT_INDENT_2).decode(), fg="white")
+        else: _echo(result, fg="white")
         return result
-    else:
-        raise click.BadOptionUsage("agent", f"Unknown agent type {agent}")
+    else: raise click.BadOptionUsage("agent", f"Unknown agent type {agent}")
 
 
 @cli.command()
 @shared_client_options
-@click.option(
-    "--server-type", type=click.Choice(["grpc", "http"]), help="Server type", default="http", show_default=True
-)
+@click.option("--server-type", type=click.Choice(["grpc", "http"]), help="Server type", default="http", show_default=True)
 @click.argument("prompt", type=click.STRING)
-@click.option(
-    "--sampling-params",
-    help="Define query options. (format: ``--opt temperature=0.8 --opt=top_k:12)",
-    required=False,
-    multiple=True,
-    callback=opt_callback,
-    metavar="ARG=VALUE[,ARG=VALUE]",
-)
+@click.option("--sampling-params", help="Define query options. (format: ``--opt temperature=0.8 --opt=top_k:12)", required=False, multiple=True, callback=opt_callback, metavar="ARG=VALUE[,ARG=VALUE]")
 @click.pass_context
-def query(
-    ctx: click.Context,
-    prompt: str,
-    endpoint: str,
-    timeout: int,
-    server_type: t.Literal["http", "grpc"],
-    output: OutputLiteral,
-    _memoized: DictStrAny,
-    **attrs: t.Any,
-) -> None:
+def query(ctx: click.Context, prompt: str, endpoint: str, timeout: int, server_type: t.Literal["http", "grpc"], output: OutputLiteral, _memoized: DictStrAny, **attrs: t.Any) -> None:
     """Ask a LLM interactively, from a terminal.
 
     \b
     ```bash
     $ openllm query --endpoint http://12.323.2.1:3000 "What is the meaning of life?"
     ```
     """
     _memoized = {k: orjson.loads(v[0]) for k, v in _memoized.items() if v}
-    if server_type == "grpc":
-        endpoint = re.sub(r"http://", "", endpoint)
-    client = (
-        openllm.client.HTTPClient(endpoint, timeout=timeout)
-        if server_type == "http"
-        else openllm.client.GrpcClient(endpoint, timeout=timeout)
-    )
-
-    input_fg = "magenta"
-    generated_fg = "cyan"
-
+    if server_type == "grpc": endpoint = re.sub(r"http://", "", endpoint)
+    client = openllm.client.HTTPClient(endpoint, timeout=timeout) if server_type == "http" else openllm.client.GrpcClient(endpoint, timeout=timeout)
+    input_fg, generated_fg = "magenta", "cyan"
     if output != "porcelain":
         _echo("==Input==\n", fg="white")
         _echo(f"{prompt}", fg=input_fg)
-
-    res = client.query(prompt, return_raw_response=True, **_memoized)
-
+    res = client.query(prompt, return_raw_response=True, **{**client.configuration, **_memoized})
     if output == "pretty":
-        full_formatted = client.llm.postprocess_generate(prompt, res["responses"])
-        response = full_formatted[len(prompt) + 1 :]
+        response = client.llm.postprocess_generate(prompt, res["responses"])
         _echo("\n\n==Responses==\n", fg="white")
-        _echo(f"{prompt} ", fg=input_fg, nl=False)
         _echo(response, fg=generated_fg)
-    elif output == "json":
-        _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
-    else:
-        _echo(res["responses"], fg="white")
-
+    elif output == "json": _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
+    else: _echo(res["responses"], fg="white")
     ctx.exit(0)
 
 
 @cli.group(name="utils")
 def utils_command() -> None:
     """Utilities Subcommand group."""
 
 
 @utils_command.command()
 @click.pass_context
 def list_bentos(ctx: click.Context):
     """List available bentos built by OpenLLM."""
     _local_bentos = {str(i.tag): i.info.labels["start_name"] for i in bentoml.list() if "start_name" in i.info.labels}
-    mapping = {
-        k: [tag for tag, name in _local_bentos.items() if name == k]
-        for k in tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())
-    }
+    mapping = {k: [tag for tag, name in _local_bentos.items() if name == k] for k in tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())}
     mapping = {k: v for k, v in mapping.items() if v}
     _echo(orjson.dumps(mapping, option=orjson.OPT_INDENT_2).decode(), fg="white")
     ctx.exit(0)
 
+@utils_command.command()
+@click.argument("bento", type=str)
+@click.pass_context
+@inject
+def dive_bentos(ctx: click.Context, bento: str, _bento_store: BentoStore = Provide[BentoMLContainer.bento_store]) -> None:
+    """Dive into a BentoLLM. This is synonymous to cd $(b get <bento>:<tag> -o path)."""
+    try: bentomodel = _bento_store.get(bento)
+    except bentoml.exceptions.NotFound: ctx.fail(f"Bento {bento} not found. Make sure to call `openllm build first`")
+    if "bundler" not in  bentomodel.info.labels or bentomodel.info.labels["bundler"] != "openllm.bundle": ctx.fail(f"Bento is either too old or not built with OpenLLM. Make sure to use ``openllm build {bentomodel.info.labels['start_name']}`` for correctness.")
+    # copy and paste this into a new shell
+    _echo(f"cd $(python -m bentoml get {bentomodel.tag!s} -o path)", fg="white")
 
-@overload
-def get_prompt(
-    model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[True] = True
-) -> str:
-    ...
 
 
 @overload
-def get_prompt(
-    model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[False] = ...
-) -> None:
-    ...
-
-
+def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[True] = True) -> str: ...
+@overload
+def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: t.Literal[False] = ...) -> None: ...
 @utils_command.command()
-@click.argument(
-    "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
-)
+@click.argument("model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]))
 @click.argument("prompt", type=click.STRING)
 @output_option
 @click.option("--format", type=click.STRING, default=None)
 @machine_option(click)
 def get_prompt(model_name: str, prompt: str, format: str | None, output: OutputLiteral, machine: bool) -> str | None:
     """Get the default prompt used by OpenLLM."""
     module = openllm.utils.EnvVarMixin(model_name).module
     try:
         template = getattr(module, "DEFAULT_PROMPT_TEMPLATE", None)
         prompt_mapping = getattr(module, "PROMPT_MAPPING", None)
-        if template is None:
-            raise click.BadArgumentUsage(f"model {model_name} does not have a default prompt template") from None
+        if template is None: raise click.BadArgumentUsage(f"model {model_name} does not have a default prompt template") from None
         if callable(template):
             if format is None:
-                if not hasattr(module, "PROMPT_MAPPING") or module.PROMPT_MAPPING is None:
-                    raise RuntimeError("Failed to find prompt mapping while DEFAULT_PROMPT_TEMPLATE is a function.")
-                raise click.BadOptionUsage(
-                    "format",
-                    f"{model_name} prompt requires passing '--format' (available format: {list(module.PROMPT_MAPPING)})",
-                )
-            if prompt_mapping is None:
-                raise click.BadArgumentUsage(
-                    f"Failed to fine prompt mapping while the default prompt for {model_name} is a callable."
-                ) from None
-            if format not in prompt_mapping:
-                raise click.BadOptionUsage(
-                    "format",
-                    f"Given format {format} is not valid for {model_name} (available format: {list(prompt_mapping)})",
-                )
+                if not hasattr(module, "PROMPT_MAPPING") or module.PROMPT_MAPPING is None: raise RuntimeError("Failed to find prompt mapping while DEFAULT_PROMPT_TEMPLATE is a function.")
+                raise click.BadOptionUsage("format", f"{model_name} prompt requires passing '--format' (available format: {list(module.PROMPT_MAPPING)})")
+            if prompt_mapping is None: raise click.BadArgumentUsage(f"Failed to fine prompt mapping while the default prompt for {model_name} is a callable.") from None
+            if format not in prompt_mapping: raise click.BadOptionUsage("format", f"Given format {format} is not valid for {model_name} (available format: {list(prompt_mapping)})")
             _prompt = template(format)
         else:
             _prompt = template
 
         # XXX: FIX ME, currently doesn't work with all different context variable
         # will need a --opt parser for this
         fully_formatted = _prompt.format(instruction=prompt)
 
-        if machine:
-            return repr(fully_formatted)
-        elif output == "porcelain":
-            _echo(repr(fully_formatted), fg="white")
-        elif output == "json":
-            _echo(orjson.dumps({"prompt": fully_formatted}, option=orjson.OPT_INDENT_2).decode(), fg="white")
+        if machine: return repr(fully_formatted)
+        elif output == "porcelain": _echo(repr(fully_formatted), fg="white")
+        elif output == "json": _echo(orjson.dumps({"prompt": fully_formatted}, option=orjson.OPT_INDENT_2).decode(), fg="white")
         else:
             _echo(f"== Prompt for {model_name} ==\n", fg="magenta")
             _echo(fully_formatted, fg="white")
-    except AttributeError:
-        raise click.ClickException(f"Failed to determine a default prompt template for {model_name}.") from None
+    except AttributeError: raise click.ClickException(f"Failed to determine a default prompt template for {model_name}.") from None
 
 
 def load_notebook_metadata() -> DictStrAny:
-    with open(os.path.join(os.path.dirname(openllm.playground.__file__), "_meta.yml"), "r") as f:
-        content = yaml.safe_load(f)
-    if not all("description" in k for k in content.values()):
-        raise ValueError("Invalid metadata file. All entries must have a 'description' key.")
+    with open(os.path.join(os.path.dirname(openllm.playground.__file__), "_meta.yml"), "r") as f: content = yaml.safe_load(f)
+    if not all("description" in k for k in content.values()): raise ValueError("Invalid metadata file. All entries must have a 'description' key.")
     return content
 
 
 @cli.command()
 @click.argument("output-dir", default=None, required=False)
-@click.option(
-    "--port",
-    envvar="JUPYTER_PORT",
-    show_envvar=True,
-    show_default=True,
-    default=8888,
-    help="Default port for Jupyter server",
-)
+@click.option("--port", envvar="JUPYTER_PORT", show_envvar=True, show_default=True, default=8888, help="Default port for Jupyter server")
 @click.pass_context
 def playground(ctx: click.Context, output_dir: str | None, port: int) -> None:
     """OpenLLM Playground.
 
     A collections of notebooks to explore the capabilities of OpenLLM.
     This includes notebooks for fine-tuning, inference, and more.
 
@@ -2546,61 +1862,39 @@
     python -m openllm.playground.falcon_tuned --help
     ```
 
     \b
     > Note: This command requires Jupyter to be installed. Install it with 'pip install "openllm[playground]"'
     """
     if not is_jupyter_available() or not is_jupytext_available() or not is_notebook_available():
-        raise RuntimeError(
-            "Playground requires 'jupyter', 'jupytext', and 'notebook'. Install it with 'pip install \"openllm[playground]\"'"
-        )
+        raise RuntimeError("Playground requires 'jupyter', 'jupytext', and 'notebook'. Install it with 'pip install \"openllm[playground]\"'")
     metadata = load_notebook_metadata()
     _temp_dir = False
     if output_dir is None:
         _temp_dir = True
         output_dir = tempfile.mkdtemp(prefix="openllm-playground-")
-    else:
-        os.makedirs(os.path.abspath(os.path.expandvars(os.path.expanduser(output_dir))), exist_ok=True)
+    else: os.makedirs(os.path.abspath(os.path.expandvars(os.path.expanduser(output_dir))), exist_ok=True)
 
     _echo("The playground notebooks will be saved to: " + os.path.abspath(output_dir), fg="blue")
     for module in pkgutil.iter_modules(openllm.playground.__path__):
         if module.ispkg or os.path.exists(os.path.join(output_dir, module.name + ".ipynb")):
-            logger.debug(
-                "Skipping: %s (%s)",
-                module.name,
-                "File already exists" if not module.ispkg else f"{module.name} is a module",
-            )
-            continue
-        if not isinstance(module.module_finder, importlib.machinery.FileFinder):
+            logger.debug("Skipping: %s (%s)", module.name, "File already exists" if not module.ispkg else f"{module.name} is a module")
             continue
+        if not isinstance(module.module_finder, importlib.machinery.FileFinder): continue
         _echo("Generating notebook for: " + module.name, fg="magenta")
         markdown_cell = nbformat.v4.new_markdown_cell(metadata[module.name]["description"])
         f = jupytext.read(os.path.join(module.module_finder.path, module.name + ".py"))
         f.cells.insert(0, markdown_cell)
         jupytext.write(f, os.path.join(output_dir, module.name + ".ipynb"), fmt="notebook")
     try:
         subprocess.check_output(
-            [
-                sys.executable,
-                "-m",
-                "jupyter",
-                "notebook",
-                "--notebook-dir",
-                output_dir,
-                "--port",
-                str(port),
-                "--no-browser",
-                "--debug",
-            ]
+            [sys.executable, "-m", "jupyter", "notebook", "--notebook-dir", output_dir, "--port", str(port), "--no-browser", "--debug"]
         )
     except subprocess.CalledProcessError as e:
         _echo(e.output, fg="red")
         raise e
     except KeyboardInterrupt:
         _echo("\nShutting down Jupyter server...", fg="yellow")
-        if _temp_dir:
-            _echo("Note: You can access the generated notebooks in: " + output_dir, fg="blue")
+        if _temp_dir: _echo("Note: You can access the generated notebooks in: " + output_dir, fg="blue")
     ctx.exit(0)
 
-
-if __name__ == "__main__":
-    cli()
+if __name__ == "__main__": cli()
```

### Comparing `openllm-0.2.7/src/openllm/client.py` & `openllm-0.2.8/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/exceptions.py` & `openllm-0.2.8/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/testing.py` & `openllm-0.2.8/src/openllm/testing.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/bundle/__init__.py` & `openllm-0.2.8/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/bundle/_package.py` & `openllm-0.2.8/src/openllm/bundle/_package.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,126 +26,96 @@
 from packaging.version import Version
 from simple_di import Provide
 from simple_di import inject
 
 import bentoml
 from bentoml._internal.bento.build_config import BentoBuildConfig
 from bentoml._internal.bento.build_config import DockerOptions
+from bentoml._internal.bento.build_config import ModelSpec
 from bentoml._internal.bento.build_config import PythonOptions
 from bentoml._internal.configuration import get_debug_mode
 from bentoml._internal.configuration.containers import BentoMLContainer
-from bentoml._internal.models.model import ModelStore
 
-from ..exceptions import OpenLLMException
 from ..utils import DEBUG
 from ..utils import EnvVarMixin
 from ..utils import codegen
 from ..utils import device_count
 from ..utils import is_flax_available
 from ..utils import is_tf_available
 from ..utils import is_torch_available
 from ..utils import pkg
-from ..utils import resolve_user_filepath
 
 
 if t.TYPE_CHECKING:
     from fs.base import FS
 
     import openllm
     from bentoml._internal.bento import BentoStore
+    from bentoml._internal.models.model import ModelStore
 
 logger = logging.getLogger(__name__)
 
 OPENLLM_DEV_BUILD = "OPENLLM_DEV_BUILD"
 
 
 def build_editable(path: str) -> str | None:
     """Build OpenLLM if the OPENLLM_DEV_BUILD environment variable is set."""
-    if str(os.environ.get(OPENLLM_DEV_BUILD, False)).lower() != "true":
-        return
-
+    if str(os.environ.get(OPENLLM_DEV_BUILD, False)).lower() != "true": return
     # We need to build the package in editable mode, so that we can import it
     from build import ProjectBuilder
     from build.env import IsolatedEnvBuilder
-
     module_location = pkg.source_locations("openllm")
-    if not module_location:
-        raise RuntimeError(
-            "Could not find the source location of OpenLLM. Make sure to unset"
-            " OPENLLM_DEV_BUILD if you are developing OpenLLM."
-        )
+    if not module_location: raise RuntimeError("Could not find the source location of OpenLLM. Make sure to unset OPENLLM_DEV_BUILD if you are developing OpenLLM.")
     pyproject_path = Path(module_location).parent.parent / "pyproject.toml"
     if os.path.isfile(pyproject_path.__fspath__()):
         logger.info("OpenLLM is installed in editable mode. Generating built wheels...")
         with IsolatedEnvBuilder() as env:
             builder = ProjectBuilder(pyproject_path.parent)
             builder.python_executable = env.executable
             builder.scripts_dir = env.scripts_dir
             env.install(builder.build_system_requires)
             return builder.build("wheel", path, config_settings={"--global-option": "--quiet"})
-    raise RuntimeError(
-        "Custom OpenLLM build is currently not supported. Please install OpenLLM from PyPI or built it from Git source."
-    )
+    raise RuntimeError("Custom OpenLLM build is currently not supported. Please install OpenLLM from PyPI or built it from Git source.")
 
 
 def handle_package_version(package: str, has_dockerfile_template: bool, lower_bound: bool = True):
     version = Version(pkg.get_pkg_version(package))
     if version.is_devrelease:
-        if has_dockerfile_template:
-            logger.warning(
-                "Installed %s has version %s as a dev release. This means you have a custom build of %s with %s. Make sure to use custom dockerfile templates (--dockerfile-template) to setup %s correctly. See https://docs.bentoml.com/en/latest/guides/containerization.html#dockerfile-template for more information.",
-                package,
-                version,
-                package,
-                "CUDA support" if "cu" in str(version) else "more features",
-                package,
-            )
+        if has_dockerfile_template: logger.warning("Installed %s has version %s as a dev release. This means you have a custom build of %s with %s. Make sure to use custom dockerfile templates (--dockerfile-template) to setup %s correctly. See https://docs.bentoml.com/en/latest/guides/containerization.html#dockerfile-template for more information.", package, version, package, "CUDA support" if "cu" in str(version) else "more features", package)
         return package
     return f"{package}>={importlib.metadata.version(package)}" if lower_bound else package
 
 
 def construct_python_options(
     llm: openllm.LLM[t.Any, t.Any],
     llm_fs: FS,
     has_dockerfile_template: bool,
     extra_dependencies: tuple[str, ...] | None = None,
     adapter_map: dict[str, str | None] | None = None,
 ) -> PythonOptions:
     packages = ["openllm"]
-    if adapter_map is not None:
-        packages += ["openllm[fine-tune]"]
+    if adapter_map is not None: packages += ["openllm[fine-tune]"]
     # NOTE: add openllm to the default dependencies
     # if users has openllm custom built wheels, it will still respect
     # that since bentoml will always install dependencies from requirements.txt
     # first, then proceed to install everything inside the wheels/ folder.
-    if extra_dependencies is not None:
-        packages += [f"openllm[{k}]" for k in extra_dependencies]
+    if extra_dependencies is not None: packages += [f"openllm[{k}]" for k in extra_dependencies]
 
     req = llm.config["requirements"]
-    if req is not None:
-        packages.extend(req)
+    if req is not None: packages.extend(req)
 
-    if str(os.environ.get("BENTOML_BUNDLE_LOCAL_BUILD", False)).lower() == "false":
-        packages.append(f"bentoml>={'.'.join([str(i) for i in pkg.pkg_version_info('bentoml')])}")
+    if str(os.environ.get("BENTOML_BUNDLE_LOCAL_BUILD", False)).lower() == "false": packages.append(f"bentoml>={'.'.join([str(i) for i in pkg.pkg_version_info('bentoml')])}")
 
     env: EnvVarMixin = llm.config["env"]
     framework_envvar = env["framework_value"]
     if framework_envvar == "flax":
-        if not is_flax_available():
-            raise ValueError(f"Flax is not available, while {env.framework} is set to 'flax'")
-        packages.extend(
-            [
-                handle_package_version("flax", has_dockerfile_template),
-                handle_package_version("jax", has_dockerfile_template),
-                handle_package_version("jaxlib", has_dockerfile_template),
-            ]
-        )
+        if not is_flax_available(): raise ValueError(f"Flax is not available, while {env.framework} is set to 'flax'")
+        packages.extend([handle_package_version("flax", has_dockerfile_template), handle_package_version("jax", has_dockerfile_template), handle_package_version("jaxlib", has_dockerfile_template)])
     elif framework_envvar == "tf":
-        if not is_tf_available():
-            raise ValueError(f"TensorFlow is not available, while {env.framework} is set to 'tf'")
+        if not is_tf_available(): raise ValueError(f"TensorFlow is not available, while {env.framework} is set to 'tf'")
         candidates = (
             "tensorflow",
             "tensorflow-cpu",
             "tensorflow-gpu",
             "tf-nightly",
             "tf-nightly-cpu",
             "tf-nightly-gpu",
@@ -154,31 +124,27 @@
             "tensorflow-rocm",
             "tensorflow-macos",
         )
         # For the metadata, we have to look for both tensorflow and tensorflow-cpu
         for candidate in candidates:
             try:
                 pkgver = handle_package_version(candidate, has_dockerfile_template)
-                if pkgver == candidate:
-                    packages.extend(["tensorflow"])
+                if pkgver == candidate: packages.extend(["tensorflow"])
                 else:
                     _tf_version = importlib.metadata.version(candidate)
                     packages.extend([f"tensorflow>={_tf_version}"])
                 break
-            except importlib.metadata.PackageNotFoundError:
-                pass
+            except importlib.metadata.PackageNotFoundError: pass
     else:
-        if not is_torch_available():
-            raise ValueError("PyTorch is not available. Make sure to have it locally installed.")
+        if not is_torch_available(): raise ValueError("PyTorch is not available. Make sure to have it locally installed.")
         packages.extend([handle_package_version("torch", has_dockerfile_template)])
 
     wheels: list[str] = []
     built_wheels = build_editable(llm_fs.getsyspath("/"))
-    if built_wheels is not None:
-        wheels.append(llm_fs.getsyspath(f"/{built_wheels.split('/')[-1]}"))
+    if built_wheels is not None: wheels.append(llm_fs.getsyspath(f"/{built_wheels.split('/')[-1]}"))
 
     return PythonOptions(packages=packages, wheels=wheels, lock_packages=False)
 
 
 def construct_docker_options(
     llm: openllm.LLM[t.Any, t.Any],
     _: FS,
@@ -203,36 +169,32 @@
         env.framework: env.framework_value,
         env.config: f"'{llm.config.model_dump_json().decode()}'",
         "OPENLLM_MODEL": llm.config["model_name"],
         "OPENLLM_SERIALIZATION": serialisation_format,
         "OPENLLM_ADAPTER_MAP": f"'{orjson.dumps(adapter_map).decode()}'",
         "BENTOML_DEBUG": str(get_debug_mode()),
         "BENTOML_CONFIG_OPTIONS": f"'{_bentoml_config_options}'",
+        env.model_id: f"/home/bentoml/bento/models/{llm.tag.path()}",  # This is the default BENTO_PATH var
     }
 
-    if adapter_map:
-        env_dict["BITSANDBYTES_NOWELCOME"] = os.environ.get("BITSANDBYTES_NOWELCOME", "1")
+    if adapter_map: env_dict["BITSANDBYTES_NOWELCOME"] = os.environ.get("BITSANDBYTES_NOWELCOME", "1")
 
-    # We need to handle None separately here, as env from subprocess doesn't
-    # accept None value.
-    _env = EnvVarMixin(
-        llm.config["model_name"], bettertransformer=bettertransformer, quantize=quantize, runtime=runtime
-    )
+    # We need to handle None separately here, as env from subprocess doesn't accept None value.
+    _env = EnvVarMixin(llm.config["model_name"], bettertransformer=bettertransformer, quantize=quantize, runtime=runtime)
 
-    if _env.bettertransformer_value is not None:
-        env_dict[_env.bettertransformer] = _env.bettertransformer_value
-    if _env.quantize_value is not None:
-        env_dict[_env.quantize] = _env.quantize_value
+    if _env.bettertransformer_value is not None: env_dict[_env.bettertransformer] = str(_env.bettertransformer_value)
+    if _env.quantize_value is not None: env_dict[_env.quantize] = _env.quantize_value
     env_dict[_env.runtime] = _env.runtime_value
 
     return DockerOptions(
         cuda_version="11.8.0",
         env=env_dict,
         system_packages=["git"],
         dockerfile_template=dockerfile_template,
+        python_version="3.9",
     )
 
 
 @inject
 def create_bento(
     bento_tag: bentoml.Tag,
     llm_fs: FS,
@@ -247,125 +209,51 @@
     runtime: t.Literal["ggml", "transformers"] = "transformers",
     serialisation_format: t.Literal["safetensors", "legacy"] = "safetensors",
     _bento_store: BentoStore = Provide[BentoMLContainer.bento_store],
     _model_store: ModelStore = Provide[BentoMLContainer.model_store],
 ) -> bentoml.Bento:
     framework_envvar = llm.config["env"]["framework_value"]
     labels = dict(llm.identifying_params)
-    labels.update({"_type": llm.llm_type, "_framework": framework_envvar, "start_name": llm.config["start_name"]})
-
-    if adapter_map:
-        labels.update(adapter_map)
-
+    labels.update({"_type": llm.llm_type, "_framework": framework_envvar, "start_name": llm.config["start_name"], "base_name_or_path": llm.model_id, "bundler": "openllm.bundle"})
+    if adapter_map: labels.update(adapter_map)
     if isinstance(workers_per_resource, str):
-        if workers_per_resource == "round_robin":
-            workers_per_resource = 1.0
-        elif workers_per_resource == "conserved":
-            workers_per_resource = 1.0 if device_count() == 0 else float(1 / device_count())
+        if workers_per_resource == "round_robin": workers_per_resource = 1.0
+        elif workers_per_resource == "conserved": workers_per_resource = 1.0 if device_count() == 0 else float(1 / device_count())
         else:
-            try:
-                workers_per_resource = float(workers_per_resource)
-            except ValueError:
-                raise ValueError(
-                    "'workers_per_resource' only accept ['round_robin', 'conserved'] as possible strategies."
-                ) from None
+            try: workers_per_resource = float(workers_per_resource)
+            except ValueError: raise ValueError("'workers_per_resource' only accept ['round_robin', 'conserved'] as possible strategies.") from None
+    elif isinstance(workers_per_resource, int): workers_per_resource = float(workers_per_resource)
 
     logger.info("Building Bento for '%s'", llm.config["start_name"])
-
-    if adapter_map is not None:
-        if build_ctx is None:
-            raise ValueError("build_ctx is required when 'adapter_map' is not None")
-        updated_mapping: dict[str, str | None] = {}
-        for adapter_id, name in adapter_map.items():
-            try:
-                resolve_user_filepath(adapter_id, build_ctx)
-                src_folder_name = os.path.basename(adapter_id)
-                src_fs = fs.open_fs(build_ctx)
-                llm_fs.makedir(src_folder_name, recreate=True)
-                fs.copy.copy_dir(src_fs, adapter_id, llm_fs, src_folder_name)
-                updated_mapping[src_folder_name] = name
-            except FileNotFoundError:
-                # this is the remote adapter, then just added back
-                # note that there is a drawback here. If the path of the local adapter
-                # path have the same name as the remote, then we currently don't support
-                # that edge case.
-                updated_mapping[adapter_id] = name
-        adapter_map = updated_mapping
-
     # add service.py definition to this temporary folder
     codegen.write_service(llm, adapter_map, llm_fs)
 
+    llm_spec = ModelSpec.from_item({"tag": str(llm.tag), "alias": llm.tag.name})
     build_config = BentoBuildConfig(
         service=f"{llm.config['service_name']}:svc",
         name=bento_tag.name,
         labels=labels,
         description=f"OpenLLM service for {llm.config['start_name']}",
         include=list(llm_fs.walk.files()),
         exclude=["/venv", "/.venv", "__pycache__/", "*.py[cod]", "*$py.class"],
-        python=construct_python_options(
-            llm,
-            llm_fs,
-            dockerfile_template is None,
-            extra_dependencies,
-            adapter_map,
-        ),
-        docker=construct_docker_options(
-            llm,
-            llm_fs,
-            workers_per_resource,
-            quantize,
-            bettertransformer,
-            adapter_map,
-            dockerfile_template,
-            runtime,
-            serialisation_format,
-        ),
-    )
-
-    bento = bentoml.Bento.create(
-        build_config=build_config,
-        version=bento_tag.version,
-        build_ctx=llm_fs.getsyspath("/"),
+        python=construct_python_options(llm, llm_fs, dockerfile_template is None, extra_dependencies, adapter_map),
+        docker=construct_docker_options(llm, llm_fs, workers_per_resource, quantize, bettertransformer, adapter_map, dockerfile_template, runtime, serialisation_format),
+        models=[llm_spec],
     )
 
-    # Now we have to format the model_id accordingly based on the model_fs
-    model_type = bento.info.labels["_type"]
-    model_framework = bento.info.labels["_framework"]
-    # the models should have the type
-    try:
-        model_store = ModelStore(bento._fs.opendir("models"))
-        model = model_store.get(f"{model_framework}-{model_type}")
-    except fs.errors.ResourceNotFound:
-        # new behaviour with BentoML models
-        model = _model_store.get(f"{model_framework}-{model_type}")
-    except bentoml.exceptions.NotFound:
-        raise OpenLLMException(f"Failed to find models for {llm.config['start_name']}") from None
-
+    bento = bentoml.Bento.create(build_config=build_config, version=bento_tag.version, build_ctx=llm_fs.getsyspath("/"))
     # NOTE: the model_id_path here are only used for setting this environment variable within the container
     # built with for BentoLLM.
     service_fs_path = fs.path.join("src", llm.config["service_name"])
     service_path = bento._fs.getsyspath(service_fs_path)
-    with open(service_path, "r") as f:
-        service_contents = f.readlines()
-
-    rel_path = f"../models/{model.tag.path()}"
+    with open(service_path, "r") as f: service_contents = f.readlines()
 
     for it in service_contents:
-        if codegen.OPENLLM_MODEL_ID in it:
-            service_contents[service_contents.index(it)] = (
-                codegen.ModelIdFormatter(rel_path).vformat(it)[: -(len(codegen.OPENLLM_MODEL_ID) + 3)] + "\n"
-            )
-        if "__bento_name__" in it:
-            service_contents[service_contents.index(it)] = it.format(__bento_name__=str(bento.tag))
+        if "__bento_name__" in it: service_contents[service_contents.index(it)] = it.format(__bento_name__=str(bento.tag))
 
     script = "".join(service_contents)
-
-    if DEBUG:
-        logger.info("Generated script:\n%s", script)
+    if DEBUG: logger.info("Generated script:\n%s", script)
 
     bento._fs.writetext(service_fs_path, script)
-
-    signatures = inspect.signature(bento.save).parameters
-    if "model_store" in signatures:
-        return bento.save(bento_store=_bento_store, model_store=_model_store)
+    if "model_store" in inspect.signature(bento.save).parameters: return bento.save(bento_store=_bento_store, model_store=_model_store)
     # backward arguments. `model_store` is added recently
     return bento.save(bento_store=_bento_store)
```

### Comparing `openllm-0.2.7/src/openllm/bundle/oci/Dockerfile-builder` & `openllm-0.2.8/src/openllm/bundle/oci/Dockerfile-builder`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/bundle/oci/__init__.py` & `openllm-0.2.8/src/openllm/utils/dummy_pt_and_triton_objects.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""OCI-related utilities for OpenLLM.
 
-## TODO
-- generate compatible Sagemaker container
-- build custom kernels and CUDA 11.8
-- compose vLLM for PagedAttention
-"""
+from __future__ import annotations
+import typing as t
+
+from ..utils import DummyMetaclass
+from ..utils import require_backends
+
+
+class MPT(metaclass=DummyMetaclass):
+    _backends = ["torch", "triton"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["torch"])
```

### Comparing `openllm-0.2.7/src/openllm/models/__init__.py` & `openllm-0.2.8/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/models/auto/__init__.py` & `openllm-0.2.8/src/openllm/models/auto/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,111 +7,64 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""This module is derived from HuggingFace's AutoConfig, AutoModel, etc."""
-
 from __future__ import annotations
+import sys
 import typing as t
-
 import openllm
-
 from ...utils import LazyModule
 from ...utils import is_flax_available
 from ...utils import is_tf_available
 from ...utils import is_torch_available
 from ...utils import is_vllm_available
-
-
 _import_structure: dict[str, list[str]] = {
     "configuration_auto": ["AutoConfig", "CONFIG_MAPPING", "CONFIG_MAPPING_NAMES"],
     "modeling_auto": ["MODEL_MAPPING_NAMES"],
     "modeling_flax_auto": ["MODEL_FLAX_MAPPING_NAMES"],
     "modeling_tf_auto": ["MODEL_TF_MAPPING_NAMES"],
     "modeling_vllm_auto": ["MODEL_VLLM_MAPPING_NAMES"],
 }
-
 try:
-    if not is_torch_available():
-        raise openllm.exceptions.MissingDependencyError
-except openllm.exceptions.MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_auto"].extend(["AutoLLM", "MODEL_MAPPING"])
-
+    if not is_torch_available(): raise openllm.exceptions.MissingDependencyError
+except openllm.exceptions.MissingDependencyError: pass
+else: _import_structure["modeling_auto"].extend(["AutoLLM", "MODEL_MAPPING"])
 try:
-    if not is_vllm_available():
-        raise openllm.exceptions.MissingDependencyError
-except openllm.exceptions.MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_vllm_auto"].extend(["AutoVLLM", "MODEL_VLLM_MAPPING"])
-
-
+    if not is_vllm_available(): raise openllm.exceptions.MissingDependencyError
+except openllm.exceptions.MissingDependencyError: pass
+else: _import_structure["modeling_vllm_auto"].extend(["AutoVLLM", "MODEL_VLLM_MAPPING"])
 try:
-    if not is_flax_available():
-        raise openllm.exceptions.MissingDependencyError
-except openllm.exceptions.MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_flax_auto"].extend(["AutoFlaxLLM", "MODEL_FLAX_MAPPING"])
-
+    if not is_flax_available(): raise openllm.exceptions.MissingDependencyError
+except openllm.exceptions.MissingDependencyError: pass
+else: _import_structure["modeling_flax_auto"].extend(["AutoFlaxLLM", "MODEL_FLAX_MAPPING"])
 try:
-    if not is_tf_available():
-        raise openllm.exceptions.MissingDependencyError
-except openllm.exceptions.MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_tf_auto"].extend(["AutoTFLLM", "MODEL_TF_MAPPING"])
-
+    if not is_tf_available(): raise openllm.exceptions.MissingDependencyError
+except openllm.exceptions.MissingDependencyError: pass
+else: _import_structure["modeling_tf_auto"].extend(["AutoTFLLM", "MODEL_TF_MAPPING"])
 if t.TYPE_CHECKING:
     from .configuration_auto import CONFIG_MAPPING as CONFIG_MAPPING
     from .configuration_auto import CONFIG_MAPPING_NAMES as CONFIG_MAPPING_NAMES
     from .configuration_auto import AutoConfig as AutoConfig
     from .modeling_auto import MODEL_MAPPING_NAMES as MODEL_MAPPING_NAMES
     from .modeling_flax_auto import MODEL_FLAX_MAPPING_NAMES as MODEL_FLAX_MAPPING_NAMES
     from .modeling_tf_auto import MODEL_TF_MAPPING_NAMES as MODEL_TF_MAPPING_NAMES
     from .modeling_vllm_auto import MODEL_VLLM_MAPPING_NAMES as MODEL_VLLM_MAPPING_NAMES
-
     try:
-        if not is_torch_available():
-            raise openllm.exceptions.MissingDependencyError
-    except openllm.exceptions.MissingDependencyError:
-        pass
-    else:
-        from .modeling_auto import MODEL_MAPPING as MODEL_MAPPING
-        from .modeling_auto import AutoLLM as AutoLLM
-
+        if not is_torch_available(): raise openllm.exceptions.MissingDependencyError
+    except openllm.exceptions.MissingDependencyError: pass
+    else: from .modeling_auto import MODEL_MAPPING as MODEL_MAPPING, AutoLLM as AutoLLM
     try:
-        if not is_vllm_available():
-            raise openllm.exceptions.MissingDependencyError
-    except openllm.exceptions.MissingDependencyError:
-        pass
-    else:
-        from .modeling_vllm_auto import MODEL_VLLM_MAPPING as MODEL_VLLM_MAPPING
-        from .modeling_vllm_auto import AutoVLLM as AutoVLLM
-
+        if not is_vllm_available(): raise openllm.exceptions.MissingDependencyError
+    except openllm.exceptions.MissingDependencyError: pass
+    else: from .modeling_vllm_auto import MODEL_VLLM_MAPPING as MODEL_VLLM_MAPPING, AutoVLLM as AutoVLLM
     try:
-        if not is_flax_available():
-            raise openllm.exceptions.MissingDependencyError
-    except openllm.exceptions.MissingDependencyError:
-        pass
-    else:
-        from .modeling_flax_auto import MODEL_FLAX_MAPPING as MODEL_FLAX_MAPPING
-        from .modeling_flax_auto import AutoFlaxLLM as AutoFlaxLLM
-
+        if not is_flax_available(): raise openllm.exceptions.MissingDependencyError
+    except openllm.exceptions.MissingDependencyError: pass
+    else: from .modeling_flax_auto import MODEL_FLAX_MAPPING as MODEL_FLAX_MAPPING, AutoFlaxLLM as AutoFlaxLLM
     try:
-        if not is_tf_available():
-            raise openllm.exceptions.MissingDependencyError
-    except openllm.exceptions.MissingDependencyError:
-        pass
-    else:
-        from .modeling_tf_auto import MODEL_TF_MAPPING as MODEL_TF_MAPPING
-        from .modeling_tf_auto import AutoTFLLM as AutoTFLLM
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_tf_available(): raise openllm.exceptions.MissingDependencyError
+    except openllm.exceptions.MissingDependencyError: pass
+    else: from .modeling_tf_auto import MODEL_TF_MAPPING as MODEL_TF_MAPPING, AutoTFLLM as AutoTFLLM
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/auto/configuration_auto.py` & `openllm-0.2.8/src/openllm/models/auto/configuration_auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,41 +7,30 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 import typing as t
 from collections import OrderedDict
-
 import inflection
-
 import openllm
-
 from ...utils import ReprMixin
-
-
 if t.TYPE_CHECKING:
     import types
-    from collections import _odict_items
-    from collections import _odict_keys
-    from collections import _odict_values
-
+    from collections import _odict_items, _odict_keys, _odict_values
     ConfigOrderedDict = OrderedDict[str, type[openllm.LLMConfig]]
-
     ConfigKeysView = _odict_keys[str, type[openllm.LLMConfig]]
     ConfigValuesView = _odict_values[str, type[openllm.LLMConfig]]
     ConfigItemsView = _odict_items[str, type[openllm.LLMConfig]]
 else:
     ConfigKeysView = ConfigValuesView = ConfigItemsView = t.Any
     ConfigOrderedDict = OrderedDict
-
 # NOTE: This is the entrypoint when adding new model config
 CONFIG_MAPPING_NAMES = OrderedDict(
     [
         ("chatglm", "ChatGLMConfig"),
         ("dolly_v2", "DollyV2Config"),
         ("falcon", "FalconConfig"),
         ("flan_t5", "FlanT5Config"),
@@ -50,108 +39,57 @@
         ("mpt", "MPTConfig"),
         ("opt", "OPTConfig"),
         ("stablelm", "StableLMConfig"),
         ("starcoder", "StarCoderConfig"),
         ("baichuan", "BaichuanConfig"),
     ]
 )
-
-
 class _LazyConfigMapping(ConfigOrderedDict, ReprMixin):
     def __init__(self, mapping: OrderedDict[t.LiteralString, t.LiteralString]):
         self._mapping = mapping
         self._extra_content: dict[str, t.Any] = {}
         self._modules: dict[str, types.ModuleType] = {}
-
     def __getitem__(self, key: str) -> t.Any:
-        if key in self._extra_content:
-            return self._extra_content[key]
+        if key in self._extra_content: return self._extra_content[key]
         if key not in self._mapping:
-            if inflection.underscore(key) in self._mapping:
-                return self.__getitem__(inflection.underscore(key))
+            if inflection.underscore(key) in self._mapping: return self.__getitem__(inflection.underscore(key))
             raise KeyError(key)
-        value = self._mapping[key]
-        module_name = inflection.underscore(key)
-        if module_name not in self._modules:
-            self._modules[module_name] = openllm.utils.EnvVarMixin(module_name).module
-        if hasattr(self._modules[module_name], value):
-            return getattr(self._modules[module_name], value)
-
-        # Some of the mappings have entries model_type -> config of another model type. In that case we try to grab the
-        # object at the top level.
+        value, module_name = self._mapping[key], inflection.underscore(key)
+        if module_name not in self._modules: self._modules[module_name] = openllm.utils.EnvVarMixin(module_name).module
+        if hasattr(self._modules[module_name], value): return getattr(self._modules[module_name], value)
+        # Some of the mappings have entries model_type -> config of another model type. In that case we try to grab the object at the top level.
         return getattr(openllm, value)
-
     @property
-    def __repr_keys__(self) -> set[str]:
-        return set(self._mapping.keys())
-
-    def __repr__(self) -> str:
-        return ReprMixin.__repr__(self)
-
-    def __repr_args__(self) -> t.Generator[tuple[str, t.Any], t.Any, t.Any]:
-        yield from self._mapping.items()
-
-    def keys(self):
-        return t.cast(ConfigKeysView, list(self._mapping.keys()) + list(self._extra_content.keys()))
-
-    def values(self):
-        return t.cast(ConfigValuesView, [self[k] for k in self._mapping.keys()] + list(self._extra_content.values()))
-
-    def items(self):
-        return t.cast(
-            ConfigItemsView, [(k, self[k]) for k in self._mapping.keys()] + list(self._extra_content.items())
-        )
-
-    def __iter__(self):
-        return iter(list(self._mapping.keys()) + list(self._extra_content.keys()))
-
-    def __contains__(self, item: t.Any):
-        return item in self._mapping or item in self._extra_content
-
+    def __repr_keys__(self) -> set[str]: return set(self._mapping.keys())
+    def __repr__(self) -> str: return ReprMixin.__repr__(self)
+    def __repr_args__(self) -> t.Generator[tuple[str, t.Any], t.Any, t.Any]: yield from self._mapping.items()
+    def keys(self): return t.cast(ConfigKeysView, list(self._mapping.keys()) + list(self._extra_content.keys()))
+    def values(self): return t.cast(ConfigValuesView, [self[k] for k in self._mapping.keys()] + list(self._extra_content.values()))
+    def items(self): return t.cast(ConfigItemsView, [(k, self[k]) for k in self._mapping.keys()] + list(self._extra_content.items()))
+    def __iter__(self): return iter(list(self._mapping.keys()) + list(self._extra_content.keys()))
+    def __contains__(self, item: t.Any): return item in self._mapping or item in self._extra_content
     def register(self, key: str, value: t.Any):
-        """Register a new configuration in this mapping."""
-        if key in self._mapping.keys():
-            raise ValueError(f"'{key}' is already used by a OpenLLM config, pick another name.")
+        if key in self._mapping.keys(): raise ValueError(f"'{key}' is already used by a OpenLLM config, pick another name.")
         self._extra_content[key] = value
-
-
 CONFIG_MAPPING: dict[str, type[openllm.LLMConfig]] = _LazyConfigMapping(CONFIG_MAPPING_NAMES)
-
 # The below handle special alias when we call underscore to the name directly
 # without processing camelcase first.
 CONFIG_NAME_ALIASES: dict[str, str] = {
     "chat_glm": "chatglm",
     "stable_lm": "stablelm",
     "star_coder": "starcoder",
     "gpt_neo_x": "gpt_neox",
     "lla_ma": "llama",
 }
-
-
 class AutoConfig:
-    def __init__(self, *_: t.Any, **__: t.Any):
-        """This metaclass should be initialised via `AutoConfig.for_model`."""
-        raise EnvironmentError(
-            "Cannot instantiate AutoConfig directly. Please use `AutoConfig.for_model(model_name)` instead."
-        )
-
+    def __init__(self, *_: t.Any, **__: t.Any): raise EnvironmentError("Cannot instantiate AutoConfig directly. Please use `AutoConfig.for_model(model_name)` instead.")
     @classmethod
     def for_model(cls, model_name: str, **attrs: t.Any) -> openllm.LLMConfig:
         model_name = inflection.underscore(model_name)
-        if model_name in CONFIG_MAPPING:
-            return CONFIG_MAPPING[model_name].model_construct_env(**attrs)
-        raise ValueError(
-            f"Unrecognized configuration class for {model_name}. "
-            f"Model name should be one of {', '.join(CONFIG_MAPPING.keys())}."
-        )
-
+        if model_name in CONFIG_MAPPING: return CONFIG_MAPPING[model_name].model_construct_env(**attrs)
+        raise ValueError(f"Unrecognized configuration class for {model_name}. Model name should be one of {', '.join(CONFIG_MAPPING.keys())}.")
     @classmethod
     def infer_class_from_name(cls, name: str) -> type[openllm.LLMConfig]:
         model_name = inflection.underscore(name)
-        if model_name in CONFIG_NAME_ALIASES:
-            model_name = CONFIG_NAME_ALIASES[model_name]
-        if model_name in CONFIG_MAPPING:
-            return CONFIG_MAPPING[model_name]
-        raise ValueError(
-            f"Unrecognized configuration class for {model_name}. "
-            f"Model name should be one of {', '.join(CONFIG_MAPPING.keys())}."
-        )
+        if model_name in CONFIG_NAME_ALIASES: model_name = CONFIG_NAME_ALIASES[model_name]
+        if model_name in CONFIG_MAPPING: return CONFIG_MAPPING[model_name]
+        raise ValueError(f"Unrecognized configuration class for {model_name}. Model name should be one of {', '.join(CONFIG_MAPPING.keys())}.")
```

### Comparing `openllm-0.2.7/src/openllm/models/auto/factory.py` & `openllm-0.2.8/src/openllm/models/auto/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,106 +7,52 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 import importlib
 import inspect
 import logging
 import sys
 import typing as t
 from collections import OrderedDict
-
 import inflection
-
 import openllm
-
 from .configuration_auto import AutoConfig
 from ...utils import ReprMixin
-
-
 # NOTE: We need to do this so that overload can register
 # correct overloads to typing registry
-if sys.version_info[:2] >= (3, 11):
-    from typing import overload
-else:
-    from typing_extensions import overload
-
-
+if sys.version_info[:2] >= (3, 11): from typing import overload
+else: from typing_extensions import overload
 if t.TYPE_CHECKING:
     import types
-    from collections import _odict_items
-    from collections import _odict_keys
-    from collections import _odict_values
-
     from ..._llm import LLMRunner
-
+    from collections import _odict_items, _odict_keys, _odict_values
     ConfigModelOrderedDict = OrderedDict[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
     ConfigModelKeysView = _odict_keys[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
     ConfigModelValuesView = _odict_values[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
     ConfigModelItemsView = _odict_items[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
 else:
     ConfigModelKeysView = ConfigModelValuesView = ConfigModelItemsView = t.Any
     ConfigModelOrderedDict = OrderedDict
-
 logger = logging.getLogger(__name__)
-
-
 class BaseAutoLLMClass:
     _model_mapping: _LazyAutoMapping
-
-    def __init__(self, *args: t.Any, **attrs: t.Any):  # noqa
-        raise EnvironmentError(
-            f"Cannot instantiate {self.__class__.__name__} directly. "
-            "Please use '{self.__class__.__name__}.Runner(model_name)' instead."
-        )
-
+    def __init__(self, *args: t.Any, **attrs: t.Any): raise EnvironmentError(f"Cannot instantiate {self.__class__.__name__} directly. Please use '{self.__class__.__name__}.Runner(model_name)' instead.")
     @overload
     @classmethod
-    def for_model(
-        cls,
-        model: str,
-        model_id: str | None = None,
-        model_version: str | None = None,
-        return_runner_kwargs: t.Literal[False] = False,
-        llm_config: openllm.LLMConfig | None = ...,
-        ensure_available: t.Literal[False, True] = ...,
-        **attrs: t.Any,
-    ) -> openllm.LLM[t.Any, t.Any]:
-        ...
-
+    def for_model(cls, model: str, model_id: str | None = None, model_version: str | None = None, return_runner_kwargs: t.Literal[False] = False, llm_config: openllm.LLMConfig | None = ..., ensure_available: t.Literal[False, True] = ..., **attrs: t.Any) -> openllm.LLM[t.Any, t.Any]: ...
     @overload
     @classmethod
-    def for_model(
-        cls,
-        model: str,
-        model_id: str | None = None,
-        model_version: str | None = None,
-        return_runner_kwargs: t.Literal[True] = ...,
-        llm_config: openllm.LLMConfig | None = ...,
-        ensure_available: t.Literal[False, True] = ...,
-        **attrs: t.Any,
-    ) -> tuple[openllm.LLM[t.Any, t.Any], dict[str, t.Any]]:
-        ...
-
+    def for_model(cls, model: str, model_id: str | None = None, model_version: str | None = None, return_runner_kwargs: t.Literal[True] = ..., llm_config: openllm.LLMConfig | None = ..., ensure_available: t.Literal[False, True] = ..., **attrs: t.Any) -> tuple[openllm.LLM[t.Any, t.Any], dict[str, t.Any]]: ...
     @classmethod
-    def for_model(
-        cls,
-        model: str,
-        model_id: str | None = None,
-        model_version: str | None = None,
-        return_runner_kwargs: bool = False,
-        llm_config: openllm.LLMConfig | None = None,
-        ensure_available: bool = False,
-        **attrs: t.Any,
-    ) -> openllm.LLM[t.Any, t.Any] | tuple[openllm.LLM[t.Any, t.Any], dict[str, t.Any]]:
+    def for_model(cls, model: str, model_id: str | None = None, model_version: str | None = None, return_runner_kwargs: bool = False, llm_config: openllm.LLMConfig | None = None, ensure_available: bool = False, **attrs: t.Any) -> openllm.LLM[t.Any, t.Any] | tuple[openllm.LLM[t.Any, t.Any], dict[str, t.Any]]:
         """The lower level API for creating a LLM instance.
 
         ```python
         >>> import openllm
         >>> llm = openllm.AutoLLM.for_model("flan-t5")
         ```
 
@@ -124,179 +70,90 @@
             # The rest of kwargs is now passed to config
             llm_config = AutoConfig.for_model(model, **attrs)
             attrs = llm_config.__openllm_extras__
         # the rest of attrs will be saved to __openllm_extras__
         if type(llm_config) in cls._model_mapping.keys():
             model_class = cls._model_mapping[type(llm_config)]
             llm = model_class.from_pretrained(model_id, model_version=model_version, llm_config=llm_config, **attrs)
-            if ensure_available:
-                llm.ensure_model_id_exists()
-            if not return_runner_kwargs:
-                return llm
+            if ensure_available: llm.ensure_model_id_exists()
+            if not return_runner_kwargs: return llm
             return llm, to_runner_attrs
-        raise ValueError(
-            f"Unrecognized configuration class {llm_config.__class__} for this kind of AutoLLM: {cls.__name__}.\n"
-            f"LLM type should be one of {', '.join(c.__name__ for c in cls._model_mapping.keys())}."
-        )
-
+        raise ValueError(f"Unrecognized configuration class {llm_config.__class__} for this kind of AutoLLM: {cls.__name__}.\nLLM type should be one of {', '.join(c.__name__ for c in cls._model_mapping.keys())}.")
     @classmethod
-    def create_runner(cls, model: str, model_id: str | None = None, **attrs: t.Any) -> LLMRunner:
+    def create_runner(cls, model: str, model_id: str | None = None, **attrs: t.Any) -> LLMRunner[t.Any, t.Any]:
         """Create a LLM Runner for the given model name.
 
         Args:
             model: The model name to instantiate.
             model_id: The pretrained model name to instantiate.
             **attrs: Additional keyword arguments passed along to the specific configuration class.
 
         Returns:
             A LLM instance.
         """
         llm, runner_attrs = cls.for_model(model, model_id, return_runner_kwargs=True, **attrs)
         return llm.to_runner(**runner_attrs)
-
     @classmethod
     def register(cls, config_class: type[openllm.LLMConfig], llm_class: type[openllm.LLM[t.Any, t.Any]]):
         """Register a new model for this class.
 
         Args:
             config_class: The configuration corresponding to the model to register.
             llm_class: The runnable to register.
         """
-        if hasattr(llm_class, "config_class") and llm_class.config_class is not config_class:
-            raise ValueError(
-                "The model class you are passing has a `config_class` attribute that is not consistent with the "
-                f"config class you passed (model has {llm_class.config_class} and you passed {config_class}. Fix "
-                "one of those so they match!"
-            )
+        if hasattr(llm_class, "config_class") and llm_class.config_class is not config_class: raise ValueError("The model class you are passing has a `config_class` attribute that is not consistent with the config class you passed (model has {llm_class.config_class} and you passed {config_class}. Fix one of those so they match!")
         cls._model_mapping.register(config_class, llm_class)
-
-
 def getattribute_from_module(module: types.ModuleType, attr: t.Any) -> t.Any:
-    if attr is None:
-        return
-    if isinstance(attr, tuple):
-        return tuple(getattribute_from_module(module, a) for a in attr)
-    if hasattr(module, attr):
-        return getattr(module, attr)
+    if attr is None: return
+    if isinstance(attr, tuple): return tuple(getattribute_from_module(module, a) for a in attr)
+    if hasattr(module, attr): return getattr(module, attr)
     # Some of the mappings have entries model_type -> object of another model type. In that case we try to grab the
     # object at the top level.
     openllm_module = importlib.import_module("openllm")
-
     if module != openllm_module:
-        try:
-            return getattribute_from_module(openllm_module, attr)
-        except ValueError:
-            raise ValueError(f"Could not find {attr} neither in {module} nor in {openllm_module}!") from None
-    else:
-        raise ValueError(f"Could not find {attr} in {openllm_module}!")
-
-
+        try: return getattribute_from_module(openllm_module, attr)
+        except ValueError: raise ValueError(f"Could not find {attr} neither in {module} nor in {openllm_module}!") from None
+    else: raise ValueError(f"Could not find {attr} in {openllm_module}!")
 class _LazyAutoMapping(ConfigModelOrderedDict, ReprMixin):
     """Based on transformers.models.auto.configuration_auto._LazyAutoMapping.
 
     This OrderedDict values() and keys() returns the list instead, so you don't
     have to do list(mapping.values()) to get the list of values.
     """
-
-    def __init__(
-        self,
-        config_mapping: OrderedDict[t.LiteralString, t.LiteralString],
-        model_mapping: OrderedDict[t.LiteralString, t.LiteralString],
-    ):
+    def __init__(self, config_mapping: OrderedDict[t.LiteralString, t.LiteralString], model_mapping: OrderedDict[t.LiteralString, t.LiteralString]):
         self._config_mapping = config_mapping
         self._reverse_config_mapping = {v: k for k, v in config_mapping.items()}
         self._model_mapping = model_mapping
         self._extra_content: dict[t.Any, t.Any] = {}
         self._modules: dict[str, types.ModuleType] = {}
-
-    def __len__(self):
-        common_keys = set(self._config_mapping.keys()).intersection(self._model_mapping.keys())
-        return len(common_keys) + len(self._extra_content)
-
+    def __len__(self): return len(set(self._config_mapping.keys()).intersection(self._model_mapping.keys())) + len(self._extra_content)
     def __getitem__(self, key: type[openllm.LLMConfig]) -> type[openllm.LLM[t.Any, t.Any]]:
-        if key in self._extra_content:
-            return self._extra_content[key]
+        if key in self._extra_content: return self._extra_content[key]
         model_type = self._reverse_config_mapping[key.__name__]
-        if model_type in self._model_mapping:
-            model_name = self._model_mapping[model_type]
-            return self._load_attr_from_module(model_type, model_name)
-
+        if model_type in self._model_mapping: return self._load_attr_from_module(model_type, self._model_mapping[model_type])
         # Maybe there was several model types associated with this config.
         model_types = [k for k, v in self._config_mapping.items() if v == key.__name__]
         for mtype in model_types:
-            if mtype in self._model_mapping:
-                model_name = self._model_mapping[mtype]
-                return self._load_attr_from_module(mtype, model_name)
+            if mtype in self._model_mapping: return self._load_attr_from_module(mtype, self._model_mapping[mtype])
         raise KeyError(key)
-
     def _load_attr_from_module(self, model_type: str, attr: str) -> t.Any:
         module_name = inflection.underscore(model_type)
-        if module_name not in self._modules:
-            self._modules[module_name] = importlib.import_module(f".{module_name}", "openllm.models")
+        if module_name not in self._modules: self._modules[module_name] = importlib.import_module(f".{module_name}", "openllm.models")
         return getattribute_from_module(self._modules[module_name], attr)
-
-    def keys(self):
-        mapping_keys = [
-            self._load_attr_from_module(key, name)
-            for key, name in self._config_mapping.items()
-            if key in self._model_mapping.keys()
-        ]
-        return t.cast(ConfigModelKeysView, mapping_keys + list(self._extra_content.keys()))
-
+    def keys(self): return t.cast(ConfigModelKeysView, [self._load_attr_from_module(key, name) for key, name in self._config_mapping.items() if key in self._model_mapping.keys()] + list(self._extra_content.keys()))
     @property
-    def __repr_keys__(self) -> set[str]:
-        return set(self._config_mapping.keys())
-
-    def __repr__(self) -> str:
-        return ReprMixin.__repr__(self)
-
-    def __repr_args__(self) -> t.Generator[tuple[str, tuple[str, str]], t.Any, t.Any]:
-        yield from (
-            (key, (value, self._model_mapping[key]))
-            for key, value in self._config_mapping.items()
-            if key in self._model_mapping
-        )
-
-    def __bool__(self):
-        return bool(self.keys())
-
-    def values(self):
-        mapping_values = [
-            self._load_attr_from_module(key, name)
-            for key, name in self._model_mapping.items()
-            if key in self._config_mapping.keys()
-        ]
-        return t.cast(ConfigModelValuesView, mapping_values + list(self._extra_content.values()))
-
-    def items(self):
-        mapping_items = [
-            (
-                self._load_attr_from_module(key, self._config_mapping[key]),
-                self._load_attr_from_module(key, self._model_mapping[key]),
-            )
-            for key in self._model_mapping.keys()
-            if key in self._config_mapping.keys()
-        ]
-        return t.cast(ConfigModelItemsView, mapping_items + list(self._extra_content.items()))
-
-    def __iter__(self):
-        return iter(self.keys())
-
+    def __repr_keys__(self) -> set[str]: return set(self._config_mapping.keys())
+    def __repr__(self) -> str: return ReprMixin.__repr__(self)
+    def __repr_args__(self) -> t.Generator[tuple[str, tuple[str, str]], t.Any, t.Any]: yield from ((key, (value, self._model_mapping[key])) for key, value in self._config_mapping.items() if key in self._model_mapping)
+    def __bool__(self): return bool(self.keys())
+    def values(self): return t.cast(ConfigModelValuesView, [self._load_attr_from_module(key, name) for key, name in self._model_mapping.items() if key in self._config_mapping.keys()] + list(self._extra_content.values()))
+    def items(self): return t.cast(ConfigModelItemsView, [(self._load_attr_from_module(key, self._config_mapping[key]), self._load_attr_from_module(key, self._model_mapping[key])) for key in self._model_mapping.keys() if key in self._config_mapping.keys()] + list(self._extra_content.items()))
+    def __iter__(self): return iter(self.keys())
     def __contains__(self, item: t.Any):
-        if item in self._extra_content:
-            return True
-        if not hasattr(item, "__name__") or item.__name__ not in self._reverse_config_mapping:
-            return False
-        model_type = self._reverse_config_mapping[item.__name__]
-        return model_type in self._model_mapping
-
+        if item in self._extra_content: return True
+        if not hasattr(item, "__name__") or item.__name__ not in self._reverse_config_mapping: return False
+        return self._reverse_config_mapping[item.__name__] in self._model_mapping
     def register(self, key: t.Any, value: t.Any):
-        """Register a new model in this mapping."""
         if hasattr(key, "__name__") and key.__name__ in self._reverse_config_mapping:
-            model_type = self._reverse_config_mapping[key.__name__]
-            if model_type in self._model_mapping.keys():
-                raise ValueError(f"'{key}' is already used by a OpenLLM model.")
-
+            if self._reverse_config_mapping[key.__name__] in self._model_mapping.keys(): raise ValueError(f"'{key}' is already used by a OpenLLM model.")
         self._extra_content[key] = value
-
-
 __all__ = ["BaseAutoLLMClass", "_LazyAutoMapping"]
```

### Comparing `openllm-0.2.7/src/openllm/models/auto/modeling_auto.py` & `openllm-0.2.8/src/openllm/models/auto/modeling_auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 from collections import OrderedDict
-
 from .configuration_auto import CONFIG_MAPPING_NAMES
 from .factory import BaseAutoLLMClass
 from .factory import _LazyAutoMapping
-
-
 MODEL_MAPPING_NAMES = OrderedDict(
     [
         ("chatglm", "ChatGLM"),
         ("dolly_v2", "DollyV2"),
         ("falcon", "Falcon"),
         ("flan_t5", "FlanT5"),
         ("gpt_neox", "GPTNeoX"),
@@ -31,13 +28,10 @@
         ("mpt", "MPT"),
         ("opt", "OPT"),
         ("stablelm", "StableLM"),
         ("starcoder", "StarCoder"),
         ("baichuan", "Baichuan"),
     ]
 )
-
 MODEL_MAPPING = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_MAPPING_NAMES)
-
-
 class AutoLLM(BaseAutoLLMClass):
     _model_mapping = MODEL_MAPPING
```

### Comparing `openllm-0.2.7/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.2.8/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,28 +7,21 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 from collections import OrderedDict
-
 from .configuration_auto import CONFIG_MAPPING_NAMES
 from .factory import BaseAutoLLMClass
 from .factory import _LazyAutoMapping
-
-
 MODEL_FLAX_MAPPING_NAMES = OrderedDict(
     [
         ("flan_t5", "FlaxFlanT5"),
         ("opt", "FlaxOPT"),
     ]
 )
-
 MODEL_FLAX_MAPPING = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_FLAX_MAPPING_NAMES)
-
-
 class AutoFlaxLLM(BaseAutoLLMClass):
     _model_mapping = MODEL_FLAX_MAPPING
```

### Comparing `openllm-0.2.7/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.2.8/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,21 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 from collections import OrderedDict
-
 from .configuration_auto import CONFIG_MAPPING_NAMES
 from .factory import BaseAutoLLMClass
 from .factory import _LazyAutoMapping
-
-
 MODEL_TF_MAPPING_NAMES = OrderedDict(
     [
         ("flan_t5", "TFFlanT5"),
         ("opt", "TFOPT"),
     ]
 )
-
 MODEL_TF_MAPPING = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_TF_MAPPING_NAMES)
-
-
 class AutoTFLLM(BaseAutoLLMClass):
     _model_mapping = MODEL_TF_MAPPING
```

### Comparing `openllm-0.2.7/src/openllm/models/auto/modeling_vllm_auto.py` & `openllm-0.2.8/src/openllm/models/auto/modeling_vllm_auto.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,27 +7,21 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 from collections import OrderedDict
-
 from .configuration_auto import CONFIG_MAPPING_NAMES
 from .factory import BaseAutoLLMClass
 from .factory import _LazyAutoMapping
-
-
 MODEL_VLLM_MAPPING_NAMES = OrderedDict(
     [
         ("llama", "VLLMLlaMA"),
+        ("opt", "VLLMOPT")
     ]
 )
-
 MODEL_VLLM_MAPPING = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_VLLM_MAPPING_NAMES)
-
-
 class AutoVLLM(BaseAutoLLMClass):
     _model_mapping = MODEL_VLLM_MAPPING
```

### Comparing `openllm-0.2.7/src/openllm/models/baichuan/__init__.py` & `openllm-0.2.8/src/openllm/models/baichuan/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,45 +7,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_cpm_kernels_available
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_baichuan": ["BaichuanConfig", "START_BAICHUAN_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_baichuan": ["BaichuanConfig", "START_BAICHUAN_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available() or not is_cpm_kernels_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_baichuan"] = ["Baichuan"]
-
+    if not is_torch_available() or not is_cpm_kernels_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_baichuan"] = ["Baichuan"]
 if t.TYPE_CHECKING:
     from .configuration_baichuan import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_baichuan import START_BAICHUAN_COMMAND_DOCSTRING as START_BAICHUAN_COMMAND_DOCSTRING
     from .configuration_baichuan import BaichuanConfig as BaichuanConfig
 
     try:
-        if not is_torch_available() or not is_cpm_kernels_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_baichuan import Baichuan as Baichuan
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available() or not is_cpm_kernels_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_baichuan import Baichuan as Baichuan
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/baichuan/configuration_baichuan.py` & `openllm-0.2.8/src/openllm/models/baichuan/configuration_baichuan.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
-
 import openllm
-
-
 class BaichuanConfig(openllm.LLMConfig):
     """Baichuan-7B is an open-source, large-scale pre-trained language model developed by Baichuan Intelligent Technology.
 
     Baichuan-7B is based on Transformer architecture,
     which contains 7 billion parameters and trained on approximately 1.2 trillion tokens.
     It supports both Chinese and English languages with a context window length of 4096.
     It has achieved the best performance among models of the same size on standard Chinese
     and English benchmarks (C-Eval, MMLU, etc).
     Refer to [Baichuan-7B's GitHub page](https://github.com/baichuan-inc/Baichuan-7B) for more information.
     """
-
     __config__ = {
         "name_type": "lowercase",
         "trust_remote_code": True,
         "timeout": 3600000,
         "requires_gpu": True,
         "url": "https://github.com/baichuan-inc/Baichuan-7B",
         "requirements": ["cpm-kernels", "sentencepiece"],
@@ -41,21 +37,18 @@
             "baichuan-inc/baichuan-13b-base",
             "baichuan-inc/baichuan-13b-chat",
             "fireballoon/baichuan-vicuna-chinese-7b",
             "fireballoon/baichuan-vicuna-7b",
             "hiyouga/baichuan-7b-sft",
         ],
     }
-
     class GenerationConfig:
         max_new_tokens: int = 2048
         top_p: float = 0.7
         temperature: float = 0.95
-
-
 START_BAICHUAN_COMMAND_DOCSTRING = """\
 Run a LLMServer for Baichuan model.
 
 \b
 > See more information about Baichuan at [baichuan-inc/Baichuan-7B](https://github.com/baichuan-inc/Baichuan-7B)
 
 \b
@@ -67,9 +60,8 @@
 Baichuan Runner will use baichuan-inc/Baichuan-7B as the default model. To change to any other
 saved pretrained Baichuan, provide ``OPENLLM_Baichuan_MODEL_ID='fireballoon/baichuan-vicuna-chinese-7b'``
 or provide `--model-id` flag when running ``openllm start baichuan``:
 
 \b
 $ openllm start baichuan --model-id='fireballoon/baichuan-vicuna-chinese-7b'
 """
-
 DEFAULT_PROMPT_TEMPLATE = """{instruction}"""
```

### Comparing `openllm-0.2.7/src/openllm/models/baichuan/modeling_baichuan.py` & `openllm-0.2.8/src/openllm/models/baichuan/modeling_baichuan.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,73 +9,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 import typing as t
-
 import openllm
-
 from .configuration_baichuan import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
-
-
 if t.TYPE_CHECKING:
     import torch
-
     import transformers
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-
-
 class Baichuan(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerBase"]):
     __openllm_internal__ = True
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        top_p: float | None = None,
-        temperature: float | None = None,
-        use_default_prompt_template: bool = False,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, top_p: float | None = None, temperature: float | None = None, use_default_prompt_template: bool = False, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
         # NOTE: The rest of attrs should be kwargs for GenerationConfig
-        generate_kwargs = {
-            "max_new_tokens": max_new_tokens,
-            "top_p": top_p,
-            "temperature": temperature,
-            **attrs,
-        }
-
+        generate_kwargs = {"max_new_tokens": max_new_tokens, "top_p": top_p, "temperature": temperature, **attrs}
         return prompt_text, generate_kwargs, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
-        return generation_result[0]
-
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
         with torch.inference_mode(), torch.autocast("cuda", dtype=torch.float16):
-            outputs = self.model.generate(
-                **inputs,
-                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-            )
+            outputs = self.model.generate(**inputs, generation_config=self.config.model_construct_env(**attrs).to_generation_config())
             return self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
```

### Comparing `openllm-0.2.7/src/openllm/models/chatglm/__init__.py` & `openllm-0.2.8/src/openllm/models/chatglm/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,45 +7,28 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_cpm_kernels_available
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_chatglm": ["ChatGLMConfig", "START_CHATGLM_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_chatglm": ["ChatGLMConfig", "START_CHATGLM_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available() or not is_cpm_kernels_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_chatglm"] = ["ChatGLM"]
-
+    if not is_torch_available() or not is_cpm_kernels_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_chatglm"] = ["ChatGLM"]
 if t.TYPE_CHECKING:
     from .configuration_chatglm import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_chatglm import START_CHATGLM_COMMAND_DOCSTRING as START_CHATGLM_COMMAND_DOCSTRING
     from .configuration_chatglm import ChatGLMConfig as ChatGLMConfig
-
     try:
-        if not is_torch_available() or not is_cpm_kernels_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_chatglm import ChatGLM as ChatGLM
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available() or not is_cpm_kernels_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_chatglm import ChatGLM as ChatGLM
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.2.8/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
-
 import openllm
-
-
 class ChatGLMConfig(openllm.LLMConfig):
     """ChatGLM is an open bilingual language model based on [General Language Model (GLM)](https://github.com/THUDM/GLM) framework.
 
     With the quantization technique, users can deploy locally on consumer-grade graphics cards
     (only 6GB of GPU memory is required at the INT4 quantization level).
 
     ChatGLM-6B uses technology similar to ChatGPT, optimized for Chinese QA and dialogue.
     The model is trained for about 1T tokens of Chinese and English corpus, supplemented by supervised fine-tuning,
     feedback bootstrap, and reinforcement learning wit human feedback.
     With only about 6.2 billion parameters, the model is able to generate answers that are in line
     with human preference.
 
     Refer to [ChatGLM's GitHub page](https://github.com/THUDM/ChatGLM-6B) for more information.
     """
-
     __config__ = {
         "name_type": "lowercase",
         "trust_remote_code": True,
         "timeout": 3600000,
         "requires_gpu": True,
         "url": "https://github.com/THUDM/ChatGLM-6B",
         "requirements": ["cpm-kernels", "sentencepiece"],
@@ -44,30 +40,25 @@
             "thudm/chatglm-6b",
             "thudm/chatglm-6b-int8",
             "thudm/chatglm-6b-int4",
             "thudm/chatglm2-6b",
             "thudm/chatglm2-6b-int4",
         ],
     }
-
     retain_history: bool = openllm.LLMConfig.Field(
         False,
         description="""Whether to retain history given to the model.
         If set to True, then the model will retain given history.""",
     )
-
     use_half_precision: bool = openllm.LLMConfig.Field(True, description="Whether to use half precision for model.")
-
     class GenerationConfig:
         max_new_tokens: int = 2048
         num_beams: int = 1
         top_p: float = 0.7
         temperature: float = 0.95
-
-
 START_CHATGLM_COMMAND_DOCSTRING = """\
 Run a LLMServer for ChatGLM model.
 
 \b
 > See more information about ChatGLM at [THUDM/ChatGLM-6b](https://huggingface.co/thudm/chatglm-6b)
 
 \b
@@ -79,9 +70,8 @@
 ChatGLM Runner will use THUDM/ChatGLM-6b as the default model. To change to any other ChatGLM
 saved pretrained, or a fine-tune ChatGLM, provide ``OPENLLM_CHATGLM_MODEL_ID='thudm/chatglm-6b-int8'``
 or provide `--model-id` flag when running ``openllm start chatglm``:
 
 \b
 $ openllm start chatglm --model-id='thudm/chatglm-6b-int8'
 """
-
 DEFAULT_PROMPT_TEMPLATE = """{instruction}"""
```

### Comparing `openllm-0.2.7/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.2.8/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,99 +8,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
+import logging
 import typing as t
-
 import bentoml
 import openllm
-
+from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
+from ..._prompt import default_formatter
 from ...utils import generate_labels
-
-
-if t.TYPE_CHECKING:
-    import torch
-
-    import transformers
-else:
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-
-
-class ChatGLM(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerFast"]):
+if t.TYPE_CHECKING: import transformers
+else: transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
+logger = logging.getLogger(__name__)
+class FlaxOPT(openllm.LLM["transformers.TFOPTForCausalLM", "transformers.GPT2Tokenizer"]):
     __openllm_internal__ = True
+    @property
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {}, {"padding_side": "left", "truncation_side": "left"}
 
-    def import_model(self, *args: t.Any, trust_remote_code: bool = True, **attrs: t.Any) -> bentoml.Model:
-        _, tokenizer_attrs = self.llm_parameters
-
-        return bentoml.transformers.save_model(
-            self.tag,
-            transformers.AutoModel.from_pretrained(self.model_id, trust_remote_code=trust_remote_code),
-            labels=generate_labels(self),
-            custom_objects={
-                "tokenizer": transformers.AutoTokenizer.from_pretrained(
-                    self.model_id, trust_remote_code=trust_remote_code, **tokenizer_attrs
-                )
-            },
-        )
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        num_beams: int | None = None,
-        top_p: float | None = None,
-        temperature: float | None = None,
-        chat_history: list[str] | None = None,
-        use_default_prompt_template: bool = False,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
-        prompt_text = ""
-
-        if use_default_prompt_template and chat_history is not None:
-            for i, (old_query, response) in enumerate(chat_history):
-                prompt_text += f"[Round {i}]\n问：{old_query}\n答：{response}\n"  # noqa: RUF001
-            prompt_text += f"[Round {len(chat_history)}]\n问：{prompt}\n答："  # noqa: RUF001
-        else:
-            prompt_text = prompt
-
-        postprocess_generate_kwargs = {"chat_history": chat_history if chat_history is not None else None}
-
-        # NOTE: The rest of attrs should be kwargs for GenerationConfig
-        generate_kwargs = {
-            "max_new_tokens": max_new_tokens,
-            "num_beams": num_beams,
-            "top_p": top_p,
-            "temperature": temperature,
-            **attrs,
-        }
-
-        return prompt_text, generate_kwargs, postprocess_generate_kwargs
-
-    def postprocess_generate(
-        self,
-        prompt: str,
-        generation_result: tuple[str, list[tuple[str, str]]],
-        *,
-        chat_history: list[tuple[str, str]] | None = None,
-        **attrs: t.Any,
-    ):
-        generated, history = generation_result
-        if self.config.retain_history:
-            assert chat_history is not None, "'retain_history' is True while there is no history provided."
-            chat_history.extend(history)
-        return generated
-
-    def generate(self, prompt: str, **attrs: t.Any) -> tuple[str, list[tuple[str, str]]]:
-        with torch.inference_mode():
-            self.model.eval()
-            # Only use half precision if the model is not yet quantized
-            if self.config.use_half_precision:
-                self.model.half()
-            return self.model.chat(
-                self.tokenizer,
-                prompt,
-                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-            )
+    def import_model(self, *args: t.Any, trust_remote_code: bool = False, **attrs: t.Any) -> bentoml.Model:
+        config, tokenizer = transformers.AutoConfig.from_pretrained(self.model_id), transformers.AutoTokenizer.from_pretrained(self.model_id, **self.llm_parameters[-1])
+        tokenizer.pad_token_id = config.pad_token_id
+        return bentoml.transformers.save_model(self.tag, transformers.FlaxAutoModelForCausalLM.from_pretrained(self.model_id, **attrs), custom_objects={"tokenizer": tokenizer}, labels=generate_labels(self))
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, temperature: float | None = None, top_k: int | None = None, num_return_sequences: int | None = None, repetition_penalty: float | None = None, use_default_prompt_template: bool = False, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+        if use_default_prompt_template:
+            template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
+            prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_k": top_k, "num_return_sequences": num_return_sequences, "repetition_penalty": repetition_penalty}, {}
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **attrs: t.Any) -> str:
+        if len(generation_result) == 1: return generation_result[0]
+        if self.config.format_outputs: return "Generated result:\n" + "\n -".join(generation_result)
+        else: return "\n".join(generation_result)
+    def generate(self, prompt: str, **attrs: t.Any) -> list[str]: return self.tokenizer.batch_decode( self.model.generate(**self.tokenizer(prompt, return_tensors="np"), do_sample=True, generation_config=self.config.model_construct_env(**attrs).to_generation_config()).sequences, skip_special_tokens=True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openllm-0.2.7/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.2.8/src/openllm/models/dolly_v2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,44 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_dolly_v2": ["DollyV2Config", "START_DOLLY_V2_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_dolly_v2": ["DollyV2Config", "START_DOLLY_V2_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_dolly_v2"] = ["DollyV2"]
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_dolly_v2"] = ["DollyV2"]
 if t.TYPE_CHECKING:
     from .configuration_dolly_v2 import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_dolly_v2 import START_DOLLY_V2_COMMAND_DOCSTRING as START_DOLLY_V2_COMMAND_DOCSTRING
     from .configuration_dolly_v2 import DollyV2Config as DollyV2Config
-
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_dolly_v2 import DollyV2 as DollyV2
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_dolly_v2 import DollyV2 as DollyV2
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.2.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,55 +9,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 import typing as t
-
 import openllm
-
-
-if t.TYPE_CHECKING:
-    from transformers import PreTrainedTokenizer
-
-
+if t.TYPE_CHECKING: import transformers
 class DollyV2Config(openllm.LLMConfig):
     """Databricks` Dolly is an instruction-following large language model trained on the Databricks machine learning platform that is licensed for commercial use.
 
     Based on pythia-12b, Dolly is trained on ~15k instruction/response fine tuning records databricks-dolly-15k
     generated by Databricks employees in capability domains from the InstructGPT paper, including brainstorming,
     classification, closed QA, generation, information extraction, open QA and summarization.
 
     dolly-v2-12b is not a state-of-the-art model, but does exhibit surprisingly high quality instruction
     following behavior not characteristic of the foundation model on which it is based.
 
     Refer to [Databricks's Dolly page](https://github.com/databrickslabs/dolly) for more information.
     """
-
     __config__ = {
         "timeout": 3600000,
         "url": "https://github.com/databrickslabs/dolly",
         "architecture": "GPTNeoXForCausalLM",
         "default_id": "databricks/dolly-v2-3b",
         "model_ids": ["databricks/dolly-v2-3b", "databricks/dolly-v2-7b", "databricks/dolly-v2-12b"],
     }
-
     return_full_text: bool = openllm.LLMConfig.Field(
         False, description="Whether to return the full prompt to the users."
     )
-
     class GenerationConfig:
         temperature: float = 0.9
         top_p: float = 0.92
         top_k: int = 5
         max_new_tokens: int = 256
         eos_token_id: int = 50277  # NOTE: from get_special_token_id(self.tokenizer, END_KEY)
-
-
 START_DOLLY_V2_COMMAND_DOCSTRING = """\
 Run a LLMServer for dolly-v2 model.
 
 \b
 > See more information about dolly-v2 at [databricks/dolly-v2-3b](https://huggingface.co/databricks/dolly-v2-3b)
 
 \b
@@ -69,38 +58,27 @@
 Dolly-v2 Runner will use databricks/dolly-v2-3b as the default model. To change to any other dolly-v2
 saved pretrained, or a fine-tune dolly-v2, provide ``OPENLLM_DOLLY_V2_MODEL_ID='databricks/dolly-v2-7b'``
 or provide `--model-id` flag when running ``openllm start dolly-v2``:
 
 \b
 $ openllm start dolly-v2 --model-id databricks/dolly-v2-7b
 """
-
 INSTRUCTION_KEY = "### Instruction:"
 RESPONSE_KEY = "### Response:"
 END_KEY = "### End"
-INTRO_BLURB = (
-    "Below is an instruction that describes a task. Write a response that appropriately completes the request."
-)
-
+INTRO_BLURB = "Below is an instruction that describes a task. Write a response that appropriately completes the request."
 # NOTE: This is the prompt that is used for generating responses using an already
 # trained model.  It ends with the response key, where the job of the model is to provide
 # the completion that follows it (i.e. the response itself).
 DEFAULT_PROMPT_TEMPLATE = """{intro}
 {instruction_key}
 {instruction}
 {response_key}
-""".format(
-    intro=INTRO_BLURB,
-    instruction_key=INSTRUCTION_KEY,
-    instruction="{instruction}",
-    response_key=RESPONSE_KEY,
-)
-
-
-def get_special_token_id(tokenizer: PreTrainedTokenizer, key: str) -> int:
+""".format(intro=INTRO_BLURB, instruction_key=INSTRUCTION_KEY, instruction="{instruction}", response_key=RESPONSE_KEY)
+def get_special_token_id(tokenizer: transformers.PreTrainedTokenizer, key: str) -> int:
     """Gets the token ID for a given string that has been added to the tokenizer as a special token.
 
     When training, we configure the tokenizer so that the sequences like "### Instruction:" and "### End" are
     treated specially and converted to a single, new token.  This retrieves the token ID each of these keys map to.
 
     Args:
         tokenizer: the tokenizer
@@ -109,10 +87,9 @@
     Raises:
         RuntimeError: if more than one ID was generated
 
     Returns:
         int: the token ID for the given key.
     """
     token_ids = tokenizer.encode(key)
-    if len(token_ids) > 1:
-        raise ValueError(f"Expected only a single token for '{key}' but found {token_ids}")
+    if len(token_ids) > 1: raise ValueError(f"Expected only a single token for '{key}' but found {token_ids}")
     return token_ids[0]
```

### Comparing `openllm-0.2.7/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.2.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,292 +11,122 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 import logging
 import re
 import typing as t
-
 import openllm
-
 from .configuration_dolly_v2 import DEFAULT_PROMPT_TEMPLATE
 from .configuration_dolly_v2 import END_KEY
 from .configuration_dolly_v2 import RESPONSE_KEY
 from .configuration_dolly_v2 import get_special_token_id
-
-
 if t.TYPE_CHECKING:
-    import tensorflow as tf
     import torch
-
     import transformers
+    import tensorflow as tf
 else:
     tf = openllm.utils.LazyLoader("tf", globals(), "tensorflow")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-
 logger = logging.getLogger(__name__)
-
-
 @t.overload
-def get_pipeline(
-    model: transformers.PreTrainedModel,
-    tokenizer: transformers.PreTrainedTokenizer,
-    _init: t.Literal[True] = True,
-    **attrs: t.Any,
-) -> transformers.Pipeline:
-    ...
-
-
+def get_pipeline(model: transformers.PreTrainedModel, tokenizer: transformers.PreTrainedTokenizer, _init: t.Literal[True] = True, **attrs: t.Any) -> transformers.Pipeline: ...
 @t.overload
-def get_pipeline(
-    model: transformers.PreTrainedModel,
-    tokenizer: transformers.PreTrainedTokenizer,
-    _init: t.Literal[False] = ...,
-    **attrs: t.Any,
-) -> type[transformers.Pipeline]:
-    ...
-
-
-def get_pipeline(
-    model: transformers.PreTrainedModel,
-    tokenizer: transformers.PreTrainedTokenizer,
-    _init: bool = False,
-    **attrs: t.Any,
-) -> type[transformers.Pipeline] | transformers.Pipeline:
+def get_pipeline(model: transformers.PreTrainedModel, tokenizer: transformers.PreTrainedTokenizer, _init: t.Literal[False] = ..., **attrs: t.Any) -> type[transformers.Pipeline]: ...
+def get_pipeline(model: transformers.PreTrainedModel, tokenizer: transformers.PreTrainedTokenizer, _init: bool = False, **attrs: t.Any) -> type[transformers.Pipeline] | transformers.Pipeline:
     class InstructionTextGenerationPipeline(transformers.Pipeline):
-        def __init__(
-            self,
-            *args: t.Any,
-            do_sample: bool = True,
-            max_new_tokens: int = 256,
-            top_p: float = 0.92,
-            top_k: int = 0,
-            **kwargs: t.Any,
-        ):
-            """Initialize the pipeline.
-
-            Args:
-                do_sample: Whether or not to use sampling. Defaults to True.
-                max_new_tokens: Max new tokens after the prompt to generate. Defaults to 128.
-                top_p: If set to float < 1, only the smallest set of most probable tokens with
-                       probabilities that add up to top_p or higher are kept for generation. Defaults to 0.92.
-                top_k: The number of highest probability vocabulary tokens to keep for top-k-filtering. Defaults to 0.
-                *args: Additional positional arguments to be passed to ``transformers.Pipeline``.
-                **kwargs: Additional keyword arguments to be passed to ``transformers.Pipeline``.
-            """
-            super().__init__(
-                *args,
-                model=model,
-                tokenizer=tokenizer,
-                do_sample=do_sample,
-                max_new_tokens=max_new_tokens,
-                top_p=top_p,
-                top_k=top_k,
-                **kwargs,
-            )
-
+        def __init__(self, *args: t.Any, do_sample: bool = True, max_new_tokens: int = 256, top_p: float = 0.92, top_k: int = 0, **kwargs: t.Any): super().__init__(*args, model=model, tokenizer=tokenizer, do_sample=do_sample, max_new_tokens=max_new_tokens, top_p=top_p, top_k=top_k, **kwargs)
         def _sanitize_parameters(self, return_full_text: bool | None = None, **generate_kwargs: t.Any):
-            if t.TYPE_CHECKING:
-                assert self.tokenizer is not None
+            if t.TYPE_CHECKING: assert self.tokenizer is not None
             preprocess_params: dict[str, t.Any] = {}
-
             # newer versions of the tokenizer configure the response key as a special token.  newer versions still may
             # append a newline to yield a single token.  find whatever token is configured for the response key.
-            tokenizer_response_key = next(
-                (token for token in self.tokenizer.additional_special_tokens if token.startswith(RESPONSE_KEY)), None
-            )
-
+            tokenizer_response_key = next((token for token in self.tokenizer.additional_special_tokens if token.startswith(RESPONSE_KEY)), None)
             response_key_token_id = None
             end_key_token_id = None
             if tokenizer_response_key:
                 try:
                     response_key_token_id = get_special_token_id(self.tokenizer, tokenizer_response_key)
                     end_key_token_id = get_special_token_id(self.tokenizer, END_KEY)
-
                     # Ensure generation stops once it generates "### End"
                     generate_kwargs["eos_token_id"] = end_key_token_id
-                except ValueError:
-                    pass
-
+                except ValueError: pass
             forward_params = generate_kwargs
             postprocess_params = {"response_key_token_id": response_key_token_id, "end_key_token_id": end_key_token_id}
-
-            if return_full_text is not None:
-                postprocess_params["return_full_text"] = return_full_text
-
+            if return_full_text is not None: postprocess_params["return_full_text"] = return_full_text
             return preprocess_params, forward_params, postprocess_params
-
         def preprocess(self, input_: str, **generate_kwargs: t.Any):
-            if t.TYPE_CHECKING:
-                assert self.tokenizer is not None
+            if t.TYPE_CHECKING: assert self.tokenizer is not None
             prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=input_)
             inputs = self.tokenizer(prompt_text, return_tensors="pt")
             inputs["prompt_text"] = prompt_text
             inputs["instruction_text"] = input_
             return inputs
-
         def _forward(self, model_inputs: dict[str, t.Any], **generate_kwargs: t.Any):
-            if t.TYPE_CHECKING:
-                assert self.tokenizer is not None
-            input_ids = model_inputs["input_ids"]
-            attention_mask = model_inputs.get("attention_mask", None)
-
-            if input_ids.shape[1] == 0:
-                input_ids = None
-                attention_mask = None
-                in_b = 1
-            else:
-                in_b = input_ids.shape[0]
-
-            generated_sequence = self.model.generate(
-                input_ids=input_ids.to(self.model.device) if input_ids is not None else None,
-                attention_mask=attention_mask.to(self.model.device) if attention_mask is not None else None,
-                pad_token_id=self.tokenizer.pad_token_id,
-                **generate_kwargs,
-            )
-
+            if t.TYPE_CHECKING: assert self.tokenizer is not None
+            input_ids, attention_mask = model_inputs["input_ids"], model_inputs.get("attention_mask", None)
+            if input_ids.shape[1] == 0: input_ids, attention_mask, in_b = None, None, 1
+            else: in_b = input_ids.shape[0]
+            generated_sequence = self.model.generate(input_ids=input_ids.to(self.model.device) if input_ids is not None else None, attention_mask=attention_mask.to(self.model.device) if attention_mask is not None else None, pad_token_id=self.tokenizer.pad_token_id, **generate_kwargs)
             out_b = generated_sequence.shape[0]
-            if self.framework == "pt":
-                generated_sequence = generated_sequence.reshape(in_b, out_b // in_b, *generated_sequence.shape[1:])
-            elif self.framework == "tf":
-                generated_sequence = tf.reshape(
-                    generated_sequence, (in_b, out_b // in_b, *generated_sequence.shape[1:])
-                )
-
+            if self.framework == "pt": generated_sequence = generated_sequence.reshape(in_b, out_b // in_b, *generated_sequence.shape[1:])
+            elif self.framework == "tf": generated_sequence = tf.reshape(generated_sequence, (in_b, out_b // in_b, *generated_sequence.shape[1:]))
             instruction_text = model_inputs.pop("instruction_text")
-            return {
-                "generated_sequence": generated_sequence,
-                "input_ids": input_ids,
-                "instruction_text": instruction_text,
-            }
-
-        def postprocess(
-            self,
-            model_outputs: dict[str, t.Any],
-            response_key_token_id: int,
-            end_key_token_id: int,
-            return_full_text: bool = False,
-        ):
-            if t.TYPE_CHECKING:
-                assert self.tokenizer is not None
-            generated_sequence = model_outputs["generated_sequence"][0]
-            instruction_text = model_outputs["instruction_text"]
+            return {"generated_sequence": generated_sequence, "input_ids": input_ids, "instruction_text": instruction_text}
 
+        def postprocess(self, model_outputs: dict[str, t.Any], response_key_token_id: int, end_key_token_id: int, return_full_text: bool = False):
+            if t.TYPE_CHECKING: assert self.tokenizer is not None
+            generated_sequence, instruction_text = model_outputs["generated_sequence"][0], model_outputs["instruction_text"]
             generated_sequence: list[list[int]] = generated_sequence.numpy().tolist()
             records: list[dict[t.Literal["generated_text"], str]] = []
             for sequence in generated_sequence:
                 # The response will be set to this variable if we can identify it.
                 decoded = None
-
                 # If we have token IDs for the response and end, then we can find the tokens and only decode between them.
                 if response_key_token_id and end_key_token_id:
                     # Find where "### Response:" is first found in the generated tokens.  Considering this is part of the
                     # prompt, we should definitely find it.  We will return the tokens found after this token.
-                    try:
-                        response_pos = sequence.index(response_key_token_id)
-                    except ValueError:
-                        logger.warning("Could not find response key %s in: %s", response_key_token_id, sequence)
-                        response_pos = None
-
+                    try: response_pos = sequence.index(response_key_token_id)
+                    except ValueError: response_pos = None
+                    if response_pos is None: logger.warning("Could not find response key %s in: %s", response_key_token_id, sequence)
                     if response_pos:
                         # Next find where "### End" is located.  The model has been trained to end its responses with this
                         # sequence (or actually, the token ID it maps to, since it is a special token).  We may not find
                         # this token, as the response could be truncated.  If we don't find it then just return everything
                         # to the end.  Note that even though we set eos_token_id, we still see the this token at the end.
-                        try:
-                            end_pos = sequence.index(end_key_token_id)
-                        except ValueError:
-                            end_pos = None
-
+                        try: end_pos = sequence.index(end_key_token_id)
+                        except ValueError: end_pos = None
                         decoded = self.tokenizer.decode(sequence[response_pos + 1 : end_pos]).strip()
-
                 if not decoded:
                     # Otherwise we'll decode everything and use a regex to find the response and end.
-
                     fully_decoded = self.tokenizer.decode(sequence)
-
                     # The response appears after "### Response:".  The model has been trained to append "### End" at the
                     # end.
                     m = re.search(r"#+\s*Response:\s*(.+?)#+\s*End", fully_decoded, flags=re.DOTALL)
-
-                    if m:
-                        decoded = m.group(1).strip()
+                    if m: decoded = m.group(1).strip()
                     else:
                         # The model might not generate the "### End" sequence before reaching the max tokens.  In this case,
                         # return everything after "### Response:".
                         m = re.search(r"#+\s*Response:\s*(.+)", fully_decoded, flags=re.DOTALL)
-                        if m:
-                            decoded = m.group(1).strip()
-                        else:
-                            logger.warning("Failed to find response in:\n%s", fully_decoded)
-
+                        if m: decoded = m.group(1).strip()
+                        else: logger.warning("Failed to find response in:\n%s", fully_decoded)
                 # If the full text is requested, then append the decoded text to the original instruction.
                 # This technically isn't the full text, as we format the instruction in the prompt the model has been
                 # trained on, but to the client it will appear to be the full text.
-                if return_full_text:
-                    decoded = f"{instruction_text}\n{decoded}"
-
+                if return_full_text: decoded = f"{instruction_text}\n{decoded}"
                 rec = {"generated_text": decoded}
-
                 records.append(rec)
-
             return records
 
-    if _init:
-        return InstructionTextGenerationPipeline()
+    if _init: return InstructionTextGenerationPipeline()
     return InstructionTextGenerationPipeline
-
-
 class DollyV2(openllm.LLM["transformers.Pipeline", "transformers.PreTrainedTokenizer"]):
     __openllm_internal__ = True
-
     @property
-    def import_kwargs(self):
-        model_kwds = {
-            "device_map": "auto" if torch.cuda.is_available() else None,
-            "torch_dtype": torch.bfloat16,
-        }
-        tokenizer_kwds = {"padding_side": "left"}
-        return model_kwds, tokenizer_kwds
-
-    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.Pipeline:
-        return get_pipeline(
-            model=transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs),
-            tokenizer=self.tokenizer,
-            _init=True,
-            return_full_text=self.config.return_full_text,
-        )
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        temperature: float | None = None,
-        top_k: int | None = None,
-        top_p: float | None = None,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
-        # NOTE: The rest of attrs should be kwargs for GenerationConfig
-        generate_kwargs = {
-            "max_new_tokens": max_new_tokens,
-            "top_k": top_k,
-            "top_p": top_p,
-            "temperature": temperature,
-            **attrs,
-        }
-
-        return prompt, generate_kwargs, {}
-
-    def postprocess_generate(
-        self, prompt: str, generation_result: list[dict[t.Literal["generated_text"], str]], **_: t.Any
-    ) -> str:
-        return generation_result[0]["generated_text"]
-
+    def import_kwargs(self): return {"device_map": "auto" if torch.cuda.is_available() else None, "torch_dtype": torch.bfloat16}, {"padding_side": "left"}
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.Pipeline: return get_pipeline(model=transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs), tokenizer=self.tokenizer, _init=True, return_full_text=self.config.return_full_text)
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, temperature: float | None = None, top_k: int | None = None, top_p: float | None = None, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]: return prompt, {"max_new_tokens": max_new_tokens, "top_k": top_k, "top_p": top_p, "temperature": temperature, **attrs}, {}
+    def postprocess_generate(self, prompt: str, generation_result: list[dict[t.Literal["generated_text"], str]], **_: t.Any) -> str: return generation_result[0]["generated_text"]
     def generate(self, prompt: str, **attrs: t.Any) -> list[dict[t.Literal["generated_text"], str]]:
-        with torch.inference_mode():
-            llm_config = self.config.model_construct_env(**attrs)
-            return self.model(
-                prompt,
-                return_full_text=llm_config.return_full_text,
-                generation_config=llm_config.to_generation_config(),
-            )
+        llm_config = self.config.model_construct_env(**attrs)
+        with torch.inference_mode(): return self.model(prompt, return_full_text=llm_config.return_full_text, generation_config=llm_config.to_generation_config())
```

### Comparing `openllm-0.2.7/src/openllm/models/falcon/__init__.py` & `openllm-0.2.8/src/openllm/models/falcon/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,44 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_falcon": ["FalconConfig", "START_FALCON_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_falcon": ["FalconConfig", "START_FALCON_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_falcon"] = ["Falcon"]
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_falcon"] = ["Falcon"]
 if t.TYPE_CHECKING:
     from .configuration_falcon import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_falcon import START_FALCON_COMMAND_DOCSTRING as START_FALCON_COMMAND_DOCSTRING
     from .configuration_falcon import FalconConfig as FalconConfig
-
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_falcon import Falcon as Falcon
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_falcon import Falcon as Falcon
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.2.8/src/openllm/models/falcon/configuration_falcon.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
-
 import openllm
-
-
 class FalconConfig(openllm.LLMConfig):
     """Falcon-7B is a 7B parameters causal decoder-only model built by TII and trained on 1,500B tokens of [RefinedWeb](https://huggingface.co/datasets/tiiuae/falcon-refinedweb) enhanced with curated corpora.
 
     It is made available under the TII Falcon LLM License.
 
     Refer to [Falcon's HuggingFace page](https://huggingface.co/tiiuae/falcon-7b) for more information.
     """
-
     __config__ = {
         "name_type": "lowercase",
         "trust_remote_code": True,
         "requires_gpu": True,
         "timeout": int(36e6),
         "url": "https://falconllm.tii.ae/",
         "requirements": ["einops", "xformers"],
@@ -46,23 +42,20 @@
                 "lora_alpha": 16,
                 "lora_dropout": 0.1,
                 "bias": "none",
                 "target_modules": ["query_key_value", "dense", "dense_h_to_4h", "dense_4h_to_h"],
             },
         ),
     }
-
     class GenerationConfig:
         max_new_tokens: int = 200
         top_k: int = 10
         num_return_sequences: int = 1
         num_beams: int = 4
         early_stopping: bool = True
-
-
 START_FALCON_COMMAND_DOCSTRING = """\
 Run a LLMServer for FalconLM model.
 
 \b
 > See more information about falcon at [tiiuae/falcon-7b](https://huggingface.co/tiiuae/falcon-7b)
 
 \b
@@ -74,12 +67,11 @@
 FalconLM Runner will use tiiuae/falcon-7b as the default model. To change to any other FalconLM
 saved pretrained, or a fine-tune FalconLM, provide ``OPENLLM_FALCON_MODEL_ID='tiiuae/falcon-7b-instruct'``
 or provide `--model-id` flag when running ``openllm start falcon``:
 
 \b
 $ openllm start falcon --model-id tiiuae/falcon-7b-instruct
 """
-
 DEFAULT_PROMPT_TEMPLATE = """{context}
 {user_name}: {instruction}
 {agent}:
 """
```

### Comparing `openllm-0.2.7/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.2.8/src/openllm/models/falcon/modeling_falcon.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,109 +7,44 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 import typing as t
-
 import openllm
-
 from .configuration_falcon import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
-
-
 if t.TYPE_CHECKING:
     import torch
-
     import transformers
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-
-
 class Falcon(openllm.LLM["transformers.PreTrainedModel", "transformers.PreTrainedTokenizerBase"]):
     __openllm_internal__ = True
-
     @property
-    def import_kwargs(self):
-        model_kwds = {"torch_dtype": torch.bfloat16, "device_map": "auto" if torch.cuda.is_available() else None}
-        tokenizer_kwds: dict[str, t.Any] = {}
-        return model_kwds, tokenizer_kwds
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        top_k: int | None = None,
-        num_return_sequences: int | None = None,
-        eos_token_id: int | None = None,
-        use_default_prompt_template: bool = False,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {"torch_dtype": torch.bfloat16, "device_map": "auto" if torch.cuda.is_available() else None}, {}
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, top_k: int | None = None, num_return_sequences: int | None = None, eos_token_id: int | None = None, use_default_prompt_template: bool = False, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument instead of "
-                    "kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        generation_config = {
-            "max_new_tokens": max_new_tokens,
-            "top_k": top_k,
-            "num_return_sequences": num_return_sequences,
-            "eos_token_id": eos_token_id,
-            **attrs,
-        }
-
-        return prompt_text, generation_config, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
-        return generation_result[0]
-
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "top_k": top_k, "num_return_sequences": num_return_sequences, "eos_token_id": eos_token_id, **attrs}, {}
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        eos_token_id = attrs.pop("eos_token_id", self.tokenizer.eos_token_id)
-        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        with torch.inference_mode(), torch.autocast("cuda", dtype=torch.float16):
-            outputs = self.model.generate(
-                input_ids=inputs["input_ids"],
-                attention_mask=inputs["attention_mask"],
-                generation_config=self.config.model_construct_env(
-                    eos_token_id=eos_token_id, **attrs
-                ).to_generation_config(),
-            )
-            return self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
-
-    def generate_one(
-        self, prompt: str, stop: list[str], **preprocess_generate_kwds: t.Any
-    ) -> list[dict[t.Literal["generated_text"], str]]:
-        from ..._generation import StopSequenceCriteria
-
-        max_new_tokens = preprocess_generate_kwds.pop("max_new_tokens", 200)
-        encoded_inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        src_len = encoded_inputs["input_ids"].shape[1]
-        stopping_criteria = preprocess_generate_kwds.pop("stopping_criteria", transformers.StoppingCriteriaList([]))
-        stopping_criteria.append(StopSequenceCriteria(stop, self.tokenizer))
-        outputs = self.model.generate(
-            encoded_inputs["input_ids"], max_new_tokens=max_new_tokens, stopping_criteria=stopping_criteria
-        )
-
-        result = self.tokenizer.decode(outputs[0].tolist()[src_len:])
+        eos_token_id, inputs = attrs.pop("eos_token_id", self.tokenizer.eos_token_id), self.tokenizer(prompt, return_tensors="pt").to(self.device)
+        with torch.inference_mode(), torch.autocast("cuda", dtype=torch.float16): return self.tokenizer.batch_decode(self.model.generate(input_ids=inputs["input_ids"], attention_mask=inputs["attention_mask"], generation_config=self.config.model_construct_env( eos_token_id=eos_token_id, **attrs).to_generation_config()), skip_special_tokens=True)
+    def generate_one(self, prompt: str, stop: list[str], **preprocess_generate_kwds: t.Any) -> list[dict[t.Literal["generated_text"], str]]:
+        max_new_tokens, encoded_inputs = preprocess_generate_kwds.pop("max_new_tokens", 200), self.tokenizer(prompt, return_tensors="pt").to(self.device)
+        src_len, stopping_criteria = encoded_inputs["input_ids"].shape[1], preprocess_generate_kwds.pop("stopping_criteria", transformers.StoppingCriteriaList([]))
+        stopping_criteria.append(openllm.StopSequenceCriteria(stop, self.tokenizer))
+        result = self.tokenizer.decode(self.model.generate(encoded_inputs["input_ids"], max_new_tokens=max_new_tokens, stopping_criteria=stopping_criteria)[0].tolist()[src_len:])
         # Inference API returns the stop sequence
         for stop_seq in stop:
-            if result.endswith(stop_seq):
-                result = result[: -len(stop_seq)]
+            if result.endswith(stop_seq): result = result[: -len(stop_seq)]
         return [{"generated_text": result}]
```

### Comparing `openllm-0.2.7/src/openllm/models/flan_t5/__init__.py` & `openllm-0.2.8/src/openllm/models/flan_t5/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,77 +9,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_flax_available
 from ...utils import is_tf_available
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_flan_t5": ["FlanT5Config", "START_FLAN_T5_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_flan_t5": ["FlanT5Config", "START_FLAN_T5_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_flan_t5"] = ["FlanT5"]
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_flan_t5"] = ["FlanT5"]
 try:
-    if not is_flax_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_flax_flan_t5"] = ["FlaxFlanT5"]
-
+    if not is_flax_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_flax_flan_t5"] = ["FlaxFlanT5"]
 try:
-    if not is_tf_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_tf_flan_t5"] = ["TFFlanT5"]
-
-
+    if not is_tf_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_tf_flan_t5"] = ["TFFlanT5"]
 if t.TYPE_CHECKING:
     from .configuration_flan_t5 import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_flan_t5 import START_FLAN_T5_COMMAND_DOCSTRING as START_FLAN_T5_COMMAND_DOCSTRING
     from .configuration_flan_t5 import FlanT5Config as FlanT5Config
-
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_flan_t5 import FlanT5 as FlanT5
-
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_flan_t5 import FlanT5 as FlanT5
     try:
-        if not is_flax_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_flax_flan_t5 import FlaxFlanT5 as FlaxFlanT5
-
+        if not is_flax_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_flax_flan_t5 import FlaxFlanT5 as FlaxFlanT5
     try:
-        if not is_tf_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_tf_flan_t5 import TFFlanT5 as TFFlanT5
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_tf_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_tf_flan_t5 import TFFlanT5 as TFFlanT5
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.2.8/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,18 +8,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
-
 import openllm
+class FlanT5Config(openllm.LLMConfig):
+    """FLAN-T5 was released in the paper [Scaling Instruction-Finetuned Language Models](https://arxiv.org/pdf/2210.11416.pdf).
 
+    It is an enhanced version of T5 that has been finetuned in a mixture of tasks.
 
+    Refer to [FLAN-T5's page](https://huggingface.co/docs/transformers/model_doc/flan-t5) for more information.
+    """
+    __config__ = {
+        "url": "https://huggingface.co/docs/transformers/model_doc/flan-t5",
+        "default_id": "google/flan-t5-large",
+        "architecture": "T5ForConditionalGeneration",
+        "model_ids": [
+            "google/flan-t5-small",
+            "google/flan-t5-base",
+            "google/flan-t5-large",
+            "google/flan-t5-xl",
+            "google/flan-t5-xxl",
+        ],
+        "model_type": "seq2seq_lm",
+    }
+    class GenerationConfig:
+        temperature: float = 0.9
+        max_new_tokens: int = 2048
+        top_k: int = 50
+        top_p: float = 0.4
+        repetition_penalty = 1.0
 START_FLAN_T5_COMMAND_DOCSTRING = """\
 Run a LLMServer for FLAN-T5 model.
 
 \b
 > See more information about FLAN-T5 at [huggingface/transformers](https://huggingface.co/docs/transformers/model_doc/flan-t5)
 
 \b
@@ -37,39 +60,8 @@
 FLAN-T5 Runner will use google/flan-t5-large as the default model. To change to any other FLAN-T5
 saved pretrained, or a fine-tune FLAN-T5, provide ``OPENLLM_FLAN_T5_MODEL_ID='google/flan-t5-xxl'``
 or provide `--model-id` flag when running ``openllm start flan-t5``:
 
 \b
 $ openllm start flan-t5 --model-id google/flan-t5-xxl
 """
-
 DEFAULT_PROMPT_TEMPLATE = """Answer the following question:\nQuestion: {instruction}\nAnswer:"""
-
-
-class FlanT5Config(openllm.LLMConfig):
-    """FLAN-T5 was released in the paper [Scaling Instruction-Finetuned Language Models](https://arxiv.org/pdf/2210.11416.pdf).
-
-    It is an enhanced version of T5 that has been finetuned in a mixture of tasks.
-
-    Refer to [FLAN-T5's page](https://huggingface.co/docs/transformers/model_doc/flan-t5) for more information.
-    """
-
-    __config__ = {
-        "url": "https://huggingface.co/docs/transformers/model_doc/flan-t5",
-        "default_id": "google/flan-t5-large",
-        "architecture": "T5ForConditionalGeneration",
-        "model_ids": [
-            "google/flan-t5-small",
-            "google/flan-t5-base",
-            "google/flan-t5-large",
-            "google/flan-t5-xl",
-            "google/flan-t5-xxl",
-        ],
-        "model_type": "seq2seq_lm",
-    }
-
-    class GenerationConfig:
-        temperature: float = 0.9
-        max_new_tokens: int = 2048
-        top_k: int = 50
-        top_p: float = 0.4
-        repetition_penalty = 1.0
```

### Comparing `openllm-0.2.7/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.2.8/src/openllm/models/gpt_neox/modeling_gpt_neox.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,76 +8,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
+import logging
 import typing as t
-
 import openllm
-
-from .configuration_flan_t5 import DEFAULT_PROMPT_TEMPLATE
+from .configuration_gpt_neox import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
-
-
-if t.TYPE_CHECKING:
-    import torch
-
-    import transformers  # noqa: F401
-else:
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-
-
-class FlanT5(openllm.LLM["transformers.T5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
+if t.TYPE_CHECKING: import torch, transformers
+else: torch, transformers = openllm.utils.LazyLoader("torch", globals(), "torch"), openllm.utils.LazyLoader("transformers", globals(), "transformers")
+logger = logging.getLogger(__name__)
+class GPTNeoX(openllm.LLM["transformers.GPTNeoXForCausalLM", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        temperature: float | None = None,
-        top_k: int | None = None,
-        top_p: float | None = None,
-        repetition_penalty: float | None = None,
-        use_default_prompt_template: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def sanitize_parameters(self, prompt: str, temperature: float | None = None, max_new_tokens: int | None = None, use_default_prompt_template: bool = True, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        generation_config = {
-            "max_new_tokens": max_new_tokens,
-            "temperature": temperature,
-            "top_k": top_k,
-            "top_p": top_p,
-            "repetition_penalty": repetition_penalty,
-        }
-        return prompt_text, generation_config, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
-        return generation_result[0]
-
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature}, {}
+    @property
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {"device_map": "auto" if torch.cuda.device_count() > 1 else None}, {}
+    def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str: return generation_result[0]
+    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.GPTNeoXForCausalLM:
+        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs)
+        if self.config.use_half_precision: model.half()
+        return model
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        with torch.inference_mode():
-            input_ids = self.tokenizer(prompt, return_tensors="pt").input_ids.to(self.device)
-            result_tensor = self.model.generate(
-                input_ids,
-                do_sample=True,
-                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-            )
-            return self.tokenizer.batch_decode(result_tensor, skip_special_tokens=True)
+        with torch.inference_mode(): return self.tokenizer.batch_decode(self.model.generate(self.tokenizer(prompt, return_tensors="pt").to(self.device).input_ids, do_sample=True, generation_config=self.config.model_construct_env(**attrs).to_generation_config(), pad_token_id=self.tokenizer.eos_token_id, stopping_criteria=transformers.StoppingCriteriaList([openllm.StopOnTokens()])))
```

### Comparing `openllm-0.2.7/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.2.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,68 +22,22 @@
 
 if t.TYPE_CHECKING:
     import transformers  # noqa: F401
 
 
 class FlaxFlanT5(openllm.LLM["transformers.FlaxT5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
     __openllm_internal__ = True
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        temperature: float | None = None,
-        top_k: int | None = None,
-        top_p: float | None = None,
-        repetition_penalty: float | None = None,
-        decoder_start_token_id: int | None = None,
-        use_default_prompt_template: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, temperature: float | None = None, top_k: int | None = None, top_p: float | None = None, repetition_penalty: float | None = None, decoder_start_token_id: int | None = None, use_default_prompt_template: bool = True, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        if decoder_start_token_id is None:
-            decoder_start_token_id = 0
-
-        generation_config = {
-            "max_new_tokens": max_new_tokens,
-            "temperature": temperature,
-            "top_k": top_k,
-            "top_p": top_p,
-            "repetition_penalty": repetition_penalty,
-            "decoder_start_token_id": decoder_start_token_id,
-        }
-        return prompt_text, generation_config, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
-        return generation_result[0]
-
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        if decoder_start_token_id is None: decoder_start_token_id = 0
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_k": top_k, "top_p": top_p, "repetition_penalty": repetition_penalty, "decoder_start_token_id": decoder_start_token_id}, {}
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        # XXX: decoder_start_token_id is extracted from https://huggingface.co/google/flan-t5-small/tree/main
-        # as it is required for encoder-decoder generation.
+        # NOTE: decoder_start_token_id is extracted from https://huggingface.co/google/flan-t5-small/tree/main as it is required for encoder-decoder generation.
         decoder_start_token_id = attrs.pop("decoder_start_token_id", 0)
-        input_ids = self.tokenizer(prompt, return_tensors="np")["input_ids"]
-        result_tensor = self.model.generate(
-            input_ids,
-            do_sample=True,
-            generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-            decoder_start_token_id=decoder_start_token_id,
-        )
-        return self.tokenizer.batch_decode(
-            result_tensor.sequences, skip_special_tokens=True, clean_up_tokenization_spaces=True
-        )
+        return self.tokenizer.batch_decode(self.model.generate(self.tokenizer(prompt, return_tensors="np")["input_ids"], do_sample=True, generation_config=self.config.model_construct_env(**attrs).to_generation_config(), decoder_start_token_id=decoder_start_token_id).sequences, skip_special_tokens=True, clean_up_tokenization_spaces=True)
```

### Comparing `openllm-0.2.7/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.2.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,70 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 import typing as t
-
 import openllm
-
 from .configuration_flan_t5 import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
-
-
-if t.TYPE_CHECKING:
-    import transformers  # noqa: F401
-
-
+if t.TYPE_CHECKING: import transformers  # noqa: F401
 class TFFlanT5(openllm.LLM["transformers.TFT5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
     __openllm_internal__ = True
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        temperature: float | None = None,
-        top_k: int | None = None,
-        top_p: float | None = None,
-        repetition_penalty: float | None = None,
-        use_default_prompt_template: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, temperature: float | None = None, top_k: int | None = None, top_p: float | None = None, repetition_penalty: float | None = None, use_default_prompt_template: bool = True, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        generation_config = {
-            "max_new_tokens": max_new_tokens,
-            "temperature": temperature,
-            "top_k": top_k,
-            "top_p": top_p,
-            "repetition_penalty": repetition_penalty,
-        }
-        return prompt_text, generation_config, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
-        return generation_result[0]
-
-    def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        input_ids = self.tokenizer(prompt, return_tensors="tf").input_ids
-        outputs = self.model.generate(
-            input_ids,
-            do_sample=True,
-            generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-        )
-        return self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_k": top_k, "top_p": top_p, "repetition_penalty": repetition_penalty}, {}
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str: return generation_result[0]
+    def generate(self, prompt: str, **attrs: t.Any) -> list[str]: return self.tokenizer.batch_decode(self.model.generate(self.tokenizer(prompt, return_tensors="tf").input_ids, do_sample=True, generation_config=self.config.model_construct_env(**attrs).to_generation_config()), skip_special_tokens=True)
```

### Comparing `openllm-0.2.7/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.2.8/src/openllm/models/gpt_neox/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,44 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_gpt_neox": ["GPTNeoXConfig", "START_GPT_NEOX_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_gpt_neox": ["GPTNeoXConfig", "START_GPT_NEOX_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_gpt_neox"] = ["GPTNeoX"]
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_gpt_neox"] = ["GPTNeoX"]
 if t.TYPE_CHECKING:
     from .configuration_gpt_neox import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_gpt_neox import START_GPT_NEOX_COMMAND_DOCSTRING as START_GPT_NEOX_COMMAND_DOCSTRING
     from .configuration_gpt_neox import GPTNeoXConfig as GPTNeoXConfig
-
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_gpt_neox import GPTNeoX as GPTNeoX
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_gpt_neox import GPTNeoX as GPTNeoX
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/gpt_neox/configuration_gpt_neox.py` & `openllm-0.2.8/src/openllm/models/gpt_neox/configuration_gpt_neox.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
-
 import openllm
-
-
 class GPTNeoXConfig(openllm.LLMConfig):
     """GPTNeoX is an autoregressive language model trained on the Pile, whose weights will be made freely and openly available to the public through a permissive license.
 
     It is, to the best of our knowledge, the largest dense autoregressive model
     that has publicly available weights at the time of submission. The training and evaluation code, as well as the model weights,
     can be found at https://github.com/EleutherAI/gpt-neox.
 
@@ -28,32 +24,27 @@
 
     Note that OpenLLM provides first-class support for all of the aforementioned model. Users can
     also use `openllm start gpt-neox` to run all of the GPTNeoX variant's model
 
     Refer to [GPTNeoX's model card](https://huggingface.co/docs/transformers/model_doc/gpt_neox)
     for more information.
     """
-
     __config__ = {
         "model_name": "gpt_neox",
         "start_name": "gpt-neox",
         "requires_gpu": True,
         "architecture": "GPTNeoXForCausalLM",
         "url": "https://github.com/EleutherAI/gpt-neox",
         "default_id": "eleutherai/gpt-neox-20b",
         "model_ids": ["eleutherai/gpt-neox-20b"],
     }
-
     use_half_precision: bool = openllm.LLMConfig.Field(True, description="Whether to use half precision for model.")
-
     class GenerationConfig:
         temperature: float = 0.9
         max_new_tokens: int = 100
-
-
 START_GPT_NEOX_COMMAND_DOCSTRING = """\
 Run a LLMServer for GPTNeoX model.
 
 \b
 > See more information about GPTNeoX at [HuggingFace's model card](https://huggingface.co/docs/transformers/model_doc/gpt_neox)
 
 \b
@@ -65,10 +56,8 @@
 GPTNeoX Runner will use EleutherAI/gpt-neox-20b as the default model. To change to any other GPTNeoX
 saved pretrained, or a fine-tune GPTNeoX, provide ``OPENLLM_GPT_NEOX_MODEL_ID='stabilityai/stablelm-tuned-alpha-3b'``
 or provide `--model-id` flag when running ``openllm start gpt-neox``:
 
 \b
 $ openllm start gpt-neox --model-id 'stabilityai/stablelm-tuned-alpha-3b'
 """
-
-
 DEFAULT_PROMPT_TEMPLATE = """{instruction}"""
```

### Comparing `openllm-0.2.7/src/openllm/models/gpt_neox/modeling_gpt_neox.py` & `openllm-0.2.8/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,92 +7,40 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 import logging
 import typing as t
-
+import bentoml
 import openllm
-
-from .configuration_gpt_neox import DEFAULT_PROMPT_TEMPLATE
+from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
-
-
-if t.TYPE_CHECKING:
-    import torch
-
-    import transformers
-else:
-    transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-
-
+from ...utils import generate_labels
+if t.TYPE_CHECKING: import transformers
+else: transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 logger = logging.getLogger(__name__)
-
-
-class GPTNeoX(openllm.LLM["transformers.GPTNeoXForCausalLM", "transformers.GPTNeoXTokenizerFast"]):
+class TFOPT(openllm.LLM["transformers.TFOPTForCausalLM", "transformers.GPT2Tokenizer"]):
     __openllm_internal__ = True
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        temperature: float | None = None,
-        max_new_tokens: int | None = None,
-        use_default_prompt_template: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    @property
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {}, {"padding_side": "left", "truncation_side": "left"}
+    def import_model(self, *args: t.Any, trust_remote_code: bool = False, **attrs: t.Any) -> bentoml.Model:
+        config, tokenizer = transformers.AutoConfig.from_pretrained(self.model_id), transformers.AutoTokenizer.from_pretrained(self.model_id, **self.llm_parameters[-1])
+        tokenizer.pad_token_id = config.pad_token_id
+        return bentoml.transformers.save_model(self.tag, transformers.TFOPTForCausalLM.from_pretrained(self.model_id, trust_remote_code=trust_remote_code, **attrs), custom_objects={"tokenizer": tokenizer}, labels=generate_labels(self))
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, temperature: float | None = None, top_k: int | None = None, num_return_sequences: int | None = None, use_default_prompt_template: bool = False, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        generation_config = {"max_new_tokens": max_new_tokens, "temperature": temperature}
-
-        return prompt_text, generation_config, {}
-
-    @property
-    def import_kwargs(self):
-        model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
-        tokenizer_kwds: dict[str, t.Any] = {}
-        return model_kwds, tokenizer_kwds
-
-    def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str:
-        return generation_result[0]
-
-    def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.GPTNeoXForCausalLM:
-        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs)
-        if self.config.use_half_precision:
-            model.half()
-        return model
-
-    def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        from ..._generation import StopOnTokens
-
-        generation_kwargs = {
-            "do_sample": True,
-            "generation_config": self.config.model_construct_env(**attrs).to_generation_config(),
-            "pad_token_id": self.tokenizer.eos_token_id,
-            "stopping_criteria": transformers.StoppingCriteriaList([StopOnTokens()]),
-        }
-
-        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        with torch.inference_mode():
-            gen_tokens = self.model.generate(inputs.input_ids, **generation_kwargs)
-            return self.tokenizer.batch_decode(gen_tokens)
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_k": top_k, "num_return_sequences": num_return_sequences}, {}
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **attrs: t.Any) -> str:
+        if len(generation_result) == 1: return generation_result[0]
+        if self.config.format_outputs: return "Generated result:\n" + "\n -".join(generation_result)
+        else: return "\n".join(generation_result)
+    def generate(self, prompt: str, **attrs: t.Any) -> list[str]: return self.tokenizer.batch_decode(self.model.generate(**self.tokenizer(prompt, return_tensors="tf"), do_sample=True, generation_config=self.config.model_construct_env(**attrs).to_generation_config()), skip_special_tokens=True)
```

### Comparing `openllm-0.2.7/src/openllm/models/llama/__init__.py` & `openllm-0.2.8/src/openllm/models/llama/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,68 +7,37 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
 from ...utils import is_vllm_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_llama": [
-        "LlaMAConfig",
-        "START_LLAMA_COMMAND_DOCSTRING",
-        "DEFAULT_PROMPT_TEMPLATE",
-        "PROMPT_MAPPING",
-    ],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_llama": ["LlaMAConfig", "START_LLAMA_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE", "PROMPT_MAPPING"]}
 try:
-    if not is_vllm_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_vllm_llama"] = ["VLLMLlaMA"]
-
+    if not is_vllm_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_vllm_llama"] = ["VLLMLlaMA"]
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_llama"] = ["LlaMA"]
-
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_llama"] = ["LlaMA"]
 if t.TYPE_CHECKING:
     from .configuration_llama import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_llama import PROMPT_MAPPING as PROMPT_MAPPING
     from .configuration_llama import START_LLAMA_COMMAND_DOCSTRING as START_LLAMA_COMMAND_DOCSTRING
     from .configuration_llama import LlaMAConfig as LlaMAConfig
-
     try:
-        if not is_vllm_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_vllm_llama import VLLMLlaMA as VLLMLlaMA
-
+        if not is_vllm_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_vllm_llama import VLLMLlaMA as VLLMLlaMA
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_llama import LlaMA as LlaMA
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_llama import LlaMA as LlaMA
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/llama/configuration_llama.py` & `openllm-0.2.8/src/openllm/models/llama/configuration_llama.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,44 +7,36 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 import typing as t
-
 import openllm
-
-
 class LlaMAConfig(openllm.LLMConfig):
     """LLaMA model was proposed in [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) by Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurelien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample.
 
     It is a collection of foundation language models ranging from 7B to 65B parameters.
 
     LlaMA also include support for the recent propsed [LlaMA-2](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)
 
     Note that all variants of LlaMA including fine-tuning, quantisation format are all supported with ``openllm.LlaMA``.
 
     Refer to [LlaMA's model card](https://huggingface.co/docs/transformers/main/model_doc/llama)
     for more information.
     """
-
-    use_llama2_prompt: bool = openllm.LLMConfig.Field(
-        True, description="Whether to use the prompt format for LlaMA 2. Disable this when working with LlaMA 1."
-    )
-
+    use_llama2_prompt: bool = openllm.LLMConfig.Field(True, description="Whether to use the prompt format for LlaMA 2. Disable this when working with LlaMA 1.")
     __config__ = {
         "model_name": "llama",
         "start_name": "llama",
         "url": "https://github.com/facebookresearch/llama",
         "default_id": "huggyllama/llama-7b",
-        "default_implementation": "pt",  # XXX: needs vLLM implementation
+        "default_implementation": {"cpu": "pt", "nvidia.com/gpu": "pt"},
         "architecture": "LlamaForCausalLM",
         "requirements": ["fairscale", "sentencepiece"],
         "model_ids": [
             "meta-llama/llama-2-70b-chat-hf",
             "meta-llama/llama-2-13b-chat-hf",
             "meta-llama/llama-2-7b-chat-hf",
             "meta-llama/llama-2-70b-hf",
@@ -65,26 +57,22 @@
                 "r": 64,
                 "lora_alpha": 16,
                 "lora_dropout": 0.1,
                 "bias": "none",
             },
         ),
     }
-
     class GenerationConfig:
         max_new_tokens: int = 256
         temperature: float = 0.45
         top_p: float = 0.95
         top_k: int = 12
-
     class SamplingParams:
         best_of: int = 1
         presence_penalty: float = 0.5
-
-
 START_LLAMA_COMMAND_DOCSTRING = """\
 Run a LLMServer for LlaMA model.
 
 \b
 > See more information about LlaMA at [LlaMA's model card](https://huggingface.co/docs/transformers/main/model_doc/llama
 
 \b
@@ -106,43 +94,18 @@
 
 \b
 OpenLLM also supports running LlaMA-2 and its fine-tune and variants. To import the LlaMA weights, one can use the following:
 
 \b
 $ CONVERTER=hf-llama2 openllm import llama /path/to/llama-2
 """
-
 SYSTEM_MESSAGE = """
 You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.
 
 If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, please don't share false information.
 """
-
-SINST_KEY = "[INST]"
-EINST_KEY = "[/INST]"
-SYS_KEY = "<<SYS>>"
-EOS_TOKEN = "</s>"
-BOS_TOKEN = "<s>"
-
-# TODO: support history
-_v2_prompt = """{start_key} {sys_key}\n{system_message}\n{sys_key}\n\n{instruction}\n{end_key} """.format(
-    start_key=SINST_KEY,
-    sys_key=SYS_KEY,
-    system_message=SYSTEM_MESSAGE,
-    instruction="{instruction}",
-    end_key=EINST_KEY,
-)
-
-# XXX: implement me
-_v1_prompt = """{instruction}"""
-
-PROMPT_MAPPING = {
-    "v1": _v1_prompt,
-    "v2": _v2_prompt,
-}
-
-
-def _get_prompt(model_type: t.Literal["v1", "v2"]) -> str:
-    return PROMPT_MAPPING[model_type]
-
-
+SINST_KEY, EINST_KEY, SYS_KEY, EOS_TOKEN, BOS_TOKEN = "[INST]", "[/INST]", "<<SYS>>", "</s>", "<s>"
+# TODO: support history and v1 prompt implementation
+_v1_prompt, _v2_prompt = """{instruction}""", """{start_key} {sys_key}\n{system_message}\n{sys_key}\n\n{instruction}\n{end_key} """.format(start_key=SINST_KEY, sys_key=SYS_KEY, system_message=SYSTEM_MESSAGE, instruction="{instruction}", end_key=EINST_KEY)
+PROMPT_MAPPING = {"v1": _v1_prompt, "v2": _v2_prompt}
+def _get_prompt(model_type: t.Literal["v1", "v2"]) -> str: return PROMPT_MAPPING[model_type]
 DEFAULT_PROMPT_TEMPLATE = _get_prompt
```

### Comparing `openllm-0.2.7/src/openllm/models/llama/modeling_llama.py` & `openllm-0.2.8/src/openllm/models/llama/modeling_llama.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,114 +7,43 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 import logging
 import typing as t
-
 import openllm
-
 from .configuration_llama import DEFAULT_PROMPT_TEMPLATE
 from ..._llm import LLMEmbeddings
 from ..._prompt import default_formatter
-
-
-if t.TYPE_CHECKING:
-    import torch
-    import torch.nn.functional as F
-
-    import transformers
-else:
-    transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    F = openllm.utils.LazyLoader("F", globals(), "torch.nn.functional")
-
-
+if t.TYPE_CHECKING: import torch, transformers, torch.nn.functional as F
+else: torch, transformers, F = openllm.utils.LazyLoader("torch", globals(), "torch"), openllm.utils.LazyLoader("transformers", globals(), "transformers"), openllm.utils.LazyLoader("F", globals(), "torch.nn.functional")
 logger = logging.getLogger(__name__)
-
-
 class LlaMA(openllm.LLM["transformers.LlamaForCausalLM", "transformers.LlamaTokenizerFast"]):
     __openllm_internal__ = True
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        top_k: int | None = None,
-        top_p: float | None = None,
-        temperature: float | None = None,
-        max_new_tokens: int | None = None,
-        use_default_prompt_template: bool = True,
-        use_llama2_prompt: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def sanitize_parameters(self, prompt: str, top_k: int | None = None, top_p: float | None = None, temperature: float | None = None, max_new_tokens: int | None = None, use_default_prompt_template: bool = True, use_llama2_prompt: bool = True, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             _PROMPT = DEFAULT_PROMPT_TEMPLATE("v2" if use_llama2_prompt else "v1")
             template_variables = default_formatter.extract_template_variables(_PROMPT)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = _PROMPT.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        generation_config = {
-            "max_new_tokens": max_new_tokens,
-            "temperature": temperature,
-            "top_p": top_p,
-            "top_k": top_k,
-        }
-
-        return prompt_text, generation_config, {}
-
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = _PROMPT.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_p": top_p, "top_k": top_k}, {}
     @property
-    def import_kwargs(self):
-        model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
-        tokenizer_kwds: dict[str, t.Any] = {}
-        return model_kwds, tokenizer_kwds
-
-    def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str:
-        return generation_result[0]
-
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {"device_map": "auto" if torch.cuda.device_count() > 1 else None}, {}
+    def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        from ..._generation import StopOnTokens
-
-        generation_kwargs = {
-            "generation_config": self.config.model_construct_env(**attrs).to_generation_config(),
-            "stopping_criteria": transformers.StoppingCriteriaList([StopOnTokens()]),
-        }
-
-        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        with torch.inference_mode():
-            gen_tokens = self.model.generate(**inputs, **generation_kwargs)
-            return self.tokenizer.batch_decode(gen_tokens, skip_special_tokens=True, clean_up_tokenization_spaces=True)
-
+        with torch.inference_mode(): return self.tokenizer.batch_decode(self.model.generate(**self.tokenizer(prompt, return_tensors="pt").to(self.device), generation_config=self.config.model_construct_env(**attrs).to_generation_config(), stopping_criteria=transformers.StoppingCriteriaList([openllm.StopOnTokens()])), skip_special_tokens=True, clean_up_tokenization_spaces=True)
     def embeddings(self, prompts: list[str]) -> LLMEmbeddings:
         encoding = self.tokenizer(prompts, padding=True, return_tensors="pt").to(self.device)
-        input_ids = encoding["input_ids"]
-        attention_mask = encoding["attention_mask"]
+        input_ids, attention_mask = encoding["input_ids"], encoding["attention_mask"]
         with torch.inference_mode():
-            model_outputs = self.model(input_ids=input_ids, attention_mask=attention_mask, output_hidden_states=True)
-            data = model_outputs.hidden_states[-1]
+            data = self.model(input_ids=input_ids, attention_mask=attention_mask, output_hidden_states=True).hidden_states[-1]
             mask = attention_mask.unsqueeze(-1).expand(data.size()).float()
             masked_embeddings = data * mask
-            sum_embeddings = torch.sum(masked_embeddings, dim=1)
-            seq_length = torch.sum(mask, dim=1)
-            embedding = sum_embeddings / seq_length
-            normalized_embeddings = F.normalize(embedding, p=2, dim=1)
-        return {
-            "embeddings": normalized_embeddings,
-            "num_tokens": torch.sum(attention_mask).item(),
-        }
+            sum_embeddings, seq_length = torch.sum(masked_embeddings, dim=1), torch.sum(mask, dim=1)
+        return LLMEmbeddings(embeddings=F.normalize(sum_embeddings / seq_length, p=2, dim=1), num_tokens=torch.sum(attention_mask).item())
```

### Comparing `openllm-0.2.7/src/openllm/models/llama/modeling_vllm_llama.py` & `openllm-0.2.8/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,94 +7,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
-import logging
 import typing as t
-
 import openllm
-
-from .configuration_llama import DEFAULT_PROMPT_TEMPLATE
+from .configuration_flan_t5 import DEFAULT_PROMPT_TEMPLATE
 from ..._prompt import default_formatter
-
-
 if t.TYPE_CHECKING:
     import torch
-    import vllm
-
-    import transformers
+    import transformers  # noqa: F401
 else:
-    transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    vllm = openllm.utils.LazyLoader("vllm", globals(), "vllm")
-
-
-logger = logging.getLogger(__name__)
-
-
-class VLLMLlaMA(openllm.LLM["vllm.LLM", "transformers.LlamaTokenizerFast"]):
+class FlanT5(openllm.LLM["transformers.T5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
     __openllm_internal__ = True
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        temperature: float | None = None,
-        max_new_tokens: int | None = None,
-        use_default_prompt_template: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def sanitize_parameters(self, prompt: str, max_new_tokens: int | None = None, temperature: float | None = None, top_k: int | None = None, top_p: float | None = None, repetition_penalty: float | None = None, use_default_prompt_template: bool = True, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             template_variables = default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        generation_config = {"max_new_tokens": max_new_tokens, "temperature": temperature}
-
-        return prompt_text, generation_config, {}
-
-    @property
-    def import_kwargs(self):
-        model_kwds = {"device_map": "auto" if torch.cuda.device_count() > 1 else None}
-        tokenizer_kwds: dict[str, t.Any] = {}
-        return model_kwds, tokenizer_kwds
-
-    def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str:
-        return generation_result[0]
-
-    def load_model(self, *args: t.Any, **attrs: t.Any) -> t.Any:
-        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, *args, **attrs)
-        if self.config.use_half_precision:
-            model.half()
-        return model
-
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_k": top_k, "top_p": top_p, "repetition_penalty": repetition_penalty}, {}
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        from ..._generation import StopOnTokens
-
-        generation_kwargs = {
-            "do_sample": True,
-            "generation_config": self.config.model_construct_env(**attrs).to_generation_config(),
-            "pad_token_id": self.tokenizer.eos_token_id,
-            "stopping_criteria": transformers.StoppingCriteriaList([StopOnTokens()]),
-        }
-
-        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        with torch.inference_mode():
-            gen_tokens = self.model.generate(inputs.input_ids, **generation_kwargs)
-            return self.tokenizer.batch_decode(gen_tokens)
+        with torch.inference_mode(): return self.tokenizer.batch_decode(self.model.generate(**self.tokenizer(prompt, return_tensors="pt").to(self.device), do_sample=True, generation_config=self.config.model_construct_env(**attrs).to_generation_config()), skip_special_tokens=True)
```

### Comparing `openllm-0.2.7/src/openllm/models/mpt/__init__.py` & `openllm-0.2.8/src/openllm/models/stablelm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,46 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_mpt": ["MPTConfig", "START_MPT_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE", "PROMPT_MAPPING"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_stablelm": ["StableLMConfig", "START_STABLELM_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_mpt"] = ["MPT"]
-
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_stablelm"] = ["StableLM"]
 if t.TYPE_CHECKING:
-    from .configuration_mpt import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
-    from .configuration_mpt import PROMPT_MAPPING as PROMPT_MAPPING
-    from .configuration_mpt import START_MPT_COMMAND_DOCSTRING as START_MPT_COMMAND_DOCSTRING
-    from .configuration_mpt import MPTConfig as MPTConfig
-
+    from .configuration_stablelm import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
+    from .configuration_stablelm import START_STABLELM_COMMAND_DOCSTRING as START_STABLELM_COMMAND_DOCSTRING
+    from .configuration_stablelm import StableLMConfig as StableLMConfig
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_mpt import MPT as MPT
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_stablelm import StableLM as StableLM
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/mpt/configuration_mpt.py` & `openllm-0.2.8/src/openllm/models/mpt/configuration_mpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,38 +7,28 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 import typing as t
-
 import openllm
-
-
-if t.TYPE_CHECKING:
-    MPTPromptType = t.Literal["default", "instruct", "chat", "storywriter"]
-else:
-    # TODO: Support Literal string for LLMConfig
-    MPTPromptType = str
-
-
+if t.TYPE_CHECKING: MPTPromptType = t.Literal["default", "instruct", "chat", "storywriter"]
+else: MPTPromptType = str
 class MPTConfig(openllm.LLMConfig):
     """MPT is a decoder-style transformer pretrained from scratch on English text and code.
 
     This model was trained by [MosaicML](https://www.mosaicml.com/).
 
     ``openllm.MPT`` encapsulate a family of MPT variants that is publicly available
     on HuggingFace. Refers [HuggingFace's MosaicML page](https://huggingface.co/mosaicml)
     for more details on specific models.
     """
-
     __config__ = {
         "name_type": "lowercase",
         "trust_remote_code": True,
         "url": "https://huggingface.co/mosaicml",
         "default_id": "mosaicml/mpt-7b-instruct",
         "timeout": int(36e6),
         "requirements": ["triton", "einops"],
@@ -49,35 +39,20 @@
             "mosaicml/mpt-7b-chat",
             "mosaicml/mpt-7b-storywriter",
             "mosaicml/mpt-30b",
             "mosaicml/mpt-30b-instruct",
             "mosaicml/mpt-30b-chat",
         ],
     }
-
-    prompt_type: MPTPromptType = openllm.LLMConfig.Field(
-        '"default"',
-        description="""Given prompt type for running MPT. Default will be inferred from model name if pretrained.""",
-    )
-
-    max_sequence_length: int = openllm.LLMConfig.Field(
-        2048,
-        description="""\
-    Max sequence length to run MPT with. Note that MPT is trained ith sequence length
-    of 2048, but with [ALiBi](https://arxiv.org/abs/2108.12409) it can set up to 4096
-    (for 7b models) and 16384 (for 30b models)
-    """,
-    )
-
+    prompt_type: MPTPromptType = openllm.LLMConfig.Field('"default"', description="""Given prompt type for running MPT. Default will be inferred from model name if pretrained.""")
+    max_sequence_length: int = openllm.LLMConfig.Field(2048, description="Max sequence length to run MPT with. Note that MPT is trained ith sequence length of 2048, but with [ALiBi](https://arxiv.org/abs/2108.12409) it can set up to 4096 (for 7b models) and 16384 (for 30b models)")
     class GenerationConfig:
         max_new_tokens: int = 128
         temperature: float = 0
         top_p: float = 0.8
-
-
 START_MPT_COMMAND_DOCSTRING = """\
 Run a LLMServer for MPT model.
 
 \b
 > See more information about MPT at [HuggingFace's MosaicML page](https://huggingface.co/mosaicml)
 
 \b
@@ -96,47 +71,20 @@
 MPT Runner will use mosaicml/mpt-7b-instruct as the default model. To change to any other MPT
 saved pretrained, or a fine-tune MPT, provide ``OPENLLM_MPT_MODEL_ID='mosaicml/mpt-30b'``
 or provide `--model-id` flag when running ``openllm start mpt``:
 
 \b
 $ openllm start mpt --model-id mosaicml/mpt-30b
 """
-
-INSTRUCTION_KEY = "### Instruction:"
-RESPONSE_KEY = "### Response:"
-END_KEY = "### End"
-INTRO_BLURB = (
-    "Below is an instruction that describes a task. Write a response that appropriately completes the request."
-)
-
+INSTRUCTION_KEY, RESPONSE_KEY, END_KEY = "### Instruction:", "### Response:", "### End"
+INTRO_BLURB = "Below is an instruction that describes a task. Write a response that appropriately completes the request."
 # NOTE: This is the prompt that is used for generating responses using an already
 # trained model.  It ends with the response key, where the job of the model is to provide
 # the completion that follows it (i.e. the response itself).
-_instruct_prompt = """{intro}
+_chat_prompt, _default_prompt, _instruct_prompt = """{instruction}""", """{instruction}""", """{intro}
 {instruction_key}
 {instruction}
 {response_key}
-""".format(
-    intro=INTRO_BLURB,
-    instruction_key=INSTRUCTION_KEY,
-    instruction="{instruction}",
-    response_key=RESPONSE_KEY,
-)
-
-_default_prompt = """{instruction}"""
-
-# TODO: XXX implement me
-_chat_prompt = """{instruction}"""
-
-PROMPT_MAPPING = {
-    "default": _default_prompt,
-    "instruct": _instruct_prompt,
-    "storywriter": _default_prompt,
-    "chat": _chat_prompt,
-}
-
-
-def _get_prompt(model_type: str) -> str:
-    return PROMPT_MAPPING[model_type]
-
-
+""".format(intro=INTRO_BLURB, instruction_key=INSTRUCTION_KEY, instruction="{instruction}", response_key=RESPONSE_KEY)
+PROMPT_MAPPING = {"default": _default_prompt, "instruct": _instruct_prompt, "storywriter": _default_prompt, "chat": _chat_prompt}
+def _get_prompt(model_type: str) -> str: return PROMPT_MAPPING[model_type]
 DEFAULT_PROMPT_TEMPLATE = _get_prompt
```

### Comparing `openllm-0.2.7/src/openllm/models/mpt/modeling_mpt.py` & `openllm-0.2.8/src/openllm/models/mpt/modeling_mpt.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,193 +11,74 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 import logging
 import typing as t
-
 import bentoml
 import openllm
-
-from .configuration_mpt import DEFAULT_PROMPT_TEMPLATE
+from .configuration_mpt import DEFAULT_PROMPT_TEMPLATE, MPTPromptType
 from ..._prompt import default_formatter
-from ...utils import generate_labels
-from ...utils import is_triton_available
-
-
-if t.TYPE_CHECKING:
-    import torch
-
-    import transformers
-
-    from .configuration_mpt import MPTPromptType
-else:
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-
+from ...utils import generate_labels, is_triton_available
+if t.TYPE_CHECKING: import transformers, torch
+else: transformers, torch = openllm.utils.LazyLoader("transformers", globals(), "transformers"), openllm.utils.LazyLoader("torch", globals(), "torch")
 logger = logging.getLogger(__name__)
-
-
-def get_mpt_config(
-    model_id_or_path: str,
-    max_sequence_length: int,
-    device: torch.device | str | int | None,
-    device_map: str | None = None,
-    trust_remote_code: bool = True,
-) -> transformers.PretrainedConfig:
+def get_mpt_config(model_id_or_path: str, max_sequence_length: int, device: torch.device | str | int | None, device_map: str | None = None, trust_remote_code: bool = True) -> transformers.PretrainedConfig:
     config = transformers.AutoConfig.from_pretrained(model_id_or_path, trust_remote_code=trust_remote_code)
-    if hasattr(config, "init_device") and device_map is None and isinstance(device, (str, torch.device)):
-        config.init_device = str(device)
-    if hasattr(config, "attn_config") and is_triton_available():
-        config.attn_config["attn_impl"] = "triton"
-    else:
-        logger.debug(
-            "'triton' is not available, Flash Attention will use the default Torch implementation. For faster inference, make sure to install triton with 'pip install \"git+https://github.com/openai/triton.git#egg=triton&subdirectory=python\"'"
-        )
+    if hasattr(config, "init_device") and device_map is None and isinstance(device, (str, torch.device)): config.init_device = str(device)
+    if hasattr(config, "attn_config") and is_triton_available(): config.attn_config["attn_impl"] = "triton"
+    else: logger.debug("'triton' is not available, Flash Attention will use the default Torch implementation. For faster inference, make sure to install triton with 'pip install \"git+https://github.com/openai/triton.git#egg=triton&subdirectory=python\"'")
     # setting max_seq_len
     config.max_seq_len = max_sequence_length
     return config
-
-
 class MPT(openllm.LLM["transformers.PreTrainedModel", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
-
-    def llm_post_init(self):
-        self.dtype = torch.bfloat16 if torch.cuda.is_available() else torch.float32
-
+    def llm_post_init(self): self.dtype = torch.bfloat16 if torch.cuda.is_available() else torch.float32
     @property
-    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]] | None:
-        model_kwds = {"torch_dtype": torch.bfloat16 if torch.cuda.is_available() else torch.float32}
-        tokenizer_kwds = {"padding_side": "left"}
-        return model_kwds, tokenizer_kwds
-
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {"torch_dtype": torch.bfloat16 if torch.cuda.is_available() else torch.float32}, {"padding_side": "left"}
     def import_model(self, *args: t.Any, trust_remote_code: bool = True, **attrs: t.Any) -> bentoml.Model:
         _, tokenizer_attrs = self.llm_parameters
-
         torch_dtype = attrs.pop("torch_dtype", self.dtype)
         device_map = attrs.pop("device_map", None)
         attrs.pop("low_cpu_mem_usage", None)
-
-        config = get_mpt_config(
-            self.model_id,
-            self.config.max_sequence_length,
-            self.device,
-            device_map=device_map,
-            trust_remote_code=trust_remote_code,
-        )
-
+        config = get_mpt_config(self.model_id, self.config.max_sequence_length, self.device, device_map=device_map, trust_remote_code=trust_remote_code)
         tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_id, **tokenizer_attrs)
-        if tokenizer.pad_token_id is None:
-            logger.warning("pad_token_id is not set. Setting it to eos_token")
-            tokenizer.pad_token = tokenizer.eos_token
-
-        model = transformers.AutoModelForCausalLM.from_pretrained(
-            self.model_id,
-            config=config,
-            torch_dtype=torch_dtype,
-            trust_remote_code=trust_remote_code,
-            device_map=device_map,
-            **attrs,
-        )
-        try:
-            return bentoml.transformers.save_model(
-                self.tag,
-                model,
-                custom_objects={"tokenizer": tokenizer},
-                labels=generate_labels(self),
-            )
-        finally:
-            torch.cuda.empty_cache()
-
+        if tokenizer.pad_token_id is None: tokenizer.pad_token = tokenizer.eos_token
+        model = transformers.AutoModelForCausalLM.from_pretrained(self.model_id, config=config, torch_dtype=torch_dtype, trust_remote_code=trust_remote_code, device_map=device_map, **attrs)
+        try: return bentoml.transformers.save_model( self.tag, model, custom_objects={"tokenizer": tokenizer}, labels=generate_labels(self))
+        finally: torch.cuda.empty_cache()
     def load_model(self, *args: t.Any, **attrs: t.Any) -> transformers.PreTrainedModel:
         torch_dtype = attrs.pop("torch_dtype", self.dtype)
         device_map = attrs.pop("device_map", None)
         trust_remote_code = attrs.pop("trust_remote_code", True)
-
-        _ref = bentoml.transformers.get(self.tag)
-        config = get_mpt_config(
-            _ref.path,
-            self.config.max_sequence_length,
-            self.device,
-            device_map=device_map,
-            trust_remote_code=trust_remote_code,
-        )
-        model = transformers.AutoModelForCausalLM.from_pretrained(
-            _ref.path,
-            config=config,
-            trust_remote_code=trust_remote_code,
-            torch_dtype=torch_dtype,
-            device_map=device_map,
-            **attrs,
-        )
+        config = get_mpt_config(self._bentomodel.path, self.config.max_sequence_length, self.device, device_map=device_map, trust_remote_code=trust_remote_code,)
+        model = transformers.AutoModelForCausalLM.from_pretrained(self._bentomodel.path, config=config, trust_remote_code=trust_remote_code, torch_dtype=torch_dtype, device_map=device_map, **attrs)
         model.tie_weights()
         return model
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        max_new_tokens: int | None = None,
-        temperature: float | None = None,
-        top_p: float | None = None,
-        prompt_type: MPTPromptType | None = None,
-        use_default_prompt_template: bool = True,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def sanitize_parameters( self, prompt: str, max_new_tokens: int | None = None, temperature: float | None = None, top_p: float | None = None, prompt_type: MPTPromptType | None = None, use_default_prompt_template: bool = True, **attrs: t.Any,) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if use_default_prompt_template:
             if prompt_type is None:
-                if "instruct" in self.model_id:
-                    prompt_type = "instruct"
-                elif "storywriter" in self.model_id:
-                    prompt_type = "storywriter"
-                elif "chat" in self.model_id:
-                    prompt_type = "chat"
-                else:
-                    prompt_type = "default"
+                if "instruct" in self.model_id: prompt_type = "instruct"
+                elif "storywriter" in self.model_id: prompt_type = "storywriter"
+                elif "chat" in self.model_id: prompt_type = "chat"
+                else: prompt_type = "default"
             _PROMPT = DEFAULT_PROMPT_TEMPLATE(prompt_type)
             template_variables = default_formatter.extract_template_variables(_PROMPT)
             prompt_variables = {k: v for k, v in attrs.items() if k in template_variables}
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
-            try:
-                prompt_text = _PROMPT.format(instruction=prompt, **prompt_variables)
-            except KeyError as e:
-                raise RuntimeError(
-                    f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. "
-                    "Use 'use_default_prompt_template=False' to disable the default prompt template."
-                ) from None
-        else:
-            prompt_text = prompt
-
-        generation_config = {
-            "max_new_tokens": max_new_tokens,
-            "temperature": temperature,
-            "top_p": top_p,
-        }
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
+            try: prompt_text = _PROMPT.format(instruction=prompt, **prompt_variables)
+            except KeyError as e: raise RuntimeError(f"Missing variable '{e.args[0]}' (required: {template_variables}) in the prompt template. Use 'use_default_prompt_template=False' to disable the default prompt template.") from None
+        else: prompt_text = prompt
+        generation_config = {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_p": top_p}
         return prompt_text, generation_config, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **attrs: t.Any) -> str:
-        return generation_result[0]
-
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **attrs: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         llm_config = self.config.model_construct_env(**attrs)
-
         inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-
-        attrs = {
-            "do_sample": False if llm_config["temperature"] == 0 else True,
-            "eos_token_id": self.tokenizer.eos_token_id,
-            "pad_token_id": self.tokenizer.pad_token_id,
-            "generation_config": llm_config.to_generation_config(),
-        }
-
+        attrs = {"do_sample": False if llm_config["temperature"] == 0 else True, "eos_token_id": self.tokenizer.eos_token_id, "pad_token_id": self.tokenizer.pad_token_id, "generation_config": llm_config.to_generation_config()}
         with torch.inference_mode():
             if torch.cuda.is_available():
                 with torch.autocast("cuda", torch.float16):
                     generated_tensors = self.model.generate(**inputs, **attrs)
-            else:
-                generated_tensors = self.model.generate(**inputs, **attrs)
-
+            else: generated_tensors = self.model.generate(**inputs, **attrs)
         return self.tokenizer.batch_decode(generated_tensors, skip_special_tokens=True)
```

### Comparing `openllm-0.2.7/src/openllm/models/opt/__init__.py` & `openllm-0.2.8/src/openllm/models/opt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,79 +7,54 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_flax_available
 from ...utils import is_tf_available
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_opt": ["OPTConfig", "START_OPT_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+from ...utils import is_vllm_available
+_import_structure: dict[str, list[str]] = {"configuration_opt": ["OPTConfig", "START_OPT_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_opt"] = ["OPT"]
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_opt"] = ["OPT"]
 try:
-    if not is_flax_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_flax_opt"] = ["FlaxOPT"]
-
+    if not is_flax_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_flax_opt"] = ["FlaxOPT"]
 try:
-    if not is_tf_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_tf_opt"] = ["TFOPT"]
-
-
+    if not is_vllm_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_vllm_opt"] = ["VLLMOPT"]
+try:
+    if not is_tf_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_tf_opt"] = ["TFOPT"]
 if t.TYPE_CHECKING:
     from .configuration_opt import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_opt import START_OPT_COMMAND_DOCSTRING as START_OPT_COMMAND_DOCSTRING
     from .configuration_opt import OPTConfig as OPTConfig
-
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_opt import OPT as OPT
-
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_opt import OPT as OPT
+    try:
+        if not is_flax_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_flax_opt import FlaxOPT as FlaxOPT
     try:
-        if not is_flax_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_flax_opt import FlaxOPT as FlaxOPT
-
+        if not is_vllm_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_vllm_opt  import VLLMOPT as VLLMOPT
     try:
-        if not is_tf_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_tf_opt import TFOPT as TFOPT
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_tf_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_tf_opt import TFOPT as TFOPT
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/opt/configuration_opt.py` & `openllm-0.2.8/src/openllm/models/opt/configuration_opt.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,32 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
-
 import openllm
-
-
 class OPTConfig(openllm.LLMConfig):
     """OPT was first introduced in [Open Pre-trained Transformer Language Models](https://arxiv.org/abs/2205.01068) and first released in [metaseq's repository](https://github.com/facebookresearch/metaseq) on May 3rd 2022 by Meta AI.
 
     OPT was predominantly pretrained with English text, but a small amount of non-English data is still present
     within the training corpus via CommonCrawl. The model was pretrained using a causal language modeling (CLM)
     objective. OPT belongs to the same family of decoder-only models like GPT-3. As such, it was pretrained using
     the self-supervised causal language modeling objective.
 
     Refer to [OPT's HuggingFace page](https://huggingface.co/docs/transformers/model_doc/opt) for more information.
     """
-
     __config__ = {
         "name_type": "lowercase",
         "trust_remote_code": False,
         "url": "https://huggingface.co/docs/transformers/model_doc/opt",
         "default_id": "facebook/opt-1.3b",
-        "architecture": "MPTForCausalLM",
+        "architecture": "OPTForCausalLM",
         "model_ids": [
             "facebook/opt-125m",
             "facebook/opt-350m",
             "facebook/opt-1.3b",
             "facebook/opt-2.7b",
             "facebook/opt-6.7b",
             "facebook/opt-66b",
@@ -49,28 +44,20 @@
                 "lora_alpha": 32,
                 "target_modules": ["q_proj", "v_proj"],
                 "lora_dropout": 0.05,
                 "bias": "none",
             },
         ),
     }
-
-    format_outputs: bool = openllm.LLMConfig.Field(
-        False,
-        description="""Whether to format the outputs. This
-    can be used when num_return_sequences > 1.""",
-    )
-
+    format_outputs: bool = openllm.LLMConfig.Field(False, description="""Whether to format the outputs. This can be used when num_return_sequences > 1.""")
     class GenerationConfig:
         top_k: int = 15
         temperature: float = 0.75
         max_new_tokens: int = 1024
         num_return_sequences: int = 1
-
-
 START_OPT_COMMAND_DOCSTRING = """\
 Run a LLMServer for OPT model.
 
 \b
 > See more information about falcon at [facebook/opt-66b](https://huggingface.co/facebook/opt-66b)
 
 \b
@@ -88,9 +75,8 @@
 OPT Runner will use facebook/opt-2.7b as the default model. To change to any other OPT
 saved pretrained, or a fine-tune OPT, provide ``OPENLLM_OPT_MODEL_ID='facebook/opt-6.7b'``
 or provide `--model-id` flag when running ``openllm start opt``:
 
 \b
 $ openllm start opt --model-id facebook/opt-6.7b
 """
-
 DEFAULT_PROMPT_TEMPLATE = """{instruction}"""
```

### Comparing `openllm-0.2.7/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.2.8/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,53 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
-
 import openllm
-
-
 class StableLMConfig(openllm.LLMConfig):
     """StableLM-Base-Alpha is a suite of 3B and 7B parameter decoder-only language models.
 
     It is pre-trained on a diverse collection of English datasets with a sequence
     length of 4096 to push beyond the context window limitations of existing open-source language models.
 
     StableLM-Tuned-Alpha is a suite of 3B and 7B parameter decoder-only language models
     built on top of the StableLM-Base-Alpha models and further fine-tuned on various chat and
     instruction-following datasets.
 
     Refer to [StableLM-tuned's model card](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
     and [StableLM-base's model card](https://huggingface.co/stabilityai/stablelm-base-alpha-7b)
     for more information.
     """
-
     __config__ = {
         "name_type": "lowercase",
         "url": "https://github.com/Stability-AI/StableLM",
         "architecture": "GPTNeoXForCausalLM",
         "default_id": "stabilityai/stablelm-tuned-alpha-3b",
         "model_ids": [
             "stabilityai/stablelm-tuned-alpha-3b",
             "stabilityai/stablelm-tuned-alpha-7b",
             "stabilityai/stablelm-base-alpha-3b",
             "stabilityai/stablelm-base-alpha-7b",
         ],
     }
-
     class GenerationConfig:
         temperature: float = 0.9
         max_new_tokens: int = 128
         top_k: int = 0
         top_p: float = 0.9
-
-
 START_STABLELM_COMMAND_DOCSTRING = """\
 Run a LLMServer for StableLM model.
 
 \b
 > See more information about StableLM at [stabilityai/stablelm-base-alpha-3b](https://huggingface.co/stabilityai/stablelm-base-alpha-3b)
 
 \b
@@ -66,16 +59,14 @@
 StableLM Runner will use stabilityai/stablelm-base-alpha-3b as the default model. To change to any other StableLM
 saved pretrained, or a fine-tune StableLM, provide ``OPENLLM_STABLELM_MODEL_ID='stabilityai/stablelm-tuned-alpha-3b'``
 or provide `--model-id` flag when running ``openllm start stablelm``:
 
 \b
 $ openllm start stablelm --model-id 'stabilityai/stablelm-tuned-alpha-3b'
 """
-
 SYSTEM_PROMPT = """<|SYSTEM|># StableLM Tuned (Alpha version)
 - StableLM is a helpful and harmless open-source AI language model developed by StabilityAI.
 - StableLM is excited to be able to help the user, but will refuse to do anything that could be considered harmful to the user.
 - StableLM is more than just an information source, StableLM is also able to write poetry, short stories, and make jokes.
 - StableLM will refuse to participate in anything that could harm a human.
 """
-
 DEFAULT_PROMPT_TEMPLATE = """{system_prompt}<|USER|>{instruction}<|ASSISTANT|>"""
```

### Comparing `openllm-0.2.7/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.2.8/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,95 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 import logging
 import typing as t
-
 import openllm
-
 from .configuration_stablelm import DEFAULT_PROMPT_TEMPLATE
 from .configuration_stablelm import SYSTEM_PROMPT
 from ..._prompt import default_formatter
-
-
-if t.TYPE_CHECKING:
-    import transformers  # noqa
-    import torch
-else:
-    transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-
-
+if t.TYPE_CHECKING: import transformers, torch
+else: transformers, torch = openllm.utils.LazyLoader("transformers", globals(), "transformers"), openllm.utils.LazyLoader("torch", globals(), "torch")
 logger = logging.getLogger(__name__)
-
-
 class StableLM(openllm.LLM["transformers.GPTNeoXForCausalLM", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
-
-    def llm_post_init(self):
-        self.bettertransformer = True if not torch.cuda.is_available() else False
-
+    def llm_post_init(self): self.bettertransformer = True if not torch.cuda.is_available() else False
     @property
-    def import_kwargs(self):
-        model_kwds = {"torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32}
-        tokenizer_kwds: dict[str, t.Any] = {}
-        return model_kwds, tokenizer_kwds
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        temperature: float | None = None,
-        max_new_tokens: int | None = None,
-        top_k: int | None = None,
-        top_p: float | None = None,
-        use_default_prompt_template: bool = False,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {"torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32}, {}
+    def sanitize_parameters(self, prompt: str, temperature: float | None = None, max_new_tokens: int | None = None, top_k: int | None = None, top_p: float | None = None, use_default_prompt_template: bool = False, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
         if "tuned" in self._model_id and use_default_prompt_template:
-            prompt_variables = {
-                k: v
-                for k, v in attrs.items()
-                if k in default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)
-            }
-            if "instruction" in prompt_variables:
-                raise RuntimeError(
-                    "'instruction' should be passed as the first argument "
-                    "instead of kwargs when 'use_default_prompt_template=True'"
-                )
+            prompt_variables = {k: v for k, v in attrs.items() if k in default_formatter.extract_template_variables(DEFAULT_PROMPT_TEMPLATE)}
+            if "instruction" in prompt_variables: raise RuntimeError("'instruction' should be passed as the first argument instead of kwargs when 'use_default_prompt_template=True'")
             system_prompt = prompt_variables.pop("system_prompt", SYSTEM_PROMPT)
             prompt_text = DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt, system_prompt=system_prompt)
-        else:
-            prompt_text = prompt
-
-        generation_config = {
-            "max_new_tokens": max_new_tokens,
-            "temperature": temperature,
-            "top_k": top_k,
-            "top_p": top_p,
-        }
-
-        return prompt_text, generation_config, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str:
-        return generation_result[0]
-
+        else: prompt_text = prompt
+        return prompt_text, {"max_new_tokens": max_new_tokens, "temperature": temperature, "top_k": top_k, "top_p": top_p}, {}
+    def postprocess_generate(self, prompt: str, generation_result: list[str], **_: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        from ..._generation import StopOnTokens
-
-        generation_kwargs = {
-            "do_sample": True,
-            "generation_config": self.config.model_construct_env(**attrs).to_generation_config(),
-            "pad_token_id": self.tokenizer.eos_token_id,
-            "stopping_criteria": transformers.StoppingCriteriaList([StopOnTokens()]),
-        }
-
-        inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-
-        with torch.inference_mode():
-            if torch.cuda.is_available():
-                with torch.autocast("cuda", torch.float16):
-                    tokens = self.model.generate(**inputs, **generation_kwargs)
-            else:
-                tokens = self.model.generate(**inputs, **generation_kwargs)
-        return [self.tokenizer.decode(tokens[0], skip_special_tokens=True)]
+        with torch.inference_mode(): return [self.tokenizer.decode(self.model.generate(**self.tokenizer(prompt, return_tensors="pt").to(self.device), do_sample=True, generation_config=self.config.model_construct_env(**attrs).to_generation_config(), pad_token_id=self.tokenizer.eos_token_id, stopping_criteria=transformers.StoppingCriteriaList([openllm.StopOnTokens()]))[0], skip_special_tokens=True)]
```

### Comparing `openllm-0.2.7/src/openllm/models/starcoder/__init__.py` & `openllm-0.2.8/src/openllm/models/starcoder/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,44 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
+import sys
 import typing as t
-
 from ...exceptions import MissingDependencyError
 from ...utils import LazyModule
 from ...utils import is_torch_available
-
-
-_import_structure: dict[str, list[str]] = {
-    "configuration_starcoder": ["StarCoderConfig", "START_STARCODER_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
-}
-
+_import_structure: dict[str, list[str]] = {"configuration_starcoder": ["StarCoderConfig", "START_STARCODER_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"]}
 try:
-    if not is_torch_available():
-        raise MissingDependencyError
-except MissingDependencyError:
-    pass
-else:
-    _import_structure["modeling_starcoder"] = ["StarCoder"]
-
+    if not is_torch_available(): raise MissingDependencyError
+except MissingDependencyError: pass
+else: _import_structure["modeling_starcoder"] = ["StarCoder"]
 if t.TYPE_CHECKING:
     from .configuration_starcoder import DEFAULT_PROMPT_TEMPLATE as DEFAULT_PROMPT_TEMPLATE
     from .configuration_starcoder import START_STARCODER_COMMAND_DOCSTRING as START_STARCODER_COMMAND_DOCSTRING
     from .configuration_starcoder import StarCoderConfig as StarCoderConfig
-
     try:
-        if not is_torch_available():
-            raise MissingDependencyError
-    except MissingDependencyError:
-        pass
-    else:
-        from .modeling_starcoder import StarCoder as StarCoder
-else:
-    import sys
-
-    sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
+        if not is_torch_available(): raise MissingDependencyError
+    except MissingDependencyError: pass
+    else: from .modeling_starcoder import StarCoder as StarCoder
+else: sys.modules[__name__] = LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `openllm-0.2.7/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.2.8/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,49 +8,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
-
 import openllm
-
-
 class StarCoderConfig(openllm.LLMConfig):
     """The StarCoder models are 15.5B parameter models trained on 80+ programming languages from [The Stack (v1.2)](https://huggingface.co/datasets/bigcode/the-stack), with opt-out requests excluded.
 
     The model uses [Multi Query Attention](https://arxiv.org/abs/1911.02150),
     [a context window of 8192 tokens](https://arxiv.org/abs/2205.14135), and was trained using the
     [Fill-in-the-Middle](https://arxiv.org/abs/2207.14255) objective on 1 trillion tokens.
 
     Refer to [StarCoder's model card](https://huggingface.co/bigcode/starcoder) for more information.
     """
-
     __config__ = {
         "name_type": "lowercase",
         "requires_gpu": True,
         "url": "https://github.com/bigcode-project/starcoder",
         "architecture": "GPTBigCodeForCausalLM",
         "requirements": ["bitsandbytes"],
         "workers_per_resource": 0.5,
         "default_id": "bigcode/starcoder",
         "model_ids": ["bigcode/starcoder", "bigcode/starcoderbase"],
     }
-
     class GenerationConfig:
         temperature: float = 0.2
         max_new_tokens: int = 256
         min_new_tokens: int = 32
         top_k: float = 50
         top_p: float = 0.95
         pad_token_id: int = 49152
         repetition_penalty: float = 1.2
-
-
 START_STARCODER_COMMAND_DOCSTRING = """\
 Run a LLMServer for StarCoder model.
 
 \b
 > See more information about StarCoder at [bigcode/starcoder](https://huggingface.co/bigcode/starcoder)
 
 \b
@@ -62,9 +55,8 @@
 StarCoder Runner will use bigcode/starcoder as the default model. To change to any other StarCoder
 saved pretrained, or a fine-tune StarCoder, provide ``OPENLLM_STARCODER_MODEL_ID='bigcode/starcoder'``
 or provide `--model-id` flag when running ``openllm start starcoder``:
 
 \b
 $ openllm start starcoder --model-id 'bigcode/starcoder'
 """
-
 DEFAULT_PROMPT_TEMPLATE = """{instruction}"""
```

### Comparing `openllm-0.2.7/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.2.8/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,147 +10,56 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 import logging
 import typing as t
-
 import bentoml
 import openllm
-
 from ...utils import generate_labels
-
-
 if t.TYPE_CHECKING:
-    import torch
-
-    import transformers
+    import torch, transformers
 else:
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-
+    torch, transformers = openllm.utils.LazyLoader("torch", globals(), "torch"), openllm.utils.LazyLoader("transformers", globals(), "transformers")
 logger = logging.getLogger(__name__)
-
-FIM_PREFIX = "<fim-prefix>"
-FIM_MIDDLE = "<fim-middle>"
-FIM_SUFFIX = "<fim-suffix>"
-FIM_PAD = "<fim-pad>"
-EOD = "<|endoftext|>"
-FIM_INDICATOR = "<FILL_HERE>"
-
-
+FIM_PREFIX, FIM_MIDDLE, FIM_SUFFIX, FIM_PAD, EOD, FIM_INDICATOR = "<fim-prefix>", "<fim-middle>", "<fim-suffix>", "<fim-pad>", "<|endoftext|>", "<FILL_HERE>"
 class StarCoder(openllm.LLM["transformers.GPTBigCodeForCausalLM", "transformers.GPT2TokenizerFast"]):
     __openllm_internal__ = True
-
     @property
-    def import_kwargs(self):
-        model_kwds = {
-            "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
-            "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32,
-        }
-        tokenizer_kwds = {"padding_side": "left"}
-        return model_kwds, tokenizer_kwds
-
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]]: return {"device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None, "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32}, {"padding_side": "left"}
     def import_model(self, *args: t.Any, trust_remote_code: bool = False, **attrs: t.Any) -> bentoml.Model:
-        _, tokenizer_attrs = self.llm_parameters
-
-        torch_dtype = attrs.pop("torch_dtype", torch.float16)
-        device_map = attrs.pop("device_map", "auto")
-
-        tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_id, **tokenizer_attrs)
-        tokenizer.add_special_tokens(
-            {
-                "additional_special_tokens": [EOD, FIM_PREFIX, FIM_MIDDLE, FIM_SUFFIX, FIM_PAD],
-                "pad_token": EOD,
-            }
-        )
-
-        model = transformers.AutoModelForCausalLM.from_pretrained(
-            self.model_id, torch_dtype=torch_dtype, device_map=device_map, **attrs
-        )
-        try:
-            return bentoml.transformers.save_model(
-                self.tag,
-                model,
-                custom_objects={"tokenizer": tokenizer},
-                labels=generate_labels(self),
-            )
-        finally:
-            # NOTE: We need to free the cache after saving here so that we can load it back later on.
-            torch.cuda.empty_cache()
-
-    def sanitize_parameters(
-        self,
-        prompt: str,
-        temperature: float | None = None,
-        top_p: float | None = None,
-        max_new_tokens: int | None = None,
-        repetition_penalty: float | None = None,
-        **attrs: t.Any,
-    ) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
-        fim_mode = FIM_INDICATOR in prompt
-        prefix, suffix = None, None
+        torch_dtype, device_map = attrs.pop("torch_dtype", torch.float16), attrs.pop("device_map", "auto")
+        tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_id, **self.llm_parameters[-1])
+        tokenizer.add_special_tokens({"additional_special_tokens": [EOD, FIM_PREFIX, FIM_MIDDLE, FIM_SUFFIX, FIM_PAD], "pad_token": EOD})
+        model = transformers.AutoModelForCausalLM.from_pretrained(self.model_id, torch_dtype=torch_dtype, device_map=device_map, **attrs)
+        try: return bentoml.transformers.save_model(self.tag, model, custom_objects={"tokenizer": tokenizer}, labels=generate_labels(self))
+        finally: torch.cuda.empty_cache()
+    def sanitize_parameters(self, prompt: str, temperature: float | None = None, top_p: float | None = None, max_new_tokens: int | None = None, repetition_penalty: float | None = None, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
+        fim_mode, prefix, suffix = FIM_INDICATOR in prompt, None, None
         if fim_mode:
-            try:
-                prefix, suffix = prompt.split(FIM_INDICATOR)
-            except Exception as err:
-                logger.error("Error while processing prompt with FIM mode:\n", exc_info=err)
-                raise ValueError(f"Only one {FIM_INDICATOR} allowed in prompt") from err
+            try: prefix, suffix = prompt.split(FIM_INDICATOR)
+            except Exception as err: raise ValueError(f"Only one {FIM_INDICATOR} allowed in prompt") from err
             prompt_text = f"{FIM_PREFIX}{prefix}{FIM_SUFFIX}{suffix}{FIM_MIDDLE}"
-        else:
-            prompt_text = prompt
-
-        generation_config = {
-            "temperature": temperature,
-            "top_p": top_p,
-            "max_new_tokens": max_new_tokens,
-            "repetition_penalty": repetition_penalty,
-            # XXX: This value is currently a hack, need more investigate why the
-            # default starcoder doesn't include the same value as santacoder EOD
-            "pad_token_id": 49152,
-            **attrs,
-        }
-
-        return prompt_text, generation_config, {}
-
-    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
-        return generation_result[0]
+        else: prompt_text = prompt
+        # XXX: This value for pad_token_id is currently a hack, need more investigate why the
+        # default starcoder doesn't include the same value as santacoder EOD
+        return prompt_text, {"temperature": temperature, "top_p": top_p, "max_new_tokens": max_new_tokens, "repetition_penalty": repetition_penalty, "pad_token_id": 49152, **attrs}, {}
 
+    def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str: return generation_result[0]
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
         with torch.inference_mode():
-            inputs = t.cast("torch.Tensor", self.tokenizer.encode(prompt, return_tensors="pt")).to(self.device)
-            result_tensor = self.model.generate(
-                inputs,
-                do_sample=True,
-                pad_token_id=self.tokenizer.eos_token_id,
-                # eos_token_id=self.tokenizer.convert_tokens_to_ids("<|end|>"), # NOTE: this is for finetuning starcoder
-                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-            )
+            # eos_token_id=self.tokenizer.convert_tokens_to_ids("<|end|>"), # NOTE: this is for finetuning starcoder
+            # NOTE: support fine-tuning starcoder
+            result_tensor = self.model.generate(self.tokenizer.encode(prompt, return_tensors="pt").to(self.device), do_sample=True, pad_token_id=self.tokenizer.eos_token_id, generation_config=self.config.model_construct_env(**attrs).to_generation_config())
             # TODO: We will probably want to return the tokenizer here so that we can manually process this
             # return (skip_special_tokens=False, clean_up_tokenization_spaces=False))
-            return self.tokenizer.batch_decode(
-                result_tensor[0],
-                skip_special_tokens=True,
-                clean_up_tokenization_spaces=True,
-            )
-
-    def generate_one(
-        self, prompt: str, stop: list[str], **preprocess_generate_kwds: t.Any
-    ) -> list[dict[t.Literal["generated_text"], str]]:
-        from ..._generation import StopSequenceCriteria
-
-        max_new_tokens = preprocess_generate_kwds.pop("max_new_tokens", 200)
-        encoded_inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
-        src_len = encoded_inputs["input_ids"].shape[1]
-        stopping_criteria = preprocess_generate_kwds.pop("stopping_criteria", transformers.StoppingCriteriaList([]))
-        stopping_criteria.append(StopSequenceCriteria(stop, self.tokenizer))
-        outputs = self.model.generate(
-            encoded_inputs["input_ids"], max_new_tokens=max_new_tokens, stopping_criteria=stopping_criteria
-        )
-
-        result = self.tokenizer.decode(outputs[0].tolist()[src_len:])
+            return self.tokenizer.batch_decode(result_tensor[0], skip_special_tokens=True, clean_up_tokenization_spaces=True)
+    def generate_one(self, prompt: str, stop: list[str], **preprocess_generate_kwds: t.Any) -> list[dict[t.Literal["generated_text"], str]]:
+        max_new_tokens, encoded_inputs = preprocess_generate_kwds.pop("max_new_tokens", 200), self.tokenizer(prompt, return_tensors="pt").to(self.device)
+        src_len, stopping_criteria = encoded_inputs["input_ids"].shape[1], preprocess_generate_kwds.pop("stopping_criteria", transformers.StoppingCriteriaList([]))
+        stopping_criteria.append(openllm.StopSequenceCriteria(stop, self.tokenizer))
+        result = self.tokenizer.decode(self.model.generate(encoded_inputs["input_ids"], max_new_tokens=max_new_tokens, stopping_criteria=stopping_criteria)[0].tolist()[src_len:])
         # Inference API returns the stop sequence
         for stop_seq in stop:
-            if result.endswith(stop_seq):
-                result = result[: -len(stop_seq)]
+            if result.endswith(stop_seq): result = result[: -len(stop_seq)]
         return [{"generated_text": result}]
```

### Comparing `openllm-0.2.7/src/openllm/playground/__init__.py` & `openllm-0.2.8/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/playground/_meta.yml` & `openllm-0.2.8/src/openllm/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/playground/falcon_tuned.py` & `openllm-0.2.8/src/openllm/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/playground/features.py` & `openllm-0.2.8/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/playground/llama2_qlora.py` & `openllm-0.2.8/src/openllm/playground/llama2_qlora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/playground/opt_tuned.py` & `openllm-0.2.8/src/openllm/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/serialisation/__init__.py` & `openllm-0.2.8/src/openllm/serialisation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
 if t.TYPE_CHECKING:
     import bentoml
     import transformers
 
     from .._llm import M
     from .._llm import T
-    from .._types import ModelProtocol
 else:
     transformers = LazyLoader("transformers", globals(), "transformers")
 
 
 def import_model(
     llm: openllm.LLM[t.Any, t.Any],
     *decls: t.Any,
@@ -88,15 +87,15 @@
         return openllm.transformers.save_pretrained(llm, save_directory, **attrs)
     elif llm.runtime == "ggml":
         return openllm.ggml.save_pretrained(llm, save_directory, **attrs)
     else:
         raise ValueError(f"Unknown runtime: {llm.config['runtime']}")
 
 
-def load_model(llm: openllm.LLM[M, t.Any], *decls: t.Any, **attrs: t.Any) -> ModelProtocol[M]:
+def load_model(llm: openllm.LLM[M, t.Any], *decls: t.Any, **attrs: t.Any) -> M:
     if llm.runtime == "transformers":
         return openllm.transformers.load_model(llm, *decls, **attrs)
     elif llm.runtime == "ggml":
         return openllm.ggml.load_model(llm, *decls, **attrs)
     else:
         raise ValueError(f"Unknown runtime: {llm.config['runtime']}")
```

### Comparing `openllm-0.2.7/src/openllm/serialisation/constants.py` & `openllm-0.2.8/src/openllm/serialisation/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 
 FRAMEWORK_TO_AUTOCLASS_MAPPING = {
     "pt": ("AutoModelForCausalLM", "AutoModelForSeq2SeqLM"),
+    # NOTE: vllm will use PyTorch implementation of transformers for serialisation
+    "vllm": ("AutoModelForCausalLM", "AutoModelForSeq2SeqLM"),
     "tf": ("TFAutoModelForCausalLM", "TFAutoModelForSeq2SeqLM"),
     "flax": ("FlaxAutoModelForCausalLM", "FlaxAutoModelForSeq2SeqLM"),
 }
 
 
 # this logic below is synonymous to handling `from_pretrained` attrs.
 HUB_ATTRS = [
```

### Comparing `openllm-0.2.7/src/openllm/serialisation/transformers.py` & `openllm-0.2.8/src/openllm/serialisation/transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,38 +22,43 @@
 from bentoml._internal.frameworks.transformers import make_default_signatures
 from bentoml._internal.models.model import ModelOptions
 
 from .constants import FRAMEWORK_TO_AUTOCLASS_MAPPING
 from .constants import HUB_ATTRS
 from ..exceptions import OpenLLMException
 from ..utils import LazyLoader
+from ..utils import LazyType
+from ..utils import device_count
 from ..utils import first_not_none
 from ..utils import generate_context
 from ..utils import generate_labels
 from ..utils import is_autogptq_available
 from ..utils import is_torch_available
 from ..utils import normalize_attrs_to_model_tokenizer_pair
 
 
 if t.TYPE_CHECKING:
     import auto_gptq as autogptq
     import torch
+    import vllm
 
     import openllm
     import transformers as _transformers
     from transformers.models.auto.auto_factory import _BaseAutoModelClass
 
     from .._llm import M
     from .._llm import T
     from .._types import DictStrAny
 else:
+    vllm = LazyLoader("vllm", globals(), "vllm")
     autogptq = LazyLoader("autogptq", globals(), "auto_gptq")
     _transformers = LazyLoader("_transformers", globals(), "transformers")
     torch = LazyLoader("torch", globals(), "torch")
 
+_object_setattr = object.__setattr__
 
 def process_transformers_config(
     model_id: str, trust_remote_code: bool, **attrs: t.Any
 ) -> tuple[_transformers.PretrainedConfig, dict[str, t.Any], dict[str, t.Any]]:
     """Process transformers config and return PretrainedConfig with hub_kwargs and the rest of kwargs."""
     config: _transformers.PretrainedConfig | None = attrs.pop("config", None)
 
@@ -144,79 +149,67 @@
     metadata: DictStrAny = {
         "safe_serialisation": safe_serialisation,
         "_quantize": quantize_method if quantize_method is not None else False,
     }
     signatures: DictStrAny = {}
     if quantize_method == "gptq":
         if not is_autogptq_available():
-            raise OpenLLMException(
-                "GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'"
-            )
-        if llm.config["model_type"] != "causal_lm":
-            raise OpenLLMException(f"GPTQ only support Causal LM (got {llm.__class__} of {llm.config['model_type']})")
+            raise OpenLLMException("GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'")
+        if llm.config["model_type"] != "causal_lm": raise OpenLLMException(f"GPTQ only support Causal LM (got {llm.__class__} of {llm.config['model_type']})")
         model = autogptq.AutoGPTQForCausalLM.from_quantized(
             llm.model_id,
             *decls,
             quantize_config=t.cast("autogptq.BaseQuantizeConfig", llm.quantization_config),
             trust_remote_code=trust_remote_code,
             use_safetensors=safe_serialisation,
             **hub_attrs,
             **attrs,
         )
-        metadata["_pretrained_class"] = model.__class__.__name__
-        metadata["_framework"] = model.model.framework
+        metadata.update({"_pretrained_class": model.__class__.__name__, "_framework": model.model.framework})
         signatures["generate"] = {"batchable": False}
     else:
-        if "quantization_config" in attrs and getattr(attrs["quantization_config"], "load_in_4bit", False):
-            # this model might be called with --quantize int4, therefore we need to pop this out
-            # since saving int4 is not yet supported
-            attrs.pop("quantization_config")
-        model = t.cast(
-            "_transformers.PreTrainedModel",
-            infer_autoclass_from_llm_config(llm, config).from_pretrained(
-                llm.model_id,
-                *decls,
-                config=config,
-                trust_remote_code=trust_remote_code,
-                **hub_attrs,
-                **attrs,
-            ),
+        # this model might be called with --quantize int4, therefore we need to pop this out
+        # since saving int4 is not yet supported
+        if "quantization_config" in attrs and getattr(attrs["quantization_config"], "load_in_4bit", False): attrs.pop("quantization_config")
+        model = infer_autoclass_from_llm_config(llm, config).from_pretrained(
+            llm.model_id,
+            *decls,
+            config=config,
+            trust_remote_code=trust_remote_code,
+            **hub_attrs,
+            **attrs,
         )
-        metadata["_pretrained_class"] = model.__class__.__name__
-        metadata["_framework"] = model.framework
+        metadata.update({"_pretrained_class": model.__class__.__name__, "_framework": model.framework})
 
     _tokenizer = infer_tokenizers_class_for_llm(llm).from_pretrained(
         llm.model_id,
         trust_remote_code=trust_remote_code,
         **hub_attrs,
         **tokenizer_attrs,
     )
-    if _tokenizer.pad_token is None:
-        _tokenizer.pad_token = _tokenizer.eos_token
+    if _tokenizer.pad_token is None: _tokenizer.pad_token = _tokenizer.eos_token
+
+    # NOTE: quick hack to set the loaded into llm object to use with save_pretrained
+    # to avoid recursive call when the model is not yet available in local store
+    _object_setattr(llm, "__llm_model__", model)
+    _object_setattr(llm, "__llm_tokenizer__", _tokenizer)
 
     try:
         with bentoml.models.create(
             llm.tag,
             module="openllm.serialisation.transformers",
             api_version="v1",
             context=generate_context(framework_name="openllm"),
             labels=generate_labels(llm),
             signatures=signatures if signatures else make_default_signatures(model),
             options=ModelOptions(),
-            external_modules=[
-                importlib.import_module(model.__module__),
-                importlib.import_module(_tokenizer.__module__),
-            ]
-            if trust_remote_code
-            else None,
+            external_modules=[importlib.import_module(model.__module__), importlib.import_module(_tokenizer.__module__)] if trust_remote_code else None,
             metadata=metadata,
         ) as bentomodel:
-            save_pretrained(
-                llm, bentomodel.path, model=model, tokenizer=_tokenizer, safe_serialization=safe_serialisation
-            )
+            save_pretrained(llm, bentomodel.path, safe_serialization=safe_serialisation)
             return bentomodel
     finally:
         # NOTE: We need to free up the cache after importing the model
         # in the case where users first run openllm start without the model
         # available locally.
         if is_torch_available() and torch.cuda.is_available():
             torch.cuda.empty_cache()
@@ -249,112 +242,86 @@
         return model
     except bentoml.exceptions.NotFound:
         if auto_import:
             return import_model(llm, trust_remote_code=llm.__llm_trust_remote_code__)
         raise
 
 
+
 def load_model(llm: openllm.LLM[M, t.Any], *decls: t.Any, **attrs: t.Any) -> M:
     """Load the model from BentoML store.
 
     By default, it will try to find check the model in the local store.
     If model is not found, it will raises a ``bentoml.exceptions.NotFound``.
     """
     config, hub_attrs, attrs = process_transformers_config(llm.model_id, llm.__llm_trust_remote_code__, **attrs)
-    metadata = llm._bentomodel.info.metadata
-    safe_serialization = first_not_none(
-        t.cast(t.Optional[bool], metadata.get("safe_serialisation", None)),
-        attrs.pop("safe_serialization", None),
-        default=llm._serialisation_format == "safetensors",
-    )
-    if "_quantize" in metadata and metadata["_quantize"] == "gptq":
-        if not is_autogptq_available():
-            raise OpenLLMException(
-                "GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'"
-            )
-        if llm.config["model_type"] != "causal_lm":
-            raise OpenLLMException(f"GPTQ only support Causal LM (got {llm.__class__} of {llm.config['model_type']})")
+    safe_serialization = first_not_none(t.cast(t.Optional[bool], llm._bentomodel.info.metadata.get("safe_serialisation", None)), attrs.pop("safe_serialization", None), default=llm._serialisation_format == "safetensors")
+    if "_quantize" in llm._bentomodel.info.metadata and llm._bentomodel.info.metadata["_quantize"] == "gptq":
+        if not is_autogptq_available(): raise OpenLLMException("GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'")
+        if llm.config["model_type"] != "causal_lm": raise OpenLLMException(f"GPTQ only support Causal LM (got {llm.__class__} of {llm.config['model_type']})")
         return autogptq.AutoGPTQForCausalLM.from_quantized(
             llm._bentomodel.path,
             *decls,
             quantize_config=t.cast("autogptq.BaseQuantizeConfig", llm.quantization_config),
             trust_remote_code=llm.__llm_trust_remote_code__,
             use_safetensors=safe_serialization,
             **hub_attrs,
             **attrs,
         )
+
     model = infer_autoclass_from_llm_config(llm, config).from_pretrained(
         llm._bentomodel.path,
         *decls,
         config=config,
         trust_remote_code=llm.__llm_trust_remote_code__,
         **hub_attrs,
         **attrs,
     )
     # NOTE: we only cast and load the model if it is not already quantized and setup correctly
-    loaded_in_kbit = (
-        getattr(model, "is_loaded_in_8bit", False)
-        or getattr(model, "is_loaded_in_4bit", False)
-        or getattr(model, "is_quantized", False)
-    )
-    if torch.cuda.is_available() and torch.cuda.device_count() == 1 and not loaded_in_kbit:
-        try:
-            model = model.to("cuda")
-        except torch.cuda.OutOfMemoryError as err:
-            raise RuntimeError(
-                f"Failed to fit {llm.config['model_name']} with model_id '{llm.model_id}' to CUDA.\nNote: You can try out '--quantize int8 | int4' for dynamic quantization."
-            ) from err
+    loaded_in_kbit = getattr(model, "is_loaded_in_8bit", False) or getattr(model, "is_loaded_in_4bit", False) or getattr(model, "is_quantized", False)
+    if torch.cuda.is_available() and device_count() == 1 and not loaded_in_kbit:
+        try: model = model.to("cuda")
+        except torch.cuda.OutOfMemoryError as err: raise RuntimeError(f"Failed to convert {llm.config['model_name']} with model_id '{llm.model_id}' to CUDA.\nNote: You can try out '--quantize int8 | int4' for dynamic quantization.") from err
     if llm.bettertransformer and llm.__llm_implementation__ == "pt" and not isinstance(model, _transformers.Pipeline):
         # BetterTransformer is currently only supported on PyTorch.
         from optimum.bettertransformer import BetterTransformer
-
-        model = BetterTransformer.transform(model)  # type: ignore
+        model = BetterTransformer.transform(model)
     return t.cast("M", model)
 
 
 def save_pretrained(
     llm: openllm.LLM[M, T],
     save_directory: str,
-    model: M | None = None,
-    tokenizer: T | None = None,
     is_main_process: bool = True,
     state_dict: DictStrAny | None = None,
     save_function: t.Callable[..., None] | None = None,
     push_to_hub: bool = False,
-    max_shard_size: int | str = "10GB",
+    max_shard_size: int | str = "2GB",
     safe_serialization: bool = False,
     variant: str | None = None,
     **attrs: t.Any,
 ) -> None:
     """Light wrapper around ``transformers.PreTrainedTokenizer.save_pretrained`` and ``transformers.PreTrainedModel.save_pretrained``."""
-    model = first_not_none(model, default=llm.__llm_model__)
-    tokenizer = first_not_none(tokenizer, default=llm.__llm_tokenizer__)
     save_function = first_not_none(save_function, default=torch.save)
     model_save_attrs, tokenizer_save_attrs = normalize_attrs_to_model_tokenizer_pair(**attrs)
     safe_serialization = safe_serialization or llm._serialisation_format == "safetensors"
-
-    if model is None or tokenizer is None:
-        raise RuntimeError("Failed to find loaded model or tokenizer to save to local store.")
-
+    # NOTE: disable safetensors for vllm
+    if llm.__llm_implementation__ == "vllm": safe_serialization = False
     if llm._quantize_method == "gptq":
-        if not is_autogptq_available():
-            raise OpenLLMException(
-                "GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'"
-            )
-        if llm.config["model_type"] != "causal_lm":
-            raise OpenLLMException(f"GPTQ only support Causal LM (got {llm.__class__} of {llm.config['model_type']})")
-        model.save_quantized(save_directory, use_safetensors=safe_serialization)
-    elif isinstance(model, _transformers.Pipeline):
-        model.save_pretrained(save_directory, safe_serialization=safe_serialization)
+        if not is_autogptq_available(): raise OpenLLMException("GPTQ quantisation requires 'auto-gptq' (Not found in local environment). Install it with 'pip install \"openllm[gptq]\"'")
+        if llm.config["model_type"] != "causal_lm": raise OpenLLMException(f"GPTQ only support Causal LM (got {llm.__class__} of {llm.config['model_type']})")
+        llm.model.save_quantized(save_directory, use_safetensors=safe_serialization)
+    elif LazyType["vllm.LLMEngine"]("vllm.LLMEngine").isinstance(llm.model): raise RuntimeError("vllm.LLMEngine cannot be serialisation directly. This happens when 'save_pretrained' is called directly after `openllm.AutoVLLM` is initialized.")
+    elif isinstance(llm.model, _transformers.Pipeline): llm.model.save_pretrained(save_directory, safe_serialization=safe_serialization)
     else:
-        model.save_pretrained(
+        llm.model.save_pretrained(
             save_directory,
             is_main_process=is_main_process,
             state_dict=state_dict,
             save_function=save_function,
             push_to_hub=push_to_hub,
             max_shard_size=max_shard_size,
             safe_serialization=safe_serialization,
             variant=variant,
-            **model_save_attrs,
+            **model_save_attrs
         )
-    tokenizer.save_pretrained(save_directory, push_to_hub=push_to_hub, **tokenizer_save_attrs)
+    llm.tokenizer.save_pretrained(save_directory, push_to_hub=push_to_hub, **tokenizer_save_attrs)
```

### Comparing `openllm-0.2.7/src/openllm/utils/__init__.py` & `openllm-0.2.8/src/openllm/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 import logging.config
 import os
 import sys
 import types
 import typing as t
 from pathlib import Path
 
-from circus.exc import ConflictError
-
 from bentoml._internal.configuration import DEBUG_ENV_VAR as _DEBUG_ENV_VAR
 from bentoml._internal.configuration import GRPC_DEBUG_ENV_VAR as _GRPC_DEBUG_ENV_VAR
 from bentoml._internal.configuration import get_debug_mode
 from bentoml._internal.configuration import get_quiet_mode
 from bentoml._internal.configuration import set_quiet_mode
 from bentoml._internal.log import configure_server_logging
 from bentoml._internal.models.model import ModelContext as _ModelContext
@@ -54,23 +52,18 @@
 
 try:
     from typing import GenericAlias as _TypingGenericAlias  # type: ignore
 except ImportError:
     # python < 3.9 does not have GenericAlias (list[int], tuple[str, ...] and so on)
     _TypingGenericAlias = ()  # type: ignore
 
-if sys.version_info < (3, 10):
-    _WithArgsTypes = (_TypingGenericAlias,)
+if sys.version_info < (3, 10): _WithArgsTypes = (_TypingGenericAlias,)
 else:
-    _WithArgsTypes: t.Any = (
-        #  _GenericAlias is the actual GenericAlias implementation
-        t._GenericAlias,  # type: ignore
-        types.GenericAlias,
-        types.UnionType,
-    )
+    #  _GenericAlias is the actual GenericAlias implementation
+    _WithArgsTypes: t.Any = (t._GenericAlias, types.GenericAlias, types.UnionType)  # type: ignore
 
 # NOTE: We need to do this so that overload can register
 # correct overloads to typing registry
 if sys.version_info[:2] >= (3, 11):
     from typing import overload as _overload
 else:
     from typing_extensions import overload as _overload
@@ -87,82 +80,68 @@
 def set_debug_mode(enabled: bool) -> None:
     # monkeypatch bentoml._internal.configuration.set_debug_mode to remove unused logs
     os.environ[_DEBUG_ENV_VAR] = str(enabled)
     os.environ[_GRPC_DEBUG_ENV_VAR] = "DEBUG" if enabled else "ERROR"
 
 
 def lenient_issubclass(cls: t.Any, class_or_tuple: type[t.Any] | tuple[type[t.Any], ...] | None) -> bool:
-    try:
-        return isinstance(cls, type) and issubclass(cls, class_or_tuple)  # type: ignore[arg-type]
+    try: return isinstance(cls, type) and issubclass(cls, class_or_tuple)  # type: ignore[arg-type]
     except TypeError:
-        if isinstance(cls, _WithArgsTypes):
-            return False
+        if isinstance(cls, _WithArgsTypes): return False
         raise
 
 
 def available_devices() -> tuple[str, ...]:
     """Return available GPU under system. Currently only supports NVIDIA GPUs."""
     from .._strategies import NvidiaGpuResource
-
     return tuple(NvidiaGpuResource.from_system())
 
 
 @functools.lru_cache(maxsize=1)
-def device_count() -> int:
-    return len(available_devices())
-
+def device_count() -> int: return len(available_devices())
 
 # equivocal setattr to save one lookup per assignment
 _object_setattr = object.__setattr__
 
-
 def non_intrusive_setattr(obj: t.Any, name: str, value: t.Any) -> None:
     """This makes sure that we don't overwrite any existing attributes on the object."""
     _setattr = functools.partial(setattr, obj) if isinstance(obj, type) else _object_setattr.__get__(obj)
+    if not hasattr(obj, name): _setattr(name, value)
 
-    if not hasattr(obj, name):
-        _setattr(name, value)
-
-
-def field_env_key(model_name: str, key: str, suffix: str | t.Literal[""] | None = None) -> str:
-    return "_".join(filter(None, map(str.upper, ["OPENLLM", model_name, suffix.strip("_") if suffix else "", key])))
-
+def field_env_key(model_name: str, key: str, suffix: str | t.Literal[""] | None = None) -> str: return "_".join(filter(None, map(str.upper, ["OPENLLM", model_name, suffix.strip("_") if suffix else "", key])))
 
+# Special debug flag controled via OPENLLMDEVDEBUG
 DEBUG = sys.flags.dev_mode or (not sys.flags.ignore_environment and bool(os.environ.get("OPENLLMDEVDEBUG")))
-
 # MYPY is like t.TYPE_CHECKING, but reserved for Mypy plugins
 MYPY = False
-
 SHOW_CODEGEN = DEBUG and int(os.environ.get("OPENLLMDEVDEBUG", str(0))) > 3
 
 
 class _ExceptionFilter(logging.Filter):
     def __init__(self, exclude_exceptions: list[type[Exception]] | None = None, **kwargs: t.Any):
-        if exclude_exceptions is None:
-            exclude_exceptions = [ConflictError]
-        else:
-            exclude_exceptions.append(ConflictError)
-
+        from circus.exc import ConflictError
+        if exclude_exceptions is None: exclude_exceptions = [ConflictError]
+        else: exclude_exceptions.append(ConflictError)
         super(_ExceptionFilter, self).__init__(**kwargs)
         self.EXCLUDE_EXCEPTIONS = exclude_exceptions
-
     def filter(self, record: logging.LogRecord) -> bool:
         if record.exc_info:
             etype, _, _ = record.exc_info
             if etype is not None:
                 for exc in self.EXCLUDE_EXCEPTIONS:
-                    if issubclass(etype, exc):
-                        return False
+                    if issubclass(etype, exc): return False
         return True
 
+class InfoFilter(logging.Filter):
+    def filter(self, record: logging.LogRecord) -> bool: return logging.INFO <= record.levelno < logging.WARNING
 
 _LOGGING_CONFIG: DictStrAny = {
     "version": 1,
     "disable_existing_loggers": True,
-    "filters": {"excfilter": {"()": _ExceptionFilter}},
+    "filters": {"excfilter": {"()": _ExceptionFilter}, "infofilter": {"()": InfoFilter}},
     "handlers": {
         "bentomlhandler": {
             "class": "logging.StreamHandler",
             "filters": ["excfilter"],
             "stream": "ext://sys.stdout",
         },
         "defaulthandler": {
@@ -207,26 +186,21 @@
     logging.config.dictConfig(_LOGGING_CONFIG)
 
 
 @functools.lru_cache(maxsize=1)
 def in_notebook() -> bool:
     try:
         from IPython.core.getipython import get_ipython
-
-        if "IPKernelApp" not in get_ipython().config:  # type: ignore
-            return False
-    except ImportError:
-        return False
-    except AttributeError:
-        return False
+        if "IPKernelApp" not in get_ipython().config: return False
+    except ImportError: return False
+    except AttributeError: return False
     return True
 
 
-_dockerenv = Path("/.dockerenv")
-_cgroup = Path("/proc/self/cgroup")
+_dockerenv, _cgroup = Path("/.dockerenv"), Path("/proc/self/cgroup")
 
 
 class suppress(contextlib.suppress, contextlib.ContextDecorator):
     """A version of contextlib.suppress with decorator support.
 
     >>> @suppress(KeyError)
     ... def key_error():
@@ -249,17 +223,15 @@
     >>> round_three = lambda x: round(x, ndigits=3)
     >>> f = compose(round_three, int.__truediv__)
     >>> [f(3*x, x+1) for x in range(1,10)]
     [1.5, 2.0, 2.25, 2.4, 2.5, 2.571, 2.625, 2.667, 2.7]
     """
 
     def compose_two(f1: AnyCallable, f2: t.Callable[P, t.Any]) -> t.Any:
-        def _(*args: P.args, **kwargs: P.kwargs) -> t.Any:
-            return f1(f2(*args, **kwargs))
-
+        def _(*args: P.args, **kwargs: P.kwargs) -> t.Any: return f1(f2(*args, **kwargs))
         return _
 
     return functools.reduce(compose_two, funcs)
 
 
 def apply(transform: AnyCallable) -> t.Callable[[AnyCallable], AnyCallable]:
     """Decorate a function with a transform function that is invoked on results returned from the decorated function.
@@ -273,25 +245,21 @@
     # [6, 5, 4]
     ```
     ```python
     get_numbers.__doc__
     # 'doc for get_numbers'
     ```
     """
-
-    def wrap(func: t.Callable[P, t.Any]) -> t.Any:
-        return functools.wraps(func)(compose(transform, func))
-
+    def wrap(func: t.Callable[P, t.Any]) -> t.Any: return functools.wraps(func)(compose(transform, func))
     return wrap
 
 
 @apply(bool)
 @suppress(FileNotFoundError)
-def _text_in_file(text: str, filename: Path) -> bool:
-    return any(text in line for line in filename.open())
+def _text_in_file(text: str, filename: Path) -> bool: return any(text in line for line in filename.open())
 
 
 def in_docker() -> bool:
     """Is this current environment running in docker?
 
     ```python
     type(in_docker())
@@ -302,110 +270,71 @@
 
 T = t.TypeVar("T")
 K = t.TypeVar("K")
 
 
 def resolve_filepath(path: str) -> str:
     """Resolve a file path to an absolute path, expand user and environment variables."""
-    try:
-        return resolve_user_filepath(path, None)
-    except FileNotFoundError:
-        return path
-
-
-def validate_is_path(maybe_path: str) -> bool:
-    return os.path.exists(os.path.dirname(resolve_filepath(maybe_path)))
+    try: return resolve_user_filepath(path, None)
+    except FileNotFoundError: return path
 
+def validate_is_path(maybe_path: str) -> bool: return os.path.exists(os.path.dirname(resolve_filepath(maybe_path)))
 
 def generate_context(framework_name: str) -> _ModelContext:
     from .import_utils import is_flax_available
     from .import_utils import is_tf_available
     from .import_utils import is_torch_available
 
     framework_versions = {"transformers": pkg.get_pkg_version("transformers")}
-    if is_torch_available():
-        framework_versions["torch"] = pkg.get_pkg_version("torch")
+    if is_torch_available(): framework_versions["torch"] = pkg.get_pkg_version("torch")
     if is_tf_available():
         from bentoml._internal.frameworks.utils.tensorflow import get_tf_version
-
         framework_versions["tensorflow"] = get_tf_version()
-    if is_flax_available():
-        framework_versions.update(
-            {
-                "flax": pkg.get_pkg_version("flax"),
-                "jax": pkg.get_pkg_version("jax"),
-                "jaxlib": pkg.get_pkg_version("jaxlib"),
-            }
-        )
+    if is_flax_available(): framework_versions.update({"flax": pkg.get_pkg_version("flax"), "jax": pkg.get_pkg_version("jax"), "jaxlib": pkg.get_pkg_version("jaxlib")})
     return _ModelContext(framework_name=framework_name, framework_versions=framework_versions)
 
-
 def generate_labels(llm: openllm.LLM[t.Any, t.Any]) -> DictStrAny:
     return {
         "runtime": llm.runtime,
         "framework": "openllm",
         "model_name": llm.config["model_name"],
         "architecture": llm.config["architecture"],
         "serialisation_format": llm._serialisation_format,
     }
 
-
 _TOKENIZER_PREFIX = "_tokenizer_"
-
-
 def normalize_attrs_to_model_tokenizer_pair(**attrs: t.Any) -> tuple[DictStrAny, DictStrAny]:
     """Normalize the given attrs to a model and tokenizer kwargs accordingly."""
     tokenizer_attrs = {k[len(_TOKENIZER_PREFIX) :]: v for k, v in attrs.items() if k.startswith(_TOKENIZER_PREFIX)}
     for k in tuple(attrs.keys()):
-        if k.startswith(_TOKENIZER_PREFIX):
-            del attrs[k]
+        if k.startswith(_TOKENIZER_PREFIX): del attrs[k]
     return attrs, tokenizer_attrs
 
-
 @_overload
-def infer_auto_class(implementation: t.Literal["pt"]) -> type[openllm.AutoLLM]:
-    ...
-
-
+def infer_auto_class(implementation: t.Literal["pt"]) -> type[openllm.AutoLLM]: ...
 @_overload
-def infer_auto_class(implementation: t.Literal["tf"]) -> type[openllm.AutoTFLLM]:
-    ...
-
-
+def infer_auto_class(implementation: t.Literal["tf"]) -> type[openllm.AutoTFLLM]: ...
 @_overload
-def infer_auto_class(implementation: t.Literal["flax"]) -> type[openllm.AutoFlaxLLM]:
-    ...
-
-
+def infer_auto_class(implementation: t.Literal["flax"]) -> type[openllm.AutoFlaxLLM]: ...
 @_overload
-def infer_auto_class(implementation: t.Literal["vllm"]) -> type[openllm.AutoVLLM]:
-    ...
-
-
-def infer_auto_class(
-    implementation: LiteralRuntime,
-) -> type[openllm.AutoLLM] | type[openllm.AutoTFLLM] | type[openllm.AutoFlaxLLM] | type[openllm.AutoVLLM]:
+def infer_auto_class(implementation: t.Literal["vllm"]) -> type[openllm.AutoVLLM]: ...
+def infer_auto_class(implementation: LiteralRuntime) -> type[openllm.AutoLLM] | type[openllm.AutoTFLLM] | type[openllm.AutoFlaxLLM] | type[openllm.AutoVLLM]:
     if implementation == "tf":
         from openllm import AutoTFLLM
-
         return AutoTFLLM
     elif implementation == "flax":
         from openllm import AutoFlaxLLM
-
         return AutoFlaxLLM
     elif implementation == "pt":
         from openllm import AutoLLM
-
         return AutoLLM
     elif implementation == "vllm":
         from openllm import AutoVLLM
-
         return AutoVLLM
-    else:
-        raise RuntimeError(f"Unknown implementation: {implementation} (supported: 'pt', 'flax', 'tf', 'vllm')")
+    else: raise RuntimeError(f"Unknown implementation: {implementation} (supported: 'pt', 'flax', 'tf', 'vllm')")
 
 
 # NOTE: The set marks contains a set of modules name
 # that are available above and are whitelisted
 # to be included in the extra_objects map.
 _whitelist_modules = {"pkg"}
```

### Comparing `openllm-0.2.7/src/openllm/utils/analytics.py` & `openllm-0.2.8/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/utils/codegen.py` & `openllm-0.2.8/src/openllm/utils/codegen.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     PartialAny = functools.partial
 
 _T = t.TypeVar("_T", bound=t.Callable[..., t.Any])
 
 logger = logging.getLogger(__name__)
 
 OPENLLM_MODEL_NAME = "# openllm: model name"
-OPENLLM_MODEL_ID = "# openllm: model id"
 OPENLLM_MODEL_ADAPTER_MAP = "# openllm: model adapter map"
 
 
 class ModelNameFormatter(string.Formatter):
     model_keyword: t.LiteralString = "__model_name__"
 
     def __init__(self, model_name: str):
@@ -162,65 +161,43 @@
         annot = annot[1:-1]
 
     return annot.startswith(_classvar_prefixes)
 
 
 def add_method_dunders(cls: type[t.Any], method_or_cls: _T, _overwrite_doc: str | None = None) -> _T:
     """Add __module__ and __qualname__ to a *method* if possible."""
-    try:
-        method_or_cls.__module__ = cls.__module__
-    except AttributeError:
-        pass
-
-    try:
-        method_or_cls.__qualname__ = f"{cls.__qualname__}.{method_or_cls.__name__}"
-    except AttributeError:
-        pass
-
-    try:
-        method_or_cls.__doc__ = (
-            _overwrite_doc or "Generated by ``openllm.LLMConfig`` for class " f"{cls.__qualname__}."
-        )
-    except AttributeError:
-        pass
-
+    try: method_or_cls.__module__ = cls.__module__
+    except AttributeError: pass
+    try: method_or_cls.__qualname__ = f"{cls.__qualname__}.{method_or_cls.__name__}"
+    except AttributeError: pass
+    try: method_or_cls.__doc__ = _overwrite_doc or "Generated by ``openllm.LLMConfig`` for class " f"{cls.__qualname__}."
+    except AttributeError: pass
     return method_or_cls
 
 
-def _compile_and_eval(script: str, globs: DictStrAny, locs: t.Any = None, filename: str = "") -> None:
-    """Exec the script with the given global (globs) and local (locs) variables."""
-    bytecode = compile(script, filename, "exec")
-    eval(bytecode, globs, locs)  # noqa: S307
-
+# Exec the script with the given global (globs) and local (locs) variables.
+def _compile_and_eval(script: str, globs: DictStrAny, locs: t.Any = None, filename: str = "") -> None: eval(compile(script, filename, "exec"), globs, locs)  # noqa: S307
 
 # ported from attrs
 def _make_method(name: str, script: str, filename: str, globs: DictStrAny) -> AnyCallable:
     """Create the method with the script given and return the method object."""
     locs: DictStrAny = {}
 
     # In order of debuggers like PDB being able to step through the code,
     # we add a fake linecache entry.
     count = 1
     base_filename = filename
     while True:
-        linecache_tuple = (
-            len(script),
-            None,
-            script.splitlines(True),
-            filename,
-        )
+        linecache_tuple = (len(script), None, script.splitlines(True), filename)
         old_val = linecache.cache.setdefault(filename, linecache_tuple)
-        if old_val == linecache_tuple:
-            break
+        if old_val == linecache_tuple: break
         else:
             filename = f"{base_filename[:-1]}-{count}>"
             count += 1
-
     _compile_and_eval(script, globs, locs, filename)
-
     return locs[name]
 
 
 def make_attr_tuple_class(cls_name: str, attr_names: t.Sequence[str]) -> type[t.Any]:
     """Create a tuple subclass to hold class attributes.
 
     The subclass is a bare tuple with properties for names.
@@ -233,52 +210,39 @@
 
     attr_class_name = f"{cls_name}Attributes"
     attr_class_template = [
         f"class {attr_class_name}(tuple):",
         "    __slots__ = ()",
     ]
     if attr_names:
-        for i, attr_name in enumerate(attr_names):
-            attr_class_template.append(f"    {attr_name} = _attrs_property(_attrs_itemgetter({i}))")
-    else:
-        attr_class_template.append("    pass")
+        for i, attr_name in enumerate(attr_names): attr_class_template.append(f"    {attr_name} = _attrs_property(_attrs_itemgetter({i}))")
+    else: attr_class_template.append("    pass")
     globs: DictStrAny = {"_attrs_itemgetter": itemgetter, "_attrs_property": property}
-    if SHOW_CODEGEN:
-        logger.info("Generated class for %s:\n\n%s", attr_class_name, "\n".join(attr_class_template))
-
+    if SHOW_CODEGEN: logger.info("Generated class for %s:\n\n%s", attr_class_name, "\n".join(attr_class_template))
     _compile_and_eval("\n".join(attr_class_template), globs)
-
     return globs[attr_class_name]
 
 
-def generate_unique_filename(cls: type[t.Any], func_name: str) -> str:
-    return f"<{cls.__name__} generated {func_name} {cls.__module__}.{getattr(cls, '__qualname__', cls.__name__)}>"
+def generate_unique_filename(cls: type[t.Any], func_name: str) -> str: return f"<{cls.__name__} generated {func_name} {cls.__module__}.{getattr(cls, '__qualname__', cls.__name__)}>"
 
 
 def generate_function(
     typ: type[t.Any],
     func_name: str,
     lines: list[str] | None,
     args: tuple[str, ...] | None,
     globs: dict[str, t.Any],
     annotations: dict[str, t.Any] | None = None,
 ) -> AnyCallable:
     from . import SHOW_CODEGEN
 
-    script = "def %s(%s):\n    %s\n" % (
-        func_name,
-        ", ".join(args) if args is not None else "",
-        "\n    ".join(lines) if lines else "pass",
-    )
+    script = "def %s(%s):\n    %s\n" % (func_name, ", ".join(args) if args is not None else "", "\n    ".join(lines) if lines else "pass")
     meth = _make_method(func_name, script, generate_unique_filename(typ, func_name), globs)
-    if annotations:
-        meth.__annotations__ = annotations
-
-    if SHOW_CODEGEN:
-        logger.info("Generated script for %s:\n\n%s", typ, script)
+    if annotations: meth.__annotations__ = annotations
+    if SHOW_CODEGEN: logger.info("Generated script for %s:\n\n%s", typ, script)
 
     return meth
 
 
 def make_env_transformer(
     cls: type[openllm.LLMConfig],
     model_name: str,
@@ -330,30 +294,20 @@
     )
 
 
 def gen_sdk(func: AnyCallable, name: str | None = None, **attrs: t.Any):
     """Enhance function with nicer Repr."""
     from .representation import ReprMixin
 
-    if name is None:
-        name = func.__name__.strip("_")
-
+    if name is None: name = func.__name__.strip("_")
     _signatures = inspect.signature(func).parameters
-
-    def _repr(self: ReprMixin) -> str:
-        return f"<generated function {name} {orjson.dumps(dict(self.__repr_args__()), option=orjson.OPT_NON_STR_KEYS | orjson.OPT_INDENT_2).decode()}>"
-
-    def _repr_args(self: ReprMixin) -> t.Iterator[t.Tuple[str, t.Any]]:
-        return ((k, _signatures[k].annotation) for k in self.__repr_keys__)
-
-    if func.__doc__ is None:
-        doc = f"Generated SDK for {func.__name__}"
-    else:
-        doc = func.__doc__
-
+    def _repr(self: ReprMixin) -> str: return f"<generated function {name} {orjson.dumps(dict(self.__repr_args__()), option=orjson.OPT_NON_STR_KEYS | orjson.OPT_INDENT_2).decode()}>"
+    def _repr_args(self: ReprMixin) -> t.Iterator[t.Tuple[str, t.Any]]: return ((k, _signatures[k].annotation) for k in self.__repr_keys__)
+    if func.__doc__ is None: doc = f"Generated SDK for {func.__name__}"
+    else: doc = func.__doc__
     return functools.update_wrapper(
         types.new_class(
             name,
             (PartialAny, ReprMixin),
             exec_body=lambda ns: ns.update(
                 {
                     "__repr_keys__": property(lambda _: [i for i in _signatures.keys() if not i.startswith("_")]),
```

### Comparing `openllm-0.2.7/src/openllm/utils/dantic.py` & `openllm-0.2.8/src/openllm/utils/dantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,47 +113,24 @@
 @overload
 def Field(
     default: _B,
     *,
     use_default_converter: t.Literal[False] = False,
     converter: _ConverterType[_B, t.Any] = ...,
     **attrs: t.Any,
-) -> t.Any:
-    ...
-
-
-# NOTE: case 2, for stubs, we set the default value None, and thus respect class var type setter
+) -> t.Any: ...
+# NOTE: case 2, specifically for boolean, probably need to report to upstream python typing
 @overload
-def Field(default: None, **attrs: t.Any) -> t.Any:
-    ...
-
-
-# NOTE: case 3, we only specify description as helpers
+def Field(default: t.Literal[True, False], description: str = ...) -> bool: ...
+# NOTE: case 3, set the default to the correct type of the classvar setter
 @overload
-def Field(*, description: str | None = ..., **attrs: t.Any) -> t.Any:
-    ...
-
-
-# NOTE: case 4, we only specify description as helpers, and default type, then correctly set _T
+def Field(default: _T | None, **attrs: t.Any) -> _T: ...
+# NOTE: case 4, we only specify description as helpers
 @overload
-def Field(
-    default: _T,
-    *,
-    ge: int | float | None = None,
-    le: int | float | None = None,
-    validator: _ValidatorType[_T] | None = None,
-    description: str | None = None,
-    env: str | None = None,
-    auto_default: bool = False,
-    use_default_converter: bool = True,
-    **attrs: t.Any,
-) -> _T:
-    ...
-
-
+def Field(*, description: str | None = ..., **attrs: t.Any) -> t.Any: ...
 def Field(
     default: t.Any = None,
     *,
     ge: int | float | None = None,
     le: int | float | None = None,
     validator: _ValidatorType[_T] | None = None,
     description: str | None = None,
```

### Comparing `openllm-0.2.7/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.2.8/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.2.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.2.8/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/utils/dummy_pt_and_triton_objects.py` & `openllm-0.2.8/src/openllm/utils/dummy_vllm_objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,12 +15,28 @@
 from __future__ import annotations
 import typing as t
 
 from ..utils import DummyMetaclass
 from ..utils import require_backends
 
 
-class MPT(metaclass=DummyMetaclass):
-    _backends = ["torch", "triton"]
+class VLLMLlaMA(metaclass=DummyMetaclass):
+    _backends = ["vllm"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
-        require_backends(self, ["torch"])
+        require_backends(self, ["vllm"])
+
+class VLLMOPT(metaclass=DummyMetaclass):
+    _backends = ["vllm"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["vllm"])
+
+
+class AutoVLLM(metaclass=DummyMetaclass):
+    _backends = ["vllm"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["vllm"])
+
+
+MODEL_VLLM_MAPPING = None
```

### Comparing `openllm-0.2.7/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.2.8/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.2.8/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/utils/import_utils.py` & `openllm-0.2.8/src/openllm/utils/import_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,119 +66,71 @@
     "agents",
     "openai",
     "playground",
     "gptq",
 }
 ENV_VARS_TRUE_VALUES = {"1", "ON", "YES", "TRUE"}
 ENV_VARS_TRUE_AND_AUTO_VALUES = ENV_VARS_TRUE_VALUES.union({"AUTO"})
-
 USE_TF = os.environ.get("USE_TF", "AUTO").upper()
 USE_TORCH = os.environ.get("USE_TORCH", "AUTO").upper()
 USE_JAX = os.environ.get("USE_FLAX", "AUTO").upper()
-
 FORCE_TF_AVAILABLE = os.environ.get("FORCE_TF_AVAILABLE", "AUTO").upper()
 
 
 def _is_package_available(package: str) -> bool:
     _package_available = importlib.util.find_spec(package) is not None
     if _package_available:
-        try:
-            importlib.metadata.version(package)
-        except importlib.metadata.PackageNotFoundError:
-            _package_available = False
+        try: importlib.metadata.version(package)
+        except importlib.metadata.PackageNotFoundError: _package_available = False
     return _package_available
 
 
 _torch_available = importlib.util.find_spec("torch") is not None
 _tf_available = importlib.util.find_spec("tensorflow") is not None
 _flax_available = importlib.util.find_spec("jax") is not None and importlib.util.find_spec("flax") is not None
 _vllm_available = importlib.util.find_spec("vllm") is not None
-
 _peft_available = _is_package_available("peft")
 _einops_available = _is_package_available("einops")
 _cpm_kernel_available = _is_package_available("cpm_kernels")
 _bitsandbytes_available = _is_package_available("bitsandbytes")
 _datasets_available = _is_package_available("datasets")
 _triton_available = _is_package_available("triton")
 _jupyter_available = _is_package_available("jupyter")
 _jupytext_available = _is_package_available("jupytext")
 _notebook_available = _is_package_available("notebook")
 _autogptq_available = _is_package_available("auto_gptq")
 
-
-def is_transformers_supports_kbit() -> bool:
-    return pkg.pkg_version_info("transformers")[:2] >= (4, 30)
-
-
-def is_transformers_supports_agent() -> bool:
-    return pkg.pkg_version_info("transformers")[:2] >= (4, 29)
-
-
-def is_jupyter_available() -> bool:
-    return _jupyter_available
-
-
-def is_jupytext_available() -> bool:
-    return _jupytext_available
-
-
-def is_notebook_available() -> bool:
-    return _notebook_available
-
-
-def is_triton_available() -> bool:
-    return _triton_available
-
-
-def is_datasets_available() -> bool:
-    return _datasets_available
-
-
-def is_peft_available() -> bool:
-    return _peft_available
-
-
-def is_einops_available() -> bool:
-    return _einops_available
-
-
-def is_cpm_kernels_available() -> bool:
-    return _cpm_kernel_available
-
-
-def is_bitsandbytes_available() -> bool:
-    return _bitsandbytes_available
-
-
-def is_autogptq_available() -> bool:
-    return _autogptq_available
-
-
-def is_vllm_available() -> bool:
-    return _vllm_available
-
+def is_transformers_supports_kbit() -> bool: return pkg.pkg_version_info("transformers")[:2] >= (4, 30)
+def is_transformers_supports_agent() -> bool: return pkg.pkg_version_info("transformers")[:2] >= (4, 29)
+def is_jupyter_available() -> bool: return _jupyter_available
+def is_jupytext_available() -> bool: return _jupytext_available
+def is_notebook_available() -> bool: return _notebook_available
+def is_triton_available() -> bool: return _triton_available
+def is_datasets_available() -> bool: return _datasets_available
+def is_peft_available() -> bool: return _peft_available
+def is_einops_available() -> bool: return _einops_available
+def is_cpm_kernels_available() -> bool: return _cpm_kernel_available
+def is_bitsandbytes_available() -> bool: return _bitsandbytes_available
+def is_autogptq_available() -> bool: return _autogptq_available
+def is_vllm_available() -> bool: return _vllm_available
 
 def is_torch_available() -> bool:
     global _torch_available
     if USE_TORCH in ENV_VARS_TRUE_AND_AUTO_VALUES and USE_TF not in ENV_VARS_TRUE_VALUES:
         if _torch_available:
-            try:
-                importlib.metadata.version("torch")
-            except importlib.metadata.PackageNotFoundError:
-                _torch_available = False
+            try: importlib.metadata.version("torch")
+            except importlib.metadata.PackageNotFoundError: _torch_available = False
     else:
         logger.info("Disabling PyTorch because USE_TF is set")
         _torch_available = False
     return _torch_available
 
-
 def is_tf_available() -> bool:
     global _tf_available
-    if FORCE_TF_AVAILABLE in ENV_VARS_TRUE_VALUES:
-        _tf_available = True
+    if FORCE_TF_AVAILABLE in ENV_VARS_TRUE_VALUES: _tf_available = True
     else:
         _tf_version = None
         if USE_TF in ENV_VARS_TRUE_AND_AUTO_VALUES and USE_TORCH not in ENV_VARS_TRUE_VALUES:
             if _tf_available:
                 candidates = (
                     "tensorflow",
                     "tensorflow-cpu",
@@ -194,61 +146,49 @@
                 )
                 _tf_version = None
                 # For the metadata, we have to look for both tensorflow and tensorflow-cpu
                 for _pkg in candidates:
                     try:
                         _tf_version = importlib.metadata.version(_pkg)
                         break
-                    except importlib.metadata.PackageNotFoundError:
-                        pass
+                    except importlib.metadata.PackageNotFoundError: pass
                 _tf_available = _tf_version is not None
             if _tf_available:
                 if _tf_version and version.parse(_tf_version) < version.parse("2"):
                     logger.info("TensorFlow found but with version %s. OpenLLM only supports TF 2.x", _tf_version)
                     _tf_available = False
         else:
             logger.info("Disabling Tensorflow because USE_TORCH is set")
             _tf_available = False
     return _tf_available
 
-
 def is_flax_available() -> bool:
     global _flax_available
     if USE_JAX in ENV_VARS_TRUE_AND_AUTO_VALUES:
         if _flax_available:
             try:
                 importlib.metadata.version("jax")
                 importlib.metadata.version("flax")
-            except importlib.metadata.PackageNotFoundError:
-                _flax_available = False
-    else:
-        _flax_available = False
+            except importlib.metadata.PackageNotFoundError: _flax_available = False
+    else: _flax_available = False
     return _flax_available
 
 
-def requires_dependencies(
-    package: str | list[str], *, extra: str | list[str] | None = None
-) -> t.Callable[[t.Callable[P, t.Any]], t.Callable[P, t.Any]]:
+def requires_dependencies(package: str | list[str], *, extra: str | list[str] | None = None) -> t.Callable[[t.Callable[P, t.Any]], t.Callable[P, t.Any]]:
     import openllm.utils
 
-    if isinstance(package, str):
-        package = [package]
-    if isinstance(extra, str):
-        extra = [extra]
+    if isinstance(package, str): package = [package]
+    if isinstance(extra, str): extra = [extra]
 
     def decorator(func: t.Callable[P, t.Any]):
         @functools.wraps(func)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> t.Any:
             for p in package:
                 cached_check: t.Callable[[], bool] | None = getattr(openllm.utils, f"is_{p}_available", None)
-                if not ((cached_check is not None and cached_check()) or _is_package_available(p)):
-                    raise ImportError(
-                        f"{func.__name__} requires '{p}' to be available locally (Currently missing)."
-                        f"Make sure to have {p} to be installed: 'pip install \"{p if not extra else 'openllm['+', '.join(extra)+']'}\"'"
-                    )
+                if not ((cached_check is not None and cached_check()) or _is_package_available(p)): raise ImportError( f"{func.__name__} requires '{p}' to be available locally (Currently missing). Make sure to have {p} to be installed: 'pip install \"{p if not extra else 'openllm['+', '.join(extra)+']'}\"'")
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
@@ -384,47 +324,34 @@
 
     It will raises ImportError generated by ``require_backends`` if users try to access attributes from given class.
     """
 
     _backends: t.List[str]
 
     def __getattribute__(cls, key: str) -> t.Any:
-        if key.startswith("_"):
-            return super().__getattribute__(key)
+        if key.startswith("_"): return super().__getattribute__(key)
         require_backends(cls, cls._backends)
 
 
 def require_backends(o: t.Any, backends: t.MutableSequence[str]) -> None:
-    if not isinstance(backends, (list, tuple)):
-        backends = list(backends)
-
+    if not isinstance(backends, (list, tuple)): backends = list(backends)
     name = o.__name__ if hasattr(o, "__name__") else o.__class__.__name__
-
     # Raise an error for users who might not realize that classes without "TF" are torch-only
-    if "torch" in backends and "tf" not in backends and not is_torch_available() and is_tf_available():
-        raise ImportError(PYTORCH_IMPORT_ERROR_WITH_TF.format(name))
-
+    if "torch" in backends and "tf" not in backends and not is_torch_available() and is_tf_available(): raise ImportError(PYTORCH_IMPORT_ERROR_WITH_TF.format(name))
     # Raise the inverse error for PyTorch users trying to load TF classes
-    if "tf" in backends and "torch" not in backends and is_torch_available() and not is_tf_available():
-        raise ImportError(TF_IMPORT_ERROR_WITH_PYTORCH.format(name))
-
+    if "tf" in backends and "torch" not in backends and is_torch_available() and not is_tf_available(): raise ImportError(TF_IMPORT_ERROR_WITH_PYTORCH.format(name))
+    # Raise an error when vLLM is not available to consider the alternative, order from PyTorch -> Tensorflow -> Flax
     if "vllm" in backends:
-        if "torch" not in backends and is_torch_available() and not is_vllm_available():
-            raise ImportError(VLLM_IMPORT_ERROR_WITH_PYTORCH.format(name))
-
-        if "tf" not in backends and is_tf_available() and not is_vllm_available():
-            raise ImportError(VLLM_IMPORT_ERROR_WITH_TF.format(name))
-
-        if "flax" not in backends and is_flax_available() and not is_vllm_available():
-            raise ImportError(VLLM_IMPORT_ERROR_WITH_FLAX.format(name))
+        if "torch" not in backends and is_torch_available() and not is_vllm_available(): raise ImportError(VLLM_IMPORT_ERROR_WITH_PYTORCH.format(name))
+        if "tf" not in backends and is_tf_available() and not is_vllm_available(): raise ImportError(VLLM_IMPORT_ERROR_WITH_TF.format(name))
+        if "flax" not in backends and is_flax_available() and not is_vllm_available(): raise ImportError(VLLM_IMPORT_ERROR_WITH_FLAX.format(name))
 
     checks = (BACKENDS_MAPPING[backend] for backend in backends)
     failed = [msg.format(name) for available, msg in checks if not available()]
-    if failed:
-        raise ImportError("".join(failed))
+    if failed: raise ImportError("".join(failed))
 
 
 class EnvVarMixin(ReprMixin):
     model_name: str
 
     @property
     def __repr_keys__(self) -> set[str]:
@@ -436,15 +363,16 @@
         quantize: str
         framework: str
         bettertransformer: str
         runtime: t.Literal["ggml", "transformers"]
 
         framework_value: LiteralRuntime
         quantize_value: str | None
-        bettertransformer_value: str | None
+        bettertransformer_value: bool | None
+        model_id_value: str | None
         runtime_value: t.Literal["ggml", "transformers"]
 
     # fmt: off
     @overload
     def __getitem__(self, item: t.Literal["config"]) -> str: ...
     @overload
     def __getitem__(self, item: t.Literal["model_id"]) -> str: ...
@@ -459,82 +387,57 @@
     @overload
     def __getitem__(self, item: t.Literal["framework_value"]) -> LiteralRuntime: ...
     @overload
     def __getitem__(self, item: t.Literal["quantize_value"]) -> str | None: ...
     @overload
     def __getitem__(self, item: t.Literal["model_id_value"]) -> str | None: ...
     @overload
-    def __getitem__(self, item: t.Literal["bettertransformer_value"]) -> str | None: ...
+    def __getitem__(self, item: t.Literal["bettertransformer_value"]) -> bool: ...
     @overload
     def __getitem__(self, item: t.Literal["runtime_value"]) -> t.Literal["ggml", "transformers"]: ...
     # fmt: on
 
     def __getitem__(self, item: str | t.Any) -> t.Any:
-        if hasattr(self, item):
-            return getattr(self, item)
+        if hasattr(self, item): return getattr(self, item)
         raise KeyError(f"Key {item} not found in {self}")
 
     def __new__(
         cls,
         model_name: str,
         implementation: LiteralRuntime = "pt",
+        model_id: str | None = None,
         bettertransformer: bool | None = None,
         quantize: t.LiteralString | None = None,
         runtime: t.Literal["ggml", "transformers"] = "transformers",
     ) -> t.Self:
         from . import codegen
         from .._configuration import field_env_key
-
         model_name = inflection.underscore(model_name)
 
         res = super().__new__(cls)
         res.model_name = model_name
 
         # gen properties env key
-        attributes = {"config", "model_id", "quantize", "framework", "bettertransformer", "runtime"}
-        for att in attributes:
-            setattr(res, att, field_env_key(model_name, att.upper()))
+        for att in {"config", "model_id", "quantize", "framework", "bettertransformer", "runtime"}: setattr(res, att, field_env_key(model_name, att.upper()))
 
         # gen properties env value
         attributes_with_values = {
             "framework": (str, implementation),
             "quantize": (str, quantize),
             "bettertransformer": (bool, bettertransformer),
-            "model_id": (str, None),
+            "model_id": (str, model_id),
             "runtime": (str, runtime),
         }
-        globs: dict[str, t.Any] = {
-            "__bool_vars_value": ENV_VARS_TRUE_VALUES,
-            "__env_get": os.getenv,
-            "self": res,
-        }
+        globs: dict[str, t.Any] = {"__bool_vars_value": ENV_VARS_TRUE_VALUES, "__env_get": os.getenv, "self": res}
 
         for attribute, (default_type, default_value) in attributes_with_values.items():
             lines: list[str] = []
-            if default_type is bool:
-                lines.append(
-                    f"return str(__env_get(self['{attribute}'], str(__env_default)).upper() in __bool_vars_value)"
-                )
-            else:
-                lines.append(f"return __env_get(self['{attribute}'], __env_default)")
+            if default_type is bool: lines.append(f"return str(__env_get(self['{attribute}'], str(__env_default)).upper() in __bool_vars_value)")
+            else: lines.append(f"return __env_get(self['{attribute}'], __env_default)")
 
-            setattr(
-                res,
-                f"{attribute}_value",
-                codegen.generate_function(
-                    cls,
-                    "_env_get_" + attribute,
-                    lines,
-                    ("__env_default",),
-                    globs,
-                )(default_value),
-            )
+            setattr(res, f"{attribute}_value", codegen.generate_function(cls, "_env_get_" + attribute, lines, ("__env_default",), globs)(default_value))
 
         return res
-
     @property
-    def start_docstring(self) -> str:
-        return getattr(self.module, f"START_{self.model_name.upper()}_COMMAND_DOCSTRING")
-
+    def start_docstring(self) -> str: return getattr(self.module, f"START_{self.model_name.upper()}_COMMAND_DOCSTRING")
     @property
-    def module(self) -> _AnnotatedLazyLoader[t.LiteralString]:
-        return _AnnotatedLazyLoader(self.model_name, globals(), f"openllm.models.{self.model_name}")
+    def module(self) -> _AnnotatedLazyLoader[t.LiteralString]: return _AnnotatedLazyLoader(self.model_name, globals(), f"openllm.models.{self.model_name}")
```

### Comparing `openllm-0.2.7/src/openllm/utils/lazy.py` & `openllm-0.2.8/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm/utils/representation.py` & `openllm-0.2.8/src/openllm/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm_client/__init__.py` & `openllm-0.2.8/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm_client/_prompt.py` & `openllm-0.2.8/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm_client/runtimes/__init__.py` & `openllm-0.2.8/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/src/openllm_client/runtimes/base.py` & `openllm-0.2.8/src/openllm_client/runtimes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,18 @@
     def __init_subclass__(cls, *, client_type: t.Literal["http", "grpc"] = "http", api_version: str = "v1"):
         """Initialise subclass for HTTP and gRPC client type."""
         cls._client_class = bentoml.client.HTTPClient if client_type == "http" else bentoml.client.GrpcClient
         cls._api_version = api_version
 
     @property
     def _hf_agent(self) -> transformers.HfAgent:
+        if not self.supports_hf_agent:
+            raise openllm.exceptions.OpenLLMException(
+                f"{self.model_name} ({self.framework}) does not support running HF agent."
+            )
         if self.__agent__ is None:
             if not openllm.utils.is_transformers_supports_agent():
                 raise RuntimeError(
                     "Current 'transformers' does not support Agent."
                     " Make sure to upgrade to at least 4.29: 'pip install -U \"transformers>=4.29\"'"
                 )
             self.__agent__ = transformers.HfAgent(urljoin(self._address, "/hf/agent"))
@@ -127,14 +131,24 @@
 
     @property
     @abstractmethod
     def configuration(self) -> dict[str, t.Any]:
         raise NotImplementedError
 
     @property
+    @abstractmethod
+    def supports_embeddings(self) -> bool:
+        raise NotImplementedError
+
+    @property
+    @abstractmethod
+    def supports_hf_agent(self) -> bool:
+        raise NotImplementedError
+
+    @property
     def llm(self) -> openllm.LLM[t.Any, t.Any]:
         if self.__llm__ is None:
             self.__llm__ = openllm.infer_auto_class(self.framework).for_model(self.model_name)
         return self.__llm__
 
     @property
     def config(self) -> openllm.LLMConfig:
```

### Comparing `openllm-0.2.7/src/openllm_client/runtimes/grpc.py` & `openllm-0.2.8/src/openllm_client/runtimes/grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,14 +76,28 @@
     def configuration(self) -> dict[str, t.Any]:
         try:
             v = self._metadata.json.struct_value.fields["configuration"].string_value
             return orjson.loads(v)
         except KeyError:
             raise RuntimeError("Malformed service endpoint. (Possible malicious)") from None
 
+    @property
+    def supports_embeddings(self) -> bool:
+        try:
+            return self._metadata.json.struct_value.fields["supports_embeddings"].bool_value
+        except KeyError:
+            raise RuntimeError("Malformed service endpoint. (Possible malicious)") from None
+
+    @property
+    def supports_hf_agent(self) -> bool:
+        try:
+            return self._metadata.json.struct_value.fields["supports_hf_agent"].bool_value
+        except KeyError:
+            raise RuntimeError("Malformed service endpoint. (Possible malicious)") from None
+
     def postprocess(self, result: Response | dict[str, t.Any]) -> openllm.GenerationOutput:
         if isinstance(result, dict):
             return openllm.GenerationOutput(**result)
 
         from google.protobuf.json_format import MessageToDict
 
         return openllm.GenerationOutput(**MessageToDict(result.json, preserving_proto_field_name=True))
```

### Comparing `openllm-0.2.7/src/openllm_client/runtimes/http.py` & `openllm-0.2.8/src/openllm_client/runtimes/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,14 +73,28 @@
     @property
     def configuration(self) -> dict[str, t.Any]:
         try:
             return orjson.loads(self._metadata["configuration"])
         except KeyError:
             raise RuntimeError("Malformed service endpoint. (Possible malicious)") from None
 
+    @property
+    def supports_embeddings(self) -> bool:
+        try:
+            return self._metadata.get("supports_embeddings", False)
+        except KeyError:
+            raise RuntimeError("Malformed service endpoint. (Possible malicious)") from None
+
+    @property
+    def supports_hf_agent(self) -> bool:
+        try:
+            return self._metadata.get("supports_hf_agent", False)
+        except KeyError:
+            raise RuntimeError("Malformed service endpoint. (Possible malicious)") from None
+
     def postprocess(self, result: dict[str, t.Any]) -> openllm.GenerationOutput:
         return openllm.GenerationOutput(**result)
 
 
 class HTTPClient(HTTPClientMixin, BaseClient[DictStrAny]):
     def __init__(self, address: str, timeout: int = 30):
         address = address if "://" in address else "http://" + address
```

### Comparing `openllm-0.2.7/tests/__init__.py` & `openllm-0.2.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/client_test.py` & `openllm-0.2.8/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/configuration_test.py` & `openllm-0.2.8/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/conftest.py` & `openllm-0.2.8/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 _PROMPT_MAPPING = {
     "qa": "Answer the following yes/no question by reasoning step-by-step. Can you write a whole Haiku in a single tweet?",
 }
 
 
 def parametrise_local_llm(
     model: str,
-) -> t.Generator[tuple[str, openllm.LLMRunner | openllm.LLM[t.Any, t.Any]], None, None]:
+) -> t.Generator[tuple[str, openllm.LLMRunner[t.Any, t.Any] | openllm.LLM[t.Any, t.Any]], None, None]:
     if model not in _FRAMEWORK_MAPPING:
         pytest.skip(f"'{model}' is not yet supported in framework testing.")
 
     runtime_impl: tuple[LiteralRuntime, ...] = tuple()
     if model in openllm.MODEL_MAPPING_NAMES:
         runtime_impl += ("pt",)
     if model in openllm.MODEL_FLAX_MAPPING_NAMES:
```

### Comparing `openllm-0.2.7/tests/models_test.py` & `openllm-0.2.8/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/package_test.py` & `openllm-0.2.8/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/strategies_test.py` & `openllm-0.2.8/tests/strategies_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 import os
-import sys
 import typing as t
 
 import pytest
 
 
 if t.TYPE_CHECKING:
     from _pytest.monkeypatch import MonkeyPatch
@@ -100,21 +99,14 @@
             "Input list should be all string type."
         )
         assert pytest.raises(ValueError, NvidiaGpuResource.validate, ["GPU-5ebe9f43", "GPU-ac33420d4628"]).match(
             "Failed to parse available GPUs UUID"
         )
 
 
-@pytest.mark.skipif(sys.platform != "darwin", reason="Test NVIDIA validation on Darwin only")
-def test_nvidia_gpu_validation_on_darwin():
-    assert pytest.raises(RuntimeError, NvidiaGpuResource.validate, ["0"]).match(
-        "GPU is not available on Darwin system."
-    )
-
-
 def test_nvidia_gpu_from_spec(monkeypatch: pytest.MonkeyPatch):
     with monkeypatch.context() as mcls:
         # to make this tests works with system that has GPU
         mcls.setenv("CUDA_VISIBLE_DEVICES", "")
         assert NvidiaGpuResource.from_spec(1) == ["0"]
         assert NvidiaGpuResource.from_spec("5") == ["0", "1", "2", "3", "4"]
         assert NvidiaGpuResource.from_spec(1) == ["0"]
```

### Comparing `openllm-0.2.7/tests/_strategies/__init__.py` & `openllm-0.2.8/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/_strategies/_configuration.py` & `openllm-0.2.8/tests/_strategies/_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         "default_id": st.text(min_size=1),
         "model_ids": st.lists(st.text(), min_size=1),
         "architecture": st.text(min_size=1),
         "url": st.text(),
         "requires_gpu": st.booleans(),
         "trust_remote_code": st.booleans(),
         "requirements": st.none() | st.lists(st.text(), min_size=1),
-        "default_implementation": st.sampled_from(["vllm", "pt", "tf", "flax"]),
+        "default_implementation": st.dictionaries(["cpu", "nvidia.com/gpu"], ["vllm", "pt", "tf", "flax"]),
         "model_type": st.sampled_from(["causal_lm", "seq2seq_lm"]),
         "runtime": st.sampled_from(["transformers", "ggml"]),
         "name_type": st.sampled_from(["dasherize", "lowercase"]),
         "timeout": st.integers(min_value=3600),
         "workers_per_resource": st.one_of(st.integers(min_value=1), st.floats(min_value=0.1, max_value=1.0)),
     }
     return draw(st.builds(ModelSettings, **kwargs))
```

### Comparing `openllm-0.2.7/tests/models/__init__.py` & `openllm-0.2.8/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/models/conftest.py` & `openllm-0.2.8/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/models/flan_t5_test.py` & `openllm-0.2.8/tests/models/flan_t5_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/models/opt_test.py` & `openllm-0.2.8/tests/models/opt_test.py`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json` & `openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json` & `openllm-0.2.8/tests/models/__snapshots__/flan_t5_test/test_flan_t5[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/models/__snapshots__/opt_test/test_opt_125m[container].json` & `openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[container].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/tests/models/__snapshots__/opt_test/test_opt_125m[local].json` & `openllm-0.2.8/tests/models/__snapshots__/opt_test/test_opt_125m[local].json`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/.gitignore` & `openllm-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/LICENSE.md` & `openllm-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.2.7/README.md` & `openllm-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 ```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/docs/transformers/model_doc/opt>opt</a></td>
-<td><a href=https://huggingface.co/docs/transformers/main/model_doc/opt#transformers.MPTForCausalLM><code>MPTForCausalLM</code></a></td>
+<td><a href=https://huggingface.co/docs/transformers/main/model_doc/opt#transformers.OPTForCausalLM><code>OPTForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 <ul><li><a href=https://huggingface.co/facebook/opt-125m><code>facebook/opt-125m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-350m><code>facebook/opt-350m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-1.3b><code>facebook/opt-1.3b</code></a></li>
```

#### html2text {}

```diff
@@ -136,15 +136,15 @@
                                                       * mosaicml/mpt-
                                                         30b-chat
                                                       * facebook/opt-
                                                         125m
                                                       * facebook/opt-
                                                         350m             ```bash pip
                                                       * facebook/opt-    install
-opt       MPTForCausalLM                  ââ      1.3b             "openllm
+opt       OPTForCausalLM                  ââ      1.3b             "openllm
                                                       * facebook/opt-    [opt]" ```
                                                         2.7b
                                                       * facebook/opt-
                                                         6.7b
                                                       * facebook/opt-66b
                                                       * stabilityai/
                                                         stablelm-tuned-
```

### Comparing `openllm-0.2.7/pyproject.toml` & `openllm-0.2.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,18 @@
     "optimum",
     "attrs>=23.1.0",
     "cattrs>=23.1.0",
     "orjson",
     "inflection",
     "tabulate[widechars]>=0.9.0",
     "httpx",
+    "click>=8.1.6",
     "typing_extensions",
     "cuda-python;platform_system!=\"Darwin\"",
-    "bitsandbytes<0.40",
+    "bitsandbytes<0.42",
 ]
 description = 'OpenLLM: Operating LLMs in production'
 dynamic = ["version"]
 keywords = [
     "MLOps",
     "AI",
     "BentoML",
@@ -68,15 +69,15 @@
 requires-python = ">=3.8"
 
 [project.scripts]
 openllm = "openllm.cli:cli"
 
 [project.urls]
 Blog = "https://modelserving.com"
-Discord = "https://l.bentoml.com/join-openllm-discord"
+Chat = "https://discord.gg/openllm"
 Documentation = "https://github.com/bentoml/openllm#readme"
 GitHub = "https://github.com/bentoml/openllm"
 History = "https://github.com/bentoml/openllm/blob/main/CHANGELOG.md"
 Homepage = "https://bentoml.com"
 Tracker = "https://github.com/bentoml/openllm/issues"
 Twitter = "https://twitter.com/bentomlai"
 
@@ -152,40 +153,17 @@
 whitelist-regex = ["test_.*"]
 
 [tool.pytest.ini_options]
 addopts = ["-rfEX", "-pno:warnings", "--snapshot-warn-unused"]
 python_files = ["test_*.py", "*_test.py"]
 testpaths = ["tests"]
 
-[tool.black]
-exclude = '''
-(
-  /(
-      \.eggs
-    | \.git
-    | \.tox
-    | \.venv
-    | _build
-    | .build
-    | bazel-*
-    | build
-    | venv
-    | lib
-    | dist
-    | tools
-  )/
-  | src/openllm/__about__.py
-)
-'''
-line-length = 119
-target-version = ["py38", "py39", "py310", "py311"]
-
 [tool.ruff]
-exclude = ["tools", "src/openllm/playground"]
-extend-include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
+extend-exclude = ["tools", "src/openllm/playground", "src/openllm/models", "src/openllm/_types.py"]
+extend-include = ["*.ipynb"]
 extend-select = [
     "B",    # flake8-bugbear
     "I",    # isort
     "G",    # flake8-logging-format
     "D",    # pydocstyle
     "W",    # pycodestyle
     "Q",    # flake8-quotes
@@ -219,20 +197,23 @@
     "D103",    # Just missing docstring for magic methods.
     "D102",
     "D101",
     "D100",
     "TCH004",  # don't move runtime import out, just warn about it
     "RUF012",  # mutable attributes to be used with ClassVar
     "B905",    # zip warning about strict, only applicable for 3.10+
+    "D105",    # magic docstring
+    "E701",    # multiple statement on single line
 ]
 line-length = 119
 target-version = "py312"
 unfixable = [
     "F401",   # Don't touch unused imports, just warn about it.
     "TCH004", # Don't touch import outside of TYPE_CHECKING block
+    "RUF100", # unused noqa, just warn about it
 ]
 [tool.ruff.flake8-type-checking]
 exempt-modules = ["typing", "typing_extensions", "."]
 runtime-evaluated-base-classes = [
     "pydantic.BaseModel",
     "openllm._configuration.LLMConfig",
     "openllm._configuration.GenerationConfig",
@@ -251,25 +232,18 @@
 relative-imports-order = "closest-to-furthest"
 [tool.ruff.flake8-quotes]
 avoid-escape = false
 [tool.ruff.extend-per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "__init__.py" = ["E402", "F401", "F403", "F811"]
 "examples/**/*" = ["D"]
-"src/openllm/_llm.py" = ["B010", "B009"]
-"src/openllm/_strategies.py" = ["B904"]
-"src/openllm/_types.py" = ["E402"]
+"src/openllm/_service.py" = ["I001", "E401"]
 "src/openllm/cli.py" = ["D301", "S101"]
-"src/openllm/models/**/*" = ["D106", "S101", "D104"]
-"src/openllm/playground/**/*" = ["E402", "F401", "PLR", "D"]
 "src/openllm/utils/dummy_*" = ["D107"]
-"src/openllm/utils/import_utils.py" = [
-    "PLW0603", # OK to ignore global access here
-    "D105",    # magic docstring
-]
+"src/openllm/utils/import_utils.py" = ["PLW0603"]
 "src/openllm_client/runtimes/*" = ["D107"]
 "tests/**/*" = [
     "S101",
     "TID252",
     "D",      # No docstring in tests
     "PT011",  # ignore too broad raises, as it can be use pytest.raises().match()
     "S307",   # Ignore eval(compile) as it is a known script execution
@@ -331,18 +305,20 @@
 reportPrivateUsage = "warning"
 reportUnknownArgumentType = "warning"
 reportUnknownMemberType = "warning"
 reportUnknownVariableType = "warning"
 typeCheckingMode = "strict"
 
 [tool.mypy]
+# TODO: remove all of the disable to ensure strict type
 disable_error_code = ["attr-defined", "name-defined", "annotation-unchecked"]
 enable_error_code = ["redundant-expr"]
 exclude = ["examples/", "tools/", "tests/", "src/openllm/playground/"]
 files = ["src/openllm", "src/openllm_client"]
+local_partial_types = true
 mypy_path = "typings"
 pretty = true
 python_version = "3.11"
 show_error_codes = true
 strict = true
 warn_return_any = false
 warn_unreachable = true
```

### Comparing `openllm-0.2.7/PKG-INFO` & `openllm-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.2.7
+Version: 0.2.8
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
-Project-URL: Discord, https://l.bentoml.com/join-openllm-discord
+Project-URL: Chat, https://discord.gg/openllm
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/openllm
 Project-URL: History, https://github.com/bentoml/openllm/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
 Project-URL: Tracker, https://github.com/bentoml/openllm/issues
 Project-URL: Twitter, https://twitter.com/bentomlai
 Author-email: Aaron Pham <aarnphm@bentoml.com>
@@ -36,16 +36,17 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: attrs>=23.1.0
 Requires-Dist: bentoml[grpc,io]>=1.0.25
-Requires-Dist: bitsandbytes<0.40
+Requires-Dist: bitsandbytes<0.42
 Requires-Dist: cattrs>=23.1.0
+Requires-Dist: click>=8.1.6
 Requires-Dist: cuda-python; platform_system != 'Darwin'
 Requires-Dist: httpx
 Requires-Dist: inflection
 Requires-Dist: optimum
 Requires-Dist: orjson
 Requires-Dist: safetensors
 Requires-Dist: tabulate[widechars]>=0.9.0
@@ -422,15 +423,15 @@
 ```
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/docs/transformers/model_doc/opt>opt</a></td>
-<td><a href=https://huggingface.co/docs/transformers/main/model_doc/opt#transformers.MPTForCausalLM><code>MPTForCausalLM</code></a></td>
+<td><a href=https://huggingface.co/docs/transformers/main/model_doc/opt#transformers.OPTForCausalLM><code>OPTForCausalLM</code></a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 <ul><li><a href=https://huggingface.co/facebook/opt-125m><code>facebook/opt-125m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-350m><code>facebook/opt-350m</code></a></li>
 <li><a href=https://huggingface.co/facebook/opt-1.3b><code>facebook/opt-1.3b</code></a></li>
```

