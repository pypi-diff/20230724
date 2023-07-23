# Comparing `tmp/kedro_mlflow-0.8.1.tar.gz` & `tmp/kedro_mlflow-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kedro_mlflow-0.8.1.tar", last modified: Sun Feb 13 22:59:49 2022, max compression
+gzip compressed data, was "dist/kedro_mlflow-0.9.0.tar", last modified: Fri Apr  1 11:31:04 2022, max compression
```

## Comparing `kedro_mlflow-0.8.1.tar` & `kedro_mlflow-0.9.0.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/workflows/check-links.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/workflows/prepare-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    27626 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12343 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10644 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/01_introduction/
--rw-r--r--   0 runner    (1001) docker     (121)     9130 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/01_introduction/01_introduction.md
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/01_introduction/02_motivation.md
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/01_introduction/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/02_installation/
--rw-r--r--   0 runner    (1001) docker     (121)     3263 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/02_installation/01_installation.md
--rw-r--r--   0 runner    (1001) docker     (121)     3908 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/02_installation/02_setup.md
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/02_installation/03_migration_guide.md
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/02_installation/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/03_getting_started/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/03_getting_started/00_intro_tutorial.md
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/03_getting_started/01_example_project.md
--rw-r--r--   0 runner    (1001) docker     (121)     7417 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/03_getting_started/02_first_steps.md
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/03_getting_started/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/
--rw-r--r--   0 runner    (1001) docker     (121)     9106 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/01_configuration.md
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/02_version_parameters.md
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/03_version_datasets.md
--rw-r--r--   0 runner    (1001) docker     (121)     5373 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/04_version_models.md
--rw-r--r--   0 runner    (1001) docker     (121)     8486 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/05_version_metrics.md
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/06_mlflow_ui.md
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/05_framework_ml/
--rw-r--r--   0 runner    (1001) docker     (121)    14061 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_framework_ml/01_why_framework.md
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_framework_ml/02_ml_project_components.md
--rw-r--r--   0 runner    (1001) docker     (121)     6641 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_framework_ml/03_framework_solutions.md
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_framework_ml/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/01_mlflow_models.md
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/02_custom_kedro_pipeline_model.md
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/03_cli_modelify.md
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/04_hook_pipeline_ml.md
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/06_interactive_use/
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/06_interactive_use/01_notebook_use.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/06_interactive_use/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/07_python_objects/
--rw-r--r--   0 runner    (1001) docker     (121)     6080 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/07_python_objects/01_DataSets.md
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/07_python_objects/02_Hooks.md
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/07_python_objects/03_Pipelines.md
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/07_python_objects/04_CLI.md
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/07_python_objects/05_Configuration.md
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/07_python_objects/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/08_API/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.config.rst
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.extras.extensions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.framework.cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.framework.hooks.rst
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.io.rst
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.mlflow.rst
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/imgs/
--rw-r--r--   0 runner    (1001) docker     (121)    17019 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/apps_interaction.png
--rw-r--r--   0 runner    (1001) docker     (121)     7613 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/default_catalog.png
--rw-r--r--   0 runner    (1001) docker     (121)    29806 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/etl_app.png
--rw-r--r--   0 runner    (1001) docker     (121)   126628 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/hook_registration_process.png
--rw-r--r--   0 runner    (1001) docker     (121)    17991 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/initialized_project.png
--rw-r--r--   0 runner    (1001) docker     (121)    74974 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/kedro_viz_params.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)    27015 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/preprocessing/all.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    21109 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/preprocessing/inference.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    24673 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/preprocessing/training.PNG
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/shared_inputs/
--rw-r--r--   0 runner    (1001) docker     (121)    28444 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/shared_inputs/all.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    24541 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/shared_inputs/inference.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    25851 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/shared_inputs/training.PNG
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (121)    24186 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/tokenizer/all.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    20332 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/tokenizer/inference.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    30055 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/tokenizer/training.PNG
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/vanilla/
--rw-r--r--   0 runner    (1001) docker     (121)    32775 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/vanilla/all.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    26663 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/vanilla/inference.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    62927 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/vanilla/training.PNG
--rw-r--r--   0 runner    (1001) docker     (121)    69355 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/mlflow_host_page.png
--rw-r--r--   0 runner    (1001) docker     (121)    66209 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/mlflow_run.png
--rw-r--r--   0 runner    (1001) docker     (121)    17183 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/mlflow_tracking_schema.png
--rw-r--r--   0 runner    (1001) docker     (121)    37892 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/mlflow_yml.png
--rw-r--r--   0 runner    (1001) docker     (121)    52135 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/once_run_project.png
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/run_with_artifact.png
--rw-r--r--   0 runner    (1001) docker     (121)    12512 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/docs/source/imgs/updated_catalog.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/config/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8054 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/config/kedro_mlflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/extras/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/extras/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/extras/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/extras/extensions/ipython.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12723 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/cli/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5267 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/node_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    11644 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/pipeline_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/artifacts/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/artifacts/mlflow_artifact_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/catalog/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/catalog/switch_catalog_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_abstract_metric_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_metric_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_metric_history_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     6436 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/models/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/models/mlflow_abstract_model_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5737 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/models/mlflow_model_logger_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3665 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/io/models/mlflow_model_saver_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/mlflow/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9605 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/mlflow/kedro_pipeline_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9677 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/pipeline/pipeline_ml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/pipeline/pipeline_ml_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/template/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/template/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/template/examples/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow/template/project/
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/template/project/mlflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/kedro_mlflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12343 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6747 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/kedro_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/mlc_config.json
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/config/test_get_mlflow_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8318 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/config/test_kedro_mlflow_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/extras/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/extras/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/extras/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/extras/extensions/test_ipython.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/framework/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8951 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    12679 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/cli/test_cli_modelify.py
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/cli/test_cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/framework/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/hooks/test_all_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)    11658 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/hooks/test_node_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    27389 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/hooks/test_pipeline_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/framework/hooks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/io/artifacts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/artifacts/test_mlflow_artifact_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/io/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6625 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/metrics/test_mlflow_metric_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/metrics/test_mlflow_metric_history_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     6642 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/metrics/test_mlflow_metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/io/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12254 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/models/test_mlflow_model_logger_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5523 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/io/models/test_mlflow_model_saver_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/mlflow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18470 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/mlflow/test_kedro_pipeline_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13864 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/pipeline/test_pipeline_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:49.000000 kedro_mlflow-0.8.1/tests/template/project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/template/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/template/project/test_mlflow_yml.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-02-13 22:59:45.000000 kedro_mlflow-0.8.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/workflows/check-links.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/workflows/prepare-release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    28088 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12968 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11209 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/01_introduction/
+-rw-r--r--   0 runner    (1001) docker     (121)    10278 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/01_introduction/01_introduction.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/01_introduction/02_motivation.md
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/01_introduction/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/02_installation/
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/02_installation/01_installation.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3870 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/02_installation/02_setup.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/02_installation/03_migration_guide.md
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/02_installation/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/03_getting_started/
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/03_getting_started/00_intro_tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/03_getting_started/01_example_project.md
+-rw-r--r--   0 runner    (1001) docker     (121)     7312 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/03_getting_started/02_first_steps.md
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/03_getting_started/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/
+-rw-r--r--   0 runner    (1001) docker     (121)     9106 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/01_configuration.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/02_version_parameters.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/03_version_datasets.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5373 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/04_version_models.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8486 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/05_version_metrics.md
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/06_mlflow_ui.md
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/05_framework_ml/
+-rw-r--r--   0 runner    (1001) docker     (121)    14061 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_framework_ml/01_why_framework.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_framework_ml/02_ml_project_components.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6641 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_framework_ml/03_framework_solutions.md
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_framework_ml/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/01_mlflow_models.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/02_custom_kedro_pipeline_model.md
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/03_cli_modelify.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/04_hook_pipeline_ml.md
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/06_interactive_use/
+-rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/06_interactive_use/01_notebook_use.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/06_interactive_use/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/07_python_objects/
+-rw-r--r--   0 runner    (1001) docker     (121)     6080 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/07_python_objects/01_DataSets.md
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/07_python_objects/02_Hooks.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/07_python_objects/03_Pipelines.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/07_python_objects/04_CLI.md
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/07_python_objects/05_Configuration.md
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/07_python_objects/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/08_API/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.config.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.extras.extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.framework.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.framework.hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.io.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.mlflow.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/imgs/
+-rw-r--r--   0 runner    (1001) docker     (121)    17019 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/apps_interaction.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7613 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/default_catalog.png
+-rw-r--r--   0 runner    (1001) docker     (121)    29806 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/etl_app.png
+-rw-r--r--   0 runner    (1001) docker     (121)   126628 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/hook_registration_process.png
+-rw-r--r--   0 runner    (1001) docker     (121)    17991 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/initialized_project.png
+-rw-r--r--   0 runner    (1001) docker     (121)    74974 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/kedro_viz_params.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)    27015 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/preprocessing/all.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    21109 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/preprocessing/inference.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    24673 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/preprocessing/training.PNG
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/shared_inputs/
+-rw-r--r--   0 runner    (1001) docker     (121)    28444 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/shared_inputs/all.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    24541 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/shared_inputs/inference.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    25851 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/shared_inputs/training.PNG
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (121)    24186 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/tokenizer/all.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    20332 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/tokenizer/inference.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    30055 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/tokenizer/training.PNG
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (121)    32775 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/vanilla/all.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    26663 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/vanilla/inference.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    62927 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/vanilla/training.PNG
+-rw-r--r--   0 runner    (1001) docker     (121)    69355 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/mlflow_host_page.png
+-rw-r--r--   0 runner    (1001) docker     (121)    66209 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/mlflow_run.png
+-rw-r--r--   0 runner    (1001) docker     (121)    17183 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/mlflow_tracking_schema.png
+-rw-r--r--   0 runner    (1001) docker     (121)    37892 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/mlflow_yml.png
+-rw-r--r--   0 runner    (1001) docker     (121)    52135 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/once_run_project.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/run_with_artifact.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12512 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/docs/source/imgs/updated_catalog.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/config/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8750 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/config/kedro_mlflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/extras/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/extras/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/extras/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/extras/extensions/ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12644 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/cli/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5139 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/node_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11397 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/pipeline_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/artifacts/mlflow_artifact_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/catalog/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/catalog/switch_catalog_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_abstract_metric_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_metric_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_metric_history_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6436 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4509 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/models/mlflow_abstract_model_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5737 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/models/mlflow_model_logger_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3665 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/io/models/mlflow_model_saver_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9905 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/mlflow/kedro_pipeline_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10775 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/pipeline/pipeline_ml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/pipeline/pipeline_ml_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/template/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/template/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/template/examples/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow/template/project/
+-rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/template/project/mlflow.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/kedro_mlflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12968 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6747 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/kedro_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/mlc_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6707 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/config/test_get_mlflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8318 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/config/test_kedro_mlflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/extras/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/extras/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/extras/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/extras/extensions/test_ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9838 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12679 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/cli/test_cli_modelify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/cli/test_cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/framework/hooks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/hooks/test_all_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11504 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/hooks/test_node_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27246 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/hooks/test_pipeline_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/framework/hooks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/io/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/artifacts/test_mlflow_artifact_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/io/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6625 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/metrics/test_mlflow_metric_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/metrics/test_mlflow_metric_history_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6642 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/metrics/test_mlflow_metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/io/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12254 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/models/test_mlflow_model_logger_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5523 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/io/models/test_mlflow_model_saver_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18470 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/mlflow/test_kedro_pipeline_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12849 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/pipeline/test_pipeline_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/template/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:04.000000 kedro_mlflow-0.9.0/tests/template/project/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/template/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/template/project/test_mlflow_yml.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-04-01 11:31:00.000000 kedro_mlflow-0.9.0/tests/test_utils.py
```

### Comparing `kedro_mlflow-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kedro_mlflow-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `kedro_mlflow-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/.github/PULL_REQUEST_TEMPLATE.md` & `kedro_mlflow-0.9.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/.github/workflows/prepare-release.yml` & `kedro_mlflow-0.9.0/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/.github/workflows/publish.yml` & `kedro_mlflow-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/.github/workflows/test.yml` & `kedro_mlflow-0.9.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     branches: [master]
 
 jobs:
   lint_and_test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: [3.6, 3.7]
+        python-version: [3.7, 3.8]
         os: [ubuntu-latest, macos-latest, windows-latest]
     env:
       OS: ${{ matrix.os }}
       PYTHON_VERSION: ${{ matrix.python-version }}
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
```

### Comparing `kedro_mlflow-0.8.1/.gitignore` & `kedro_mlflow-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/.pre-commit-config.yaml` & `kedro_mlflow-0.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 exclude: ^kedro_mlflow/template/project/run.py$
 repos:
     - repo: https://github.com/psf/black
-      rev: 21.10b0
+      rev: 22.3.0
       hooks:
           - id: black
             language_version: python3.7
     - repo: https://github.com/timothycrosley/isort
       rev: 5.10.1
       hooks:
           - id: isort
```

### Comparing `kedro_mlflow-0.8.1/.readthedocs.yml` & `kedro_mlflow-0.9.0/.readthedocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 
 # Optionally build your docs in additional formats such as PDF
 formats:
   - pdf
 
 # Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.6
+  version: 3.8
   install:
     - method: pip
       path: .
       extra_requirements:
        - doc
