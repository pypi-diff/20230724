# Comparing `tmp/ibm-generative-ai-0.2.2.tar.gz` & `tmp/ibm-generative-ai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-generative-ai-0.2.2.tar", last modified: Tue Jul 11 17:19:45 2023, max compression
+gzip compressed data, was "ibm-generative-ai-0.2.3.tar", last modified: Mon Jul 24 16:54:37 2023, max compression
```

## Comparing `ibm-generative-ai-0.2.2.tar` & `ibm-generative-ai-0.2.3.tar`

### file list

```diff
@@ -1,272 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.935201 ibm-generative-ai-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/01_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/02_feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/03_documentation_update.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/EXTENSIONS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/GETTING_STARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/STARTER_TEAM.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/SUPPORT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/assets/pull_request_from_fork_to_base.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/_templates/custom_landing_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.947201 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.947201 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/async.examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/async.examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/extensions.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/prompts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/prompts.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.credentials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.files_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.history_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.token_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.tunes_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.services.request_handler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.services.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.services.service_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/local_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.927201 ibm-generative-ai-0.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.947201 ibm-generative-ai-0.2.2/examples/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/async-flaky-request-handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/async-flaky-responses-ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/generate-all-models.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/history-async.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/load_token_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/logging_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.955201 ibm-generative-ai-0.2.2/examples/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/alice_bob_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/alice_bob_talk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.955201 ibm-generative-ai-0.2.2/examples/user/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/country-capital.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/penguins2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/complete_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/country-capital-qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/explain_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/generate_with_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/gpt_chat_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/grid_search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/grid_search_params_greeating.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/jsonprompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/jsonprompt_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/langchain_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/localserver/localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/localserver/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/logprob_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/many_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/model_as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt-raw-string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_csv_random_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_from_all_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_from_all_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_reuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/prompt_templating/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/file_to_tune.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/summarization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompts/Country-Capital-Factual-QA
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/saving_prompts_as_hf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/self-reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/self_instruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/examples/user/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/instruction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/self-reflection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/synth-animal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/tokenize-sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/innersource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.931201 ibm-generative-ai-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/genai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/exceptions/genai_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.931201 ibm-generative-ai-0.2.2/src/genai/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/save_huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/custom_model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/local_api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/extensions/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/pandas/prompt_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/prompt_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/routers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/tunes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/files_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/generate_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/history_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/token_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/tunes_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.971202 ibm-generative-ai-0.2.2/src/genai/services/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/tune_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.971202 ibm-generative-ai-0.2.2/src/genai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/search_space_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/watsonx_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.971202 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.975202 ibm-generative-ai-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.979202 ibm-generative-ai-0.2.2/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/age-gender.csv
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-content.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-multivar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub-noheader.csv
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub.csv
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub.json
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/csv_file.csv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/csv_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/file_to_tune.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/file_to_tune.json
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/file_to_tune.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/invalid-content-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/invalid-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/prompt_contents.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/response_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/story.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/story_sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_save_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_sub_from_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/test_terms_of_use.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_generate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_model_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_prompt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_prompt_pattern_watsonx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_service_interface_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_tunes.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/01_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/02_feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/03_documentation_update.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/EXTENSIONS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/STARTER_TEAM.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/SUPPORT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/documentation/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/assets/pull_request_from_fork_to_base.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/_templates/custom_landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.592310 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.592310 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/async.examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/async.examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/extensions.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/prompts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/prompts.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.files_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.history_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.token_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.tunes_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.services.request_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.services.service_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/local_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.576309 ibm-generative-ai-0.2.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.596310 ibm-generative-ai-0.2.3/examples/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/async-flaky-request-handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/async-flaky-responses-ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/generate-all-models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/history-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/load_token_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/logging_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.600310 ibm-generative-ai-0.2.3/examples/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/alice_bob_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/alice_bob_talk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/country-capital.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/penguins2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/complete_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/country-capital-qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/explain_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/generate_with_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/gpt_chat_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/grid_search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/grid_search_params_greeating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/jsonprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/jsonprompt_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/langchain_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/localserver/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/localserver/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/logprob_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/many_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/model_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt-raw-string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_csv_random_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_from_all_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_from_all_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompt_templating/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/summarization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompts/Country-Capital-Factual-QA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/saving_prompts_as_hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/self-reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/self_instruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/examples/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/instruction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/self-reflection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/synth-animal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/tokenize-sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.580309 ibm-generative-ai-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/genai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/exceptions/genai_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.580309 ibm-generative-ai-0.2.3/src/genai/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/save_huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/custom_model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/local_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/extensions/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/pandas/prompt_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/prompt_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/tunes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/files_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/generate_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/history_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/token_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/tunes_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.616311 ibm-generative-ai-0.2.3/src/genai/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/tune_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.616311 ibm-generative-ai-0.2.3/src/genai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/search_space_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/watsonx_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.616311 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.620311 ibm-generative-ai-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.624311 ibm-generative-ai-0.2.3/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/age-gender.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-content.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-multivar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub-noheader.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/csv_file.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/csv_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/file_to_tune.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/file_to_tune.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/invalid-content-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/invalid-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/prompt_contents.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/response_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/story.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/story_sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_save_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_sub_from_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/test_terms_of_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_generate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_model_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_prompt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_prompt_pattern_watsonx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_service_interface_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_tunes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_version.py
```

### Comparing `ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/01_bug_report.md` & `ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/01_bug_report.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/02_feature_request.md` & `ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/02_feature_request.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/03_documentation_update.md` & `ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/03_documentation_update.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.github/PULL_REQUEST_TEMPLATE.md` & `ibm-generative-ai-0.2.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.github/workflows/documentation.yml` & `ibm-generative-ai-0.2.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.github/workflows/integration-test.yml` & `ibm-generative-ai-0.2.3/.github/workflows/integration-test.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.github/workflows/main.yml` & `ibm-generative-ai-0.2.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.github/workflows/python-publish.yml` & `ibm-generative-ai-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.gitignore` & `ibm-generative-ai-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/.pre-commit-config.yaml` & `ibm-generative-ai-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/CODE_OF_CONDUCT.md` & `ibm-generative-ai-0.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/CONTRIBUTING.md` & `ibm-generative-ai-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/EXTENSIONS.md` & `ibm-generative-ai-0.2.3/EXTENSIONS.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 - official open-source extensions (supported by the project team)
 - third-party open-source extensions
 
 ## Open-source "Gen AI official" extensions
 Extensions that are meant for public use from the get-go should instead be developed as official open-source extensions. Examples of official extensions that have already been released are LangChain, Pandas, and Hugging Face extensions.
 
 ### Ownership and location
