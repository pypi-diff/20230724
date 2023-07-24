# Comparing `tmp/scicookie-0.3.0.tar.gz` & `tmp/scicookie-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicookie-0.3.0.tar", max compression
+gzip compressed data, was "scicookie-0.4.0.tar", max compression
```

## Comparing `scicookie-0.3.0.tar` & `scicookie-0.4.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0     1551 2023-07-05 20:50:33.388224 scicookie-0.3.0/LICENSE
--rw-r--r--   0        0        0     2060 2023-07-05 20:54:30.191225 scicookie-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       77 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/__init__.py
--rw-r--r--   0        0        0      115 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/__main__.py
--rw-r--r--   0        0        0     3132 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/cli.py
--rw-r--r--   0        0        0     1787 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/cookiecutter.json
--rw-r--r--   0        0        0     7388 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/hooks/post_gen_project.py
--rw-r--r--   0        0        0      359 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      969 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/logs.py
--rw-r--r--   0        0        0     1417 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/profile.py
--rw-r--r--   0        0        0     3888 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/profiles/base.yaml
--rw-r--r--   0        0        0      770 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/profiles/osl.yaml
--rw-r--r--   0        0        0     2122 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/ui.py
--rw-r--r--   0        0        0      292 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     4617 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      892 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1712 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
--rw-r--r--   0        0        0     2550 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      342 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1387 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      814 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1666 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1274 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     2867 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2295 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
--rw-r--r--   0        0        0     5996 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0     3092 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     3325 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0     1717 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml
--rw-r--r--   0        0        0     3963 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml
--rw-r--r--   0        0        0      400 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/meson.build
--rw-r--r--   0        0        0     3886 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy-pyproject.toml
--rw-r--r--   0        0        0     3880 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml
--rw-r--r--   0        0        0     2567 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml
--rw-r--r--   0        0        0     3745 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml
--rw-r--r--   0        0        0     6433 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
--rw-r--r--   0        0        0     6434 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5488 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
--rw-r--r--   0        0        0     5488 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
--rw-r--r--   0        0        0      575 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
--rw-r--r--   0        0        0     1998 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
--rw-r--r--   0        0        0      300 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
--rw-r--r--   0        0        0       54 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
--rw-r--r--   0        0        0      182 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
--rw-r--r--   0        0        0       20 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
--rw-r--r--   0        0        0     8386 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
--rw-r--r--   0        0        0     1116 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
--rw-r--r--   0        0        0     3386 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
--rw-r--r--   0        0        0      996 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
--rw-r--r--   0        0        0      967 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
--rw-r--r--   0        0        0      151 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
--rw-r--r--   0        0        0     4398 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
--rwxr-xr-x   0        0        0     5275 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
--rw-r--r--   0        0        0      374 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
--rw-r--r--   0        0        0      829 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
--rw-r--r--   0        0        0       30 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
--rw-r--r--   0        0        0    16493 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
--rw-r--r--   0        0        0     6843 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
--rw-r--r--   0        0        0     1558 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
--rw-r--r--   0        0        0       61 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1266 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0      809 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
--rw-r--r--   0        0        0      631 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
--rw-r--r--   0        0        0       19 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 scicookie-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1551 2023-07-24 13:13:07.393521 scicookie-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2064 2023-07-24 13:15:26.460894 scicookie-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/__main__.py
+-rw-r--r--   0        0        0     3108 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/cli.py
+-rw-r--r--   0        0        0     1740 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/cookiecutter.json
+-rw-r--r--   0        0        0     7634 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      359 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      969 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/logs.py
+-rw-r--r--   0        0        0     1417 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/profile.py
+-rw-r--r--   0        0        0     3911 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/profiles/base.yaml
+-rw-r--r--   0        0        0      781 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/profiles/osl.yaml
+-rw-r--r--   0        0        0     2122 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/ui.py
+-rw-r--r--   0        0        0      292 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     4617 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      892 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1712 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
+-rw-r--r--   0        0        0     2550 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      342 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1387 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      845 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1715 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1274 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     2867 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2295 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
+-rw-r--r--   0        0        0     5996 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0     3154 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0     3324 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0     1717 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml
+-rw-r--r--   0        0        0     4175 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml
+-rw-r--r--   0        0        0     4211 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch-pyproject.toml
+-rw-r--r--   0        0        0      400 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/meson.build
+-rw-r--r--   0        0        0     4098 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy-pyproject.toml
+-rw-r--r--   0        0        0     4092 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml
+-rw-r--r--   0        0        0     2779 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml
+-rw-r--r--   0        0        0     3745 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml
+-rw-r--r--   0        0        0     6433 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
+-rw-r--r--   0        0        0     6434 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5488 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
+-rw-r--r--   0        0        0     5488 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
+-rw-r--r--   0        0        0      634 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
+-rw-r--r--   0        0        0     1998 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
+-rw-r--r--   0        0        0      300 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
+-rw-r--r--   0        0        0       54 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
+-rw-r--r--   0        0        0      182 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
+-rw-r--r--   0        0        0       20 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
+-rw-r--r--   0        0        0     9068 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
+-rw-r--r--   0        0        0     1116 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
+-rw-r--r--   0        0        0     3386 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
+-rw-r--r--   0        0        0      996 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
+-rw-r--r--   0        0        0      967 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
+-rw-r--r--   0        0        0      151 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
+-rw-r--r--   0        0        0     4398 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
+-rwxr-xr-x   0        0        0     5275 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      374 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
+-rw-r--r--   0        0        0      829 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
+-rw-r--r--   0        0        0       30 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
+-rw-r--r--   0        0        0    16493 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
+-rw-r--r--   0        0        0     6843 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
+-rw-r--r--   0        0        0     1558 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
+-rw-r--r--   0        0        0       61 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1266 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0      809 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
+-rw-r--r--   0        0        0      631 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
+-rw-r--r--   0        0        0       19 2023-07-24 13:13:07.397521 scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 scicookie-0.4.0/PKG-INFO
```

### Comparing `scicookie-0.3.0/LICENSE` & `scicookie-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/pyproject.toml` & `scicookie-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scicookie"
-version = "0.3.0"  # semantic-release
+version = "0.4.0"  # semantic-release
 description = "Cookiecutter template for a Python package"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD"
 include = [
     {path = "src/scicookie/cookiecutter.json"},
     {path = "src/scicookie/{{cookiecutter.project_slug}}"},
     {path = "src/scicookie/hooks"},
@@ -13,32 +13,32 @@
 [tool.poetry.scripts]
 "scicookie" = "scicookie.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 cookieninja = "1.0.0"
 sh = "^2.0.4"
-pyyaml = ">=5"
 colorama = "^0.4.6"
 inquirer = "^3.1.3"
+pyyaml = ">=6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7"
 black = ">=22"
 isort = ">=5"
 pre-commit = ">=3"
 ruff = ">=0.0.272"
 mypy = ">=1"
 pytest-cov = ">=3"
 pytest-cookies = ">=0.6.1"
 Sphinx = ">=4.4"
 jupyterlab = ">=3.5.1"
 jupyter-book = ">=0.12.3"
 myst-parser = ">=0.15"
-makim = "1.8.1"
+makim = "1.8.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
```

### Comparing `scicookie-0.3.0/src/scicookie/cli.py` & `scicookie-0.4.0/src/scicookie/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,38 +27,36 @@
     if isinstance(answer_definition, str):
         return answer_definition
 
     return answer_definition[0]
 
 
 def call_cookiecutter(profile: Profile, answers: dict):
-    """Call coociecutter/cookieninja with the parameters from the TUI."""
+    """Call cookiecutter/cookieninja with the parameters from the TUI."""
     answers_profile = {}
     cookie_args = []
     questions = profile.config
 
     with open(COOKIECUTTER_FILE_PATH) as f:
-        coockiecutter_config = json.load(f)
+        cookiecutter_config = json.load(f)
 
     # fill the answers with default value
     for question_id, question in questions.items():
         if not question.get("enabled", False) or question.get("control_flow"):
             continue
 
         if question.get("type") == "multiple-choices":
             for choice in question.get("choices", {}):
                 choice_id = f"use_{choice.replace('-', '_')}"
                 answers_profile[choice_id] = "no"
             continue
 
         answers_profile[question_id] = question.get(
             "default"
-        ) or _get_cookiecutter_default_answer(
-            coockiecutter_config[question_id]
-        )
+        ) or _get_cookiecutter_default_answer(cookiecutter_config[question_id])
 
     for question_id, answer in answers.items():
         if answer in [None, ""] or questions[question_id].get("control_flow"):
             continue
 
         if questions[question_id].get("type") != "multiple-choices":
             answers_profile[question_id] = answer
