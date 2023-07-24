# Comparing `tmp/pykoi-0.0.0.tar.gz` & `tmp/pykoi-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykoi-0.0.0.tar", max compression
+gzip compressed data, was "pykoi-0.0.1.tar", max compression
```

## Comparing `pykoi-0.0.0.tar` & `pykoi-0.0.1.tar`

### file list

```diff
@@ -1,4 +1,66 @@
--rw-r--r--   0        0        0        0 2023-07-23 21:54:19.850587 pykoi-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-23 21:54:19.850546 pykoi-0.0.0/pykoi/__init__.py
--rw-r--r--   0        0        0      264 2023-07-23 21:54:41.930026 pykoi-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 pykoi-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 05:48:22.776468 pykoi-0.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      442 2023-07-24 08:01:06.918220 pykoi-0.0.1/README.md
+-rw-r--r--   0        0        0      344 2023-07-24 06:45:28.869332 pykoi-0.0.1/pykoi/__init__.py
+-rw-r--r--   0        0        0     8814 2023-07-24 06:54:35.491952 pykoi-0.0.1/pykoi/application.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:48:22.778002 pykoi-0.0.1/pykoi/component/__init__.py
+-rw-r--r--   0        0        0     3910 2023-07-24 05:48:22.778068 pykoi-0.0.1/pykoi/component/base.py
+-rw-r--r--   0        0        0     1033 2023-07-24 05:48:22.778116 pykoi-0.0.1/pykoi/component/chatbot_database_factory.py
+-rw-r--r--   0        0        0      139 2023-07-24 05:48:22.778157 pykoi-0.0.1/pykoi/component/constants.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:48:22.778499 pykoi-0.0.1/pykoi/db/__init__.py
+-rw-r--r--   0        0        0     7345 2023-07-24 05:48:22.778595 pykoi-0.0.1/pykoi/db/qa_database.py
+-rw-r--r--   0        0        0     5768 2023-07-24 05:48:22.778641 pykoi-0.0.1/pykoi/db/ranking_database.py
+-rw-r--r--   0        0        0      248 2023-07-24 05:48:22.778722 pykoi-0.0.1/pykoi/frontend/.gitignore
+-rw-r--r--   0        0        0     2956 2023-07-24 05:48:22.778789 pykoi-0.0.1/pykoi/frontend/README.md
+-rw-r--r--   0        0        0    91356 2023-07-24 05:48:22.779327 pykoi-0.0.1/pykoi/frontend/dist/assets/index-918eba54.js
+-rw-r--r--   0        0        0    22972 2023-07-24 05:48:22.779667 pykoi-0.0.1/pykoi/frontend/dist/assets/index-cf40d152.css
+-rw-r--r--   0        0        0      452 2023-07-24 05:48:22.779737 pykoi-0.0.1/pykoi/frontend/dist/index.html
+-rw-r--r--   0        0        0     1498 2023-07-24 05:48:22.779799 pykoi-0.0.1/pykoi/frontend/dist/vite.svg
+-rw-r--r--   0        0        0      360 2023-07-24 05:48:22.779852 pykoi-0.0.1/pykoi/frontend/index.html
+-rw-r--r--   0        0        0      938 2023-07-24 05:48:22.779903 pykoi-0.0.1/pykoi/frontend/jsconfig.json
+-rw-r--r--   0        0        0      540 2023-07-24 05:48:22.779955 pykoi-0.0.1/pykoi/frontend/package.json
+-rw-r--r--   0        0        0     1498 2023-07-24 05:48:22.780032 pykoi-0.0.1/pykoi/frontend/public/vite.svg
+-rw-r--r--   0        0        0     1500 2023-07-24 05:48:22.780119 pykoi-0.0.1/pykoi/frontend/src/App.svelte
+-rw-r--r--   0        0        0    10286 2023-07-24 05:48:22.780215 pykoi-0.0.1/pykoi/frontend/src/app.css
+-rw-r--r--   0        0        0     1951 2023-07-24 05:48:22.780300 pykoi-0.0.1/pykoi/frontend/src/assets/svelte.svg
+-rw-r--r--   0        0        0     4901 2023-07-24 05:48:22.780451 pykoi-0.0.1/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte
+-rw-r--r--   0        0        0      290 2023-07-24 05:48:22.780533 pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/Chat.svelte
+-rw-r--r--   0        0        0     8876 2023-07-24 05:48:22.780624 pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte
+-rw-r--r--   0        0        0     8705 2023-07-24 05:48:22.780670 pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte
+-rw-r--r--   0        0        0     3905 2023-07-24 05:48:22.780801 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte
+-rw-r--r--   0        0        0     3905 2023-07-24 05:48:22.780875 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte
+-rw-r--r--   0        0        0     3890 2023-07-24 05:48:22.780930 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte
+-rw-r--r--   0        0        0     4421 2023-07-24 05:48:22.780990 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte
+-rw-r--r--   0        0        0     2701 2023-07-24 05:48:22.781055 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte
+-rw-r--r--   0        0        0     2638 2023-07-24 05:48:22.781111 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte
+-rw-r--r--   0        0        0     1384 2023-07-24 05:48:22.781164 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte
+-rw-r--r--   0        0        0     1055 2023-07-24 05:48:22.781214 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte
+-rw-r--r--   0        0        0     3326 2023-07-24 05:48:22.781273 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/Feedback.svelte
+-rw-r--r--   0        0        0     4317 2023-07-24 05:48:22.781387 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Bar.svelte
+-rw-r--r--   0        0        0      507 2023-07-24 05:48:22.781437 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Cell.svelte
+-rw-r--r--   0        0        0     3898 2023-07-24 05:48:22.781481 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte
+-rw-r--r--   0        0        0     3910 2023-07-24 05:48:22.781525 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/LineChart.svelte
+-rw-r--r--   0        0        0     3611 2023-07-24 05:48:22.781587 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte
+-rw-r--r--   0        0        0     5069 2023-07-24 05:48:22.781652 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Table.svelte
+-rw-r--r--   0        0        0     1804 2023-07-24 05:48:22.781705 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/data.js
+-rw-r--r--   0        0        0      584 2023-07-24 05:48:22.781759 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/store.js
+-rw-r--r--   0        0        0      380 2023-07-24 05:48:22.781878 pykoi-0.0.1/pykoi/frontend/src/lib/UIComponents/Dropdown.svelte
+-rw-r--r--   0        0        0      191 2023-07-24 05:48:22.781939 pykoi-0.0.1/pykoi/frontend/src/main.js
+-rw-r--r--   0        0        0     6818 2023-07-24 05:48:22.782013 pykoi-0.0.1/pykoi/frontend/src/normalize.css
+-rw-r--r--   0        0        0      542 2023-07-24 05:48:22.782090 pykoi-0.0.1/pykoi/frontend/src/store.js
+-rw-r--r--   0        0        0     9194 2023-07-24 05:48:22.782137 pykoi-0.0.1/pykoi/frontend/src/styles.css
+-rw-r--r--   0        0        0     1743 2023-07-24 05:48:22.782192 pykoi-0.0.1/pykoi/frontend/src/utils.js
+-rw-r--r--   0        0        0       71 2023-07-24 05:48:22.782236 pykoi-0.0.1/pykoi/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      228 2023-07-24 05:48:22.782288 pykoi-0.0.1/pykoi/frontend/svelte.config.js
+-rw-r--r--   0        0        0      177 2023-07-24 05:48:22.782338 pykoi-0.0.1/pykoi/frontend/vite.config.js
+-rw-r--r--   0        0        0        0 2023-07-24 05:48:22.782390 pykoi-0.0.1/pykoi/llm/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-24 05:48:22.782469 pykoi-0.0.1/pykoi/llm/abs_llm.py
+-rw-r--r--   0        0        0      455 2023-07-24 07:45:46.634814 pykoi-0.0.1/pykoi/llm/constants.py
+-rw-r--r--   0        0        0     2818 2023-07-24 05:48:22.782596 pykoi-0.0.1/pykoi/llm/huggingface.py
+-rw-r--r--   0        0        0     2077 2023-07-24 07:46:28.170787 pykoi-0.0.1/pykoi/llm/model_factory.py
+-rw-r--r--   0        0        0     2205 2023-07-24 05:48:22.782707 pykoi-0.0.1/pykoi/llm/openai.py
+-rw-r--r--   0        0        0     3465 2023-07-24 08:51:40.226463 pykoi-0.0.1/pykoi/llm/peft_huggingface.py
+-rw-r--r--   0        0        0        0 2023-07-24 05:48:22.782816 pykoi-0.0.1/pykoi/rlhf/__init__.py
+-rw-r--r--   0        0        0    32326 2023-07-24 06:50:21.614734 pykoi-0.0.1/pykoi/rlhf/rlhf.py
+-rw-r--r--   0        0        0     1014 2023-07-24 05:48:22.783034 pykoi-0.0.1/pykoi/state.py
+-rw-r--r--   0        0        0      612 2023-07-24 09:27:54.670355 pykoi-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 pykoi-0.0.1/PKG-INFO
```