-Open-source extensions should be submitted directly to the [IBM Generative AI open-source repository](https://github.com/IBM/ibm-generative-ai) and should be developed following the [open-source Gen AI contribution guide](https://github.com/IBM/ibm-generative-ai/blob/main/DEVELOPMENT.md). Open-source official extensions are typically developed by the Gen AI team, or in collaboration with them. Providing maintenance to open-source official extensions is responsability of the Gen AI team.
+Open-source extensions should be submitted directly to the [IBM Generative AI open-source repository](https://github.com/IBM/ibm-generative-ai) and should be developed following the [open-source Gen AI contribution guide](https://github.com/IBM/ibm-generative-ai/blob/main/CONTRIBUTING.md). Open-source official extensions are typically developed by the Gen AI team, or in collaboration with them. Providing maintenance to open-source official extensions is responsability of the Gen AI team.
 
 ## Open-source "third-party" extensions
 All other extensions neither implemented nor officially maintained by the Gen AI team are referred to as open-source third-party extensions.
 
 ### Ownership and location
 Open-source third-party extensions can live anywhere, inside [IBM organization](https://github.com/IBM/), the wider Github universe, or other contributors' own Github spaces (e.g., other IBM teams, clients, partners). Maintaining these extensions would be the responsibility of their owners.
```

### Comparing `ibm-generative-ai-0.2.2/GETTING_STARTED.md` & `ibm-generative-ai-0.2.3/GETTING_STARTED.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # Getting Started Guideline
 
 ## <a name='TableofContents'></a>Table of Contents
 
-<!-- vscode-markdown-toc -->
 * [Table of Contents](#table-of-contents)
 * [Installation](#installation)
 * [Gen AI Endpoint](#gen-ai-endpoint)
     * [Example](#example)
 * [Examples](#examples)
     * [Async Example](#async-example)
     * [Synchronous Example](#synchronous-example)
 * [Tips and Troubleshooting](#tips-and-troubleshooting)
+    * [Model Availability](#model-availability)
     * [Enabling Logs](#enabling-logs)
     * [Experimenting with a Large Number of Prompts](#many-prompts)
 * [Extensions](#extensions)
     * [LangChain Extension](#langchain-extension)
 * [Support](#support)
 
 ## <a name='Installation'></a>Installation
 
 ```bash
 pip install ibm-generative-ai
 ```
+
 #### <a name='KnownIssueFixes:'></a>Known Issue Fixes:
+
 - **[SSL Issue]** If you run into "SSL_CERTIFICATE_VERIFY_FAILED" please run the following code snippet here: [support](SUPPORT.md).
 
 ### <a name='Prerequisites'></a>Prerequisites
+
 Python version >= 3.9
 
 Pip version >= 22.0.1
 
 Check your pip version with `pip --version` and if needed run the following command to upgrade pip.
 
 ```bash
@@ -66,21 +69,19 @@
 # creds object
 creds = Credentials(api_key=my_api_key, api_endpoint=my_api_endpoint)
 
 # Now start using GenAI!
 
 ```
 
-
 ## <a name='Examples'></a>Examples
 
 There are a number of examples you can try in the [`examples/user`](examples/user) directory.
 Login to [workbench.res.ibm.com](https://workbench.res.ibm.com/) and get your GenAI API key. Then, create a `.env` file and assign the `GENAI_KEY` value as below example. [More information](#gen-ai-endpoint)
 
-
 ```ini
 GENAI_KEY=YOUR_GENAI_API_KEY
 # GENAI_API=GENAI_API_ENDPOINT << for a different endpoint
 ```
 
 ### <a name='AsyncExample'></a>Async Example
 
@@ -180,14 +181,48 @@
 for response in responses:
     print(f"Generated text: {response.generated_text}")
 
 ```
 
 ## <a name='TipsAndTroubleshooting'></a>Tips and Troubleshooting
 
+### <a name='Model Availability'></a>Model Availability
+To test the reachability of your endpoint and availability of desired model, use the following utility script with your model details:
+```python
+import os
+
+from dotenv import load_dotenv
+
+from genai.credentials import Credentials
+from genai.model import Model
+
+# make sure you have a .env file under genai root with
+# GENAI_KEY=<your-genai-key>
+# GENAI_API=<your-genai-api endpoint>
+load_dotenv()
+api_key = os.getenv("GENAI_KEY", None)
+api_url = os.getenv("GENAI_API", None)
+creds = Credentials(api_key, api_endpoint=api_url)
+
+print("======= List of all available models =======")
+for m in Model.models(credentials=creds):
+    print(m)
+
+print("====== Checking availability of a specific model =======")
+model_id = "<string-id-of-model>"
+model = Model(model_id, params=None, credentials=creds)
+print(f"Model availability for {model_id}: {model.available()}")
+
+print("====== Display model card =======")
+model = Model(model_id, params=None, credentials=creds)
+model_info = model.info()
+print(f"Model info for {model_id}: \n{model_info}")
+print(f"Extract fields from model card (e.g., token_limit): {model_info.token_limit}")
+```
+
 ### <a name='EnablingLogs'></a>Enabling Logs
 
 If you're building an application or example and would like to see the GENAI logs, you can enable them in the following way:
 
 ```python
 import logging
 import os
@@ -219,14 +254,15 @@
 
 To learn more about logging in python, you can follow the tutorial [here](https://docs.python.org/3/howto/logging.html).
 
 ### <a name='ManyPrompts'></a>Experimenting with a Large Number of Prompts
 
 Since generating responses for a large number of prompts can be time-consuming and there could be unforeseen circumstances such as internet connectivity issues, here are some strategies
 to work with:
+
 - Start with a small number of prompts to prototype the code. You can enable logging as described above for debugging during prototyping.
 - Include exception handling in sensitive sections such as callbacks.
 - Checkpoint/save prompts and received responses periodically.
 - Check examples in `examples/user` directory and modify them for your needs.
 
 ```python
 def my_callback(result):
@@ -253,18 +289,21 @@
 
 GenAI currently supports a langchain extension and more extensions are in the pipeline. Please reach out to
 us if you want support for some framework as an extension or want to design an extension yourself.
 
 ### <a name='LangChainExtension'></a>LangChain Extension
 
 Install the langchain extension as follows:
+
 ```bash
 pip install "ibm-generative-ai[langchain]"
 ```
+
 Currently the langchain extension allows IBM Generative AI models to be wrapped as Langchain LLMs and translation between genai PromptPatterns and LangChain PromptTemplates. Below are sample snippets
+
 ```python
 import os
 from dotenv import load_dotenv
 import genai.extensions.langchain
 from genai.extensions.langchain import LangChainInterface
 from genai.schemas import GenerateParams
 from genai import Credentials, Model, PromptPattern
@@ -288,17 +327,10 @@
 template = seed_pattern.langchain.as_template()
 pattern = PromptPattern.langchain.from_template(template)
 
 print(langchain_model(template.format(question="What is life?")))
 print(genai_model.generate([pattern.sub("question", "What is life?")])[0].generated_text)
 ```
 
-## <a name='[Deprecated] Model Types'></a>[Deprecated] Model Types
-
-Model types can be imported from the [ModelType class](src/genai/schemas/models.py). If you want to use a model that is not included in this class, you can pass it as a string as exemplified [here](src/genai/schemas/models.py).
-
-Models can be selected by passing their string id to the Model class as exemplified [here](src/genai/schemas/models.py).
-
-
 ## <a name='Support'></a>Support
 
 Need help? Check out how to get [support](SUPPORT.md)
```

### Comparing `ibm-generative-ai-0.2.2/LICENSE` & `ibm-generative-ai-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/PKG-INFO` & `ibm-generative-ai-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.2.2
+Version: 0.2.3
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>, Ja Young Lee <younglee@ibm.com>, Adriana Meza Soria <adriana.meza.soria@ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
```

### Comparing `ibm-generative-ai-0.2.2/README.md` & `ibm-generative-ai-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/STARTER_TEAM.md` & `ibm-generative-ai-0.2.3/STARTER_TEAM.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/SUPPORT.md` & `ibm-generative-ai-0.2.3/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/assets/pull_request_from_fork_to_base.png` & `ibm-generative-ai-0.2.3/documentation/assets/pull_request_from_fork_to_base.png`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/Makefile` & `ibm-generative-ai-0.2.3/documentation/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/make.bat` & `ibm-generative-ai-0.2.3/documentation/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/_templates/custom_landing_page.html` & `ibm-generative-ai-0.2.3/documentation/docs/source/_templates/custom_landing_page.html`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/conf.py` & `ibm-generative-ai-0.2.3/documentation/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/index.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/async.examples.user.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/async.examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/examples.user.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/extensions.user.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/extensions.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/prompts.user.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/prompts.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/local_server.rst` & `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/local_server.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/dev/async-flaky-request-handler.py` & `ibm-generative-ai-0.2.3/examples/dev/async-flaky-request-handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import random
 
 import httpx
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType, TokenParams
+from genai.schemas import GenerateParams, TokenParams
 from genai.services.connection_manager import ConnectionManager
 from genai.services.request_handler import RequestHandler
 
 logging.basicConfig(level="ERROR")
 
 
 class FlakyRequestHandler(RequestHandler):
@@ -76,11 +76,11 @@
 
 
 # Instantiate parameters for text generation
 generate_params = GenerateParams(decoding_method="sample", max_new_tokens=5, min_new_tokens=1)
 tokenize_params = TokenParams(return_tokens=True)
 
 
-flan_ul2 = Model(ModelType.FLAN_UL2, params=generate_params, credentials=creds)
+flan_ul2 = Model("google/flan-ul2", params=generate_params, credentials=creds)
 prompts = ["Generate a random number > {}: ".format(i) for i in range(25)]
 for response in flan_ul2.generate_async(prompts, ordered=True):
     pass
```

### Comparing `ibm-generative-ai-0.2.2/examples/dev/async-flaky-responses-ordered.py` & `ibm-generative-ai-0.2.3/examples/dev/async-flaky-responses-ordered.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 import random
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, GenAiException, Model
-from genai.schemas import GenerateParams, ModelType, TokenParams
+from genai.schemas import GenerateParams, TokenParams
 from genai.services.async_generator import AsyncResponseGenerator
 
 num_requests = 0
 
 
 class FlakyAsyncResponseGenerator(AsyncResponseGenerator):
     async def _get_response_json(self, model, inputs, params, options):
@@ -79,29 +79,29 @@
 
 
 # Instantiate parameters for text generation
 generate_params = GenerateParams(decoding_method="sample", max_new_tokens=5, min_new_tokens=1)
 tokenize_params = TokenParams(return_tokens=True)
 
 
-flan_ul2 = FlakyModel(ModelType.FLAN_UL2_20B, params=generate_params, credentials=creds)
+flan_ul2 = FlakyModel("google/flan-ul2", params=generate_params, credentials=creds)
 prompts = ["Generate a random number > {}: ".format(i) for i in range(17)]
 print("======== Async Generate with ordered=True ======== ")
 counter = 0
 for response in flan_ul2.generate_async(prompts, ordered=True):
     counter += 1
     if response is not None:
         print(counter, ":", response.input_text, " --> ", response.generated_text)
     else:
         print(counter, ":", None)
 
 num_requests = 0
 
 # Instantiate a model proxy object to send your requests
-flan_ul2 = FlakyModel(ModelType.FLAN_UL2_20B, params=tokenize_params, credentials=creds)
+flan_ul2 = FlakyModel("google/flan-ul2", params=tokenize_params, credentials=creds)
 prompts = ["Generate a random number > {}: ".format(i) for i in range(23)]
 print("======== Async Tokenize with ordered=True ======== ")
 counter = 0
 for response in flan_ul2.tokenize_async(prompts, ordered=True):
     counter += 1
     if response is not None:
         print(counter, ":", response.input_text, " --> ", response.tokens)
```

### Comparing `ibm-generative-ai-0.2.2/examples/dev/generate-all-models.py` & `ibm-generative-ai-0.2.3/examples/dev/generate-all-models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 creds = Credentials(api_key)  # credentials object to access GENAI
 
@@ -20,14 +20,15 @@
     " value does not yield to iterating over all the unique symbols,"
     " rather it represents all the symbols mapping to a single value"
     " by a single symbol during iteration. For example, if there are"
     " three symbols symb1, symb2, symb3 mapping to one value then"
     " during iteration it will do symb1 symb1 symb1 due to how it"
     " maps internally. ===="
 )
-for key, modelid in ModelType.__members__.items():
+for model_card in Model.models(credentials=creds):
+    modelid = model_card.id
     model = Model(modelid, params=params, credentials=creds)
     responses = [response.generated_text for response in model.generate(prompts)]
     print(modelid, ":", responses)
     model = Model(modelid.value, params=params, credentials=creds)
     responses = [response.generated_text for response in model.generate(prompts)]
     print(modelid.value, ":", responses)
```

### Comparing `ibm-generative-ai-0.2.2/examples/dev/history-async.py` & `ibm-generative-ai-0.2.3/examples/dev/history-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/dev/logging_example.py` & `ibm-generative-ai-0.2.3/examples/dev/logging_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 logging.basicConfig(level=logging.INFO)
 
 # Most GEN-ai logs are at Debug level, so you can specifically enable
 # or change the genai logging level here
 logging.getLogger("genai").setLevel(logging.DEBUG)
 
@@ -18,12 +18,12 @@
 api_key = os.getenv("GENAI_KEY", None)
 creds = Credentials(api_key)  # credentials object to access GENAI
 
 # Instantiate parameters for text generation
 params = GenerateParams(decoding_method="sample", max_new_tokens=10)
 
 # Instantiate a model proxy object to send your requests
-flan_ul2 = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+flan_ul2 = Model("google/flan-ul2", params=params, credentials=creds)
 
 prompts = ["Hello! How are you?", "How's the weather?"]
 for response in flan_ul2.generate_async(prompts):
     print(f"Prompt: {response.input_text}\nResponse: {response.generated_text}")
```

### Comparing `ibm-generative-ai-0.2.2/examples/user/alice_bob_qa.py` & `ibm-generative-ai-0.2.3/examples/user/alice_bob_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/alice_bob_talk.py` & `ibm-generative-ai-0.2.3/examples/user/alice_bob_talk.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/assets/penguins.csv` & `ibm-generative-ai-0.2.3/examples/user/assets/penguins.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/assets/penguins2.csv` & `ibm-generative-ai-0.2.3/examples/user/assets/penguins2.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.json` & `ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.jsonl` & `ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/async_callback.py` & `ibm-generative-ai-0.2.3/examples/user/async_callback.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/async_greetings.py` & `ibm-generative-ai-0.2.3/examples/user/async_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/async_ordered.py` & `ibm-generative-ai-0.2.3/examples/user/async_ordered.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/async_tokenize.py` & `ibm-generative-ai-0.2.3/examples/user/async_tokenize.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/complete_my_code.py` & `ibm-generative-ai-0.2.3/examples/user/complete_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/country-capital-qa.py` & `ibm-generative-ai-0.2.3/examples/user/country-capital-qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/explain_my_code.py` & `ibm-generative-ai-0.2.3/examples/user/explain_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/generate_with_input_text.py` & `ibm-generative-ai-0.2.3/examples/user/generate_with_input_text.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/gpt_chat_bash.py` & `ibm-generative-ai-0.2.3/examples/user/gpt_chat_bash.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/grid_search_params.py` & `ibm-generative-ai-0.2.3/examples/user/grid_search_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/grid_search_params_greeating.py` & `ibm-generative-ai-0.2.3/examples/user/grid_search_params_greeating.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/history.py` & `ibm-generative-ai-0.2.3/examples/user/history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/jsonprompt.py` & `ibm-generative-ai-0.2.3/examples/user/jsonprompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/jsonprompt_multi.py` & `ibm-generative-ai-0.2.3/examples/user/jsonprompt_multi.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/langchain_qa.py` & `ibm-generative-ai-0.2.3/examples/user/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/localserver/localserver.py` & `ibm-generative-ai-0.2.3/examples/user/localserver/localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/logprob_returns.py` & `ibm-generative-ai-0.2.3/examples/user/logprob_returns.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/many_greetings.py` & `ibm-generative-ai-0.2.3/examples/user/many_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/model_as_string.py` & `ibm-generative-ai-0.2.3/examples/user/model_as_string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt-raw-string.py` & `ibm-generative-ai-0.2.3/examples/user/prompt-raw-string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_csv_random_rows.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_csv_random_rows.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_from_all_csv.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_from_all_csv.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_from_all_dataframe.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_from_all_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_from_dataframe.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_from_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_reuse.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_reuse.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-output.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import os
+import pathlib
 
 from dotenv import load_dotenv
 
-from genai.model import Credentials, Model
+from genai.credentials import Credentials
+from genai.model import Model
+from genai.options import Options
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_url = os.getenv("GENAI_API", None)
+PATH = pathlib.Path(__file__).parent.resolve()
 
 creds = Credentials(api_key, api_endpoint=api_url)
 params = GenerateParams(temperature=0.5)
 
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 _template = """
 {{instruction}}
 
 {{#list}}
 
@@ -32,21 +36,27 @@
 """
 
 print("\n------------- Mustaches Prompt Template -------------\n")
 pt = PromptPattern.from_watsonx(credentials=creds, name="list-qa-airport-3", template=_template)
 print(f"\nPrompt: {pt}")
 
 
-print("\n------------- Rendered Prompt -------------\n")
+print("\n------------- Response -------------\n")
+options = Options(
+    watsonx_template=pt,
+    watsonx_data={
+        "instruction": "blaahh",
+        "list": [
+            {"country": "Canada", "capital": "Ottawa", "airport": "YOW"},
+            {"country": "Germany", "capital": "Berlin", "airport": "BER"},
+            {"country": "USA", "capital": "Washington", "airport": "DCA"},
+        ],
+    },
+)
+
 inputs = ["Spain", "Finland", "Iraq", "India", "Bangladesh"]
-data = {
-    "list": [
-        {"country": "Canada", "capital": "Ottawa", "airport": "YOW"},
-        {"country": "Germany", "capital": "Berlin", "airport": "BER"},
-        {"country": "USA", "capital": "Washington", "airport": "DCA"},
-    ]
-}
-
-rendered_prompts = pt.render(inputs=inputs, data=data)
-for pt in rendered_prompts:
-    print(pt)
-    print("- - - - ")
+for resp in model.generate_async(inputs * 10, options=options, hide_progressbar=True):
+    print(f"\nCountry: {resp.input_text} \n{resp.generated_text}")
+
+
+for resp in model.tokenize_async(inputs, options=options, return_tokens=True):
+    print(resp)
```

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 import pathlib
 
 from dotenv import load_dotenv
 
-from genai.model import Credentials, Model
+from genai.credentials import Credentials
+from genai.model import Model
 from genai.options import Options
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_url = os.getenv("GENAI_API", None)
 PATH = pathlib.Path(__file__).parent.resolve()
 
 creds = Credentials(api_key, api_endpoint=api_url)
 params = GenerateParams(temperature=0.5)
 
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 _template = """
 {{instruction}}
 
 {{#list}}
 
@@ -48,14 +49,11 @@
             {"country": "Canada", "capital": "Ottawa", "airport": "YOW"},
             {"country": "Germany", "capital": "Berlin", "airport": "BER"},
             {"country": "USA", "capital": "Washington", "airport": "DCA"},
         ],
     },
 )
 
-inputs = ["Spain", "Finland", "Iraq", "India", "Bangladesh"]
-for resp in model.generate_async(inputs * 10, options=options, hide_progressbar=True):
-    print(f"\nCountry: {resp.input_text} \n{resp.generated_text}")
-
 
-for resp in model.tokenize_async(inputs, options=options, return_tokens=True):
-    print(resp)
+responses = model.generate_as_completed(["Spain", "Finland", "Iraq", "India", "Bangladesh"], options=options)
+for resp in responses:
+    print(f"\nCountry: {resp.input_text} \n{resp.generated_text}")
```

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import os
-import pathlib
 
 from dotenv import load_dotenv
 
-from genai.model import Credentials, Model
-from genai.options import Options
+from genai.credentials import Credentials
+from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_url = os.getenv("GENAI_API", None)
-PATH = pathlib.Path(__file__).parent.resolve()
 
 creds = Credentials(api_key, api_endpoint=api_url)
 params = GenerateParams(temperature=0.5)
 
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 _template = """
 {{instruction}}
 
 {{#list}}
 
@@ -35,24 +33,21 @@
 """
 
 print("\n------------- Mustaches Prompt Template -------------\n")
 pt = PromptPattern.from_watsonx(credentials=creds, name="list-qa-airport-3", template=_template)
 print(f"\nPrompt: {pt}")
 
 
-print("\n------------- Response -------------\n")
-options = Options(
-    watsonx_template=pt,
-    watsonx_data={
-        "instruction": "blaahh",
-        "list": [
-            {"country": "Canada", "capital": "Ottawa", "airport": "YOW"},
-            {"country": "Germany", "capital": "Berlin", "airport": "BER"},
-            {"country": "USA", "capital": "Washington", "airport": "DCA"},
-        ],
-    },
-)
-
-
-responses = model.generate_as_completed(["Spain", "Finland", "Iraq", "India", "Bangladesh"], options=options)
-for resp in responses:
-    print(f"\nCountry: {resp.input_text} \n{resp.generated_text}")
+print("\n------------- Rendered Prompt -------------\n")
+inputs = ["Spain", "Finland", "Iraq", "India", "Bangladesh"]
+data = {
+    "list": [
+        {"country": "Canada", "capital": "Ottawa", "airport": "YOW"},
+        {"country": "Germany", "capital": "Berlin", "airport": "BER"},
+        {"country": "USA", "capital": "Washington", "airport": "DCA"},
+    ]
+}
+
+rendered_prompts = pt.render(inputs=inputs, data=data)
+for pt in rendered_prompts:
+    print(pt)
+    print("- - - - ")
```

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-templating.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-templating.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/classification.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,34 +106,46 @@
         print(status)
         time.sleep(20)
         status = tuned_model.status()
     else:
         if status in ["FAILED", "HALTED"]:
             print("Model tuning failed or halted")
         else:
+            print("Model info:\n")
+            print(tuned_model.info())
+            time.sleep(5)
+
             prompt = input("Enter a prompt:\n")
             genparams = GenerateParams(
                 decoding_method="greedy",
                 max_new_tokens=50,
                 min_new_tokens=1,
             )
             print("Answer = ", tuned_model.generate([prompt])[0].generated_text)
+            time.sleep(5)
+
+            print("~~~~~~~ List of all models ~~~~~~")
+            for m in Model.models(credentials=creds):
+                print(m, "\n")
+            time.sleep(10)
 
-            print("~~~~~~~ Listing tunes and getting tune metadata with TuneManager ~~~~~")
+            print("~~~~~~~ Getting list of all tuned models with TuneManager ~~~~~")
 
-            list_params = TunesListParams(limit=5, offset=0)
+            list_params = TunesListParams(limit=50, offset=0)
 
             tune_list = TuneManager.list_tunes(credentials=creds, params=list_params)
             print("\n\nList of tunes: \n\n")
             for tune in tune_list.results:
                 print(tune, "\n")
+            time.sleep(10)
 
             tune_get_result = TuneManager.get_tune(credentials=creds, tune_id=tuned_model.model)
             print(
                 "\n\n~~~~~ Metadata for a single tune with TuneManager ~~~~: \n\n",
                 tune_get_result,
             )
+            time.sleep(5)
 
             print("~~~~~~~ Deleting a tuned model ~~~~~")
             to_delete = input("Delete this model? (y/N):\n")
             if to_delete == "y":
                 tuned_model.delete()
```

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/file_to_tune.jsonl` & `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/file_to_tune.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/files_manager.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/files_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/summarization.py` & `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/summarization.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py` & `ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py` & `ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/saving_prompts_as_hf_dataset.py` & `ibm-generative-ai-0.2.3/examples/user/saving_prompts_as_hf_dataset.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/self-reflection.py` & `ibm-generative-ai-0.2.3/examples/user/self-reflection.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/self_instruct.py` & `ibm-generative-ai-0.2.3/examples/user/self_instruct.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/streaming.py` & `ibm-generative-ai-0.2.3/examples/user/streaming.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/tokenize-sync.py` & `ibm-generative-ai-0.2.3/examples/user/tokenize-sync.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/examples/user/tokens.py` & `ibm-generative-ai-0.2.3/examples/user/tokens.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/pyproject.toml` & `ibm-generative-ai-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/credentials.py` & `ibm-generative-ai-0.2.3/src/genai/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/exceptions/genai_exception.py` & `ibm-generative-ai-0.2.3/src/genai/exceptions/genai_exception.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/save_huggingface.py` & `ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/extensions/langchain/llm.py` & `ibm-generative-ai-0.2.3/src/genai/extensions/langchain/llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Wrapper around IBM GENAI APIs for use in langchain"""
 import logging
-from typing import Any, List, Mapping, Optional, Union
+from typing import Any, List, Mapping, Optional
 
 from pydantic import BaseModel, Extra
 
 try:
     from langchain.llms.base import LLM
     from langchain.llms.utils import enforce_stop_tokens
 except ImportError:
     raise ImportError("Could not import langchain: Please install ibm-generative-ai[langchain] extension.")
 
 from genai import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["LangChainInterface"]
 
 
 class LangChainInterface(LLM, BaseModel):
@@ -24,19 +24,19 @@
     To use, you should have the ``genai`` python package installed
     and initialize the credentials attribute of this class with
     an instance of ``genai.Credentials``. Model specific parameters
     can be passed through to the constructor using the ``params``
     parameter, which is an instance of GenerateParams.
     Example:
         .. code-block:: python
-            llm = LangChainInterface(model=ModelType.FLAN_UL2, credentials=creds)
+            llm = LangChainInterface(model="google/flan-ul2", credentials=creds)
     """
 
     credentials: Credentials = None
-    model: Optional[Union[ModelType, str]] = None
+    model: Optional[str] = None
     params: Optional[GenerateParams] = None
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
 
@@ -59,15 +59,15 @@
         Args:
             prompt: The prompt to pass into the model.
             stop: Optional list of stop words to use when generating.
         Returns:
             The string generated by the model.
         Example:
             .. code-block:: python
-                llm = LangChainInterface(model_id=ModelType.FLAN_UL2, credentials=creds)
+                llm = LangChainInterface(model_id="google/flan-ul2", credentials=creds)
                 response = llm("What is a molecule")
         """
         params = self.params or GenerateParams()
         model = Model(model=self.model, params=params, credentials=self.credentials)
         text = model.generate(prompts=[prompt])[0].generated_text
         logger.info("Output of GENAI call: {}".format(text))
         if stop is not None:
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/extensions/langchain/prompt.py` & `ibm-generative-ai-0.2.3/src/genai/extensions/langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/extensions/localserver/custom_model_interface.py` & `ibm-generative-ai-0.2.3/src/genai/extensions/localserver/custom_model_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/extensions/localserver/local_api_server.py` & `ibm-generative-ai-0.2.3/src/genai/extensions/localserver/local_api_server.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/extensions/pandas/prompt_sub.py` & `ibm-generative-ai-0.2.3/src/genai/extensions/pandas/prompt_sub.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/metadata.py` & `ibm-generative-ai-0.2.3/src/genai/metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/model.py` & `ibm-generative-ai-0.2.3/src/genai/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,46 +6,50 @@
 from tqdm import tqdm
 
 from genai.credentials import Credentials
 from genai.exceptions import GenAiException
 from genai.metadata import Metadata
 from genai.options import Options
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType, TokenParams
+from genai.schemas import GenerateParams, TokenParams
 from genai.schemas.responses import (
     GenerateResponse,
     GenerateResult,
     GenerateStreamResponse,
+    ModelCard,
+    ModelList,
     TokenizeResponse,
     TokenizeResult,
+    TuneGetResponse,
 )
 from genai.schemas.tunes_params import (
     CreateTuneHyperParams,
     CreateTuneParams,
     TunesListParams,
 )
 from genai.services import AsyncResponseGenerator, ServiceInterface
 from genai.services.tune_manager import TuneManager
+from genai.utils.service_utils import _get_service
 
 logger = logging.getLogger(__name__)
 
 
 class Model:
     _accessors = set()
 
     def __init__(
         self,
-        model: Union[ModelType, str],
+        model: str,
         params: Union[GenerateParams, TokenParams, Any] = None,
         credentials: Credentials = None,
     ):
         """Instantiates the Model Interface
 
         Args:
-            model (Union[ModelType, str]): The type of model to use
+            model (str): The type of model to use
             params (Union[GenerateParams, TokenParams]): Parameters to use during generate requests
             credentials (Credentials): The API Credentials
         """
         logger.debug(f"Model Created:  Model: {model}, endpoint: {credentials.api_endpoint}")
         self.model = model
         self.params = params
         self.creds = credentials
@@ -342,27 +346,58 @@
             training_file_ids=training_file_ids,
             validation_file_ids=validation_file_ids,
             parameters=hyperparameters or CreateTuneHyperParams(),
         )
         tune = TuneManager.create_tune(service=self.service, params=params)
         return Model(model=tune.id, params=None, credentials=self.creds)
 
-    def status(self):
-        """Get status of the model, currently supports only tuned models.
+    def status(self) -> TuneGetResponse:
+        """Get status of a tuned model.
 
         Returns:
             str: Status of a tuned model
         """
-        params = TunesListParams()
-        tunes = TuneManager.list_tunes(service=self.service, params=params).results
-        id_to_status = {t.id: t.status for t in tunes}
-        if self.model not in id_to_status:
-            raise GenAiException(ValueError("Tuned model not found. Currently method supports only tuned models."))
-        return id_to_status[self.model]
+        tune = TuneManager.get_tune(tune_id=self.model, service=self.service)
+        return tune.status
 
     def delete(self):
         params = TunesListParams()
         tunes = TuneManager.list_tunes(service=self.service, params=params).results
         id_to_status = {t.id: t.status for t in tunes}
         if self.model not in id_to_status:
             raise GenAiException(ValueError("Tuned model not found. Currently method supports only tuned models."))
         TuneManager.delete_tune(service=self.service, tune_id=self.model)
+
+    @staticmethod
+    def models(credentials: Credentials = None, service: ServiceInterface = None) -> list[ModelCard]:
+        """Get a list of models
+
+        Args:
+            credentials (Credentials): Credentials
+            service (ServiceInterface): Service Interface
+
+        Returns:
+            list[ModelCard]: A list of available models
+        """
+        service = _get_service(credentials, service)
+        response = service.models()
+        cards = ModelList(**response.json()).results
+        return cards
+
+    def available(self) -> bool:
+        """Check if the model is available. Note that for tuned models
+        the model could still be in the process of tuning.
+
+        Returns:
+            bool: Boolean indicating model availability
+        """
+        idset = set(m.id for m in Model.models(service=self.service))
+        return self.model in idset
+
+    def info(self) -> Union[ModelCard, None]:
+        """Get info of the model
+
+        Returns:
+            Union[ModelCard, TuneInfoResult, None]: Model info
+        """
+        id_to_model = {m.id: m for m in Model.models(service=self.service)}
+        return id_to_model.get(self.model, None)
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/prompt_pattern.py` & `ibm-generative-ai-0.2.3/src/genai/prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/routers/files.py` & `ibm-generative-ai-0.2.3/src/genai/routers/files.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/routers/prompt_template.py` & `ibm-generative-ai-0.2.3/src/genai/routers/prompt_template.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/routers/tunes.py` & `ibm-generative-ai-0.2.3/src/genai/routers/tunes.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/schemas/__init__.py` & `ibm-generative-ai-0.2.3/src/genai/schemas/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from genai.schemas.generate_params import (
     GenerateParams,
     LengthPenalty,
     Return,
     ReturnOptions,
 )
 from genai.schemas.history_params import HistoryParams
-from genai.schemas.models import ModelType
 from genai.schemas.responses import GenerateResult, TokenizeResult
 from genai.schemas.token_params import TokenParams
 from genai.schemas.tunes_params import (
     CreateTuneHyperParams,
     CreateTuneParams,
     TunesListParams,
 )
@@ -20,15 +19,14 @@
     "Descriptions",
     "GenerateParams",
     "LengthPenalty",
     "Return",
     "ReturnOptions",
     "TokenParams",
     "HistoryParams",
-    "ModelType",
     "GenerateResult",
     "TokenizeResult",
     "FileListParams",
     "MultipartFormData",
     "TunesListParams",
     "CreateTuneParams",
     "CreateTuneHyperParams",
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/schemas/descriptions.py` & `ibm-generative-ai-0.2.3/src/genai/schemas/descriptions.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/schemas/files_params.py` & `ibm-generative-ai-0.2.3/src/genai/schemas/files_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/schemas/generate_params.py` & `ibm-generative-ai-0.2.3/src/genai/schemas/generate_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 # Fix       : We created a "returns" attribute which gets mapped to the "return"
 #             dictionary key in the sanitize method of ServiceInterface.
 # Link to doc : https://workbench.res.ibm.com/docs/api-reference#generate
 
 
 class GenerateParams(BaseModel):
     class Config:
-        anystr_strip_whitespace: True
-        extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.allow
         allow_population_by_field_name = True
 
     decoding_method: Optional[Literal["greedy", "sample"]] = Field(None, description=tx.DECODING_METHOD)
     length_penalty: Optional[LengthPenalty] = Field(None, description=tx.LENGTH_PENALTY)
     max_new_tokens: Optional[int] = Field(None, description=tx.MAX_NEW_TOKEN)
     min_new_tokens: Optional[int] = Field(None, description=tx.MIN_NEW_TOKEN)
     random_seed: Optional[int] = Field(None, description=tx.RANDOM_SEED, ge=1, le=9999)
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/schemas/history_params.py` & `ibm-generative-ai-0.2.3/src/genai/schemas/history_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/schemas/responses.py` & `ibm-generative-ai-0.2.3/src/genai/schemas/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from datetime import datetime
 from enum import Enum
 from typing import Any, List, Optional, Union
 
 from pydantic import BaseModel, Extra, root_validator
 
 from genai.schemas.generate_params import GenerateParams
-from genai.schemas.models import ModelType
 
 logger = logging.getLogger(__name__)
 
 
 class StopReasonEnum(str, Enum):
     NOT_FINISHED = "Possibly more tokens to be streamed"
     MAX_TOKENS = "Maximum requested tokens reached"
@@ -72,15 +71,15 @@
     stop_reason: str
     generated_tokens: Optional[list[GeneratedToken]]
     input_text: Optional[str]
     seed: Optional[int]
 
 
 class GenerateResponse(GenAiResponseModel):
-    model_id: Union[ModelType, str]
+    model_id: str
     created_at: datetime
     results: List[GenerateResult]
 
 
 class GenerateStreamResponse(GenAiResponseModel):
     generated_text: Optional[str]
     generated_token_count: Optional[int]
@@ -94,15 +93,15 @@
 class TokenizeResult(GenAiResponseModel):
     token_count: Optional[int]
     tokens: Optional[List[str]]
     input_text: Optional[str]
 
 
 class TokenizeResponse(GenAiResponseModel):
-    model_id: Union[ModelType, str]
+    model_id: str
     created_at: datetime
     results: List[TokenizeResult]
 
 
 class HistoryResultRequest(GenAiResponseModel):
     inputs: list[str]
     model_id: str
@@ -223,7 +222,19 @@
     id: str
     file_name: str
     created_at: str
 
 
 class TuneGetResponse(GenAiResponseModel):
     results: Optional[TuneInfoResult]
+
+
+class ModelCard(GenAiResponseModel):
+    id: Optional[str]
+    name: Optional[str]
+    size: Optional[str]
+    source_model_id: Optional[str]
+    token_limit: Optional[Union[int, Any]]
+
+
+class ModelList(GenAiResponseModel):
+    results: list[ModelCard]
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/schemas/tunes_params.py` & `ibm-generative-ai-0.2.3/src/genai/schemas/tunes_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/__init__.py` & `ibm-generative-ai-0.2.3/src/genai/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/async_generator.py` & `ibm-generative-ai-0.2.3/src/genai/services/async_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class AsyncResponseGenerator:
     def __init__(
         self, model_id, prompts, params, service, fn="generate", ordered=False, callback=None, options: Options = None
     ):
         """Instantiates the ConcurrentWrapper Interface.
 
         Args:
-            model_id (ModelType): The type of model to use
+            model_id (str): The type of model to use
             prompts (list): List of prompts
             params (GenerateParams): Parameters to use during generate requests
             service (ServiceInterface): The service interface
             fn (Literal["generate", "tokenize"]): Function to call from service
             callback (Callable[[GenerateResult], Any]): callback to execute once a prompt is successfully received.
         """
         self.model_id = model_id
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/connection_manager.py` & `ibm-generative-ai-0.2.3/src/genai/services/connection_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/file_manager.py` & `ibm-generative-ai-0.2.3/src/genai/services/file_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/prompt_template_manager.py` & `ibm-generative-ai-0.2.3/src/genai/services/prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/request_handler.py` & `ibm-generative-ai-0.2.3/src/genai/services/request_handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/service_interface.py` & `ibm-generative-ai-0.2.3/src/genai/services/service_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from httpx import Response
+from httpx import ConnectError, Response
 
 from genai.exceptions import GenAiException
 from genai.options import Options
 from genai.routers import FilesRouter, PromptTemplateRouter, TunesRouter
 from genai.schemas import GenerateParams, HistoryParams, TokenParams
 from genai.services import RequestHandler
 from genai.utils.request_utils import sanitize_params
 
+__all__ = ["ServiceInterface"]
+
 
 class ServiceInterface:
     GENERATE = "/generate"
     TOKENIZE = "/tokenize"
     HISTORY = "/requests"
     TOU = "/user"
+    MODELS = "/models"
 
     def __init__(self, service_url: str, api_key: str) -> None:
         """Initialize ServiceInterface.
 
         Args:
             service_url (str): Base URL for querying.
             api_key (str): User API key for authorization.
@@ -24,14 +27,30 @@
         """
         self.service_url = service_url.rstrip("/")
         self.key = api_key
         self._prompt_templating = PromptTemplateRouter(service_url=service_url, api_key=api_key)
         self._files = FilesRouter(service_url=service_url, api_key=api_key)
         self._tunes = TunesRouter(service_url=service_url, api_key=api_key)
 
+    def models(self):
+        """Generate a completion text for the given model, inputs, and params.
+
+        Returns:
+            Any: json from querying for text completion.
+        """
+        try:
+            endpoint = self.service_url + ServiceInterface.MODELS
+            return RequestHandler.get(endpoint, key=self.key)
+        except ConnectError as e:
+            raise GenAiException(
+                Exception("Endpoint unreachable. Please check connectivity.\nRaw error message = {}".format(e))
+            )
+        except Exception as e:
+            raise GenAiException(e)
+
     def generate(
         self, model: str, inputs: list, params: GenerateParams = None, streaming: bool = False, options: Options = None
     ):
         """Generate a completion text for the given model, inputs, and params.
 
         Args:
             model (str): Model id.
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/services/tune_manager.py` & `ibm-generative-ai-0.2.3/src/genai/services/tune_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             tune_id: ID of the tune to fetch from the server.
             credentials (Credentials, optional): Credentials object. Defaults to None.
                 If not providec, service must be provided.
             service (ServiceInterface, optional): ServiceInterface object. Defaults to None.
                 If not provided, credentials must be provided.
 
         Returns:
-            TuneGetResponse: Response from the server.
+            TuneInfoResult: Response from the server.
         """
         service = _get_service(credentials, service)
         try:
             response = service._tunes.get_tune(tune_id=tune_id)
             if response.status_code == 200:
                 response = response.json()
                 responses = TuneGetResponse(**response)
```

### Comparing `ibm-generative-ai-0.2.2/src/genai/utils/extensions.py` & `ibm-generative-ai-0.2.3/src/genai/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/utils/json_utils.py` & `ibm-generative-ai-0.2.3/src/genai/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/utils/search_space_params.py` & `ibm-generative-ai-0.2.3/src/genai/utils/search_space_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/genai/utils/service_utils.py` & `ibm-generative-ai-0.2.3/src/genai/utils/service_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/PKG-INFO` & `ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.2.2
+Version: 0.2.3
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>, Ja Young Lee <younglee@ibm.com>, Adriana Meza Soria <adriana.meza.soria@ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
```

### Comparing `ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/SOURCES.txt` & `ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 CONTRIBUTING.md
 EXTENSIONS.md
 GETTING_STARTED.md
 LICENSE
 README.md
 STARTER_TEAM.md
 SUPPORT.md
-innersource.yaml
 pyproject.toml
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/01_bug_report.md
 .github/ISSUE_TEMPLATE/02_feature_request.md
 .github/ISSUE_TEMPLATE/03_documentation_update.md
 .github/ISSUE_TEMPLATE/config.yaml
 .github/workflows/documentation.yml
@@ -41,15 +40,14 @@
 documentation/docs/source/rst_source/genai.prompt.quickstart.rst
 documentation/docs/source/rst_source/genai.prompt.rst
 documentation/docs/source/rst_source/genai.rst
 documentation/docs/source/rst_source/genai.schemas.descriptions.rst
 documentation/docs/source/rst_source/genai.schemas.files_params.rst
 documentation/docs/source/rst_source/genai.schemas.generate_params.rst
 documentation/docs/source/rst_source/genai.schemas.history_params.rst
-documentation/docs/source/rst_source/genai.schemas.models.rst
 documentation/docs/source/rst_source/genai.schemas.responses.rst
 documentation/docs/source/rst_source/genai.schemas.rst
 documentation/docs/source/rst_source/genai.schemas.token_params.rst
 documentation/docs/source/rst_source/genai.schemas.tunes_params.rst
 documentation/docs/source/rst_source/genai.services.request_handler.rst
 documentation/docs/source/rst_source/genai.services.rst
 documentation/docs/source/rst_source/genai.services.service_interface.rst
@@ -85,14 +83,15 @@
 examples/user/history.py
 examples/user/jsonprompt.py
 examples/user/jsonprompt_multi.py
 examples/user/langchain_qa.py
 examples/user/logprob_returns.py
 examples/user/many_greetings.py
 examples/user/model_as_string.py
+examples/user/model_utils.py
 examples/user/prompt-raw-string.py
 examples/user/prompt_csv_random_rows.py
 examples/user/prompt_from_all_csv.py
 examples/user/prompt_from_all_dataframe.py
 examples/user/prompt_from_dataframe.py
 examples/user/prompt_reuse.py
 examples/user/saving_prompts_as_hf_dataset.py
@@ -149,15 +148,14 @@
 src/genai/routers/prompt_template.py
 src/genai/routers/tunes.py
 src/genai/schemas/__init__.py
 src/genai/schemas/descriptions.py
 src/genai/schemas/files_params.py
 src/genai/schemas/generate_params.py
 src/genai/schemas/history_params.py
-src/genai/schemas/models.py
 src/genai/schemas/responses.py
 src/genai/schemas/token_params.py
 src/genai/schemas/tunes_params.py
 src/genai/services/__init__.py
 src/genai/services/async_generator.py
 src/genai/services/connection_manager.py
 src/genai/services/file_manager.py
```

### Comparing `ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/requires.txt` & `ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/assets/file_to_tune.json` & `ibm-generative-ai-0.2.3/tests/assets/file_to_tune.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/assets/file_to_tune.jsonl` & `ibm-generative-ai-0.2.3/tests/assets/file_to_tune.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/assets/response_helper.py` & `ibm-generative-ai-0.2.3/tests/assets/response_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -219,14 +219,66 @@
             response = {
                 "results": [results],
                 "totalCount": 1,
             }
         return response
 
     @staticmethod
+    def get_tune(**kwargs):
+        response = {
+            "results": {
+                "id": "google/flan-t5-xl-mpt-oP8G21Dj-2023-04-11-18-11-54",
+                "name": "Tune #1 google/flan-t5-xl (3B)",
+                "model_id": "google/google/flan-t5-xl",
+                "method_id": "mpt",
+                "model_name": "google/flan-t5-xl (3B)",
+                "status_message": "",
+                "task_id": "generation",
+                "status": "COMPLETED",
+                "parameters": {"batch_size": 4, "num_epochs": 12},
+                "created_at": "2023-04-11T18:11:54.000Z",
+                "validation_files": [],
+                "training_files": [
+                    {
+                        "id": "60d54ad5-b9d7-4acb-99d6-870ff31c9222",
+                        "file_name": "file.json",
+                        "created_at": "2023-04-24 10:26:02+02",
+                    }
+                ],
+                "evaluation_files": [],
+                "datapoints": {
+                    "loss": [{"data": {"epoch": 0, "value": 1.9922}, "timestamp": "2023-05-07T09:05:56.000Z"}]
+                },
+            }
+        }
+
+        return response
+
+    @staticmethod
+    def models(**kwargs):
+        return {
+            "results": [
+                {
+                    "id": "google/flan-t5-xl",
+                    "name": "flan-t5-xl (3B)",
+                    "size": "3B",
+                    "source_model_id": None,
+                    "token_limit": 4096,
+                },
+                {
+                    "id": "flan-t5-xl-mpt-XmHNkJWk-2023-07-18-17-00-34",
+                    "name": "flan-t5-xxl (11B)",
+                    "size": "11B",
+                    "source_model_id": "google/flan-t5-xl",
+                    "token_limit": 4096,
+                },
+            ]
+        }
+
+    @staticmethod
     def create_tune(**kwargs):
         model_id = kwargs["model_id"] if "model_id" in kwargs else "google/flan-t5-xxl"
         name = kwargs["name"] if "name" in kwargs else "Tune #2 google/flan-t5-xxl (3B)"
         response = {
             "results": {
                 "id": "google/flan-t5-xxl-mpt-Bok9gSo3-2023-04-11-18-00-57",
                 "name": name,
```

### Comparing `ibm-generative-ai-0.2.2/tests/extensions/test_langchain.py` & `ibm-generative-ai-0.2.3/tests/extensions/test_langchain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from genai import Credentials
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 from genai.schemas.responses import GenerateResponse
 from genai.services import ServiceInterface
 from tests.assets.response_helper import SimpleResponse
 
 
 @pytest.mark.extension
 class TestLangChain:
@@ -28,22 +28,22 @@
     def prompts(self):
         return ["Hi! How's the weather, eh?"]
 
     @patch("genai.services.RequestHandler.post")
     def test_langchain_interface(self, mocked_post_request, credentials, params, prompts):
         from genai.extensions.langchain import LangChainInterface
 
-        GENERATE_RESPONSE = SimpleResponse.generate(model=ModelType.FLAN_UL2, inputs=prompts, params=params)
+        GENERATE_RESPONSE = SimpleResponse.generate(model="google/flan-ul2", inputs=prompts, params=params)
         expected_generated_response = GenerateResponse(**GENERATE_RESPONSE)
 
         response = MagicMock(status_code=200)
         response.json.return_value = GENERATE_RESPONSE
         mocked_post_request.return_value = response
 
-        model = LangChainInterface(model=ModelType.FLAN_UL2, params=params, credentials=credentials)
+        model = LangChainInterface(model="google/flan-ul2", params=params, credentials=credentials)
         observed = model(prompts[0])
         assert observed == expected_generated_response.results[0].generated_text
 
     def test_prompt_translator(self):
         from langchain import PromptTemplate
 
         import genai.extensions.langchain  # noqa
```

### Comparing `ibm-generative-ai-0.2.2/tests/extensions/test_localserver.py` & `ibm-generative-ai-0.2.3/tests/extensions/test_localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/extensions/test_save_huggingface.py` & `ibm-generative-ai-0.2.3/tests/extensions/test_save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/extensions/test_sub_from_pandas.py` & `ibm-generative-ai-0.2.3/tests/extensions/test_sub_from_pandas.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/integration/conftest.py` & `ibm-generative-ai-0.2.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/integration/test_examples.py` & `ibm-generative-ai-0.2.3/tests/integration/test_examples.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_concurrent.py` & `ibm-generative-ai-0.2.3/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_files.py` & `ibm-generative-ai-0.2.3/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_generate_schema.py` & `ibm-generative-ai-0.2.3/tests/test_generate_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,7 +264,14 @@
     def test_truncate_input_tokens_valid_type(self, request_body):
         params = request_body["params"]
         assert isinstance(params.truncate_input_tokens, int)
 
     def test_returns_raises_warning(self):
         with pytest.deprecated_call():
             GenerateParams(returns=Return())
+
+    def test_optional_fields(self):
+        try:
+            genparams = GenerateParams(answer=42)
+            assert genparams.answer == 42
+        except ValidationError as e:
+            assert False, "Extra fields not parsed: {}".format(e)
```

### Comparing `ibm-generative-ai-0.2.2/tests/test_generate_service.py` & `ibm-generative-ai-0.2.3/tests/test_generate_service.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_history.py` & `ibm-generative-ai-0.2.3/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_json_utils.py` & `ibm-generative-ai-0.2.3/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_logging.py` & `ibm-generative-ai-0.2.3/tests/test_logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 
 import pytest
 
 from genai import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 logger = logging.getLogger()
 logger.addHandler(logging.StreamHandler())
 
 
 @pytest.mark.unit
 class TestLogging:
     def test_no_leaked_logs(self, caplog):
         credentials = Credentials("GENAI_API_KEY")
         params = GenerateParams()
-        Model(ModelType.FLAN_UL2, params=params, credentials=credentials)
+        Model("google/flan-ul2", params=params, credentials=credentials)
 
         assert len(caplog.records) == 0
 
     def test_basic_logs(self, caplog):
         caplog.set_level(logging.DEBUG)
 
         credentials = Credentials("GENAI_API_KEY")
         params = GenerateParams()
-        Model(ModelType.FLAN_UL2, params=params, credentials=credentials)
-        # Enums are converted to strings slightly differently across python 3.9, 3.10 and 3.11
-        assert any(x in caplog.text for x in [ModelType.FLAN_UL2, ModelType.FLAN_UL2.value, "ModelType.FLAN_UL2"])
+        Model("google/flan-ul2", params=params, credentials=credentials)
+
+        assert "google/flan-ul2" in caplog.text
```

### Comparing `ibm-generative-ai-0.2.2/tests/test_metadata.py` & `ibm-generative-ai-0.2.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_model.py` & `ibm-generative-ai-0.2.3/tests/test_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from genai import Credentials, Model
 from genai.exceptions import GenAiException
-from genai.schemas import GenerateParams, ModelType
-from genai.schemas.responses import GenerateResponse, TokenizeResponse
+from genai.schemas import GenerateParams
+from genai.schemas.responses import (
+    GenerateResponse,
+    ModelCard,
+    ModelList,
+    TokenizeResponse,
+)
 from genai.schemas.tunes_params import CreateTuneHyperParams
 from genai.services import ServiceInterface
 from tests.assets.response_helper import SimpleResponse
 
 
 @pytest.mark.unit
 class TestModel:
@@ -39,61 +44,61 @@
     def prompts(self):
         return ["a", "b", "c", "d", "e"]
 
     @patch("genai.services.RequestHandler.post")
     def test_generate(self, mocked_post_request, credentials, params, prompts):
         """Tests that we can call the generate endpoint"""
 
-        GENERATE_RESPONSE = SimpleResponse.generate(model=ModelType.FLAN_UL2, inputs=prompts, params=params)
+        GENERATE_RESPONSE = SimpleResponse.generate(model="google/flan-ul2", inputs=prompts, params=params)
         expected_generated_response = GenerateResponse(**GENERATE_RESPONSE)
 
         response = MagicMock(status_code=200)
         response.json.return_value = GENERATE_RESPONSE
         mocked_post_request.return_value = response
 
-        model = Model(ModelType.FLAN_UL2, params=params, credentials=credentials)
+        model = Model("google/flan-ul2", params=params, credentials=credentials)
 
         responses = model.generate_as_completed(prompts=prompts)
         responses_list = list(responses)
 
         assert responses_list == expected_generated_response.results
         for i, response in enumerate(responses_list):
             assert response.input_text == prompts[i]
 
     @patch("genai.services.RequestHandler.post")
     def test_generate_throws_exception_for_non_200(self, mock_service_generate, credentials, params, prompts):
         """Tests that the GenAiException is thrown if the status code is not 200"""
 
         mock_service_generate.return_value = MagicMock(status_code=500)
 
-        model = Model(ModelType.FLAN_UL2, params=params, credentials=credentials)
+        model = Model("google/flan-ul2", params=params, credentials=credentials)
 
         with pytest.raises(GenAiException):
             model.generate(prompts=prompts)
 
     @patch("genai.services.RequestHandler.post", side_effect=Exception("some general error"))
     def test_generate_throws_exception_for_generic_exception(self, credentials, params, prompts):
         """Tests that the GenAiException is thrown if a generic Exception is raised"""
-        model = Model(ModelType.FLAN_UL2, params=params, credentials=credentials)
+        model = Model("google/flan-ul2", params=params, credentials=credentials)
 
         with pytest.raises(GenAiException, match="some general error"):
             model.generate(prompts=prompts)
 
     @patch("genai.services.RequestHandler.post")
     def test_tokenize(self, mocked_post_request, credentials, params):
         """Tests that we can call the tokenize endpoint"""
 
-        TOKENIZE_RESPONSE = SimpleResponse.tokenize(model=ModelType.FLAN_UL2, inputs=["a", "b", "c"])
+        TOKENIZE_RESPONSE = SimpleResponse.tokenize(model="google/flan-ul2", inputs=["a", "b", "c"])
         expected_token_response = TokenizeResponse(**TOKENIZE_RESPONSE)
 
         mock_response = MagicMock(status_code=200)
         mock_response.json.return_value = TOKENIZE_RESPONSE
         mocked_post_request.return_value = mock_response
 
-        model = Model(ModelType.FLAN_UL2, params=params, credentials=credentials)
+        model = Model("google/flan-ul2", params=params, credentials=credentials)
 
         responses = model.tokenize(["a", "b", "c"], False)
 
         assert responses == expected_token_response.results
 
     @patch("genai.services.RequestHandler.post")
     def test_create_tune(self, mock_requests, credentials):
@@ -112,17 +117,57 @@
         )
         assert tuned_model.model == expected_response["results"]["id"]
 
     @patch("genai.services.RequestHandler.get")
     def test_status(self, mock_requests, credentials):
         label = "test_label"
         model_id = self.model
-        tune_id = SimpleResponse.create_tune(model_id=model_id, name=label)["results"]["id"]
+        tune_id = SimpleResponse.get_tune(model_id=model_id, name=label)["results"]["id"]
 
         tuned_model = Model(tune_id, params=None, credentials=credentials)
 
-        expected_response = SimpleResponse.tunes()
+        expected_response = SimpleResponse.get_tune()
         mock_response = MagicMock(status_code=200)
         mock_response.json.return_value = expected_response
         mock_requests.return_value = mock_response
 
-        assert tuned_model.status() == expected_response["results"][0]["status"]
+        assert tuned_model.status() == expected_response["results"]["status"]
+
+    @patch("genai.services.RequestHandler.get")
+    def test_info(self, mock_requests, credentials):
+        model_id = "google/flan-t5-xl"
+        response = SimpleResponse.models()
+        card = [m for m in response["results"] if m["id"] == model_id]
+        info = ModelCard(**card[0])
+
+        mock_response = MagicMock(status_code=200)
+        mock_response.json.return_value = response
+        mock_requests.return_value = mock_response
+
+        model = Model(model_id, params=None, credentials=credentials)
+        assert info == model.info()
+
+    @patch("genai.services.RequestHandler.get")
+    def test_models(self, mock_requests, credentials):
+        response = SimpleResponse.models()
+
+        mock_response = MagicMock(status_code=200)
+        mock_response.json.return_value = response
+        mock_requests.return_value = mock_response
+
+        assert Model.models(service=self.service) == ModelList(**response).results
+
+    @patch("genai.services.RequestHandler.get")
+    def test_available(self, mock_requests, credentials):
+        response = SimpleResponse.models()
+
+        mock_response = MagicMock(status_code=200)
+        mock_response.json.return_value = response
+        mock_requests.return_value = mock_response
+
+        model_id = "google/flan-t5-xl"
+        model = Model(model_id, params=None, credentials=credentials)
+        assert model.available() is True
+
+        model_id = "random"
+        model = Model(model_id, params=None, credentials=credentials)
+        assert model.available() is False
```

### Comparing `ibm-generative-ai-0.2.2/tests/test_model_async.py` & `ibm-generative-ai-0.2.3/tests/test_model_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest.mock import AsyncMock
 
 import pytest
 
 from genai import Credentials, Model
-from genai.schemas import GenerateParams, ModelType, TokenParams
+from genai.schemas import GenerateParams, TokenParams
 from genai.schemas.responses import GenerateResponse, TokenizeResponse
 from genai.services import ServiceInterface
 from tests.assets.response_helper import SimpleResponse
 
 
 @pytest.mark.unit
 class TestModelAsync:
@@ -42,15 +42,15 @@
         prompts = ["TEST_PROMPT"] * num_prompts
         expected = SimpleResponse.generate_response_array_async(
             model=self.model, inputs=prompts, params=generate_params
         )
         creds = Credentials("TEST_API_KEY")
         mock_generate_json.side_effect = expected
 
-        model = Model(ModelType.FLAN_UL2, params=generate_params, credentials=creds)
+        model = Model("google/flan-ul2", params=generate_params, credentials=creds)
 
         counter = 0
         responses = list(model.generate_async(prompts))
         for batch_idx in range(len(expected)):
             for result in GenerateResponse(**expected[batch_idx]).results:
                 assert responses[counter] == result
                 assert prompts[counter] == result.input_text
@@ -63,15 +63,15 @@
         prompts = ["TEST_PROMPT " + str(i) for i in range(num_prompts)]
         expected = SimpleResponse.tokenize_response_array_async(
             model=self.model, inputs=prompts, params=tokenize_params
         )
         creds = Credentials("TEST_API_KEY")
         mock_tokenize_json.side_effect = expected
 
-        model = Model(ModelType.FLAN_UL2, params=tokenize_params, credentials=creds)
+        model = Model("google/flan-ul2", params=tokenize_params, credentials=creds)
 
         counter = 0
         responses = list(model.tokenize_async(prompts))
         for batch_idx in range(len(expected)):
             for result in TokenizeResponse(**expected[batch_idx]).results:
                 assert responses[counter] == result
                 assert prompts[counter] == result.input_text
@@ -88,15 +88,15 @@
         message = ""
 
         def tasks_completed(result):
             nonlocal message
             message += result.generated_text
 
         prompts = ["TEST_PROMPT"] * num_prompts
-        model = Model(ModelType.FLAN_UL2, params=generate_params, credentials=creds)
+        model = Model("google/flan-ul2", params=generate_params, credentials=creds)
 
         for result in model.generate_async(prompts, callback=tasks_completed):
             pass
 
         assert message == GenerateResponse(**single_response).results[0].generated_text * num_prompts
 
     @pytest.mark.asyncio
@@ -110,13 +110,13 @@
         message = []
 
         def tasks_completed(result):
             nonlocal message
             message += result.tokens
 
         prompts = ["TEST_PROMPT"] * num_prompts
-        model = Model(ModelType.FLAN_UL2, params=tokenize_params, credentials=creds)
+        model = Model("google/flan-ul2", params=tokenize_params, credentials=creds)
 
         for result in model.tokenize_async(prompts, callback=tasks_completed):
             pass
 
         assert message == TokenizeResponse(**expected[0]).results[0].tokens * num_prompts
```

### Comparing `ibm-generative-ai-0.2.2/tests/test_prompt_pattern.py` & `ibm-generative-ai-0.2.3/tests/test_prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_prompt_pattern_watsonx.py` & `ibm-generative-ai-0.2.3/tests/test_prompt_pattern_watsonx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_prompt_template_manager.py` & `ibm-generative-ai-0.2.3/tests/test_prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_request_handler.py` & `ibm-generative-ai-0.2.3/tests/test_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_schema_validation.py` & `ibm-generative-ai-0.2.3/tests/test_schema_validation.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_service_interface.py` & `ibm-generative-ai-0.2.3/tests/test_service_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_service_interface_async.py` & `ibm-generative-ai-0.2.3/tests/test_service_interface_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_service_utils.py` & `ibm-generative-ai-0.2.3/tests/test_service_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_token.py` & `ibm-generative-ai-0.2.3/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.2/tests/test_tunes.py` & `ibm-generative-ai-0.2.3/tests/test_tunes.py`

 * *Files identical despite different names*