```

### Comparing `scicookie-0.3.0/src/scicookie/cookiecutter.json` & `scicookie-0.4.0/src/scicookie/cookiecutter.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9842342342342342%*

 * *Differences: {"'build_system'": "{insert: [(5, 'hatch')]}",*

 * * "'project_short_description'": "'This Project aims to ...'"}*

```diff
@@ -2,15 +2,16 @@
     "author_email": "zoro@one.piece",
     "author_full_name": "Roronoa Zoro",
     "build_system": [
         "poetry",
         "flit",
         "mesonpy",
         "setuptools",
-        "pdm"
+        "pdm",
+        "hatch"
     ],
     "code_of_conduct": [
         "None",
         "contributor-covenant",
         "citizen-code-of-conduct"
     ],
     "command_line_interface": [
@@ -42,15 +43,15 @@
         "BSD 3 Clause",
         "ISC license",
         "Apache Software License 2.0",
         "GNU General Public License v3",
         "Other"
     ],
     "project_name": "OSL Python package",
-    "project_short_description": "OSL Python Package contains all the boilerplate you need to create a Python package.",
+    "project_short_description": "This Project aims to ...",
     "project_slug": "{{ cookiecutter.project_name.lower().replace(' ', '-') }}",
     "project_url": "https://{{ cookiecutter.project_slug }}.com",
     "project_version": "0.1.0",
     "roadmap_document": [
         "None",
         "pytorch-ignite-roadmap"
     ],
```