```

### Comparing `kedro_mlflow-0.8.1/CHANGELOG.md` & `kedro_mlflow-0.9.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.9.0] - 2022-04-01
+
+### Added
+
+-   :sparkles: Add support for `kedro=0.18.X`
+-   :sparkles: `kedro-mlflow` is now available on `conda-forge` and can be installed with `conda install kedro-mlflow`. This is retroactive to `kedro-mlflow==0.8.1` ([#118](https://github.com/Galileo-Galilei/kedro-mlflow/issues/118))
+
+### Removed
+
+-   :boom: :wastebasket: Drop support for `kedro=0.17.X`
+
 ## [0.8.1] - 2022-02-13
 
 ### Added
 
 -   :sparkles: Open the UI in the default browser when the `mlflow_tracking_uri` in `mlflow.yml` is a http address instead of launching the ui server. ([#275](https://github.com/Galileo-Galilei/kedro-mlflow/issues/275))
 
 ### Fixed
@@ -164,15 +175,15 @@
 ### Added
 
 -   :arrow_up: `kedro-mlflow` now supports `kedro>=0.16.5` ([#62](https://github.com/Galileo-Galilei/kedro-mlflow/issues/62))
 -   :sparkles: `kedro-mlflow` now supports configuring the project in `pyproject.toml`  (_Only for kedro>=0.16.5_) ([#96](https://github.com/Galileo-Galilei/kedro-mlflow/issues/96))
 -   :sparkles: `pipeline_ml_factory` now accepts that `inference` pipeline `inputs` may be in `training` pipeline `inputs` ([#71](https://github.com/Galileo-Galilei/kedro-mlflow/issues/71))
 -   :sparkles: `pipeline_ml_factory` now infer automatically the schema of the input dataset to validate data automatically at inference time. The output schema can be declared manually in `model_signature` argument ([#70](https://github.com/Galileo-Galilei/kedro-mlflow/issues/70))
 -   :sparkles: Add two DataSets for model logging and saving: `MlflowModelLoggerDataSet` and `MlflowModelSaverDataSet` ([#12](https://github.com/Galileo-Galilei/kedro-mlflow/issues/12))
--   :sparkles: `MlflowPipelineHook` and `MlflowNodeHook` are now [auto-registered](https://kedro.readthedocs.io/en/latest/07_extend_kedro/02_hooks.html#registering-your-hook-implementations-with-kedro) if you use `kedro>=0.16.4` ([#29](https://github.com/Galileo-Galilei/kedro-mlflow/issues/29))
+-   :sparkles: `MlflowPipelineHook` and `MlflowNodeHook` are now [auto-registered](https://kedro.readthedocs.io/en/latest/extend_kedro/hooks.html#registering-your-hook-implementations-with-kedro) if you use `kedro>=0.16.4` ([#29](https://github.com/Galileo-Galilei/kedro-mlflow/issues/29))
 
 ### Fixed
 
 -   :zap: `get_mlflow_config` now uses the Kedro `ProjectContext` `ConfigLoader` to get configs ([#66](https://github.com/Galileo-Galilei/kedro-mlflow/issues/66)). This indirectly solves the following issues:
     -   `get_mlflow_config` now works in interactive mode if `load_context` is called  with a path different from the working directory ([#30](https://github.com/Galileo-Galilei/kedro-mlflow/issues/30))
     -   kedro_mlflow now works fine with kedro jupyter notebook independently of the working directory ([#64](https://github.com/Galileo-Galilei/kedro-mlflow/issues/64))
     -   You can use global variables in `mlflow.yml` which is now properly parsed if you use a `TemplatedConfigLoader` ([#72](https://github.com/Galileo-Galilei/kedro-mlflow/issues/72))
@@ -279,15 +290,17 @@
 ### Added
 
 -   :sparkles: Add cli `kedro mlflow init` to udpdate the template and `kedro mlflow ui` to open `mlflow` user interface with your project configuration
 -   :sparkles: Add hooks `MlflowNodeHook` and `MlflowPipelineHook` for parameters autologging and model autologging
 -   :sparkles: Add `MlflowDataSet` for artifacts autologging
 -   :sparkles: Add `PipelineMl` class and its `pipeline_ml` factory for pipeline packaging and service
 
-[Unreleased]: https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.8.1...HEAD
+[Unreleased]: https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.9.0...HEAD
+
+[0.9.0]: https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.8.1...0.9.0
 
 [0.8.1]: https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.8.0...0.8.1
 
 [0.8.0]: https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.7.6...0.8.0
 
 [0.7.6]: https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.7.5...0.7.6
```

### Comparing `kedro_mlflow-0.8.1/CODE_OF_CONDUCT.md` & `kedro_mlflow-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/CONTRIBUTING.md` & `kedro_mlflow-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/LICENSE` & `kedro_mlflow-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/PKG-INFO` & `kedro_mlflow-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: kedro_mlflow
-Version: 0.8.1
+Version: 0.9.0
 Summary: A kedro-plugin to use mlflow in your kedro projects
 Home-page: https://github.com/Galileo-Galilei/kedro-mlflow
 Author: Yolan Honoré-Rougé
 License: Apache Software License (Apache 2.0)
 Description: **General informations**
         
-        [![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg)](https://pypi.org/project/kedro-mlflow/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+        [![Python Version](https://img.shields.io/pypi/pyversions/kedro-mlflow)](https://pypi.org/project/kedro-mlflow/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
         [![SemVer](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
         
         ----------------------------------------------------------
-        | Software repository | Latest release                                                                                       | Total downloads                                                                              |
-        | ------------------- | ---------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
-        | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-mlflow.svg)](https://pypi.org/project/kedro-mlflow/) | [![Downloads](https://pepy.tech/badge/kedro-mlflow)](https://pepy.tech/project/kedro-mlflow) |
+        | Package manager | Software repository | Latest release                                                                                                                                | Total downloads                                                                                                                 |
+        | --------------- | ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
+        | ``pip``         | PyPI                | [![PyPI version](https://badge.fury.io/py/kedro-mlflow.svg)](https://pypi.org/project/kedro-mlflow/)                                          | [![Downloads](https://pepy.tech/badge/kedro-mlflow)](https://pepy.tech/project/kedro-mlflow)                                    |
+        | ``conda``       | conda-forge         | [![conda version](https://img.shields.io/conda/vn/conda-forge/kedro-mlflow?color=bright%20green)](https://anaconda.org/search?q=kedro+mlflow) | [![Downloads](https://img.shields.io/conda/dn/conda-forge/kedro-mlflow?color=blue)](https://anaconda.org/search?q=kedro+mlflow) |
         
         **Code health**
         
         ----------------------------------------------------------
         | Branch   | Tests                                                                                                                                                                                            | Coverage                                                                                                                                                         | Links                                                                                                                                                                                                           | Documentation                                                                                                                           | Deployment                                                                                                                                                                                                | Activity                                                                                                                                                            |
         | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | `master` | [![test](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/test/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Atest+branch%3Amaster) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master) | [![links](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/check-links/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Acheck-links+branch%3Amaster) | [![Documentation](https://readthedocs.org/projects/kedro-mlflow/badge/?version=stable)](https://kedro-mlflow.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/publish/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=branch%3Amaster+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-mlflow/0.8.1)](https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.8.1...master) |
+        | `master` | [![test](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/test/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Atest+branch%3Amaster) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master) | [![links](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/check-links/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Acheck-links+branch%3Amaster) | [![Documentation](https://readthedocs.org/projects/kedro-mlflow/badge/?version=stable)](https://kedro-mlflow.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/publish/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=branch%3Amaster+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-mlflow/0.9.0)](https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.9.0...master) |
         
         # What is kedro-mlflow?
         
-        ``kedro-mlflow`` is a [kedro-plugin](https://kedro.readthedocs.io/en/stable/07_extend_kedro/04_plugins.html) for lightweight and portable integration of [mlflow](https://mlflow.org/docs/latest/index.html) capabilities inside [kedro](https://kedro.readthedocs.io/en/stable/index.html) projects. It enforces [``Kedro`` principles](https://kedro.readthedocs.io/en/stable/12_faq/01_faq.html?highlight=principles#what-is-the-philosophy-behind-kedro) to make mlflow usage as production ready as possible. Its core functionalities are :
+        ``kedro-mlflow`` is a [kedro-plugin](https://kedro.readthedocs.io/en/stable/extend_kedro/plugins.html) for lightweight and portable integration of [mlflow](https://mlflow.org/docs/latest/index.html) capabilities inside [kedro](https://kedro.readthedocs.io/en/stable/index.html) projects. It enforces [``Kedro`` principles](https://kedro.readthedocs.io/en/stable/12_faq/01_faq.html?highlight=principles#what-is-the-philosophy-behind-kedro) to make mlflow usage as production ready as possible. Its core functionalities are :
         
         - **versioning**: `kedro-mlflow` intends to enhance reproducibility for machine learning experimentation. With `kedro-mlflow` installed, you can effortlessly register your parameters or your datasets with minimal configuration in a kedro run. Later, you will be able to browse your runs in the mlflow UI, and retrieve the runs you want. This is directly linked to [Mlflow Tracking](https://www.mlflow.org/docs/latest/tracking.html).
         - **model packaging**: ``kedro-mlflow`` intends to be be an agnostic machine learning framework for people who want to write portable, production ready machine learning pipelines. It offers a convenient API to convert a Kedro pipeline to a ``model`` in the mlflow sense. Consequently, you can *API-fy* or serve your Kedro pipeline with one line of code, or share a model with without worrying of the preprocessing to be made for further use. This is directly linked to [Mlflow Models](https://www.mlflow.org/docs/latest/models.html).
         
         # How do I install kedro-mlflow?
         
         **Important: ``kedro-mlflow`` is only compatible with ``kedro>=0.16.0`` and ``mlflow>=1.0.0``. If you have a project created with an older version of ``Kedro``, see this [migration guide](https://github.com/quantumblacklabs/kedro/blob/master/RELEASE.md#migration-guide-from-kedro-015-to-016).**
@@ -41,15 +42,15 @@
         
         If you want to use the most up to date version of the package which is under development and not released yet, you can install the package from github:
         
         ```console
         pip install --upgrade git+https://github.com/Galileo-Galilei/kedro-mlflow.git
         ```
         
-        I strongly recommend to use ``conda`` (a package manager) to create an environment and to read [``kedro`` installation guide](https://kedro.readthedocs.io/en/latest/02_get_started/02_install.html).
+        I strongly recommend to use ``conda`` (a package manager) to create an environment and to read [``kedro`` installation guide](https://kedro.readthedocs.io/en/latest/get_started/install.html).
         
         # Getting started
         
         The documentation contains:
         
         - [A  "hello world" example](https://kedro-mlflow.readthedocs.io/en/latest/source/03_getting_started/index.html) which demonstrates how you to **setup your project**, **version parameters** and **datasets**, and browse your runs in the UI.
         - A section for [advanced machine learning versioning](https://kedro-mlflow.readthedocs.io/en/latest/source/04_experimentation_tracking/index.html) to show more advanced features (mlflow configuration through the plugin, package and serve a kedro ``Pipeline``...)
@@ -87,23 +88,24 @@
         - [Takieddine Kadiri](https://github.com/takikadiri)
         
         Many thanks to [Adrian Piotr Kruszewski](https://github.com/akruszewski) for his past work on the repo.
         
 Keywords: kedro-plugin,mlflow,model versioning,model packaging,pipelines,machine learning,data pipelines,data science,data engineering
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Kedro
 Classifier: Environment :: Plugins
 Classifier: Framework :: Kedro
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6, <3.9
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: extras
```

### Comparing `kedro_mlflow-0.8.1/README.md` & `kedro_mlflow-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 **General informations**
 
-[![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg)](https://pypi.org/project/kedro-mlflow/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+[![Python Version](https://img.shields.io/pypi/pyversions/kedro-mlflow)](https://pypi.org/project/kedro-mlflow/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 [![SemVer](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
 
 ----------------------------------------------------------
-| Software repository | Latest release                                                                                       | Total downloads                                                                              |
-| ------------------- | ---------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
-| Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-mlflow.svg)](https://pypi.org/project/kedro-mlflow/) | [![Downloads](https://pepy.tech/badge/kedro-mlflow)](https://pepy.tech/project/kedro-mlflow) |
+| Package manager | Software repository | Latest release                                                                                                                                | Total downloads                                                                                                                 |
+| --------------- | ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
+| ``pip``         | PyPI                | [![PyPI version](https://badge.fury.io/py/kedro-mlflow.svg)](https://pypi.org/project/kedro-mlflow/)                                          | [![Downloads](https://pepy.tech/badge/kedro-mlflow)](https://pepy.tech/project/kedro-mlflow)                                    |
+| ``conda``       | conda-forge         | [![conda version](https://img.shields.io/conda/vn/conda-forge/kedro-mlflow?color=bright%20green)](https://anaconda.org/search?q=kedro+mlflow) | [![Downloads](https://img.shields.io/conda/dn/conda-forge/kedro-mlflow?color=blue)](https://anaconda.org/search?q=kedro+mlflow) |
 
 **Code health**
 
 ----------------------------------------------------------
 | Branch   | Tests                                                                                                                                                                                            | Coverage                                                                                                                                                         | Links                                                                                                                                                                                                           | Documentation                                                                                                                           | Deployment                                                                                                                                                                                                | Activity                                                                                                                                                            |
 | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `master` | [![test](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/test/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Atest+branch%3Amaster) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master) | [![links](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/check-links/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Acheck-links+branch%3Amaster) | [![Documentation](https://readthedocs.org/projects/kedro-mlflow/badge/?version=stable)](https://kedro-mlflow.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/publish/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=branch%3Amaster+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-mlflow/0.8.1)](https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.8.1...master) |
+| `master` | [![test](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/test/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Atest+branch%3Amaster) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master) | [![links](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/check-links/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Acheck-links+branch%3Amaster) | [![Documentation](https://readthedocs.org/projects/kedro-mlflow/badge/?version=stable)](https://kedro-mlflow.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/publish/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=branch%3Amaster+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-mlflow/0.9.0)](https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.9.0...master) |
 
 # What is kedro-mlflow?
 
-``kedro-mlflow`` is a [kedro-plugin](https://kedro.readthedocs.io/en/stable/07_extend_kedro/04_plugins.html) for lightweight and portable integration of [mlflow](https://mlflow.org/docs/latest/index.html) capabilities inside [kedro](https://kedro.readthedocs.io/en/stable/index.html) projects. It enforces [``Kedro`` principles](https://kedro.readthedocs.io/en/stable/12_faq/01_faq.html?highlight=principles#what-is-the-philosophy-behind-kedro) to make mlflow usage as production ready as possible. Its core functionalities are :
+``kedro-mlflow`` is a [kedro-plugin](https://kedro.readthedocs.io/en/stable/extend_kedro/plugins.html) for lightweight and portable integration of [mlflow](https://mlflow.org/docs/latest/index.html) capabilities inside [kedro](https://kedro.readthedocs.io/en/stable/index.html) projects. It enforces [``Kedro`` principles](https://kedro.readthedocs.io/en/stable/12_faq/01_faq.html?highlight=principles#what-is-the-philosophy-behind-kedro) to make mlflow usage as production ready as possible. Its core functionalities are :
 
 - **versioning**: `kedro-mlflow` intends to enhance reproducibility for machine learning experimentation. With `kedro-mlflow` installed, you can effortlessly register your parameters or your datasets with minimal configuration in a kedro run. Later, you will be able to browse your runs in the mlflow UI, and retrieve the runs you want. This is directly linked to [Mlflow Tracking](https://www.mlflow.org/docs/latest/tracking.html).
 - **model packaging**: ``kedro-mlflow`` intends to be be an agnostic machine learning framework for people who want to write portable, production ready machine learning pipelines. It offers a convenient API to convert a Kedro pipeline to a ``model`` in the mlflow sense. Consequently, you can *API-fy* or serve your Kedro pipeline with one line of code, or share a model with without worrying of the preprocessing to be made for further use. This is directly linked to [Mlflow Models](https://www.mlflow.org/docs/latest/models.html).
 
 # How do I install kedro-mlflow?
 
 **Important: ``kedro-mlflow`` is only compatible with ``kedro>=0.16.0`` and ``mlflow>=1.0.0``. If you have a project created with an older version of ``Kedro``, see this [migration guide](https://github.com/quantumblacklabs/kedro/blob/master/RELEASE.md#migration-guide-from-kedro-015-to-016).**
@@ -34,15 +35,15 @@
 
 If you want to use the most up to date version of the package which is under development and not released yet, you can install the package from github:
 
 ```console
 pip install --upgrade git+https://github.com/Galileo-Galilei/kedro-mlflow.git
 ```
 
-I strongly recommend to use ``conda`` (a package manager) to create an environment and to read [``kedro`` installation guide](https://kedro.readthedocs.io/en/latest/02_get_started/02_install.html).
+I strongly recommend to use ``conda`` (a package manager) to create an environment and to read [``kedro`` installation guide](https://kedro.readthedocs.io/en/latest/get_started/install.html).
 
 # Getting started
 
 The documentation contains:
 
 - [A  "hello world" example](https://kedro-mlflow.readthedocs.io/en/latest/source/03_getting_started/index.html) which demonstrates how you to **setup your project**, **version parameters** and **datasets**, and browse your runs in the UI.
 - A section for [advanced machine learning versioning](https://kedro-mlflow.readthedocs.io/en/latest/source/04_experimentation_tracking/index.html) to show more advanced features (mlflow configuration through the plugin, package and serve a kedro ``Pipeline``...)
```

### Comparing `kedro_mlflow-0.8.1/docs/Makefile` & `kedro_mlflow-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/conf.py` & `kedro_mlflow-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/index.rst` & `kedro_mlflow-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/make.bat` & `kedro_mlflow-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/01_introduction/01_introduction.md` & `kedro_mlflow-0.9.0/docs/source/01_introduction/01_introduction.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 For more details, see [Mlflow's official documentation](https://www.mlflow.org/docs/latest/index.html).
 
 ## A brief comparison between ``Kedro`` and ``Mlflow``
 
 While ``Kedro`` and ``Mlflow`` do not compete in the same field, they provide some overlapping functionalities. ``Mlflow`` is specifically dedicated to machine learning and its lifecycle management, while ``Kedro`` focusing on data pipeline development. Below chart compare the different functionalities:
 
-|Functionality |Kedro          |Mlflow         |
-|:-------------|:--------------|:--------------|
-|I/O abstraction | various ``AbstractDataSet`` | N/A |
-|I/O configuration files |- ``catalog.yml`` <br> - ``parameters.yml``          |``MLproject``|
-|Compute abstraction|- ``Pipeline`` <br> - ``Node``| N/A |
-|Compute configuration files|- ``hooks.py`` <br> - ``run.py``| `MLproject` |
-|Parameters and data versioning| - ``Journal`` <br> - ``AbstractVersionedDataSet`` |- ``log_metric``<br> - ``log_artifact``<br> - ``log_param``|
-|Cli execution|command ``kedro run``|command ``mlflow run``|
-|Code packaging|command ``kedro package``|N/A|
-|Model packaging|N/A|- ``Mlflow Models`` (``mlflow.XXX.log_model`` functions) <br> - ``Mlflow Flavours``|
-|Model service|N/A |commands ``mlflow models {serve/predict/deploy}``|
+| Functionality                  | Kedro                                             | Mlflow                                                                              |
+| :----------------------------- | :------------------------------------------------ | :---------------------------------------------------------------------------------- |
+| I/O abstraction                | various ``AbstractDataSet``                       | N/A                                                                                 |
+| I/O configuration files        | - ``catalog.yml`` <br> - ``parameters.yml``       | ``MLproject``                                                                       |
+| Compute abstraction            | - ``Pipeline`` <br> - ``Node``                    | N/A                                                                                 |
+| Compute configuration files    | - ``hooks.py`` <br> - ``run.py``                  | `MLproject`                                                                         |
+| Parameters and data versioning | - ``Journal`` <br> - ``AbstractVersionedDataSet`` | - ``log_metric``<br> - ``log_artifact``<br> - ``log_param``                         |
+| Cli execution                  | command ``kedro run``                             | command ``mlflow run``                                                              |
+| Code packaging                 | command ``kedro package``                         | N/A                                                                                 |
+| Model packaging                | N/A                                               | - ``Mlflow Models`` (``mlflow.XXX.log_model`` functions) <br> - ``Mlflow Flavours`` |
+| Model service                  | N/A                                               | commands ``mlflow models {serve/predict/deploy}``                                   |
 
 We discuss hereafter how the two libraries compete on the different functionalities and eventually complete each others.
 
 ### Configuration and prototyping: Kedro 1 - 0 Mlflow
 
 ``Mlflow`` and ``Kedro`` are essentially overlapping on the way they offer a dedicated configuration files for running the pipeline from CLI. However:  
 
@@ -43,15 +43,17 @@
 - ``Kedro`` offers a bunch of files (``catalog.yml``, ``parameters.yml``, ``pipeline.py``) and their associated abstraction (``AbstractDataSet``, ``DataCatalog``, ``Pipeline`` and ``node`` objects). ``Kedro`` is much more opinionated: each object has a dedicated place (and only one!) in the template. This makes the framework both **exploration and production oriented**. The downside is that it could make the learning curve a bit sharper since a newcomer has to learn all ``Kedro`` specifications. It also provides a ``kedro-viz`` plugin to visualize the DAG interactively, which is particularly handy in medium-to-big projects.
 
 
 > **``Kedro`` is a clear winner here, since it provides more functionnalities than ``Mlflow``. It handles very well _by design_ the exploration phase of data science projects when Mlflow is less flexible.**
 
 ### Versioning: Kedro 1 - 1 Mlflow
 
-The ``Kedro`` [``Journal`` aims at reproducibility](https://kedro.readthedocs.io/en/latest/kedro.versioning.journal.Journal.html), but is not focused on machine learning. The `Journal` keeps track of two elements:
+** This section will be updated soon with the brand new experiment tracking functionality of kedro**
+
+The ``Kedro`` ``Journal`` aimed at reproducibility (it was removed in ``kedro==0.18``), but is not focused on machine learning. The `Journal` keeps track of two elements:
 
 - the CLI arguments, including *on the fly* parameters. This makes the command used to run the pipeline fully reproducible.
 - the ``AbstractVersionedDataSet`` for which versioning is activated. It consists in copying the data whom ``versioned`` argument is ``True`` when the ``save`` method of the ``AbstractVersionedDataSet`` is called.
 This approach suffers from two main drawbacks:
   - the configuration is assumed immutable (including parameters), which is not realistic ni machine learning projects where they are very volatile. To fix this, the ``git sha`` has been recently added to the ``Journal``, but it has still some bugs in my experience (including the fact that the current ``git sha`` is logged even if the pipeline is ran with uncommitted change, which prevents reproducibility). This is still recent and will likely evolve in the future.
   - there is no support for browsing old runs, which prevents [cleaning the database with old and unused datasets](https://github.com/quantumblacklabs/kedro/issues/406), compare runs between each other...
```

### Comparing `kedro_mlflow-0.8.1/docs/source/01_introduction/02_motivation.md` & `kedro_mlflow-0.9.0/docs/source/01_introduction/02_motivation.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/02_installation/01_installation.md` & `kedro_mlflow-0.9.0/docs/source/02_installation/01_installation.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Pre-requisites
 
 ### Create a virtual environment
 
 I strongly recommend to use ``conda`` (a package manager) to create an environment in order to avoid version conflicts between packages.
 
-I also recommend to read [Kedro installation guide](https://kedro.readthedocs.io/en/latest/02_get_started/02_install.html) to set up your Kedro project.
+I also recommend to read [Kedro installation guide](https://kedro.readthedocs.io/en/latest/get_started/install.html) to set up your Kedro project.
 
 ```console
 conda create -n <your-environment-name> python=<3.[6-8].X>
 ```
 
 For the rest of the section, we assume the envirpnment is activated:
 
@@ -73,18 +73,18 @@
 v0.16.<x>
 
 kedro allows teams to create analytics
 projects. It is developed as part of
 the Kedro initiative at QuantumBlack.
 
 Installed plugins:
-kedro_mlflow: 0.8.1 (hooks:global,project)
+kedro_mlflow: 0.9.0 (hooks:global,project)
 ```
 
-The version ``0.8.1`` of the plugin is installed and has both global and project commands.
+The version ``0.9.0`` of the plugin is installed and has both global and project commands.
 
 That's it! You are now ready to go!
 
 ## Available commands
 
 With the ``kedro mlflow -h`` command outside of a kedro project, you now see the following output:
```

### Comparing `kedro_mlflow-0.8.1/docs/source/02_installation/02_setup.md` & `kedro_mlflow-0.9.0/docs/source/02_installation/02_setup.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Initialize your Kedro project
 
 This section assume that [you have installed `kedro-mlflow` in your virtual environment](./01_installation.md).
 
 ## Create a kedro project
 
-This plugin must be used in an existing kedro project. If you do not have a kedro project yet, you can create it with ``kedro new`` command. [See the kedro docs for a tutorial](https://kedro.readthedocs.io/en/latest/02_get_started/04_new_project.html).
+This plugin must be used in an existing kedro project. If you do not have a kedro project yet, you can create it with ``kedro new`` command. [See the kedro docs for a tutorial](https://kedro.readthedocs.io/en/latest/get_started/new_project.html).
 
 If you do not have a real-world project, you can use a kedro example and [follow the "Getting started" example](../03_getting_started/01_example_project.md) to make a demo of this plugin out of the box.
 
 ## Activate `kedro-mlflow` in your kedro project
 
 In order to use the ``kedro-mlflow`` plugin, you need to setup its configuration and declare its hooks. Those 2 actions are detailled in the following paragraphs.
 
@@ -38,40 +38,38 @@
 
 ```console
 kedro mlflow init --env=<other-environment>
 ```
 
 ### Declaring ``kedro-mlflow`` hooks
 
-``kedro_mlflow`` hooks implementations must be registered with Kedro. There are three ways of registering [hooks](https://kedro.readthedocs.io/en/latest/07_extend_kedro/02_hooks.html).
+``kedro_mlflow`` hooks implementations must be registered with Kedro. There are three ways of registering [hooks](https://kedro.readthedocs.io/en/latest/extend_kedro/hooks.html).
 
 **Note that you must register the two hooks provided by kedro-mlflow** (``MlflowPipelineHook`` and ``MlflowNodeHook``) for the plugin to work.
 
 #### Declaring hooks through auto-discovery (for `kedro>=0.16.4`) [Default behaviour]
 
-If you use `kedro>=0.16.4`, `kedro-mlflow` hooks are auto-registered automatically by default without any action from your side. You can [disable this behaviour](https://kedro.readthedocs.io/en/latest/07_extend_kedro/02_hooks.html#disable-auto-registered-plugins-hooks) in your `.kedro.yml` or your `pyproject.toml` file.
+If you use `kedro>=0.16.4`, `kedro-mlflow` hooks are auto-registered automatically by default without any action from your side. You can [disable this behaviour](https://kedro.readthedocs.io/en/latest/extend_kedro/hooks.html#disable-auto-registered-plugins-hooks) in your `.kedro.yml` or your `pyproject.toml` file.
 
 #### Declaring hooks through code, in ``ProjectContext`` (for `kedro>=0.16.0, <=0.16.3`)
 
 By declaring `mlflow_pipeline_hook` and `mlflow_node_hook` in ``(src/package_name/run.py) ProjectContext``:
 
 ```python
 from kedro_mlflow.framework.hooks import mlflow_pipeline_hook, mlflow_node_hook
 
+
 class ProjectContext(KedroContext):
     """Users can override the remaining methods from the parent class here,
     or create new ones (e.g. as required by plugins)
     """
 
     project_name = "<project-name>"
-    project_version = "0.16.X" # must be >=0.16.0
-    hooks = (
-        mlflow_pipeline_hook,
-        mlflow_node_hook
-    )
+    project_version = "0.16.X"  # must be >=0.16.0
+    hooks = (mlflow_pipeline_hook, mlflow_node_hook)
 ```
 
 #### Declaring hooks through static configuration in `.kedro.yml` or `pyproject.toml` **[Only for kedro >= 0.16.5 if you have disabled auto-registration]**
 
 In case you have disabled hooks for plugin, you can add them manually by declaring `mlflow_pipeline_hook` and `mlflow_node_hook` in ``.kedro.yml`` :
 
 ```yaml
```

### Comparing `kedro_mlflow-0.8.1/docs/source/02_installation/03_migration_guide.md` & `kedro_mlflow-0.9.0/docs/source/02_installation/03_migration_guide.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/03_getting_started/00_intro_tutorial.md` & `kedro_mlflow-0.9.0/docs/source/03_getting_started/00_intro_tutorial.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/03_getting_started/01_example_project.md` & `kedro_mlflow-0.9.0/docs/source/03_getting_started/01_example_project.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Example project
 
 ## Install the plugin in a virtual environment
 
 Create a conda environment and install ``kedro-mlflow`` (this will automatically install ``kedro>=0.16.0``).
 
 ```console
-conda create -n km_example python=3.6.8 --yes
+conda create -n km_example python=3.9 --yes
 conda activate km_example
-pip install kedro-mlflow==0.8.1
+pip install kedro-mlflow==0.9.0
 ```
 
 ## Install the toy project
 
-For this end to end example, we will use the [kedro starter](https://kedro.readthedocs.io/en/latest/02_get_started/06_starters.html) with the [iris dataset](https://github.com/quantumblacklabs/kedro-starter-pandas-iris).
+For this end to end example, we will use the [kedro starter](https://kedro.readthedocs.io/en/latest/get_started/starters.html) with the [iris dataset](https://github.com/quantumblacklabs/kedro-starter-pandas-iris).
 
 We use this project because:
 
 - it covers most of the common use cases
 - it is compatible with older version of ``Kedro`` so newcomers are used to it
 - it is maintained by ``Kedro`` maintainers and therefore enforces some best practices.
```

### Comparing `kedro_mlflow-0.8.1/docs/source/03_getting_started/02_first_steps.md` & `kedro_mlflow-0.9.0/docs/source/03_getting_started/02_first_steps.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 ```console
 kedro run
 ```
 
 If the pipeline executes properly, you should see the following log:
 
 ```console
-2020-07-13 21:29:24,939 - kedro.versioning.journal - WARNING - Unable to git describe path/to/km-example
 2020-07-13 21:29:25,401 - kedro.io.data_catalog - INFO - Loading data from `example_iris_data` (CSVDataSet)...
 2020-07-13 21:29:25,562 - kedro.io.data_catalog - INFO - Loading data from `params:example_test_data_ratio` (MemoryDataSet)...
 2020-07-13 21:29:25,969 - kedro.pipeline.node - INFO - Running node: split_data([example_iris_data,params:example_test_data_ratio]) -> [example_test_x,example_test_y,example_train_x,example_train_y]
 2020-07-13 21:29:26,053 - kedro.io.data_catalog - INFO - Saving data to `example_train_x` (MemoryDataSet)...
 2020-07-13 21:29:26,368 - kedro.io.data_catalog - INFO - Saving data to `example_train_y` (MemoryDataSet)...
 2020-07-13 21:29:26,484 - kedro.io.data_catalog - INFO - Saving data to `example_test_x` (MemoryDataSet)...
 2020-07-13 21:29:26,486 - kedro.io.data_catalog - INFO - Saving data to `example_test_y` (MemoryDataSet)...
```

### Comparing `kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/01_configuration.md` & `kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/01_configuration.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/02_version_parameters.md` & `kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/02_version_parameters.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ### How are parameters detected by the plugin?
 
 The hook **detects parameters through their prefix ``params:`` or the value ``parameters``**. These are the [reserved keywords used by Kedro to define parameters](https://kedro.readthedocs.io/en/stable/03_tutorial/04_create_pipelines.html?highlight=params%3A#working-with-multiple-pipelines) in the ``pipeline.py`` file(s).  
 
 ### How can I register a parameter if I use a ``TemplatedConfigLoader``?
 
-If you [use a ``TemplatedConfigLoader``](https://kedro.readthedocs.io/en/latest/04_kedro_project_setup/02_configuration.html#templating-configuration) to enable dynamic parameters contruction at runtime or dependency between configuration files, and if we assume your ``src/<project-name>/run.py`` file looks like:
+If you [use a ``TemplatedConfigLoader``](https://kedro.readthedocs.io/en/latest/kedro_project_setup/configuration.html#templating-configuration) to enable dynamic parameters contruction at runtime or dependency between configuration files, and if we assume your ``src/<project-name>/run.py`` file looks like:
 
 ```python
 from kedro.config import TemplatedConfigLoader  # new import
 from datetime import date
 
 
 class ProjectContext(KedroContext):
```

### Comparing `kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/03_version_datasets.md` & `kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/03_version_datasets.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/04_version_models.md` & `kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/04_version_models.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/05_version_metrics.md` & `kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/05_version_metrics.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/04_experimentation_tracking/06_mlflow_ui.md` & `kedro_mlflow-0.9.0/docs/source/04_experimentation_tracking/06_mlflow_ui.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/05_framework_ml/01_why_framework.md` & `kedro_mlflow-0.9.0/docs/source/05_framework_ml/01_why_framework.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/05_framework_ml/02_ml_project_components.md` & `kedro_mlflow-0.9.0/docs/source/05_framework_ml/02_ml_project_components.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/05_framework_ml/03_framework_solutions.md` & `kedro_mlflow-0.9.0/docs/source/05_framework_ml/03_framework_solutions.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/01_mlflow_models.md` & `kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/01_mlflow_models.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/02_custom_kedro_pipeline_model.md` & `kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/02_custom_kedro_pipeline_model.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/03_cli_modelify.md` & `kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/03_cli_modelify.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/05_pipeline_serving/04_hook_pipeline_ml.md` & `kedro_mlflow-0.9.0/docs/source/05_pipeline_serving/04_hook_pipeline_ml.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/06_interactive_use/01_notebook_use.md` & `kedro_mlflow-0.9.0/docs/source/06_interactive_use/01_notebook_use.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 Open your notebook / ipython session with the Kedro CLI:
 
 ```bash
 kedro jupyter notebook
 ```
 
-Kedro [creates a bunch of global variables](https://kedro.readthedocs.io/en/latest/11_tools_integration/02_ipython.html#kedro-and-jupyter), including a `session` which are automatically accessible. It also registers some line_magic from plugins, including `%=reload_kedro_mlflow` from `kedro-mlflow`.
+Kedro [creates a bunch of global variables](https://kedro.readthedocs.io/en/latest/tools_integration/ipython.html#kedro-and-jupyter), including a `session` which are automatically accessible. It also registers some line_magic from plugins, including `%=reload_kedro_mlflow` from `kedro-mlflow`.
 
 In your first cell, launch:
-```python
+```
 %reload_kedro_mlflow
 ```
 
 This automatically:
 - load and setup (create the tracking uri, export credentials...) the mlflow configuration of your `mlflow.yml`
 - import ``mlflow`` which is now accessible in your notebook
 - Create a `mlflow_client` object with your mlflow server settings, which is now accessible in your notebook
@@ -38,33 +38,33 @@
 
 ## Difference with running through the CLI
 
 - The DataSets `load` and `save` methods works as usual. You can call `catalog.save("my_artifact_dataset", data)` inside a cell, and your data will be logged in mlflow properly (assuming "my_artifact_dataset" is a `kedro_mlflow.io.MlflowArtifactDataSet`).
 - The `hooks` which setup configuration are only accessible if you run the session interactive, e.g.:
 ```python
 session.run(
-    pipeline_name = "my_ml_pipeline",
-    tags = "training",
-    from_inputs = "data_2",
-    to_outputs = "data_7"
-    )
+    pipeline_name="my_ml_pipeline",
+    tags="training",
+    from_inputs="data_2",
+    to_outputs="data_7",
+)
 ```
 but it is not very likely in a notebook.
 
 ## Guidelines and best practices suggestions
 
 During experimentation phase, you will likely not run entire pipelines (or sub pipelines filtered out between some inputs and outputs). Hence, you cannot benefit from Kedro's ``hooks`` (and hence from ``kedro-mlflow`` tracking). From this moment on, perfect reproducbility is impossible to achieve: there is no chance that you manage to maintain a perfectly linear workflow, as you will go back and forth modifying parameters and code to create your model.
 
 I suggest to :
 - **focus on versioning parameters and metrics**. The goal is to finetune your hyperparameters and to be able to remember later the best setup. It is not very important to this stage to version all parameters (e.g. preprocessing ones) nor models (after all you will need an entire pipeline to predict and it is very unlikely that you will need to reuse these experiment models one day.) It may be interesting to use ``mlflow.autolog()`` feature to have a easy basic setup.
 - **transition quickly to kedro pipelines**. For instance, when you preprocessing is roughly defined, try to put it in kedro pipelines. You can then use notebooks to experiment / perfom hyperparameter tuning while keeping preprocessing "fixed" to enhance reproducibility. You can run this pipeline interactively with :
 
 ```python
-res=session.run(
-    pipeline_name = "my_preprocessing_pipeline",
-    tags = "training",
-    from_inputs = "data_2",
-    to_outputs = "data_7"
-    )
+res = session.run(
+    pipeline_name="my_preprocessing_pipeline",
+    tags="training",
+    from_inputs="data_2",
+    to_outputs="data_7",
+)
 ```
 
 ``res`` is a python dict with the outputs of your pipeline (e.g. a "preprocessed_data" ``pandas.DataFrame``), and you can use it interactively in your notebook.
```

### Comparing `kedro_mlflow-0.8.1/docs/source/07_python_objects/01_DataSets.md` & `kedro_mlflow-0.9.0/docs/source/07_python_objects/01_DataSets.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/07_python_objects/02_Hooks.md` & `kedro_mlflow-0.9.0/docs/source/07_python_objects/02_Hooks.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/07_python_objects/03_Pipelines.md` & `kedro_mlflow-0.9.0/docs/source/07_python_objects/03_Pipelines.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/07_python_objects/04_CLI.md` & `kedro_mlflow-0.9.0/docs/source/07_python_objects/04_CLI.md`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/08_API/kedro_mlflow.io.rst` & `kedro_mlflow-0.9.0/docs/source/08_API/kedro_mlflow.io.rst`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/apps_interaction.png` & `kedro_mlflow-0.9.0/docs/source/imgs/apps_interaction.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/default_catalog.png` & `kedro_mlflow-0.9.0/docs/source/imgs/default_catalog.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/etl_app.png` & `kedro_mlflow-0.9.0/docs/source/imgs/etl_app.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/hook_registration_process.png` & `kedro_mlflow-0.9.0/docs/source/imgs/hook_registration_process.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/initialized_project.png` & `kedro_mlflow-0.9.0/docs/source/imgs/initialized_project.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/kedro_viz_params.png` & `kedro_mlflow-0.9.0/docs/source/imgs/kedro_viz_params.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/preprocessing/all.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/preprocessing/all.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/preprocessing/inference.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/preprocessing/inference.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/preprocessing/training.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/preprocessing/training.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/shared_inputs/all.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/shared_inputs/all.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/shared_inputs/inference.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/shared_inputs/inference.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/shared_inputs/training.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/shared_inputs/training.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/tokenizer/all.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/tokenizer/all.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/tokenizer/inference.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/tokenizer/inference.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/tokenizer/training.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/tokenizer/training.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/vanilla/all.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/vanilla/all.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/vanilla/inference.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/vanilla/inference.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/ml_pipeline/vanilla/training.PNG` & `kedro_mlflow-0.9.0/docs/source/imgs/ml_pipeline/vanilla/training.PNG`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/mlflow_host_page.png` & `kedro_mlflow-0.9.0/docs/source/imgs/mlflow_host_page.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/mlflow_run.png` & `kedro_mlflow-0.9.0/docs/source/imgs/mlflow_run.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/mlflow_tracking_schema.png` & `kedro_mlflow-0.9.0/docs/source/imgs/mlflow_tracking_schema.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/mlflow_yml.png` & `kedro_mlflow-0.9.0/docs/source/imgs/mlflow_yml.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/once_run_project.png` & `kedro_mlflow-0.9.0/docs/source/imgs/once_run_project.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/run_with_artifact.png` & `kedro_mlflow-0.9.0/docs/source/imgs/run_with_artifact.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/docs/source/imgs/updated_catalog.png` & `kedro_mlflow-0.9.0/docs/source/imgs/updated_catalog.png`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/config/kedro_mlflow_config.py` & `kedro_mlflow-0.9.0/kedro_mlflow/config/kedro_mlflow_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 from pathlib import Path, PurePath
 from typing import Dict, List, Optional
 from urllib.parse import urlparse
 
+import kedro.framework.session.session as kfss  # necessary to access the global variable _active_session of the namespace
 import mlflow
 from kedro.config import MissingConfigException
-from kedro.framework.session import KedroSession, get_current_session
+from kedro.framework.session import KedroSession  # , get_current_session
 from kedro.framework.startup import _is_project
 from mlflow.entities import Experiment
 from mlflow.tracking.client import MlflowClient
 from pydantic import BaseModel, PrivateAttr, StrictBool, validator
 from typing_extensions import Literal
 
 
@@ -120,15 +121,15 @@
         # we set the configuration now: it takes priority
         # if it has already be set in export_credentials
         mlflow.set_tracking_uri(self.server.mlflow_tracking_uri)
 
         self._set_experiment()
 
     def _export_credentials(self, session: KedroSession = None):
-        session = session or get_current_session()
+        session = session or _get_current_session()
         context = session.load_context()
         conf_creds = context._get_config_credentials()
         mlflow_creds = conf_creds.get(self.server.credentials, {})
         for key, value in mlflow_creds.items():
             os.environ[key] = value
 
     def _set_experiment(self):
@@ -212,18 +213,35 @@
 
 
 class KedroMlflowConfigError(Exception):
     """Error occurred when loading the configuration"""
 
 
 def get_mlflow_config(session: Optional[KedroSession] = None):
-    session = session or get_current_session()
+    session = session or _get_current_session()
     context = session.load_context()
     try:
-        conf_mlflow_yml = context.config_loader.get("mlflow*", "mlflow*/**")
+        conf_mlflow_yml = context._config_loader.get("mlflow*", "mlflow*/**")
     except MissingConfigException:
         raise KedroMlflowConfigError(
             "No 'mlflow.yml' config file found in environment. Use ``kedro mlflow init`` command in CLI to create a default config file."
         )
     conf_mlflow_yml["project_path"] = context.project_path
     mlflow_config = KedroMlflowConfig.parse_obj(conf_mlflow_yml)
     return mlflow_config
+
+
+def _get_current_session(silent: bool = False) -> Optional["KedroSession"]:
+    """Fetch the active ``KedroSession`` instance.
+    Args:
+        silent: Indicates to suppress the error if no active session was found.
+    Raises:
+        RuntimeError: If no active session was found and `silent` is False.
+    Returns:
+        KedroSession instance.
+    """
+
+    # _active_session is a global variable from kedro itself
+    if not kfss._active_session and not silent:
+        raise RuntimeError("There is no active Kedro session.")
+
+    return kfss._active_session
```

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/extras/extensions/ipython.py` & `kedro_mlflow-0.9.0/kedro_mlflow/extras/extensions/ipython.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/framework/cli/cli.py` & `kedro_mlflow-0.9.0/kedro_mlflow/framework/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from logging import getLogger
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Dict, Optional, Union
 
 import click
 import mlflow
-from kedro.framework.project import pipelines
+from kedro.framework.project import pipelines, settings
 from kedro.framework.session import KedroSession
 from kedro.framework.startup import _is_project, bootstrap_project
 from mlflow.models import infer_signature
 from packaging import version
 
 from kedro_mlflow.config import get_mlflow_config
 from kedro_mlflow.framework.cli.cli_utils import write_jinja_template
@@ -84,17 +84,15 @@
     used for run parametrization when calling "kedro run" command.
     """
 
     # get constants
     mlflow_yml = "mlflow.yml"
     project_path = Path().cwd()
     project_metadata = bootstrap_project(project_path)
-    session = KedroSession.create(project_path=project_path)
-    context = session.load_context()
-    mlflow_yml_path = project_path / context.CONF_ROOT / env / mlflow_yml
+    mlflow_yml_path = project_path / settings.CONF_SOURCE / env / mlflow_yml
 
     # mlflow.yml is just a static file,
     # but the name of the experiment is set to be the same as the project
     if mlflow_yml_path.is_file() and not force:
         click.secho(
             click.style(
                 f"A 'mlflow.yml' already exists at '{mlflow_yml_path}' You can use the ``--force`` option to override it.",
@@ -108,22 +106,22 @@
                 is_cookiecutter=False,
                 dst=mlflow_yml_path,
                 python_package=project_metadata.package_name,
             )
         except FileNotFoundError:
             click.secho(
                 click.style(
-                    f"No env '{env}' found. Please check this folder exists inside '{context.CONF_ROOT}' folder.",
+                    f"No env '{env}' found. Please check this folder exists inside '{settings.CONF_SOURCE}' folder.",
                     fg="red",
                 )
             )
         if not silent:
             click.secho(
                 click.style(
-                    f"'{context.CONF_ROOT}/{env}/{mlflow_yml}' successfully updated.",
+                    f"'{settings.CONF_SOURCE}/{env}/{mlflow_yml}' successfully updated.",
                     fg="green",
                 )
             )
 
 
 @mlflow_commands.command()
 @click.option(
```

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/framework/cli/cli_utils.py` & `kedro_mlflow-0.9.0/kedro_mlflow/framework/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/node_hook.py` & `kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/node_hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ) -> None:
         """Hook to be invoked before a pipeline runs.
         Args:
             run_params: The params needed for the given run.
                 Should be identical to the data logged by Journal.
                 # @fixme: this needs to be modelled explicitly as code, instead of comment
                 Schema: {
-                    "run_id": str,
                     "project_path": str,
                     "env": str,
                     "kedro_version": str,
                     "tags": Optional[List[str]],
                     "from_nodes": Optional[List[str]],
                     "to_nodes": Optional[List[str]],
                     "node_names": Optional[List[str]],
@@ -60,29 +59,23 @@
             self.sep = mlflow_config.tracking.params.dict_params.sep
             self.long_params_strategy = (
                 mlflow_config.tracking.params.long_params_strategy
             )
 
     @hook_impl
     def before_node_run(
-        self,
-        node: Node,
-        catalog: DataCatalog,
-        inputs: Dict[str, Any],
-        is_async: bool,
-        run_id: str,
+        self, node: Node, catalog: DataCatalog, inputs: Dict[str, Any], is_async: bool
     ) -> None:
         """Hook to be invoked before a node runs.
         This hook logs all the parameters of the nodes in mlflow.
         Args:
             node: The ``Node`` to run.
             catalog: A ``DataCatalog`` containing the node's inputs and outputs.
             inputs: The dictionary of inputs dataset.
             is_async: Whether the node was run in ``async`` mode.
-            run_id: The id of the run.
         """
 
         # only parameters will be logged. Artifacts must be declared manually in the catalog
         if self._is_mlflow_enabled:
             params_inputs = {}
             for k, v in inputs.items():
                 # detect parameters automatically based on kedro reserved names
```

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/pipeline_hook.py` & `kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/pipeline_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from tempfile import TemporaryDirectory
 from typing import Any, Dict
 
 import mlflow
 from kedro.framework.hooks import hook_impl
 from kedro.io import DataCatalog
 from kedro.pipeline import Pipeline
-from kedro.versioning.journal import _git_sha
 from mlflow.entities import RunStatus
 from mlflow.models import infer_signature
 
 from kedro_mlflow.config import get_mlflow_config
 from kedro_mlflow.framework.hooks.utils import _assert_mlflow_enabled
 from kedro_mlflow.io.catalog.switch_catalog_logging import switch_catalog_logging
 from kedro_mlflow.io.metrics import (
@@ -32,15 +31,14 @@
         self,
         catalog: DataCatalog,
         conf_catalog: Dict[str, Any],
         conf_creds: Dict[str, Any],
         feed_dict: Dict[str, Any],
         save_version: str,
         load_versions: str,
-        run_id: str,
     ):
 
         for name, dataset in catalog._data_sets.items():
 
             if isinstance(dataset, MlflowMetricsDataSet) and dataset._prefix is None:
                 if dataset._run_id is not None:
                     catalog._data_sets[name] = MlflowMetricsDataSet(
@@ -85,15 +83,14 @@
     ) -> None:
         """Hook to be invoked before a pipeline runs.
         Args:
             run_params: The params needed for the given run.
                 Should be identical to the data logged by Journal.
                 # @fixme: this needs to be modelled explicitly as code, instead of comment
                 Schema: {
-                    "run_id": str,
                     "project_path": str,
                     "env": str,
                     "kedro_version": str,
                     "tags": Optional[List[str]],
                     "from_nodes": Optional[List[str]],
                     "to_nodes": Optional[List[str]],
                     "node_names": Optional[List[str]],
@@ -120,15 +117,15 @@
                 nested=mlflow_config.tracking.run.nested,
             )
             # Set tags only for run parameters that have values.
             mlflow.set_tags({k: v for k, v in run_params.items() if v})
             # add manually git sha for consistency with the journal
             # TODO : this does not take into account not committed files, so it
             # does not ensure reproducibility. Define what to do.
-            mlflow.set_tag("git_sha", _git_sha(run_params["project_path"]))
+
             mlflow.set_tag(
                 "kedro_command",
                 _generate_kedro_command(
                     tags=run_params["tags"],
                     node_names=run_params["node_names"],
                     from_nodes=run_params["from_nodes"],
                     to_nodes=run_params["to_nodes"],
@@ -152,15 +149,14 @@
     ) -> None:
         """Hook to be invoked after a pipeline runs.
         Args:
             run_params: The params needed for the given run.
                 Should be identical to the data logged by Journal.
                 # @fixme: this needs to be modelled explicitly as code, instead of comment
                 Schema: {
-                    "run_id": str,
                     "project_path": str,
                     "env": str,
                     "kedro_version": str,
                     "tags": Optional[List[str]],
                     "from_nodes": Optional[List[str]],
                     "to_nodes": Optional[List[str]],
                     "node_names": Optional[List[str]],
@@ -218,15 +214,14 @@
 
         Args:
             error: (Not used) The uncaught exception thrown during the pipeline run.
             run_params: (Not used) The params used to run the pipeline.
                 Should be identical to the data logged by Journal with the following schema::
 
                    {
-                     "run_id": str
                      "project_path": str,
                      "env": str,
                      "kedro_version": str,
                      "tags": Optional[List[str]],
                      "from_nodes": Optional[List[str]],
                      "to_nodes": Optional[List[str]],
                      "node_names": Optional[List[str]],
```

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/framework/hooks/utils.py` & `kedro_mlflow-0.9.0/kedro_mlflow/framework/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/artifacts/mlflow_artifact_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/artifacts/mlflow_artifact_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_abstract_metric_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_abstract_metric_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_metric_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_metric_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_metric_history_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_metric_history_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/metrics/mlflow_metrics_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/metrics/mlflow_metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/models/mlflow_abstract_model_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/models/mlflow_abstract_model_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/models/mlflow_model_logger_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/models/mlflow_model_logger_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/io/models/mlflow_model_saver_dataset.py` & `kedro_mlflow-0.9.0/kedro_mlflow/io/models/mlflow_model_saver_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/mlflow/kedro_pipeline_model.py` & `kedro_mlflow-0.9.0/kedro_mlflow/mlflow/kedro_pipeline_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 from kedro.extras.datasets.pickle import PickleDataSet
+from kedro.framework.hooks import _create_hook_manager
 from kedro.io import DataCatalog, MemoryDataSet
 from kedro.pipeline import Pipeline
 from kedro.runner import AbstractRunner, SequentialRunner
 from mlflow.pyfunc import PythonModel
 
 from kedro_mlflow.pipeline.pipeline_ml import PipelineML
 
@@ -206,21 +207,27 @@
             updated_catalog._data_sets[name]._filepath = Path(uri)
             self.loaded_catalog.save(name=name, data=updated_catalog.load(name))
 
     def predict(self, context, model_input):
         # TODO : checkout out how to pass extra args in predict
         # for instance, to enable parallelization
 
+        # we create an empty hook manager but do NOT register hooks
+        # because we want this model be executable outside of a kedro project
+        hook_manager = _create_hook_manager()
+
         self.loaded_catalog.save(
             name=self.input_name,
             data=model_input,
         )
 
         run_output = self.runner.run(
-            pipeline=self.pipeline, catalog=self.loaded_catalog
+            pipeline=self.pipeline,
+            catalog=self.loaded_catalog,
+            hook_manager=hook_manager,
         )
 
         # unpack the result to avoid messing the json
         # file with the name of the Kedro dataset
         unpacked_output = run_output[self.output_name]
 
         return unpacked_output
```

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/pipeline/pipeline_ml.py` & `kedro_mlflow-0.9.0/kedro_mlflow/pipeline/pipeline_ml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Dict, Iterable, Optional, Union
+from typing import Dict, Iterable, Optional, Union
 
 from kedro.pipeline import Pipeline
 from kedro.pipeline.node import Node
 
 MSG_NOT_IMPLEMENTED = (
     "This method is not implemented because it does"
     "not make sense for 'PipelineML'."
@@ -166,18 +166,26 @@
         return None
 
     def _turn_pipeline_to_ml(self, pipeline: Pipeline):
         return PipelineML(
             nodes=pipeline.nodes, inference=self.inference, input_name=self.input_name
         )
 
+    def only_nodes(self, *node_names: str) -> "Pipeline":  # pragma: no cover
+        raise NotImplementedError(MSG_NOT_IMPLEMENTED)
+
+    def only_nodes_with_namespace(
+        self, node_namespace: str
+    ) -> "Pipeline":  # pragma: no cover
+        raise NotImplementedError(MSG_NOT_IMPLEMENTED)
+
     def only_nodes_with_inputs(self, *inputs: str) -> "PipelineML":  # pragma: no cover
         raise NotImplementedError(MSG_NOT_IMPLEMENTED)
 
-    def from_inputs(self, *inputs: str) -> "PipelineML":
+    def from_inputs(self, *inputs: str) -> "PipelineML":  # pragma: no cover
         # exceptionnally, we don't call super() because it raises
         # a self._check_degrees_of_freedom() error even if valid cases
         # this is because the pipeline is reconstructed node by node
         # (only the first node may lead to invalid pipeline (e.g.
         # with not all artifacts)), even if the whole pipeline is ok
         # we want the call to self._check_degrees_of_freedom() only call at the end.
         pipeline = self.training.from_inputs(*inputs)
@@ -185,46 +193,66 @@
 
     def only_nodes_with_outputs(
         self, *outputs: str
     ) -> "PipelineML":  # pragma: no cover
         raise NotImplementedError(MSG_NOT_IMPLEMENTED)
 
     def to_outputs(self, *outputs: str) -> "PipelineML":  # pragma: no cover
-        raise NotImplementedError(MSG_NOT_IMPLEMENTED)
+        # see from_inputs for an explanation of why we don't call super()
+        pipeline = self.training.from_nodes(*outputs)
+        return self._turn_pipeline_to_ml(pipeline)
 
-    def from_nodes(self, *node_names: str) -> "PipelineML":
+    def from_nodes(self, *node_names: str) -> "PipelineML":  # pragma: no cover
         # see from_inputs for an explanation of why we don't call super()
         pipeline = self.training.from_nodes(*node_names)
         return self._turn_pipeline_to_ml(pipeline)
 
-    def to_nodes(self, *node_names: str) -> "PipelineML":
+    def to_nodes(self, *node_names: str) -> "PipelineML":  # pragma: no cover
         # see from_inputs for an explanation of why we don't call super()
         pipeline = self.training.to_nodes(*node_names)
         return self._turn_pipeline_to_ml(pipeline)
 
-    def only_nodes_with_tags(self, *tags: str) -> "PipelineML":
+    def only_nodes_with_tags(self, *tags: str) -> "PipelineML":  # pragma: no cover
         # see from_inputs for an explanation of why we don't call super()
         pipeline = self.training.only_nodes_with_tags(*tags)
         return self._turn_pipeline_to_ml(pipeline)
 
-    def decorate(self, *decorators: Callable) -> "PipelineML":
-        pipeline = super().decorate(*decorators)
-        return self._turn_pipeline_to_ml(pipeline)
-
     def tag(self, tags: Union[str, Iterable[str]]) -> "PipelineML":
         pipeline = super().tag(*tags)
         return self._turn_pipeline_to_ml(pipeline)
 
+    def filter(
+        self,
+        tags: Iterable[str] = None,
+        from_nodes: Iterable[str] = None,
+        to_nodes: Iterable[str] = None,
+        node_names: Iterable[str] = None,
+        from_inputs: Iterable[str] = None,
+        to_outputs: Iterable[str] = None,
+        node_namespace: str = None,
+    ) -> "Pipeline":
+        # see from_inputs for an explanation of why we don't call super()
+        pipeline = self.training.filter(
+            tags=tags,
+            from_nodes=from_nodes,
+            to_nodes=to_nodes,
+            node_names=node_names,
+            from_inputs=from_inputs,
+            to_outputs=to_outputs,
+            node_namespace=node_namespace,
+        )
+        return self._turn_pipeline_to_ml(pipeline)
+
     def __add__(self, other):  # pragma: no cover
         raise NotImplementedError(MSG_NOT_IMPLEMENTED)
 
     def __sub__(self, other):  # pragma: no cover
         raise NotImplementedError(MSG_NOT_IMPLEMENTED)
 
-    def __and__(self, other):
+    def __and__(self, other):  # pragma: no cover
         # kept for compatibility with KedroContext _filter_pipelinefunction
         new_pipeline = super().__and__(other)
         return self._turn_pipeline_to_ml(new_pipeline)
 
     def __or__(self, other):  # pragma: no cover
         raise NotImplementedError(MSG_NOT_IMPLEMENTED)
```

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/pipeline/pipeline_ml_factory.py` & `kedro_mlflow-0.9.0/kedro_mlflow/pipeline/pipeline_ml_factory.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow/template/project/mlflow.yml` & `kedro_mlflow-0.9.0/kedro_mlflow/template/project/mlflow.yml`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow.egg-info/PKG-INFO` & `kedro_mlflow-0.9.0/kedro_mlflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: kedro-mlflow
-Version: 0.8.1
+Version: 0.9.0
 Summary: A kedro-plugin to use mlflow in your kedro projects
 Home-page: https://github.com/Galileo-Galilei/kedro-mlflow
 Author: Yolan Honoré-Rougé
 License: Apache Software License (Apache 2.0)
 Description: **General informations**
         
-        [![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg)](https://pypi.org/project/kedro-mlflow/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+        [![Python Version](https://img.shields.io/pypi/pyversions/kedro-mlflow)](https://pypi.org/project/kedro-mlflow/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
         [![SemVer](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
         
         ----------------------------------------------------------
-        | Software repository | Latest release                                                                                       | Total downloads                                                                              |
-        | ------------------- | ---------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
-        | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-mlflow.svg)](https://pypi.org/project/kedro-mlflow/) | [![Downloads](https://pepy.tech/badge/kedro-mlflow)](https://pepy.tech/project/kedro-mlflow) |
+        | Package manager | Software repository | Latest release                                                                                                                                | Total downloads                                                                                                                 |
+        | --------------- | ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
+        | ``pip``         | PyPI                | [![PyPI version](https://badge.fury.io/py/kedro-mlflow.svg)](https://pypi.org/project/kedro-mlflow/)                                          | [![Downloads](https://pepy.tech/badge/kedro-mlflow)](https://pepy.tech/project/kedro-mlflow)                                    |
+        | ``conda``       | conda-forge         | [![conda version](https://img.shields.io/conda/vn/conda-forge/kedro-mlflow?color=bright%20green)](https://anaconda.org/search?q=kedro+mlflow) | [![Downloads](https://img.shields.io/conda/dn/conda-forge/kedro-mlflow?color=blue)](https://anaconda.org/search?q=kedro+mlflow) |
         
         **Code health**
         
         ----------------------------------------------------------
         | Branch   | Tests                                                                                                                                                                                            | Coverage                                                                                                                                                         | Links                                                                                                                                                                                                           | Documentation                                                                                                                           | Deployment                                                                                                                                                                                                | Activity                                                                                                                                                            |
         | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | `master` | [![test](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/test/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Atest+branch%3Amaster) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master) | [![links](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/check-links/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Acheck-links+branch%3Amaster) | [![Documentation](https://readthedocs.org/projects/kedro-mlflow/badge/?version=stable)](https://kedro-mlflow.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/publish/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=branch%3Amaster+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-mlflow/0.8.1)](https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.8.1...master) |
+        | `master` | [![test](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/test/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Atest+branch%3Amaster) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-mlflow/branch/master) | [![links](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/check-links/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=workflow%3Acheck-links+branch%3Amaster) | [![Documentation](https://readthedocs.org/projects/kedro-mlflow/badge/?version=stable)](https://kedro-mlflow.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-mlflow/workflows/publish/badge.svg?branch=master)](https://github.com/Galileo-Galilei/kedro-mlflow/actions?query=branch%3Amaster+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-mlflow/0.9.0)](https://github.com/Galileo-Galilei/kedro-mlflow/compare/0.9.0...master) |
         
         # What is kedro-mlflow?
         
-        ``kedro-mlflow`` is a [kedro-plugin](https://kedro.readthedocs.io/en/stable/07_extend_kedro/04_plugins.html) for lightweight and portable integration of [mlflow](https://mlflow.org/docs/latest/index.html) capabilities inside [kedro](https://kedro.readthedocs.io/en/stable/index.html) projects. It enforces [``Kedro`` principles](https://kedro.readthedocs.io/en/stable/12_faq/01_faq.html?highlight=principles#what-is-the-philosophy-behind-kedro) to make mlflow usage as production ready as possible. Its core functionalities are :
+        ``kedro-mlflow`` is a [kedro-plugin](https://kedro.readthedocs.io/en/stable/extend_kedro/plugins.html) for lightweight and portable integration of [mlflow](https://mlflow.org/docs/latest/index.html) capabilities inside [kedro](https://kedro.readthedocs.io/en/stable/index.html) projects. It enforces [``Kedro`` principles](https://kedro.readthedocs.io/en/stable/12_faq/01_faq.html?highlight=principles#what-is-the-philosophy-behind-kedro) to make mlflow usage as production ready as possible. Its core functionalities are :
         
         - **versioning**: `kedro-mlflow` intends to enhance reproducibility for machine learning experimentation. With `kedro-mlflow` installed, you can effortlessly register your parameters or your datasets with minimal configuration in a kedro run. Later, you will be able to browse your runs in the mlflow UI, and retrieve the runs you want. This is directly linked to [Mlflow Tracking](https://www.mlflow.org/docs/latest/tracking.html).
         - **model packaging**: ``kedro-mlflow`` intends to be be an agnostic machine learning framework for people who want to write portable, production ready machine learning pipelines. It offers a convenient API to convert a Kedro pipeline to a ``model`` in the mlflow sense. Consequently, you can *API-fy* or serve your Kedro pipeline with one line of code, or share a model with without worrying of the preprocessing to be made for further use. This is directly linked to [Mlflow Models](https://www.mlflow.org/docs/latest/models.html).
         
         # How do I install kedro-mlflow?
         
         **Important: ``kedro-mlflow`` is only compatible with ``kedro>=0.16.0`` and ``mlflow>=1.0.0``. If you have a project created with an older version of ``Kedro``, see this [migration guide](https://github.com/quantumblacklabs/kedro/blob/master/RELEASE.md#migration-guide-from-kedro-015-to-016).**
@@ -41,15 +42,15 @@
         
         If you want to use the most up to date version of the package which is under development and not released yet, you can install the package from github:
         
         ```console
         pip install --upgrade git+https://github.com/Galileo-Galilei/kedro-mlflow.git
         ```
         
-        I strongly recommend to use ``conda`` (a package manager) to create an environment and to read [``kedro`` installation guide](https://kedro.readthedocs.io/en/latest/02_get_started/02_install.html).
+        I strongly recommend to use ``conda`` (a package manager) to create an environment and to read [``kedro`` installation guide](https://kedro.readthedocs.io/en/latest/get_started/install.html).
         
         # Getting started
         
         The documentation contains:
         
         - [A  "hello world" example](https://kedro-mlflow.readthedocs.io/en/latest/source/03_getting_started/index.html) which demonstrates how you to **setup your project**, **version parameters** and **datasets**, and browse your runs in the UI.
         - A section for [advanced machine learning versioning](https://kedro-mlflow.readthedocs.io/en/latest/source/04_experimentation_tracking/index.html) to show more advanced features (mlflow configuration through the plugin, package and serve a kedro ``Pipeline``...)
@@ -87,23 +88,24 @@
         - [Takieddine Kadiri](https://github.com/takikadiri)
         
         Many thanks to [Adrian Piotr Kruszewski](https://github.com/akruszewski) for his past work on the repo.
         
 Keywords: kedro-plugin,mlflow,model versioning,model packaging,pipelines,machine learning,data pipelines,data science,data engineering
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Kedro
 Classifier: Environment :: Plugins
 Classifier: Framework :: Kedro
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6, <3.9
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: extras
```

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow.egg-info/SOURCES.txt` & `kedro_mlflow-0.9.0/kedro_mlflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/kedro_mlflow.egg-info/requires.txt` & `kedro_mlflow-0.9.0/kedro_mlflow.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-kedro<0.18.0,>=0.17.1
+kedro<0.19.0,>=0.18.0
 mlflow<2.0.0,>=1.0.0
 pydantic<2.0.0,>=1.0.0
 
 [dev]
 pre-commit<3.0.0,>=2.0.0
 jupyter<2.0.0,>=1.0.0
 
 [doc]
-sphinx==4.4.0
+sphinx<5.0.0,>=4.5.0
 recommonmark==0.7.1
 sphinx_rtd_theme==1.0.0
 sphinx-markdown-tables==0.0.15
 sphinx-click==3.1.0
 sphinx_copybutton==0.5.0
 pandas<2.0.0,>=1.0.0
 numpy<2.0.0,>=1.0.0
@@ -22,9 +22,9 @@
 [test]
 pytest<8.0.0,>=5.4.0
 pytest-cov<4.0.0,>=2.8.0
 pytest-lazy-fixture<1.0.0,>=0.6.0
 pytest-mock<4.0.0,>=3.1.0
 scikit-learn<1.1.0,>=0.23.0
 flake8==4.0.1
-black==21.10b0
+black==22.3
 isort==5.10.1
```

### Comparing `kedro_mlflow-0.8.1/setup.cfg` & `kedro_mlflow-0.9.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.1
+current_version = 0.9.0
 
 [tool:pytest]
 addopts = --cov=kedro_mlflow --cov-report=html tests/
 
 [flake8]
 ignore = E203, E266, E501, W503
 max-line-length = 88
@@ -13,21 +13,15 @@
 
 [bumpversion:file:setup.py]
 
 [bumpversion:file:kedro_mlflow/__init__.py]
 
 [bumpversion:file:README.md]
 
-[bumpversion:file:docs/source/01_introduction/02_motivation.md]
-
 [bumpversion:file:docs/source/02_installation/01_installation.md]
 
 [bumpversion:file:docs/source/03_getting_started/01_example_project.md]
 
-[bumpversion:file:docs/source/04_experimentation_tracking/02_version_parameters.md]
-
-[bumpversion:file:docs/source/04_experimentation_tracking/03_version_datasets.md]
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `kedro_mlflow-0.8.1/setup.py` & `kedro_mlflow-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 # Get the long description from the README file
 with open((HERE / "README.md").as_posix(), encoding="utf-8") as file_handler:
     README = file_handler.read()
 
 
 setup(
     name=NAME,
-    version="0.8.1",  # this will be bumped automatically by bump2version
+    version="0.9.0",  # this will be bumped automatically by bump2version
     description="A kedro-plugin to use mlflow in your kedro projects",
     license="Apache Software License (Apache 2.0)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Galileo-Galilei/kedro-mlflow",
-    python_requires=">=3.6, <3.9",
+    python_requires=">=3.7, <3.11",
     packages=find_packages(exclude=["docs*", "tests*"]),
     setup_requires=["setuptools_scm"],
     include_package_data=True,
     install_requires=base_requirements,
     extras_require={
         "doc": [
-            "sphinx==4.4.0",
+            "sphinx>=4.5.0,<5.0.0",
             "recommonmark==0.7.1",
             "sphinx_rtd_theme==1.0.0",
             "sphinx-markdown-tables==0.0.15",
             "sphinx-click==3.1.0",
             "sphinx_copybutton==0.5.0",
             "pandas>=1.0.0, <2.0.0",  # avoid to make readthedocs load rc version
             "numpy>=1.0.0, <2.0.0",  # bug on windows for numpy 1.19.0->1.19.4
@@ -50,15 +50,15 @@
         "test": [
             "pytest>=5.4.0, <8.0.0",
             "pytest-cov>=2.8.0, <4.0.0",
             "pytest-lazy-fixture>=0.6.0, <1.0.0",
             "pytest-mock>=3.1.0, <4.0.0",
             "scikit-learn>=0.23.0, <1.1.0",
             "flake8==4.0.1",  # ensure consistency with pre-commit
-            "black==21.10b0",  # pin black version because it is not compatible with a pip range (because of non semver version number)
+            "black==22.3",  # pin black version because it is not compatible with a pip range (because of non semver version number)
             "isort==5.10.1",  # ensure consistency with pre-commit
         ],
         "dev": [
             "pre-commit>=2.0.0,<3.0.0",
             "jupyter>=1.0.0,<2.0.0",
         ],
         "extras": ["notebook>=6.0.0"],
@@ -79,17 +79,18 @@
             "line_magic = kedro_mlflow.extras.extensions.ipython:reload_kedro_mlflow"
         ],
     },
     zip_safe=False,
     keywords="kedro-plugin, mlflow, model versioning, model packaging, pipelines, machine learning, data pipelines, data science, data engineering",
     classifiers=[
         "Development Status :: 4 - Beta",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Framework :: Kedro",
         "Environment :: Plugins",
         "Framework :: Kedro",
         "Intended Audience :: Developers",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
```

### Comparing `kedro_mlflow-0.8.1/tests/config/test_kedro_mlflow_config.py` & `kedro_mlflow-0.9.0/tests/config/test_kedro_mlflow_config.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/extras/extensions/test_ipython.py` & `kedro_mlflow-0.9.0/tests/extras/extensions/test_ipython.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/framework/cli/test_cli.py` & `kedro_mlflow-0.9.0/tests/framework/cli/test_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pytest
 import yaml
 from click.testing import CliRunner
 from cookiecutter.main import cookiecutter
 from kedro import __version__ as kedro_version
 from kedro.framework.cli.cli import info
 from kedro.framework.cli.starters import TEMPLATE_PATH
+from kedro.framework.project import _ProjectSettings
 from kedro.framework.session import KedroSession
 from kedro.framework.startup import bootstrap_project
 
 from kedro_mlflow.config import get_mlflow_config
 from kedro_mlflow.config.kedro_mlflow_config import KedroMlflowConfig
 from kedro_mlflow.framework.cli.cli import init as cli_init
 from kedro_mlflow.framework.cli.cli import mlflow_commands as cli_mlflow
@@ -28,14 +29,36 @@
     for cmd_detailed in cmd_list_detailed:
         cmd_match = re.search(r"\w+(?=  )", string=cmd_detailed)
         if cmd_match is not None:
             cmd_list.append(cmd_match.group(0))
     return cmd_list
 
 
+@pytest.fixture(autouse=True)
+def mock_validate_settings(mocker):
+    # KedroSession eagerly validates that a project's settings.py is correct by
+    # importing it. settings.py does not actually exists as part of this test suite
+    # since we are testing session in isolation, so the validation is patched.
+    mocker.patch("kedro.framework.session.session.validate_settings")
+
+
+def _mock_imported_settings_paths(mocker, mock_settings):
+    for path in [
+        "kedro.framework.project.settings",
+        "kedro.framework.session.session.settings",
+    ]:
+        mocker.patch(path, mock_settings)
+    return mock_settings
+
+
+@pytest.fixture
+def mock_settings_fake_project(mocker):
+    return _mock_imported_settings_paths(mocker, _ProjectSettings())
+
+
 def test_cli_global_discovered(monkeypatch, tmp_path):
     monkeypatch.chdir(tmp_path)
     cli_runner = CliRunner()
     result = cli_runner.invoke(info)
 
     assert result.exit_code == 0
     assert "kedro_mlflow" in result.output
@@ -74,53 +97,61 @@
     assert result.exit_code == 0
 
     # check mlflow.yml file
     assert "'conf/local/mlflow.yml' successfully updated." in result.output
     assert (kedro_project / "conf" / "local" / "mlflow.yml").is_file()
 
 
-def test_cli_init_existing_config(monkeypatch, kedro_project_with_mlflow_conf):
+def test_cli_init_existing_config(
+    monkeypatch, kedro_project_with_mlflow_conf, mock_settings_fake_project
+):
     # "kedro_project" is a pytest.fixture declared in conftest
     cli_runner = CliRunner()
     monkeypatch.chdir(kedro_project_with_mlflow_conf)
     bootstrap_project(kedro_project_with_mlflow_conf)
 
     with KedroSession.create(
         "fake_project", project_path=kedro_project_with_mlflow_conf
-    ) as session:
-        context = session.load_context()
+    ):
         # emulate first call by writing a mlflow.yml file
         yaml_str = yaml.dump(dict(server=dict(mlflow_tracking_uri="toto")))
         (
-            kedro_project_with_mlflow_conf / context.CONF_ROOT / "local" / "mlflow.yml"
+            kedro_project_with_mlflow_conf
+            / mock_settings_fake_project.CONF_SOURCE
+            / "local"
+            / "mlflow.yml"
         ).write_text(yaml_str)
 
         result = cli_runner.invoke(cli_init)
 
         # check an error message is raised
         assert "A 'mlflow.yml' already exists" in result.output
 
         # check the file remains unmodified
         assert get_mlflow_config().server.mlflow_tracking_uri.endswith("toto")
 
 
-def test_cli_init_existing_config_force_option(monkeypatch, kedro_project):
+def test_cli_init_existing_config_force_option(
+    monkeypatch, kedro_project, mock_settings_fake_project
+):
     # "kedro_project" is a pytest.fixture declared in conftest
     monkeypatch.chdir(kedro_project)
     cli_runner = CliRunner()
 
     bootstrap_project(kedro_project)
-    with KedroSession.create(project_path=kedro_project) as session:
-        context = session.load_context()
+    with KedroSession.create(project_path=kedro_project):
 
         # emulate first call by writing a mlflow.yml file
         yaml_str = yaml.dump(dict(mlflow_tracking_uri="toto"))
-        (kedro_project / context.CONF_ROOT / "local" / "mlflow.yml").write_text(
-            yaml_str
-        )
+        (
+            kedro_project
+            / mock_settings_fake_project.CONF_SOURCE
+            / "local"
+            / "mlflow.yml"
+        ).write_text(yaml_str)
 
         result = cli_runner.invoke(cli_init, args="--force")
 
         # check an error message is raised
         assert "successfully updated" in result.output
 
         # check the file remains unmodified
```

### Comparing `kedro_mlflow-0.8.1/tests/framework/cli/test_cli_modelify.py` & `kedro_mlflow-0.9.0/tests/framework/cli/test_cli_modelify.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/framework/cli/test_cli_utils.py` & `kedro_mlflow-0.9.0/tests/framework/cli/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/framework/hooks/test_all_hooks.py` & `kedro_mlflow-0.9.0/tests/framework/hooks/test_all_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 import pytest
 import toml
 import yaml
 from kedro import __version__ as kedro_version
 from kedro.config import ConfigLoader
 from kedro.framework.hooks import hook_impl
-from kedro.framework.hooks.manager import get_hook_manager
+
+# from kedro.framework.hooks.manager import get_hook_manager
 from kedro.framework.project import (
     Validator,
     _ProjectPipelines,
     _ProjectSettings,
     configure_project,
 )
 from kedro.framework.session import KedroSession
 from kedro.io import DataCatalog
 from kedro.pipeline import Pipeline, node
-from kedro.versioning import Journal
 from mlflow.tracking import MlflowClient
 
 from kedro_mlflow.config import get_mlflow_config
 from kedro_mlflow.framework.hooks import MlflowNodeHook, MlflowPipelineHook
 
 MOCK_PACKAGE_NAME = "mock_package_name"
 
@@ -117,21 +117,21 @@
         #     "recursive": True,
         #     "sep": ".",
         #     "long_parameters_strategy": "fail",
         # },
     )
 
 
-@pytest.fixture(autouse=True)
-def clear_hook_manager():
-    yield
-    hook_manager = get_hook_manager()
-    plugins = hook_manager.get_plugins()
-    for plugin in plugins:
-        hook_manager.unregister(plugin)
+# @pytest.fixture(autouse=True)
+# def clear_hook_manager():
+#     yield
+#     hook_manager = get_hook_manager()
+#     plugins = hook_manager.get_plugins()
+#     for plugin in plugins:
+#         hook_manager.unregister(plugin)
 
 
 @pytest.fixture(autouse=True)
 def config_dir(
     kedro_project_path, catalog_config, local_logging_config, mlflow_config_wo_tracking
 ):
     catalog_yml = kedro_project_path / "conf" / "base" / "catalog.yml"
@@ -165,18 +165,17 @@
     @hook_impl
     def register_catalog(
         self,
         catalog: Optional[Dict[str, Dict[str, Any]]],
         credentials: Dict[str, Dict[str, Any]],
         load_versions: Dict[str, str],
         save_version: str,
-        journal: Journal,
     ) -> DataCatalog:
         return DataCatalog.from_config(
-            catalog, credentials, load_versions, save_version, journal
+            catalog, credentials, load_versions, save_version
         )
 
 
 def _mock_imported_settings_paths(mocker, mock_settings):
     for path in [
         "kedro.framework.context.context.settings",
         "kedro.framework.session.session.settings",
@@ -255,16 +254,19 @@
 def mock_session(
     mocker, mock_settings_with_mlflow_hooks, kedro_project_path
 ):  # pylint: disable=unused-argument
 
     # we need to patch "kedro.framework.session.session.validate_settings" instead of
     # "kedro.framework.project.validate_settings" because it is imported
     mocker.patch("kedro.framework.session.session.validate_settings")
+    # idem, we patch we need to patch "kedro.framework.session.session._register_hooks_setuptools" instead of
+    # "kedro.framework.hooks.manager._register_hooks_setuptools" because it is imported
+
     mocker.patch(
-        "kedro.framework.project._register_hooks_setuptools"
+        "kedro.framework.session.session._register_hooks_setuptools"
     )  # prevent registering the one of the plugins which are already installed
     configure_project(MOCK_PACKAGE_NAME)
     return KedroSession.create(MOCK_PACKAGE_NAME, kedro_project_path)
 
 
 def test_deactivated_tracking_but_not_for_given_pipeline(
     mocker, config_dir, kedro_project_path, mock_session
```

### Comparing `kedro_mlflow-0.8.1/tests/framework/hooks/test_node_hook.py` & `kedro_mlflow-0.9.0/tests/framework/hooks/test_node_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,14 @@
                 catalog=dummy_catalog,
             )
             mlflow_node_hook.before_node_run(
                 node=dummy_node,
                 catalog=dummy_catalog,
                 inputs=node_inputs,
                 is_async=False,
-                run_id="132",
             )
             run_id = mlflow.active_run().info.run_id
 
         mlflow_client = MlflowClient(mlflow_tracking_uri)
         current_run = mlflow_client.get_run(run_id)
         assert current_run.data.params == expected
 
@@ -211,15 +210,14 @@
                 catalog=DataCatalog(),
             )
             mlflow_node_hook.before_node_run(
                 node=node(func=lambda x: x, inputs=dict(x="a"), outputs=None),
                 catalog=DataCatalog(),  # can be empty
                 inputs=node_inputs,
                 is_async=False,
-                run_id="132",
             )
             run_id = mlflow.active_run().info.run_id
 
         mlflow_client = MlflowClient(mlflow_tracking_uri)
         current_run = mlflow_client.get_run(run_id)
         assert current_run.data.params == {"my_param": param_value}
 
@@ -258,15 +256,14 @@
                 catalog=DataCatalog(),
             )
             mlflow_node_hook.before_node_run(
                 node=node(func=lambda x: x, inputs=dict(x="a"), outputs=None),
                 catalog=DataCatalog(),  # can be empty
                 inputs=node_inputs,
                 is_async=False,
-                run_id="132",
             )
             run_id = mlflow.active_run().info.run_id
 
         mlflow_client = MlflowClient(mlflow_tracking_uri)
         current_run = mlflow_client.get_run(run_id)
         assert current_run.data.params == {
             "my_param": param_value[0:MAX_PARAM_VAL_LENGTH]
@@ -320,15 +317,14 @@
                 ValueError, match=f"Parameter 'my_param' length is {param_length}"
             ):
                 mlflow_node_hook.before_node_run(
                     node=node(func=lambda x: x, inputs=dict(x="a"), outputs=None),
                     catalog=DataCatalog(),  # can be empty
                     inputs=node_inputs,
                     is_async=False,
-                    run_id="132",
                 )
 
 
 @pytest.mark.parametrize(
     "param_length",
     [MAX_PARAM_VAL_LENGTH + 20],
 )
@@ -370,15 +366,14 @@
             # But we have enforced failure (which is slightly different from mlflow
             # behaviour)
             mlflow_node_hook.before_node_run(
                 node=node(func=lambda x: x, inputs=dict(x="a"), outputs=None),
                 catalog=DataCatalog(),  # can be empty
                 inputs=node_inputs,
                 is_async=False,
-                run_id="132",
             )
             run_id = mlflow.active_run().info.run_id
 
         mlflow_client = MlflowClient(mlflow_tracking_uri)
         current_run = mlflow_client.get_run(run_id)
         assert current_run.data.params == {}
         assert {
```

### Comparing `kedro_mlflow-0.8.1/tests/framework/hooks/test_pipeline_hook.py` & `kedro_mlflow-0.9.0/tests/framework/hooks/test_pipeline_hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from kedro.framework.hooks import hook_impl
 from kedro.framework.project import Validator, _ProjectPipelines, _ProjectSettings
 from kedro.framework.session import KedroSession
 from kedro.framework.startup import bootstrap_project
 from kedro.io import DataCatalog, MemoryDataSet
 from kedro.pipeline import Pipeline, node
 from kedro.runner import SequentialRunner
-from kedro.versioning import Journal
 from mlflow.entities import RunStatus
 from mlflow.models import infer_signature
 from mlflow.tracking import MlflowClient
 
 from kedro_mlflow.config import get_mlflow_config
 from kedro_mlflow.framework.hooks.pipeline_hook import (
     MlflowPipelineHook,
@@ -104,18 +103,17 @@
     @hook_impl
     def register_catalog(
         self,
         catalog: Optional[Dict[str, Dict[str, Any]]],
         credentials: Dict[str, Dict[str, Any]],
         load_versions: Dict[str, str],
         save_version: str,
-        journal: Journal,
     ) -> DataCatalog:
         return DataCatalog.from_config(
-            catalog, credentials, load_versions, save_version, journal
+            catalog, credentials, load_versions, save_version
         )
 
 
 def _mock_imported_settings_paths(mocker, mock_settings):
     for path in [
         "kedro.framework.context.context.settings",
         "kedro.framework.session.session.settings",
@@ -352,15 +350,14 @@
     dummy_signature = infer_signature(input_data)
     return dummy_signature
 
 
 @pytest.fixture
 def dummy_run_params(tmp_path):
     dummy_run_params = {
-        "run_id": "abcdef",
         "project_path": tmp_path.as_posix(),
         "env": "local",
         "kedro_version": "0.16.0",
         "tags": [],
         "from_nodes": [],
         "to_nodes": [],
         "node_names": [],
@@ -384,33 +381,32 @@
     env_from_dict,
     pipeline_to_run,
     dummy_catalog,
     dummy_run_params,
 ):
 
     bootstrap_project(kedro_project_with_mlflow_conf)
-    with KedroSession.create(project_path=kedro_project_with_mlflow_conf):
+    with KedroSession.create(project_path=kedro_project_with_mlflow_conf) as session:
         # config_with_base_mlflow_conf is a conftest fixture
         pipeline_hook = MlflowPipelineHook()
         runner = SequentialRunner()
         pipeline_hook.after_catalog_created(
             catalog=dummy_catalog,
             # `after_catalog_created` is not using any of below arguments,
             # so we are setting them to empty values.
             conf_catalog={},
             conf_creds={},
             feed_dict={},
             save_version="",
             load_versions="",
-            run_id=dummy_run_params["run_id"],
         )
         pipeline_hook.before_pipeline_run(
             run_params=dummy_run_params, pipeline=pipeline_to_run, catalog=dummy_catalog
         )
-        runner.run(pipeline_to_run, dummy_catalog)
+        runner.run(pipeline_to_run, dummy_catalog, session._hook_manager)
         run_id = mlflow.active_run().info.run_id
         pipeline_hook.after_pipeline_run(
             run_params=dummy_run_params, pipeline=pipeline_to_run, catalog=dummy_catalog
         )
         # test : parameters should have been logged
         mlflow_conf = get_mlflow_config()
         mlflow_client = MlflowClient(mlflow_conf.server.mlflow_tracking_uri)
@@ -459,29 +455,28 @@
     dummy_catalog,
     dummy_run_params,
     copy_mode,
     expected,
 ):
     # config_with_base_mlflow_conf is a conftest fixture
     bootstrap_project(kedro_project_with_mlflow_conf)
-    with KedroSession.create(project_path=kedro_project_with_mlflow_conf):
+    with KedroSession.create(project_path=kedro_project_with_mlflow_conf) as session:
 
         pipeline_hook = MlflowPipelineHook()
         runner = SequentialRunner()
 
         pipeline_hook.after_catalog_created(
             catalog=dummy_catalog,
             # `after_catalog_created` is not using any of arguments bellow,
             # so we are setting them to empty values.
             conf_catalog={},
             conf_creds={},
             feed_dict={},
             save_version="",
             load_versions="",
-            run_id=dummy_run_params["run_id"],
         )
 
         pipeline_to_run = pipeline_ml_factory(
             training=dummy_pipeline_ml.training,
             inference=dummy_pipeline_ml.inference,
             input_name=dummy_pipeline_ml.input_name,
             log_model_kwargs={
@@ -491,15 +486,15 @@
             kpm_kwargs={
                 "copy_mode": copy_mode,
             },
         )
         pipeline_hook.before_pipeline_run(
             run_params=dummy_run_params, pipeline=pipeline_to_run, catalog=dummy_catalog
         )
-        runner.run(pipeline_to_run, dummy_catalog)
+        runner.run(pipeline_to_run, dummy_catalog, session._hook_manager)
         run_id = mlflow.active_run().info.run_id
         pipeline_hook.after_pipeline_run(
             run_params=dummy_run_params, pipeline=pipeline_to_run, catalog=dummy_catalog
         )
 
         mlflow_tracking_uri = (kedro_project_with_mlflow_conf / "mlruns").as_uri()
         mlflow.set_tracking_uri(mlflow_tracking_uri)
@@ -515,15 +510,15 @@
 
 
 def test_mlflow_pipeline_hook_metric_metrics_with_run_id(
     kedro_project_with_mlflow_conf, dummy_pipeline_ml, dummy_run_params
 ):
 
     bootstrap_project(kedro_project_with_mlflow_conf)
-    with KedroSession.create(project_path=kedro_project_with_mlflow_conf):
+    with KedroSession.create(project_path=kedro_project_with_mlflow_conf) as session:
 
         mlflow_conf = get_mlflow_config()
         mlflow.set_tracking_uri(mlflow_conf.server.mlflow_tracking_uri)
 
         with mlflow.start_run():
             existing_run_id = mlflow.active_run().info.run_id
 
@@ -558,22 +553,21 @@
             # `after_catalog_created` is not using any of arguments bellow,
             # so we are setting them to empty values.
             conf_catalog={},
             conf_creds={},
             feed_dict={},
             save_version="",
             load_versions="",
-            run_id=dummy_run_params["run_id"],
         )
         pipeline_hook.before_pipeline_run(
             run_params=dummy_run_params,
             pipeline=dummy_pipeline_ml,
             catalog=dummy_catalog_with_run_id,
         )
-        runner.run(dummy_pipeline_ml, dummy_catalog_with_run_id)
+        runner.run(dummy_pipeline_ml, dummy_catalog_with_run_id, session._hook_manager)
 
         current_run_id = mlflow.active_run().info.run_id
 
         pipeline_hook.after_pipeline_run(
             run_params=dummy_run_params,
             pipeline=dummy_pipeline_ml,
             catalog=dummy_catalog_with_run_id,
@@ -614,15 +608,15 @@
     kedro_project_with_mlflow_conf,  # a fixture to be in a kedro project
     tmp_path,
     pipeline_ml_with_parameters,
     dummy_run_params,
 ):
     # config_with_base_mlflow_conf is a conftest fixture
     bootstrap_project(kedro_project_with_mlflow_conf)
-    with KedroSession.create(project_path=kedro_project_with_mlflow_conf):
+    with KedroSession.create(project_path=kedro_project_with_mlflow_conf) as session:
 
         mlflow_conf = get_mlflow_config()
         mlflow.set_tracking_uri(mlflow_conf.server.mlflow_tracking_uri)
 
         catalog_with_parameters = DataCatalog(
             {
                 "data": MemoryDataSet(pd.DataFrame(data=[1], columns=["a"])),
@@ -644,22 +638,23 @@
             # `after_catalog_created` is not using any of arguments bellow,
             # so we are setting them to empty values.
             conf_catalog={},
             conf_creds={},
             feed_dict={},
             save_version="",
             load_versions="",
-            run_id=dummy_run_params["run_id"],
         )
         pipeline_hook.before_pipeline_run(
             run_params=dummy_run_params,
             pipeline=pipeline_ml_with_parameters,
             catalog=catalog_with_parameters,
         )
-        runner.run(pipeline_ml_with_parameters, catalog_with_parameters)
+        runner.run(
+            pipeline_ml_with_parameters, catalog_with_parameters, session._hook_manager
+        )
 
         current_run_id = mlflow.active_run().info.run_id
 
         # This is what we want to test: model must be saved and the parameters automatically persisted on disk
         pipeline_hook.after_pipeline_run(
             run_params=dummy_run_params,
             pipeline=pipeline_ml_with_parameters,
@@ -695,15 +690,15 @@
     dummy_catalog,
     dummy_run_params,
     model_signature,
     expected_signature,
 ):
     # config_with_base_mlflow_conf is a conftest fixture
     bootstrap_project(kedro_project_with_mlflow_conf)
-    with KedroSession.create(project_path=kedro_project_with_mlflow_conf):
+    with KedroSession.create(project_path=kedro_project_with_mlflow_conf) as session:
         pipeline_hook = MlflowPipelineHook()
         runner = SequentialRunner()
 
         pipeline_to_run = pipeline_ml_factory(
             training=dummy_pipeline.only_nodes_with_tags("training"),
             inference=dummy_pipeline.only_nodes_with_tags("inference"),
             input_name="raw_data",
@@ -719,20 +714,19 @@
             # `after_catalog_created` is not using any of arguments bellow,
             # so we are setting them to empty values.
             conf_catalog={},
             conf_creds={},
             feed_dict={},
             save_version="",
             load_versions="",
-            run_id=dummy_run_params["run_id"],
         )
         pipeline_hook.before_pipeline_run(
             run_params=dummy_run_params, pipeline=pipeline_to_run, catalog=dummy_catalog
         )
-        runner.run(pipeline_to_run, dummy_catalog)
+        runner.run(pipeline_to_run, dummy_catalog, session._hook_manager)
         run_id = mlflow.active_run().info.run_id
         pipeline_hook.after_pipeline_run(
             run_params=dummy_run_params, pipeline=pipeline_to_run, catalog=dummy_catalog
         )
 
         # test : parameters should have been logged
         trained_model = mlflow.pyfunc.load_model(f"runs:/{run_id}/model")
```

### Comparing `kedro_mlflow-0.8.1/tests/framework/hooks/test_utils.py` & `kedro_mlflow-0.9.0/tests/framework/hooks/test_utils.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/io/artifacts/test_mlflow_artifact_dataset.py` & `kedro_mlflow-0.9.0/tests/io/artifacts/test_mlflow_artifact_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/io/metrics/test_mlflow_metric_dataset.py` & `kedro_mlflow-0.9.0/tests/io/metrics/test_mlflow_metric_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/io/metrics/test_mlflow_metric_history_dataset.py` & `kedro_mlflow-0.9.0/tests/io/metrics/test_mlflow_metric_history_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/io/metrics/test_mlflow_metrics_dataset.py` & `kedro_mlflow-0.9.0/tests/io/metrics/test_mlflow_metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/io/models/test_mlflow_model_logger_dataset.py` & `kedro_mlflow-0.9.0/tests/io/models/test_mlflow_model_logger_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/io/models/test_mlflow_model_saver_dataset.py` & `kedro_mlflow-0.9.0/tests/io/models/test_mlflow_model_saver_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/mlflow/test_kedro_pipeline_model.py` & `kedro_mlflow-0.9.0/tests/mlflow/test_kedro_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `kedro_mlflow-0.8.1/tests/pipeline/test_pipeline_ml.py` & `kedro_mlflow-0.9.0/tests/pipeline/test_pipeline_ml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pytest
-from kedro import __version__ as KEDRO_VERSION
 from kedro.extras.datasets.pandas import CSVDataSet
-from kedro.framework.context import KedroContext
 from kedro.io import DataCatalog, MemoryDataSet
 from kedro.pipeline import Pipeline, node
 
 from kedro_mlflow.pipeline import pipeline_ml_factory
 from kedro_mlflow.pipeline.pipeline_ml import KedroMlflowPipelineMLError, PipelineML
 
 
@@ -82,15 +80,15 @@
 def pipeline_ml_with_intermediary_artifacts():
     full_pipeline = Pipeline(
         [
             node(
                 func=preprocess_fun,
                 inputs="raw_data",
                 outputs="data",
-                tags=["training"],
+                tags=["training", "preprocessing"],
             ),
             node(
                 func=fit_encoder_fun,
                 inputs="data",
                 outputs="encoder",
                 tags=["training"],
             ),
@@ -193,28 +191,14 @@
         inference=full_pipeline.only_nodes_with_tags("inference"),
         input_name="data",
     )
     return pipeline_ml_with_parameters
 
 
 @pytest.fixture
-def dummy_context(tmp_path, kedro_project, mocker):
-    class DummyContext(KedroContext):
-        project_name = "fake project"
-        package_name = "fake_project"
-        project_version = KEDRO_VERSION
-
-        def _get_pipelines(self):
-            return {"__default__": Pipeline([])}
-
-    dummy_context = DummyContext("fake_package", tmp_path.as_posix())
-    return dummy_context
-
-
-@pytest.fixture
 def dummy_catalog():
     dummy_catalog = DataCatalog(
         {
             "raw_data": MemoryDataSet(),
             "data": MemoryDataSet(),
             "model": CSVDataSet("fake/path/to/model.csv"),
         }
@@ -273,43 +257,40 @@
         (None, None, ["train_fun([data]) -> [model]"], None, None),
         (None, None, None, ["train_fun([data]) -> [model]"], None),
         (None, None, None, None, ["data"]),
     ],
 )
 def test_filtering_pipeline_ml(
     mocker,
-    dummy_context,
     pipeline_with_tag,
     pipeline_ml_with_tag,
     tags,
     from_nodes,
     to_nodes,
     node_names,
     from_inputs,
 ):
     """When the pipeline is filtered by the context (e.g calling only_nodes_with_tags,
     from_inputs...), it must return a PipelineML instance with unmodified inference.
     We loop dynamically on the arguments of the function in case of kedro
     modify the filters.
     """
 
-    # dummy_context, pipeline_with_tag, pipeline_ml_with_tag are fixture in conftest
+    # pipeline_with_tag, pipeline_ml_with_tag are fixture in conftest
 
     # remember : the arguments are iterable, so do not pass string directly (e.g ["training"] rather than training)
-    filtered_pipeline = dummy_context._filter_pipeline(
-        pipeline=pipeline_with_tag,
+    filtered_pipeline = pipeline_with_tag.filter(
         tags=tags,
         from_nodes=from_nodes,
         to_nodes=to_nodes,
         node_names=node_names,
         from_inputs=from_inputs,
     )
 
-    filtered_pipeline_ml = dummy_context._filter_pipeline(
-        pipeline=pipeline_ml_with_tag,
+    filtered_pipeline_ml = pipeline_ml_with_tag.filter(
         tags=tags,
         from_nodes=from_nodes,
         to_nodes=to_nodes,
         node_names=node_names,
         from_inputs=from_inputs,
     )
 
@@ -334,15 +315,14 @@
         (["preprocessing"], None, None, None, None),
         (None, None, ["preprocess_fun([raw_data]) -> [data]"], None, None),
         (None, None, None, ["preprocess_fun([raw_data]) -> [data]"], None),
     ],
 )
 def test_filtering_generate_invalid_pipeline_ml(
     mocker,
-    dummy_context,
     pipeline_ml_obj,
     tags,
     from_nodes,
     to_nodes,
     node_names,
     from_inputs,
 ):
@@ -351,27 +331,23 @@
     but not the same than previously is generated, it should be catched.
     """
     # remember : the arguments are iterable, so do not pass string directly (e.g ["training"] rather than training)
     with pytest.raises(
         KedroMlflowPipelineMLError,
         match="No free input is allowed",
     ):
-        dummy_context._filter_pipeline(
-            pipeline=pipeline_ml_obj,
+        pipeline_ml_obj.filter(
             tags=tags,
             from_nodes=from_nodes,
             to_nodes=to_nodes,
             node_names=node_names,
             from_inputs=from_inputs,
         )
 
 
-# add a test to check number of inputs of dummy_context._filter_pipeline
-# if they add new filters, Pipeline Ml must be modified accordingly
-
 # def test_pipeline_ml_preserve_tags():
 #     pass
 
 
 def test_too_many_free_inputs():
     with pytest.raises(KedroMlflowPipelineMLError, match="No free input is allowed"):
         pipeline_ml_factory(
@@ -398,22 +374,14 @@
 
 
 def test_tagging(pipeline_ml_with_tag):
     new_pl = pipeline_ml_with_tag.tag(["hello"])
     assert all(["hello" in node.tags for node in new_pl.nodes])
 
 
-def test_decorate(pipeline_ml_with_tag):
-    def fake_dec(x):
-        return x
-
-    new_pl = pipeline_ml_with_tag.decorate(fake_dec)
-    assert all([fake_dec in node._decorators for node in new_pl.nodes])
-
-
 def test_invalid_input_name(pipeline_ml_with_tag):
     with pytest.raises(
         KedroMlflowPipelineMLError,
         match="input_name='whoops_bad_name' but it must be an input of 'inference'",
     ):
         pipeline_ml_with_tag.input_name = "whoops_bad_name"
```

### Comparing `kedro_mlflow-0.8.1/tests/template/project/test_mlflow_yml.py` & `kedro_mlflow-0.9.0/tests/template/project/test_mlflow_yml.py`

 * *Files identical despite different names*