### Comparing `scicookie-0.3.0/src/scicookie/hooks/post_gen_project.py` & `scicookie-0.4.0/src/scicookie/hooks/post_gen_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 BUILD_SYSTEM = "flit"
 {% elif cookiecutter.build_system == "mesonpy" -%}
 BUILD_SYSTEM = "mesonpy"
 {% elif cookiecutter.build_system == "setuptools" -%}
 BUILD_SYSTEM = "setuptools"
 {% elif cookiecutter.build_system == "pdm" -%}
 BUILD_SYSTEM = "pdm"
+{% elif cookiecutter.build_system == "hatch" -%}
+BUILD_SYSTEM = "hatch"
 {%- else %}
 BUILD_SYSTEM = None
 {%- endif %}
 
 
 def remove_dirs(dirs: list):
     for dirs in dirs:
@@ -176,14 +178,19 @@
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
     elif BUILD_SYSTEM == "pdm":
         shutil.move(
             build_system_dir / "pdm-pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
+    elif BUILD_SYSTEM == "hatch":
+        shutil.move(
+            build_system_dir / "hatch-pyproject.toml",
+            PROJECT_DIRECTORY / 'pyproject.toml'
+        )     
     else:
         shutil.move(
             build_system_dir / "base-pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
     remove_dir("build-system")
```

### Comparing `scicookie-0.3.0/src/scicookie/logs.py` & `scicookie-0.4.0/src/scicookie/logs.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/profile.py` & `scicookie-0.4.0/src/scicookie/profile.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/profiles/base.yaml` & `scicookie-0.4.0/src/scicookie/profiles/base.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-author_name:
+author_full_name:
   message: Author's name
   help: See more at https://
   type: text
   default: Roronoa Zoro
   enabled: true
 
 author_email:
@@ -15,15 +15,15 @@
 project_name:
   message: Project name the title of the project
   help: ""
   type: text
   default: OSL Python package
   enabled: true
 
-project_description:
+project_short_description:
   message: Project short description
   help: ""
   type: text
   default: This Project aims to ...
   enabled: true
 
 project_slug:
@@ -82,14 +82,15 @@
   type: single-choice
   choices:
     - poetry
     - flit
     - mesonpy
     - setuptools
     - pdm
+    - hatch
   enabled: false
 
 command_line_interface:
   message: Select the Command Line Interface (CLI)
   help: ""
   type: single-choice
   choices:
```

### Comparing `scicookie-0.3.0/src/scicookie/profiles/osl.yaml` & `scicookie-0.4.0/src/scicookie/profiles/osl.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-author_name:
+author_full_name:
   enabled: true
 
 author_email:
   enabled: true
 
 project_name:
   enabled: true
 
-project_description:
+project_short_description:
   enabled: true
 
 project_slug:
   enabled: true
 
 package_slug:
   enabled: true
```

### Comparing `scicookie-0.3.0/src/scicookie/ui.py` & `scicookie-0.4.0/src/scicookie/ui.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     - uses: actions/checkout@v3
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniconda-version: "latest"
         mamba-version: "1.*"
         environment-file: conda/dev.yaml
         channels: conda-forge,nodefaults
+        channel-priority: true
         activate-environment: {{ cookiecutter.project_slug }}
         use-mamba: true
         miniforge-variant: Mambaforge
 
     - name: Install dependencies
       run: poetry install
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,23 @@
       run:
         shell: bash -l {0}
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: conda-incubator/setup-miniconda@v2
-      with:
-        miniconda-version: "latest"
-        mamba-version: "1.*"
-        environment-file: conda/dev.yaml
-        channels: conda-forge,nodefaults
-        activate-environment: {{ cookiecutter.project_slug }}
-        use-mamba: true
-        miniforge-variant: Mambaforge
+        with:
+          miniconda-version: "latest"
+          mamba-version: "1.*"
+          environment-file: conda/dev.yaml
+          channels: conda-forge,nodefaults
+          channel-priority: true
+          activate-environment: {{ cookiecutter.project_slug }}
+          use-mamba: true
+          miniforge-variant: Mambaforge
 
       - name: Install deps
         run: poetry install
 
       - name: Run semantic release (for tests)
         if: ${{ "{{ github.event_name != 'workflow_dispatch' }}" }}
         env:
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
 	flit build
 {%- elif cookiecutter.build_system == "mesonpy" %}
 	meson build
 {%- elif cookiecutter.build_system == "setuptools" %}
 	python -m build
 {%- elif cookiecutter.build_system == "pdm" %}
 	pdm build
+{%- elif cookiecutter.build_system == "hatch" %}
+	hatch build
 {%- endif %}
 
 .PHONY:release-ci
 release-ci:
 	$(RELEASE_APP) --ci
 
 .PHONY:release-dry
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/README.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   reproduce our development and production environments without any conflicts or
   inconsistencies.
 
   With Docker, we can easily share our application with others and deploy it to
   different environments. This streamlines our development, testing, deployment,
   and collaboration workflows, making the entire process more efficient.
 {%- elif cookiecutter.use_containers == 'Podman' %}
-* Integration with DevOps tools: Podman in your Python project helps us
+* Integration with DevOps tools: Podman in our Python project helps us
   achieve a more secure, efficient, and flexible containerization strategy, and
   give us more control over application's dependencies and configurations.
   Podman allows us to manage containers without the need for a daemon, providing a
   more secure and lightweight solution.
 
   With Podman, we can easily create and run containers, as well as manage their
   lifecycle and resources. This integration has improved our development and
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 
 [project]
 name = "{{ cookiecutter.project_slug }}"
 authors = [
   { name = "{{ cookiecutter.author_full_name }}", email = "{{ cookiecutter.author_email }}" },
 ]
 description = "{{ cookiecutter.project_short_description }}"
+{% if cookiecutter.project_layout == "src" -%}
+packages = [
+  {include = "{{ cookiecutter.package_slug }}", from="src"},
+]
+{% else -%}
+packages = [
+  {include = "{{ cookiecutter.package_slug }}"},
+]
+{% endif -%}
 readme = "README.md"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
 {%- if cookiecutter.project_license == "MIT" %}
   "License :: OSI Approved :: MIT License",
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy-pyproject.toml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 [build-system]
-build-backend = "mesonpy"
-requires = ["meson", "meson-python"]
+requires = ["pdm-backend"]
+build-backend = "pdm.backend"
 
 
 [project]
 name = "{{ cookiecutter.project_slug }}"
 description = "{{ cookiecutter.project_short_description }}"
 authors = [
   { name = "{{ cookiecutter.author_full_name }}", email = "{{ cookiecutter.author_email }}" },
 ]
+{% if cookiecutter.project_layout == "src" -%}
+packages = [
+  {include = "{{ cookiecutter.package_slug }}", from="src"},
+]
+{% else -%}
+packages = [
+  {include = "{{ cookiecutter.package_slug }}"},
+]
+{% endif -%}
 readme = "README.md"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
 {%- if cookiecutter.project_license == "MIT" %}
   "License :: OSI Approved :: MIT License",
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch-pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [build-system]
-requires = ["pdm-backend"]
-build-backend = "pdm.backend"
-
+requires = ["hatchling>=1.17.1"]
+build-backend = "hatchling.build"
 
 [project]
 name = "{{ cookiecutter.project_slug }}"
-description = "{{ cookiecutter.project_short_description }}"
 authors = [
   { name = "{{ cookiecutter.author_full_name }}", email = "{{ cookiecutter.author_email }}" },
 ]
+description = "{{ cookiecutter.project_short_description }}"
 readme = "README.md"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
 {%- if cookiecutter.project_license == "MIT" %}
   "License :: OSI Approved :: MIT License",
@@ -31,93 +30,99 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
-dynamic = ["version"]
-requires-python = ">=3.8"
+version = "{{ cookiecutter.project_version }}"
+requires-python = ">=3.8.1"
 dependencies = [
 {# keep this line here #}
 {%- if cookiecutter.use_pytest == "yes" -%}
-    "pytest>=7.3.2",
+    "pytest >= 7.3.2",
 {% if cookiecutter.use_coverage == "yes" -%}
-    "pytest-cov>=4.1.0",
+    "pytest-cov >= 4.1.0",
 {% endif %}
 {%- endif -%}{#- end of use_pytest -#}
 {%- if cookiecutter.use_hypothesis == "yes" -%}
-    "hypothesis>=6.0",
+    "hypothesis >= 6.0",
 {% endif %}
 {%- if cookiecutter.use_coverage == "yes" -%}
-    "coverage>=7.2.7",
+    "coverage >= 7.2.7",
 {% endif %}
 {%- if cookiecutter.use_blue == "yes" -%}
-    "blue>=0.9.1",
+    "blue >= 0.9.1",
 {% endif %}
 {%- if cookiecutter.use_black == "yes" -%}
-    "black>=23.3.0",
+    "black >= 23.3.0",
 {% endif %}
 {%- if cookiecutter.use_isort == "yes" -%}
-    "isort>=5.12.0",
+    "isort >= 5.12.0",
 {% endif %}
 {%- if cookiecutter.use_pre_commit -%}
-    "pre-commit>=3.3.2",
+    "pre-commit >= 3.3.2",
 {% endif %}
 {%- if cookiecutter.use_flake8 == "yes" -%}
-    "flake8>=4.0.1, <7",
+    "flake8 >= 4.0.1, < 7",
 {% endif %}
 {%- if cookiecutter.use_ruff == "yes" -%}
-    "ruff>=0.0.272",
+    "ruff >= 0.0.272",
 {% endif %}
 {%- if cookiecutter.use_mypy == "yes" -%}
-    "mypy>=1.3.0",
+    "mypy >= 1.3.0",
 {% endif %}
 {%- if cookiecutter.use_bandit == "yes" -%}
-    "bandit>=1.7.5",
+    "bandit >= 1.7.5",
 {% endif %}
 {%- if cookiecutter.use_pydocstyle == "yes" -%}
-    "pydocstyle>=6.3.0",
+    "pydocstyle >= 6.3.0",
 {% endif %}
 {%- if cookiecutter.use_vulture == "yes" -%}
-    "vulture>=2.7",
+    "vulture >= 2.7",
 {% endif %}
 {%- if cookiecutter.use_mccabe == "yes" -%}
-    "mccabe>=0.6.1",
+    "mccabe >= 0.6.1",
 {% endif %}
 {%- if cookiecutter.use_containers in ['Docker', 'Podman'] -%}
 # if you want to use docker-compose from your system, remove compose-go here
-    "compose-go>=2.18.1",
+    "compose-go >= 2.18.1",
 {% endif %}
-    "ipython<8",
-    "ipykernel>=6.0.0",
 {%- if cookiecutter.documentation_engine == 'mkdocs' -%}
-    "Jinja2>=3.1.2",
-    "mkdocs>=1.4.3",
-    "mkdocs-exclude>=1.0.2",
-    "mkdocs-jupyter>=0.24.1",
-    "mkdocs-literate-nav>=0.6.0",
-    "mkdocs-macros-plugin>=0.7.0, <1",
-    "mkdocs-material>=9.1.15",
-    "mkdocstrings>=0.21.2",
-    "mkdocstrings-python>=1.1.2",
+    "Jinja2 >= 3.1.2",
+    "mkdocs >= 1.4.3",
+    "mkdocs-exclude >= 1.0.2",
+    "mkdocs-jupyter >= 0.24.1",
+    "mkdocs-literate-nav >= 0.6.0",
+    "mkdocs-macros-plugin >= 0.7.0, < 1",
+    "mkdocs-material >= 9.1.15",
+    "mkdocstrings >= 0.21.2",
+    "mkdocstrings-python >= 1.1.2",
 {% elif cookiecutter.documentation_engine == 'sphinx' -%}
-    "Sphinx>=6.2.1",
-    "sphinx-rtd-theme>=1.2.2",
-    "importlib-metadata>=6.5.1",
-    "myst-parser>=0.19.2",
-    "nbsphinx>=0.9.2",
-    "pandoc>=2.3",
+    "Sphinx >= 6.2.1",
+    "sphinx-rtd-theme >= 1.2.2",
+    "importlib-metadata >= 6.5.1",
+    "myst-parser >= 0.19.2",
+    "nbsphinx >= 0.9.2",
+    "pandoc >= 2.3",
 {% elif cookiecutter.documentation_engine == 'jupyter-book' -%}
-    "jupyter-book>=0.15.1",
-    "myst-parser>=0.18.1",
+    "jupyter-book >= 0.15.1",
+    "myst-parser >= 0.18.1",
 {% endif %}
 ]
 
 [project.urls]
 Homepage = "{{ cookiecutter.project_url }}"
 "Bug Tracker" = "{{ cookiecutter.project_url }}/issues"
 Discussions = "{{ cookiecutter.project_url }}/discussions"
 Changelog = "{{ cookiecutter.project_url }}/releases"
 
+[tool.hatch.version]
+{# keep this line here #}
+{%- if cookiecutter.project_layout == 'flat' -%}
+path = "{{ cookiecutter.package_slug }}/__init__.py"
+{% elif cookiecutter.project_layout == 'src' -%}
+path = "src/{{ cookiecutter.package_slug }}/__init__.py"
+{% endif %}
+
 {% include "build-system/base-pyproject.toml" %}
 {#- keep this line at the end of the file -#}
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 [tool.poetry]
 name = "{{ cookiecutter.project_slug }}"
 version = "{{ cookiecutter.project_version }}"  # semantic-release
 description = "{{ cookiecutter.project_short_description }}"
 authors = ["{{ cookiecutter.author_full_name }} <{{ cookiecutter.author_email }}>"]
+{% if cookiecutter.project_layout == "src" -%}
+packages = [
+  {include = "{{ cookiecutter.package_slug }}", from="src"},
+]
+{% else -%}
+packages = [
+  {include = "{{ cookiecutter.package_slug }}"},
+]
+{% endif -%}
 license = "{{ cookiecutter.project_license }}"
 exclude = [
   ".git/*",
   ".env*",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 {%- elif cookiecutter.build_system == "mesonpy" %}
   - meson-python
 {%- elif cookiecutter.build_system == "setuptools" %}
   - setuptools
   - build
 {%- elif cookiecutter.build_system == "pdm" %}
   - pdm
+{%- elif cookiecutter.build_system == "hatch" %}
+  - hatch
 {%- endif %}
   - nodejs  # used by semantic-release
   - shellcheck
 {%- if cookiecutter.documentation_engine == "sphinx" %}
   - pandoc
 {%- endif %}
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md`

 * *Files 18% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 {%- elif cookiecutter.build_system == "pdm" -%}
 In addition, you should know that to build our package we use
 [PDM](https://pdm.fming.dev/), it's a build system for Python projects.
 It provides an efficient and fast way to manage project dependencies, as
 well as build and distribute code. It is fast to install, has built-in
 virtualenv, offers support for different package sources, and provides
 an easy way to distribute code.
+[Hatch](https://hatch.pypa.io): It's a Python Package that is compatible build backend used by Hatch, a modern, extensible Python project manager. It provides a standardized build system with reproducible builds by default, robust environment management with support for custom scripts, easy publishing to PyPI or other indexes, version management, and configurable project generation with sane defaults. Hatchling might support multiple programming languages and offer language-specific options for building projects in different languages. It could also provide customization and extensibility options, allowing you to incorporate plugins or scripts for tailored build processes.
 
 {%- endif %}
 
 Contributions are welcome, and they are greatly appreciated! Every little bit
 helps, and credit will always be given.
 
 You can contribute in many ways:
```

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.package_slug}}.py` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.package_slug}}.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py` & `scicookie-0.4.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.3.0/PKG-INFO` & `scicookie-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scicookie
-Version: 0.3.0
+Version: 0.4.0
 Summary: Cookiecutter template for a Python package
 License: BSD
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: cookieninja (==1.0.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
-Requires-Dist: pyyaml (>=5)
+Requires-Dist: pyyaml (>=6.0.1)
 Requires-Dist: sh (>=2.0.4,<3.0.0)
```

