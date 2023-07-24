# Comparing `tmp/ansible-navigator-3.4.0.tar.gz` & `tmp/ansible-navigator-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-navigator-3.4.0.tar", last modified: Mon Jun 12 13:01:13 2023, max compression
+gzip compressed data, was "ansible-navigator-3.4.1.tar", last modified: Mon Jul 24 13:07:42 2023, max compression
```

## Comparing `ansible-navigator-3.4.0.tar` & `ansible-navigator-3.4.1.tar`

### file list

```diff
@@ -1,253 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.483214 ansible-navigator-3.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/chronographer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-12 13:01:13.483214 ansible-navigator-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/docs/.generated/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/.generated/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/_ext/regenerate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/contributing/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/contributing/guidelines.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.447213 ansible-navigator-3.4.0/docs/contributing/images/
--rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/contributing/images/test_tree_view.png
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/contributing/security.md
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/settings.md
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/docs/subcommands.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.451213 ansible-navigator-3.4.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.dark_vs.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.source.json.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.source.shell.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.source.yaml.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.text.html.basic.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.text.html.derivative.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.text.html.markdown.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/licenses/LICENSE.text.log.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:01:13.483214 ansible-navigator-3.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.439213 ansible-navigator-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.451213 ansible-navigator-3.4.0/src/ansible_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 13:01:13.000000 ansible-navigator-3.4.0/src/ansible_navigator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/_version_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/action_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/action_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/action_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.467213 ansible-navigator-3.4.0/src/ansible_navigator/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/back.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/help_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/quit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/sample_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/sample_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/sample_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/serialize_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/serialize_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/app_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.467213 ansible-navigator-3.4.0/src/ansible_navigator/command_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/command_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/command_runner/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.471214 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
--rw-r--r--   0 runner    (1001) docker     (123)    31712 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    48249 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/content_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.471214 ansible-navigator-3.4.0/src/ansible_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/ansible-navigator.json
--rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/catalog_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.475214 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/source.json.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/source.shell.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/source.yaml.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.html.basic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.html.derivative.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.html.markdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.log.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/help.md
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/image_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/images_dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/settings-sample.template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/settings-schema.partial.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.475214 ansible-navigator-3.4.0/src/ansible_navigator/data/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/themes/dark_vs.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/themes/terminal_colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/data/welcome.md
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.475214 ansible-navigator-3.4.0/src/ansible_navigator/image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/image_manager/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/image_manager/introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/image_manager/introspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/image_manager/puller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.475214 ansible-navigator-3.4.0/src/ansible_navigator/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/ansible_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/ansible_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/ansible_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/command_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/runner/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.479214 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/fchainmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/grammars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.483214 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/curses_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/curses_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_curses_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_working.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/menu_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/ui_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.483214 ansible-navigator-3.4.0/src/ansible_navigator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/dict_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/dot_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/packaged_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.483214 ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/src/ansible_navigator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:01:13.455213 ansible-navigator-3.4.0/src/ansible_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-12 13:01:13.000000 ansible-navigator-3.4.0/src/ansible_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-12 13:01:13.000000 ansible-navigator-3.4.0/src/ansible_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:01:13.000000 ansible-navigator-3.4.0/src/ansible_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 13:01:13.000000 ansible-navigator-3.4.0/src/ansible_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-12 13:01:13.000000 ansible-navigator-3.4.0/src/ansible_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 13:01:13.000000 ansible-navigator-3.4.0/src/ansible_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-12 13:00:51.000000 ansible-navigator-3.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.202743 ansible-navigator-3.4.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.202743 ansible-navigator-3.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/chronographer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.github/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/images/test_tree_view.png
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.210743 ansible-navigator-3.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.210743 ansible-navigator-3.4.1/docs/.generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/.generated/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.210743 ansible-navigator-3.4.1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/_ext/regenerate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.214743 ansible-navigator-3.4.1/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/guidelines.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.214743 ansible-navigator-3.4.1/docs/contributing/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/images/test_tree_view.png
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/security.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/subcommands.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.222743 ansible-navigator-3.4.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.asottile_tm_tokenize.all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.dark_vs.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.source.json.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.source.shell.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.source.yaml.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.html.basic.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.html.derivative.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.html.markdown.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.log.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.186743 ansible-navigator-3.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.230743 ansible-navigator-3.4.1/src/ansible_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/_version_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/action_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/action_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/action_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.250743 ansible-navigator-3.4.1/src/ansible_navigator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/back.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/help_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/quit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/app_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.250743 ansible-navigator-3.4.1/src/ansible_navigator/command_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/command_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/command_runner/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.258742 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/defs_presentable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49073 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/content_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.262743 ansible-navigator-3.4.1/src/ansible_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/catalog_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.262743 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/log.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.json.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.yaml.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.basic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.derivative.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.log.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/help.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/image_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/images_dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/settings-sample.template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/settings-schema.partial.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.262743 ansible-navigator-3.4.1/src/ansible_navigator/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/themes/dark_vs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/themes/terminal_colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.266743 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/introspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/puller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.266743 ansible-navigator-3.4.1/src/ansible_navigator/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/command_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.278742 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/fchainmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.286743 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_curses_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/menu_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/src/ansible_navigator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/dict_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/dot_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/packaged_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.234742 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-24 13:07:42.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/tox.ini
```

### Comparing `ansible-navigator-3.4.0/.config/dictionary.txt` & `ansible-navigator-3.4.1/.config/dictionary.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,64 +27,65 @@
 000001a0: 6162 6c65 730a 6578 746c 696e 6b73 0a66  ables.extlinks.f
 000001b0: 6163 656c 6573 7375 7365 720a 6665 646f  acelessuser.fedo
 000001c0: 7261 7072 6f6a 6563 740a 666f 6e74 6177  raproject.fontaw
 000001d0: 6573 6f6d 650a 6671 636e 0a66 726f 6d6c  esome.fqcn.froml
 000001e0: 6973 740a 6865 6164 6572 6c69 6e6b 0a68  ist.headerlink.h
 000001f0: 656c 7063 6f6e 6669 670a 686f 7374 7661  elpconfig.hostva
 00000200: 7273 0a68 7265 6673 0a68 746d 6c70 726f  rs.hrefs.htmlpro
-00000210: 6f66 6572 0a68 7474 7061 7069 0a69 6d70  ofer.httpapi.imp
-00000220: 6f72 7461 626c 6573 0a69 6e6c 696e 6568  ortables.inlineh
-00000230: 696c 6974 650a 696e 7465 7273 7068 696e  ilite.intersphin
-00000240: 780a 696e 7472 6f73 7065 6374 6f72 0a69  x.introspector.i
-00000250: 7361 7474 790a 6a73 6f6e 7363 6865 6d61  satty.jsonschema
-00000260: 0a6b 6565 7065 6e64 730a 6b65 6765 7820  .keepends.kegex 
-00000270: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00000280: 416e 2061 6374 696f 6e27 7320 7265 6765  An action's rege
-00000290: 780a 6b65 6765 7865 730a 6c65 6e74 6578  x.kegexes.lentex
-000002a0: 740a 6c65 7665 6c6e 616d 650a 6c69 626f  t.levelname.libo
-000002b0: 6e69 670a 6c69 6768 7462 756c 6273 0a6c  nig.lightbulbs.l
-000002c0: 696e 656e 756d 730a 6c69 6e6b 6368 6563  inenums.linkchec
-000002d0: 6b0a 6c69 6e74 6162 6c65 0a6c 696e 7461  k.lintable.linta
-000002e0: 626c 6573 0a6d 6167 6963 6c69 6e6b 0a6d  bles.magiclink.m
-000002f0: 6173 6b61 626c 6573 0a6d 6178 7370 6c69  askables.maxspli
-00000300: 740a 6d6b 646f 6373 0a6d 6b64 6f63 7374  t.mkdocs.mkdocst
-00000310: 7269 6e67 730a 6d6f 6475 6c65 6175 7468  rings.moduleauth
-00000320: 6f72 0a6d 7175 6575 6520 2020 2020 2020  or.mqueue       
-00000330: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
-00000340: 2f67 6974 6875 622e 636f 6d2f 616e 7369  /github.com/ansi
-00000350: 626c 652f 616e 7369 626c 652d 7275 6e6e  ble/ansible-runn
-00000360: 6572 2f69 7373 7565 732f 3938 340a 6d79  er/issues/984.my
-00000370: 7072 6f6a 6563 740a 6e65 7463 6f6d 6d6f  project.netcommo
-00000380: 6e20 2020 2020 2020 2020 2020 2320 416e  n           # An
-00000390: 7369 626c 6520 6e65 7477 6f72 6b20 636f  sible network co
-000003a0: 6c6c 6563 7469 6f6e 2c20 7365 656e 2069  llection, seen i
-000003b0: 6e20 7465 7374 7320 616e 6420 5245 4144  n tests and READ
-000003c0: 4d45 0a6e 6574 636f 6e66 0a6e 6974 7069  ME.netconf.nitpi
-000003d0: 636b 790a 6e6f 6e62 6c6f 636b 696e 670a  cky.nonblocking.
-000003e0: 6f6c 646d 6173 6b0a 6f6e 656c 696e 650a  oldmask.oneline.
-000003f0: 6f6e 6967 7572 756d 6163 6666 690a 6f70  onigurumacffi.op
-00000400: 656e 7365 6172 6368 0a6f 7866 6f72 6463  ensearch.oxfordc
-00000410: 6f6d 6d61 0a70 6167 6576 6965 770a 7072  omma.pageview.pr
-00000420: 6563 6c65 6172 0a70 7265 636f 6d6d 616e  eclear.precomman
-00000430: 640a 7072 656d 616e 656e 740a 7075 6c6c  d.premanent.pull
-00000440: 6162 6c65 0a70 796d 646f 776e 0a70 796d  able.pymdown.pym
-00000450: 646f 776e 780a 7265 6468 6174 696e 7369  downx.redhatinsi
-00000460: 6768 7473 0a72 6570 7265 7365 6e74 6572  ghts.representer
-00000470: 0a72 6574 7572 6e64 6f63 730a 7275 6e74  .returndocs.runt
-00000480: 696d 6573 0a73 6372 6f6c 6c62 6163 6b0a  imes.scrollback.
-00000490: 7365 6374 696f 6e61 7574 686f 720a 7365  sectionauthor.se
-000004a0: 7475 7074 6f6f 6c73 2020 2020 2020 2020  tuptools        
-000004b0: 2020 2320 5573 6564 2069 6e20 5f76 6572    # Used in _ver
-000004c0: 7369 6f6e 2e70 7969 0a73 6d61 7274 7175  sion.pyi.smartqu
-000004d0: 6f74 6573 0a73 6f6d 6576 616c 7565 0a73  otes.somevalue.s
-000004e0: 7461 7465 6d61 6368 696e 650a 7374 7269  tatemachine.stri
-000004f0: 7073 7061 6365 730a 7375 6261 6374 696f  pspaces.subactio
-00000500: 6e0a 7375 6273 6368 656d 610a 7375 7065  n.subschema.supe
-00000510: 7266 656e 6365 730a 7465 6d70 6c61 7461  rfences.templata
-00000520: 626c 650a 7465 6d70 6c61 7465 640a 7465  ble.templated.te
-00000530: 6d70 6c61 7469 6e67 0a74 6573 7468 6f73  mplating.testhos
-00000540: 740a 7465 7374 6e61 6d65 0a74 6f70 6261  t.testname.topba
-00000550: 720a 7472 6163 6562 6163 6b73 0a74 7275  r.tracebacks.tru
-00000560: 6563 6f6c 6f72 0a75 7365 6669 7874 7572  ecolor.usefixtur
-00000570: 6573 0a75 7365 7262 6173 650a 7669 6577  es.userbase.view
-00000580: 636f 6465 0a76 6f6c 6d6f 756e 740a 776f  code.volmount.wo
-00000590: 726b 6469 720a 786d 7373 0a              rkdir.xmss.
+00000210: 6f66 6572 0a68 7474 7061 7069 0a69 676e  ofer.httpapi.ign
+00000220: 6f72 6573 7061 6365 0a69 6d70 6f72 7461  orespace.importa
+00000230: 626c 6573 0a69 6e6c 696e 6568 696c 6974  bles.inlinehilit
+00000240: 650a 696e 7465 7273 7068 696e 780a 696e  e.intersphinx.in
+00000250: 7472 6f73 7065 6374 6f72 0a69 7361 7474  trospector.isatt
+00000260: 790a 6a73 6f6e 7363 6865 6d61 0a6b 6565  y.jsonschema.kee
+00000270: 7065 6e64 730a 6b65 6765 7820 2020 2020  pends.kegex     
+00000280: 2020 2020 2020 2020 2020 2320 416e 2061            # An a
+00000290: 6374 696f 6e27 7320 7265 6765 780a 6b65  ction's regex.ke
+000002a0: 6765 7865 730a 6c65 6e74 6578 740a 6c65  gexes.lentext.le
+000002b0: 7665 6c6e 616d 650a 6c69 626f 6e69 670a  velname.libonig.
+000002c0: 6c69 6768 7462 756c 6273 0a6c 696e 656e  lightbulbs.linen
+000002d0: 756d 730a 6c69 6e6b 6368 6563 6b0a 6c69  ums.linkcheck.li
+000002e0: 6e74 6162 6c65 0a6c 696e 7461 626c 6573  ntable.lintables
+000002f0: 0a6d 6167 6963 6c69 6e6b 0a6d 6173 6b61  .magiclink.maska
+00000300: 626c 6573 0a6d 6178 7370 6c69 740a 6d6b  bles.maxsplit.mk
+00000310: 646f 6373 0a6d 6b64 6f63 7374 7269 6e67  docs.mkdocstring
+00000320: 730a 6d6f 6475 6c65 6175 7468 6f72 0a6d  s.moduleauthor.m
+00000330: 7175 6575 6520 2020 2020 2020 2020 2020  queue           
+00000340: 2020 2023 2068 7474 7073 3a2f 2f67 6974     # https://git
+00000350: 6875 622e 636f 6d2f 616e 7369 626c 652f  hub.com/ansible/
+00000360: 616e 7369 626c 652d 7275 6e6e 6572 2f69  ansible-runner/i
+00000370: 7373 7565 732f 3938 340a 6d79 7072 6f6a  ssues/984.myproj
+00000380: 6563 740a 6e65 7463 6f6d 6d6f 6e20 2020  ect.netcommon   
+00000390: 2020 2020 2020 2020 2320 416e 7369 626c          # Ansibl
+000003a0: 6520 6e65 7477 6f72 6b20 636f 6c6c 6563  e network collec
+000003b0: 7469 6f6e 2c20 7365 656e 2069 6e20 7465  tion, seen in te
+000003c0: 7374 7320 616e 6420 5245 4144 4d45 0a6e  sts and README.n
+000003d0: 6574 636f 6e66 0a6e 6974 7069 636b 790a  etconf.nitpicky.
+000003e0: 6e6f 6e62 6c6f 636b 696e 670a 6f6c 646d  nonblocking.oldm
+000003f0: 6173 6b0a 6f6e 656c 696e 650a 6f6e 6967  ask.oneline.onig
+00000400: 7572 756d 6163 6666 690a 6f70 656e 7365  urumacffi.opense
+00000410: 6172 6368 0a6f 7866 6f72 6463 6f6d 6d61  arch.oxfordcomma
+00000420: 0a70 6167 6576 6965 770a 7072 6563 6c65  .pageview.precle
+00000430: 6172 0a70 7265 636f 6d6d 616e 640a 7072  ar.precommand.pr
+00000440: 656d 616e 656e 740a 7075 6c6c 6162 6c65  emanent.pullable
+00000450: 0a70 796d 646f 776e 0a70 796d 646f 776e  .pymdown.pymdown
+00000460: 780a 7265 6468 6174 696e 7369 6768 7473  x.redhatinsights
+00000470: 0a72 6570 7265 7365 6e74 6572 0a72 6574  .representer.ret
+00000480: 7572 6e64 6f63 730a 7275 6e74 696d 6573  urndocs.runtimes
+00000490: 0a73 6372 6f6c 6c62 6163 6b0a 7365 6374  .scrollback.sect
+000004a0: 696f 6e61 7574 686f 720a 7365 7475 7074  ionauthor.setupt
+000004b0: 6f6f 6c73 2020 2020 2020 2020 2020 2320  ools          # 
+000004c0: 5573 6564 2069 6e20 5f76 6572 7369 6f6e  Used in _version
+000004d0: 2e70 7969 0a73 6d61 7274 7175 6f74 6573  .pyi.smartquotes
+000004e0: 0a73 6f6d 6576 616c 7565 0a73 7461 7465  .somevalue.state
+000004f0: 6d61 6368 696e 650a 7374 7269 7073 7061  machine.stripspa
+00000500: 6365 730a 7375 6261 6374 696f 6e0a 7375  ces.subaction.su
+00000510: 6273 6368 656d 610a 7375 7065 7266 656e  bschema.superfen
+00000520: 6365 730a 7465 6d70 6c61 7461 626c 650a  ces.templatable.
+00000530: 7465 6d70 6c61 7465 640a 7465 6d70 6c61  templated.templa
+00000540: 7469 6e67 0a74 6573 7468 6f73 740a 7465  ting.testhost.te
+00000550: 7374 6e61 6d65 0a74 6f70 6261 720a 7472  stname.topbar.tr
+00000560: 6163 6562 6163 6b73 0a74 7275 6563 6f6c  acebacks.truecol
+00000570: 6f72 0a75 7365 6669 7874 7572 6573 0a75  or.usefixtures.u
+00000580: 7365 7262 6173 650a 7669 6577 636f 6465  serbase.viewcode
+00000590: 0a76 6f6c 6d6f 756e 740a 776f 726b 6469  .volmount.workdi
+000005a0: 720a 786d 7373 0a                        r.xmss.
```

### Comparing `ansible-navigator-3.4.0/.flake8` & `ansible-navigator-3.4.1/.flake8`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.git_archival.txt` & `ansible-navigator-3.4.1/.git_archival.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.github/CONTRIBUTING.md` & `ansible-navigator-3.4.1/.github/CONTRIBUTING.md`

 * *Files 13% similar despite different names*

```diff
@@ -107,14 +107,40 @@
 
 Hover to the **Testing** icon in the Activity Bar to see VSCode test tree. From
 there expand and reach to the desired unit or integration test and hit
 `Run Test` or `Debug Test` appropriately.
 
 ![VSCode test tree](images/test_tree_view.png)
 
+### Overview of Base Entry Points and Summary of src files
+
+- `src/ansible_navigator/cli.py` acts as the main entry point where the
+  application starts.
+- `src/ansible_navigator/ui.py` contains show() function which is the entry
+  point for rendering the UI.
+- `src/ansible_navigator/actions` has the implementation of all the actions
+  ansible-navigator can perform (i.e. its [subcommands]) like run, collections,
+  images, doc, inventory, settings and a lot more.
+- `src/ansible_navigator/command_runner` command runner is a wrapper around
+  subprocess to run shell commands.
+- `src/ansible_navigator/configuration_subsystem` herein lies the logic behind
+  all the CLI parameters from their declaration to processing.
+- `src/ansible_navigator/data` this directory includes non-python files and
+  stand alone scripts that will be run from inside an execution environment.
+- `src/ansible_navigator/image_manager` contains all the operations related to
+  introspect, access, pull container images.
+- `src/ansible_navigator/runner` herein lies ability for all the interaction
+  with ansible-runner.
+- `src/ansible_navigator/tm_tokenize` has the tokenization subsystem which
+  allows for syntax highlighting of json and yaml files.
+- `src/ansible_navigator/ui_framework` has the implementation of our
+  user-interface.
+- `src/ansible_navigator/utils` consists of all the common utilities use
+  throughout the application.
+
 ### Configure VSCode settings
 
 Once we are inside vscode with project installed, we should see a `.vscode`
 folder in our workspace. Having a launch configuration file is beneficial
 because it allow us to configure and save debugging setup details. VS Code keeps
 debugging configuration information in a `launch.json` file located in a
 `.vscode` folder in our workspace (project root folder).
@@ -132,70 +158,48 @@
 - Hover to the **Run and Debug** icon in the Activity Bar to start the debugger.
 
 At this point, the debugger should hit your breakpoint and start the debugging
 session.
 
 ### Debug Ansible-Navigator Subcommands
 
-Ansible-Navigator comes in with bunch of [sub-commands]. To debug around any
-specific subcommand, we will need to add `args` attribute (arguments passed to
-the program to debug) in our launch.json configuration file.
+Ansible-Navigator comes in with bunch of [subcommands]. To debug around any
+specific subcommand, use the **Run and Debug** drop down menu to select the
+appropriate entry from launch.json configuration. We add `args` attribute
+(arguments passed to the program to debug) in our launch.json configuration
+file.
 
-[sub-commands]: https://ansible-navigator.readthedocs.io/subcommands/
+[subcommands]: https://ansible-navigator.readthedocs.io/subcommands/
 
 **Example:**
 
-- Debug `ansible-navigator run` subcommand, use _args_ attribute, provide
-  absolute path to the playbook as mentioned. Following configuration will allow
-  to debug `ansible-navigator site.yml --mode stdout`.
+- To Debug `ansible-navigator run` subcommand, use _args_ attribute, provide
+  playbook name and absolute path to the playbook in _cwd_. Following
+  configuration will allow to debug `ansible-navigator site.yml --mode stdout`.
 
 ```json
 {
   "version": "0.2.0",
   "configurations": [
     {
       "name": "Debug subcommand: run",
       "type": "python",
       "request": "launch",
       "module": "ansible_navigator",
-      "args": ["run", "../Path/to/Playbook/site.yml", "--mode", "stdout"],
-      "cwd": "${workspaceFolder}/src",
+      "args": ["run", "site.yml", "--mode", "stdout"],
+      "cwd": "/home/user/../path/to/the/playbook",
       "justMyCode": false
     }
   ]
 }
 ```
 
-- Debug `ansible-navigator exec` subcommand using _args_ with some parameter.
-  Following configuration will allow to debug `ansible-navigator exec -- pwd`.
-
-```json
-{
-  "version": "0.2.0",
-  "configurations": [
-     {
-      "name": "Debug subcommand: exec",
-      "type": "python",
-      "request": "launch",
-      "module": "ansible_navigator",
-      "args": ["exec", "--", "pwd"],
-      "cwd": "${workspaceFolder}/src",
-      "justMyCode": false
-    }
-}
-```
-
-- To debug subcommand `ansible-navigator images`, add one more attribute as
-  `"args": ["images"]` in our previously configured launch.json.
-- To debug subcommand `ansible-navigator collections`, add one more attribute as
-  `"args": ["collections"]` in launch.json, and so on.
-- Moreover, to debug subcommands with some parameter use
-  `"args": ["subcommand-name", "--", "parameter"]`
-- While debugging any subcommand with arguments, make sure to use one _args_
-  entry at a time in our configuration (comment/remove the ones not in use).
+Similar configuration entries are present inside the launch.json file to debug
+different subcommands. Choose an entry from the drop-down while debugging and
+modify accordingly if needed.
 
 ### Useful Links
 
 - VS code debugging [guide].
 - Facilitate [Python Debugger] (pdb) in navigator for pure command line
   debugging.
```

### Comparing `ansible-navigator-3.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.github/SECURITY.md` & `ansible-navigator-3.4.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.github/dependabot.yml` & `ansible-navigator-3.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.github/workflows/release.yml` & `ansible-navigator-3.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.github/workflows/tox.yml` & `ansible-navigator-3.4.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.gitignore` & `ansible-navigator-3.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.pre-commit-config.yaml` & `ansible-navigator-3.4.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 exclude: >
   (?x)^(
     _readthedocs|
     .tox
   )$
 repos:
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.9-for-vscode"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         # Original hook implementation is flaky due to *several* bugs described
         # in https://github.com/prettier/prettier/issues/12364
         # a) CI=1 needed to avoid incomplete output
         # b) two executions are needed because --list-different works correctly
         # only when run with --check as with --write the output will also
@@ -30,21 +30,21 @@
         pass_filenames: false
         args: []
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
 
   - repo: https://github.com/psf/black.git
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         language_version: python3
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.278"
     hooks:
       - id: ruff
         args:
           - "--exit-non-zero-on-fix"
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
     rev: v6.31.0
@@ -85,15 +85,15 @@
     # Allow json comments, trailing commas
     # https://github.com/pre-commit/pre-commit-hooks/issues/395
     rev: v1.0.0
     hooks:
       - id: check-json5
 
   - repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.34.0
+    rev: v0.35.0
     hooks:
       - id: markdownlint
         exclude: >
           (?x)^
             (
               \.github/ISSUE_TEMPLATE/\w+|
               docs/(
@@ -102,15 +102,15 @@
               )|
               README|
               src/ansible_navigator/data/(help|welcome)
             )\.md
           $
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         # NOTE: dout is part of the stdout action regex
         args: ["-L", "dout"]
         # We exclude generated and external files as they are not directly under
         # our control, so we cannot fix spelling in them.
         exclude: >
@@ -136,20 +136,20 @@
         language_version: python3
         additional_dependencies:
           - darglint
           - flake8-docstrings # uses pydocstyle
 
   - repo: https://github.com/asottile/pyupgrade
     # keep it after flake8
-    rev: v3.4.0
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         args: ["--py39-plus"]
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
           - jinja2
           - libtmux
           - pytest
           - pytest-mock
```

### Comparing `ansible-navigator-3.4.0/.prettierignore` & `ansible-navigator-3.4.1/.prettierignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.vscode/launch.json` & `ansible-navigator-3.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/.vscode/settings.json` & `ansible-navigator-3.4.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/LICENSE` & `ansible-navigator-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/PKG-INFO` & `ansible-navigator-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.4.0
+Version: 3.4.1
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.4.0/README.md` & `ansible-navigator-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/cspell.config.yaml` & `ansible-navigator-3.4.1/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/docs/_ext/regenerate_docs.py` & `ansible-navigator-3.4.1/docs/_ext/regenerate_docs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/docs/contributing/guidelines.md` & `ansible-navigator-3.4.1/docs/contributing/guidelines.md`

 * *Files 13% similar despite different names*

```diff
@@ -107,14 +107,40 @@
 
 Hover to the **Testing** icon in the Activity Bar to see VSCode test tree. From
 there expand and reach to the desired unit or integration test and hit
 `Run Test` or `Debug Test` appropriately.
 
 ![VSCode test tree](images/test_tree_view.png)
 
+### Overview of Base Entry Points and Summary of src files
+
+- `src/ansible_navigator/cli.py` acts as the main entry point where the
+  application starts.
+- `src/ansible_navigator/ui.py` contains show() function which is the entry
+  point for rendering the UI.
+- `src/ansible_navigator/actions` has the implementation of all the actions
+  ansible-navigator can perform (i.e. its [subcommands]) like run, collections,
+  images, doc, inventory, settings and a lot more.
+- `src/ansible_navigator/command_runner` command runner is a wrapper around
+  subprocess to run shell commands.
+- `src/ansible_navigator/configuration_subsystem` herein lies the logic behind
+  all the CLI parameters from their declaration to processing.
+- `src/ansible_navigator/data` this directory includes non-python files and
+  stand alone scripts that will be run from inside an execution environment.
+- `src/ansible_navigator/image_manager` contains all the operations related to
+  introspect, access, pull container images.
+- `src/ansible_navigator/runner` herein lies ability for all the interaction
+  with ansible-runner.
+- `src/ansible_navigator/tm_tokenize` has the tokenization subsystem which
+  allows for syntax highlighting of json and yaml files.
+- `src/ansible_navigator/ui_framework` has the implementation of our
+  user-interface.
+- `src/ansible_navigator/utils` consists of all the common utilities use
+  throughout the application.
+
 ### Configure VSCode settings
 
 Once we are inside vscode with project installed, we should see a `.vscode`
 folder in our workspace. Having a launch configuration file is beneficial
 because it allow us to configure and save debugging setup details. VS Code keeps
 debugging configuration information in a `launch.json` file located in a
 `.vscode` folder in our workspace (project root folder).
@@ -132,70 +158,48 @@
 - Hover to the **Run and Debug** icon in the Activity Bar to start the debugger.
 
 At this point, the debugger should hit your breakpoint and start the debugging
 session.
 
 ### Debug Ansible-Navigator Subcommands
 
-Ansible-Navigator comes in with bunch of [sub-commands]. To debug around any
-specific subcommand, we will need to add `args` attribute (arguments passed to
-the program to debug) in our launch.json configuration file.
+Ansible-Navigator comes in with bunch of [subcommands]. To debug around any
+specific subcommand, use the **Run and Debug** drop down menu to select the
+appropriate entry from launch.json configuration. We add `args` attribute
+(arguments passed to the program to debug) in our launch.json configuration
+file.
 
-[sub-commands]: https://ansible-navigator.readthedocs.io/subcommands/
+[subcommands]: https://ansible-navigator.readthedocs.io/subcommands/
 
 **Example:**
 
-- Debug `ansible-navigator run` subcommand, use _args_ attribute, provide
-  absolute path to the playbook as mentioned. Following configuration will allow
-  to debug `ansible-navigator site.yml --mode stdout`.
+- To Debug `ansible-navigator run` subcommand, use _args_ attribute, provide
+  playbook name and absolute path to the playbook in _cwd_. Following
+  configuration will allow to debug `ansible-navigator site.yml --mode stdout`.
 
 ```json
 {
   "version": "0.2.0",
   "configurations": [
     {
       "name": "Debug subcommand: run",
       "type": "python",
       "request": "launch",
       "module": "ansible_navigator",
-      "args": ["run", "../Path/to/Playbook/site.yml", "--mode", "stdout"],
-      "cwd": "${workspaceFolder}/src",
+      "args": ["run", "site.yml", "--mode", "stdout"],
+      "cwd": "/home/user/../path/to/the/playbook",
       "justMyCode": false
     }
   ]
 }
 ```
 
-- Debug `ansible-navigator exec` subcommand using _args_ with some parameter.
-  Following configuration will allow to debug `ansible-navigator exec -- pwd`.
-
-```json
-{
-  "version": "0.2.0",
-  "configurations": [
-     {
-      "name": "Debug subcommand: exec",
-      "type": "python",
-      "request": "launch",
-      "module": "ansible_navigator",
-      "args": ["exec", "--", "pwd"],
-      "cwd": "${workspaceFolder}/src",
-      "justMyCode": false
-    }
-}
-```
-
-- To debug subcommand `ansible-navigator images`, add one more attribute as
-  `"args": ["images"]` in our previously configured launch.json.
-- To debug subcommand `ansible-navigator collections`, add one more attribute as
-  `"args": ["collections"]` in launch.json, and so on.
-- Moreover, to debug subcommands with some parameter use
-  `"args": ["subcommand-name", "--", "parameter"]`
-- While debugging any subcommand with arguments, make sure to use one _args_
-  entry at a time in our configuration (comment/remove the ones not in use).
+Similar configuration entries are present inside the launch.json file to debug
+different subcommands. Choose an entry from the drop-down while debugging and
+modify accordingly if needed.
 
 ### Useful Links
 
 - VS code debugging [guide].
 - Facilitate [Python Debugger] (pdb) in navigator for pure command line
   debugging.
```

### Comparing `ansible-navigator-3.4.0/docs/contributing/images/test_tree_view.png` & `ansible-navigator-3.4.1/.github/images/test_tree_view.png`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/docs/contributing/security.md` & `ansible-navigator-3.4.1/docs/contributing/security.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/docs/faq.md` & `ansible-navigator-3.4.1/docs/faq.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Frequently asked questions
 
 [TOC]
 
+## Execution environments
+
+### What is an execution environment?
+
+An execution environment is a container image serving as an Ansible control
+node.
+
+See the
+[Getting started with Execution Environments guide](https://docs.ansible.com/ansible/devel/getting_started_ee/index.html)
+for details.
+
 ## The `ansible.cfg` file
 
 ### Where should the `ansible.cfg` file go when using an execution environment?
 
 The easiest place to have the `ansible.cfg` is in the project directory adjacent
 to the playbook. The playbook directory is automatically mounted in the
 execution environment and the `ansible.cfg` file will be found. If the
@@ -260,27 +271,37 @@
 $ export ANSIBLE_VAULT_PASSWORD_FILE=.vault_password
 # Pass the variable into the execution-environment
 $ ansible-navigator run --pass-environment-variable ANSIBLE_VAULT_PASSWORD_FILE site.yml
 ```
 
 2. Store the vault password in an environment variable
 
+Chances are that your environment prohibits saving passwords in clear text on
+disk. If you are subject to such a rule, then this will obviously include any
+command history file your shell saves to disk.
+
+In case you use bash, you can leverage
+[HISTCONTROL](https://www.gnu.org/software/bash/manual/html_node/Bash-Variables.html#index-HISTCONTROL)
+and an
+[environment](https://www.gnu.org/software/bash/manual/html_node/Environment.html)
+variable as shown in the following example.
+
 ```bash
 $ touch ~/.vault_password.sh
 $ chmod 700 ~/.vault_password.sh
 $ echo -e '#!/bin/sh\necho ${ANSIBLE_VAULT_PASSWORD}' >> ~/.vault_password.sh
 # Link the password file into the current working directory
 $ ln ~/.vault_password.sh .
 # The leading space here is necessary to keep the command out of the command history
 # by using an environment variable prefixed with ANSIBLE it will automatically get passed
 # into the execution environment
-$  export ANSIBLE_VAULT_SECRET=my_password
-# Set the environment variable to the location of the file
-$ ANSIBLE_VAULT_PASSWORD_FILE=.vault_password.sh
-$ ansible-navigator run site.yml
+$ HISTCONTROL=ignorespace
+$  export ANSIBLE_VAULT_PASSWORD=my_password
+# Set the environment variable to the location of the file when executing ansible-navigator
+$ ANSIBLE_VAULT_PASSWORD_FILE=.vault_password.sh ansible-navigator run site.yml
 ```
 
 Additional information about `ansible-vault` can be found
 [here](https://docs.ansible.com/ansible/latest/user_guide/vault.html)
 
 ## Other
```

### Comparing `ansible-navigator-3.4.0/docs/installation.md` & `ansible-navigator-3.4.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/docs/settings.md` & `ansible-navigator-3.4.1/docs/settings.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/docs/subcommands.md` & `ansible-navigator-3.4.1/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/licenses/LICENSE.asottile_tm_tokenize.all.txt` & `ansible-navigator-3.4.1/licenses/LICENSE.asottile_tm_tokenize.all.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/licenses/LICENSE.dark_vs.json.txt` & `ansible-navigator-3.4.1/licenses/LICENSE.dark_vs.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/licenses/LICENSE.source.json.json.txt` & `ansible-navigator-3.4.1/licenses/LICENSE.source.json.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/licenses/LICENSE.source.shell.json.txt` & `ansible-navigator-3.4.1/licenses/LICENSE.source.shell.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/licenses/LICENSE.source.yaml.json.txt` & `ansible-navigator-3.4.1/licenses/LICENSE.source.yaml.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/licenses/LICENSE.text.html.markdown.json.txt` & `ansible-navigator-3.4.1/licenses/LICENSE.text.html.markdown.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/licenses/LICENSE.text.log.json.txt` & `ansible-navigator-3.4.1/licenses/LICENSE.text.log.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/mkdocs.yml` & `ansible-navigator-3.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/mypy.ini` & `ansible-navigator-3.4.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/pyproject.toml` & `ansible-navigator-3.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -267,20 +267,23 @@
   'DTZ003', # The use of `datetime.datetime.utcnow()` is not allowed, use `datetime.datetime.now(tz=)` instead
   'DTZ005', # The use of `datetime.datetime.now()` without `tz` argument is not allowed
   'ERA001', # [*] Found commented-out code
   'F401', # [*] `ansible_navigator.version.__version__` imported but unused
   'FBT001', # Boolean positional arg in function definition
   'FBT002', # Boolean default value in function definition
   'FBT003', # Boolean positional value in function call
+  'FIX001', # Line contains FIXME
+  'FIX002', # Line contains TODO
   'INP001', # File `docs/_ext/regenerate_docs.py` is part of an implicit namespace package. Add an `__init__.py`.
   'N802', # Function name `formatTime` should be lowercase
   'N806', # Variable `FType` in function should be lowercase
   'N812', # Lowercase `__version_collection_doc_cache__` imported as non-lowercase `VERSION_CDC`
   'N813', # Camelcase `Action` imported as lowercase `stdout_action`
   'N817', # CamelCase `Constants` imported as acronym `C`
+  'PERF203', # `try`-`except` within a loop incurs performance overhead
   'PGH003', # Use specific rule codes when ignoring type issues
   'PIE810', # [*] Call `startswith` once with a `tuple`
   'PLC1901', # `self.fs_source == ""` can be simplified to `not self.fs_source` as an empty string is falsey
   'PLR0911', # Too many return statements (8 > 6)
   'PLR0912', # Too many branches (13 > 12)
   'PLR0913', # Too many arguments to function call (7 > 5)
   'PLR0915', # Too many statements (58 > 50)
@@ -320,14 +323,15 @@
   'PYI021', # Docstrings should not be included in stubs
   'RET501', # [*] Do not explicitly `return None` in function if it is the only possible return value
   'RET503', # [*] Missing explicit `return` at the end of function able to return non-`None` value
   'RET504', # Unnecessary variable assignment before `return` statement
   'RET505', # Unnecessary `else` after `return` statement
   'RUF005', # [*] Consider `[self._name, *shlex.split(self._interaction.action.match.groupdict()["params"] or "")]` instead of concatenation
   'RUF009', # Do not perform function call `PresentableCliParameters` in dataclass defaults
+  'RUF012', # Mutable class attributes should be annotated with `typing.ClassVar`
   'RUF100', # [*] Unused `noqa` directive (unused: `E731`)
   'S101', # Use of `assert` detected
   'S103', # `os.chmod` setting a permissive mask `0o777` on file or directory
   'S108', # Probable insecure usage of temporary file or directory: "/tmp"
   'S110', # `try`-`except`-`pass` detected, consider logging the exception
   'S311', # Standard pseudo-random generators are not suitable for cryptographic purposes
   'S602', # `subprocess` call with `shell=True` identified, security issue
@@ -335,14 +339,15 @@
   'S605', # Starting a process with a shell, possible injection detected
   'S607', # Starting a process with a partial executable path
   'SLF001', # Private member accessed: `_ui`
   'T201', # `print` found
   'TCH001', # Move application import `ansible_navigator.configuration_subsystem.definitions.SettingsEntry` into a type-checking block
   'TCH002', # Move third-party import `ansible_runner.Runner` into a type-checking block
   'TCH003', # Move standard library import `re.Pattern` into a type-checking block
+  'TD001', # Invalid TODO tag: `FIXME`
   'TD002', # Missing author in TODO
   'TD003', # Missing issue link on the line following this TODO
   'TRY003', # Avoid specifying long messages outside the exception class
   'TRY004', # Prefer `TypeError` exception for invalid type
   'TRY300', # Consider moving this statement to an `else` block
   'TRY301', # Abstract `raise` to an inner function
   'TRY400', # Use `logging.exception` instead of `logging.error`
```

### Comparing `ansible-navigator-3.4.0/requirements.txt` & `ansible-navigator-3.4.1/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,116 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
+# This file is autogenerated by pip-compile with Python 3.9
 # To update, run:
 #
-#    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --strip-extras setup.cfg
+#    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=resolvelib --unsafe-package=ruamel-yaml-clib pyproject.toml
 #
 ansible-builder==3.0.0
-ansible-core==2.14.3
-ansible-runner==2.3.2
-attrs==22.2.0
-beautifulsoup4==4.12.0
+ansible-core==2.15.1
+ansible-runner==2.3.3
+attrs==23.1.0
+beautifulsoup4==4.12.2
 bindep==2.11.0
-cairocffi==1.5.0
+cairocffi==1.6.0
 cairosvg==2.7.0
-certifi==2022.12.7
+certifi==2023.5.7
 cffi==1.15.1
 cfgv==3.3.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
-coverage==7.2.2
+coverage==7.2.7
 coverage-enable-subprocess==1.0
-cryptography==40.0.1
+cryptography==41.0.1
 csscompressor==0.9.5
 cssselect2==0.7.0
 darglint==1.8.1
 defusedxml==0.7.1
 distlib==0.3.6
 distro==1.8.0
-docutils==0.19
-exceptiongroup==1.1.1
+docutils==0.20.1
+exceptiongroup==1.1.2
 execnet==1.9.0
-filelock==3.10.6
+filelock==3.12.2
 flake8==6.0.0
 flake8-docstrings==1.7.0
 ghp-import==2.1.0
-griffe==0.25.5
+griffe==0.31.0
 htmlmin2==0.1.13
-identify==2.5.22
+identify==2.5.24
 idna==3.4
-importlib-metadata==6.1.0 ; python_version < "3.10.0"
+importlib-metadata==6.2.1 ; python_version < "3.10.0"
+importlib-resources==5.0.7
 iniconfig==2.0.0
 jinja2==3.1.2
 jsmin==3.0.1
-jsonschema==4.17.3
+jsonschema==4.18.0
+jsonschema-specifications==2023.6.1
 libtmux==0.16.1
 lockfile==0.12.2
 markdown==3.3.7
-markdown-exec==1.4.0
+markdown-exec==1.6.0
 markdown-include==0.8.1
-markupsafe==2.1.2
+markupsafe==2.1.3
 mccabe==0.7.0
 mergedeep==1.3.4
-mkdocs==1.4.2
-mkdocs-ansible==0.1.2
+mkdocs==1.4.3
+mkdocs-ansible==0.1.6
 mkdocs-autorefs==0.4.1
-mkdocs-gen-files==0.4.0
-mkdocs-htmlproofer-plugin==0.11.0
-mkdocs-material==9.1.4
+mkdocs-gen-files==0.5.0
+mkdocs-htmlproofer-plugin==0.13.1
+mkdocs-material==9.1.18
 mkdocs-material-extensions==1.1.1
 mkdocs-minify-plugin==0.6.4
-mkdocs-monorepo-plugin==1.0.4
-mkdocstrings==0.20.0
-mkdocstrings-python==0.8.3
-nodeenv==1.7.0
+mkdocs-monorepo-plugin==1.0.5
+mkdocstrings==0.22.0
+mkdocstrings-python==1.1.2
+nodeenv==1.8.0
 onigurumacffi==1.2.0
-packaging==23.0
+packaging==23.1
 parsley==1.3
 pbr==5.11.1
 pexpect==4.8.0
-pillow==9.4.0
-pipdeptree==2.7.0
-platformdirs==3.2.0
-pluggy==1.0.0
-pre-commit==3.2.1
+pillow==10.0.0
+pipdeptree==2.9.3
+platformdirs==3.8.0
+pluggy==1.2.0
+pre-commit==3.3.3
 ptyprocess==0.7.0
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 pyflakes==3.0.1
-pygments==2.14.0
-pymdown-extensions==9.10
-pyrsistent==0.19.3
-pytest==7.2.2
-pytest-mock==3.10.0
+pygments==2.15.1
+pymdown-extensions==10.0.1
+pytest==7.4.0
+pytest-mock==3.11.1
 pytest-plus==0.4.0
-pytest-subtests==0.10.0
-pytest-xdist==3.2.1
+pytest-subtests==0.11.0
+pytest-xdist==3.3.1
 python-daemon==3.0.1
 python-dateutil==2.8.2
 python-slugify==8.0.1
 pyyaml==6.0
 pyyaml-env-tag==0.1
-regex==2023.3.23
-requests==2.28.2
+referencing==0.29.1
+regex==2023.6.3
+requests==2.31.0
 requirements-parser==0.5.0
-resolvelib==0.8.1
+rpds-py==0.7.1
 six==1.16.0
 snowballstemmer==2.2.0
-soupsieve==2.4
+soupsieve==2.4.1
 text-unidecode==1.3
 tinycss2==1.2.1
 tomli==2.0.1
-types-setuptools==67.6.0.5
-typing-extensions==4.5.0 ; python_version < "3.10.0"
-tzdata==2023.2
-urllib3==1.26.15
-virtualenv==20.21.0
+types-setuptools==68.0.0.1
+typing-extensions==4.7.1 ; python_version < "3.10.0"
+tzdata==2023.3
+urllib3==2.0.3
+virtualenv==20.23.1
 watchdog==3.0.0
 webencodings==0.5.1
 zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
-# setuptools
+# resolvelib
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/_version_doc_cache.py` & `ansible-navigator-3.4.1/src/ansible_navigator/_version_doc_cache.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/action_base.py` & `ansible-navigator-3.4.1/src/ansible_navigator/action_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/action_defs.py` & `ansible-navigator-3.4.1/src/ansible_navigator/action_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/action_runner.py` & `ansible-navigator-3.4.1/src/ansible_navigator/action_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/__init__.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/_actions.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/_actions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/back.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/back.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/builder.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/collections.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/collections.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/config.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/doc.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/exec.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/exec.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/filter.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/filter.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/help_doc.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/help_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/images.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/images.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/inventory.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/lint.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/lint.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/log.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/log.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/open_file.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/open_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/quit.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/quit.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/refresh.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/refresh.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/rerun.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/rerun.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/run.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/run.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/sample_form.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/sample_notification.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_notification.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/sample_working.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/save.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/save.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/select.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/select.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/serialize_json.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_json.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/serialize_yaml.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/settings.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/settings.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/stdout.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/stdout.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/template.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/template.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/welcome.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/welcome.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/actions/write_file.py` & `ansible-navigator-3.4.1/src/ansible_navigator/actions/write_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/app_public.py` & `ansible-navigator-3.4.1/src/ansible_navigator/app_public.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/cli.py` & `ansible-navigator-3.4.1/src/ansible_navigator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,25 @@
 def log_dependencies() -> list[LogMessage]:
     """Retrieve installed packages and log as debug.
 
     :returns: All packages, version and location
     """
     pkgs = []
     found = []
+    messages: list[LogMessage] = []
     for _python_name, pkg_names in importlib_metadata.packages_distributions().items():
         for pkg_name in pkg_names:
             if pkg_name not in found:
                 found.append(pkg_name)
-                spec = find_spec(pkg_name)
+                try:
+                    spec = find_spec(pkg_name)
+                except ModuleNotFoundError:
+                    message = f"Package '{pkg_name}' is missing"
+                    messages.append(LogMessage(level=logging.DEBUG, message=message))
+                    continue
                 _location = spec.origin if spec else ""
                 _version = version(pkg_name)
                 pkgs.append(f"{pkg_name}=={_version} {_location}")
 
     pkgs.sort()
     messages = [LogMessage(level=logging.DEBUG, message=pkg) for pkg in pkgs]
     return messages
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/command_runner/command_runner.py` & `ansible-navigator-3.4.1/src/ansible_navigator/command_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/__init__.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/configurator.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/configurator.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/definitions.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/defs_presentable.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,19 @@
     settings_file_path: str | None = None
     settings_source: C = C.NOT_SET
 
 
 navigator_subcommands = [
     SubCommand(
         name="builder",
-        description="Build execution environment (container image)",
+        description=(
+            "Build [execution environment]"
+            "(https://docs.ansible.com/ansible/devel/getting_started_ee/index.html) "
+            "(container image)"
+        ),
         epilog=(
             "Note: 'ansible-navigator builder' additionally supports"
             " the same parameters as the 'ansible-builder' command."
             " For more information about these, try "
             " 'ansible-navigator builder --help-builder --mode stdout'"
         ),
         version_added="v2.0",
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import contextlib
 import importlib
 import logging
 import os
 import shlex
 import shutil
+import subprocess
 import sys
 import zoneinfo
 
 from functools import partialmethod
 from itertools import chain
 from itertools import repeat
 from pathlib import Path
@@ -651,14 +652,32 @@
                         message=(
                             "Try 'pip install ansible-lint' or consider using an execution "
                             "environment which provides ansible-lint."
                         ),
                         prefix=ExitPrefix.HINT,
                     ),
                 )
+            else:
+                try:
+                    subprocess.run("ansible-lint --version", shell=True, check=True)
+                except subprocess.CalledProcessError:
+                    exit_messages.append(
+                        ExitMessage(
+                            message=("ansible-lint does not seem to be installed correctly.")
+                        ),
+                    )
+                    exit_messages.append(
+                        ExitMessage(
+                            message=(
+                                "Ensure the command `ansible-lint --version` can be run prior to"
+                                " using ansible-navigator"
+                            ),
+                            prefix=ExitPrefix.HINT,
+                        ),
+                    )
 
         if isinstance(entry.value.current, str) and config.app == "lint":
             entry_name = entry.settings_file_path(prefix="")
             entry_source = entry.value.source
             source = abs_user_path(entry.value.current)
             try:
                 mount = VolumeMount(
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/parser.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/transform.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/transform.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/configuration_subsystem/utils.py` & `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/constants.py` & `ansible-navigator-3.4.1/src/ansible_navigator/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/content_defs.py` & `ansible-navigator-3.4.1/src/ansible_navigator/content_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/ansible-navigator.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/ansible-navigator.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/catalog_collections.py` & `ansible-navigator-3.4.1/src/ansible_navigator/data/catalog_collections.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/JSON.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/html.tmLanguage.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/log.tmLanguage.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/log.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/markdown.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/source.json.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.json.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/source.shell.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.shell.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/source.yaml.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.yaml.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.html.basic.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.basic.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.html.derivative.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.derivative.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.html.markdown.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.markdown.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/text.log.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.log.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/yaml.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/help.md` & `ansible-navigator-3.4.1/src/ansible_navigator/data/help.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/image_introspect.py` & `ansible-navigator-3.4.1/src/ansible_navigator/data/image_introspect.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Introspect an execution environment image."""
 from __future__ import annotations
 
 import json
-import multiprocessing
+import os
 import re
 import subprocess
 import sys
+import threading
 
 from queue import Queue
 from types import SimpleNamespace
 from typing import Any
 from typing import Callable
+from typing import Union
 
 
-PROCESSES = (multiprocessing.cpu_count() - 1) or 1
+JSONTypes = Union[bool, int, str, dict, list]
 
 
 class Command(SimpleNamespace):
     """Abstraction for a details about a shell command."""
 
     id_: str
     command: str
@@ -43,15 +45,15 @@
         )
         command.stdout = proc_out.stdout
     except subprocess.CalledProcessError as exc:
         command.stderr = str(exc.stderr)
         command.errors = [str(exc.stderr)]
 
 
-def worker(pending_queue: multiprocessing.Queue, completed_queue: multiprocessing.Queue) -> None:
+def worker(pending_queue: Queue, completed_queue: Queue) -> None:
     """Run a command from pending, parse, and place in completed.
 
     :param pending_queue: A queue with plugins to process
     :param completed_queue: The queue in which extracted documentation will be placed
     """
     while True:
         command = pending_queue.get()
@@ -72,48 +74,28 @@
     """
 
     def __init__(self):
         """Initialize the command runner."""
         self._completed_queue: Queue | None = None
         self._pending_queue: Queue | None = None
 
-    @staticmethod
-    def run_single_process(command_classes: Any):
-        """Run commands with a single process.
-
-        :param command_classes: All command classes to be run
-        :returns: The results from running all commands
-        """
-        all_commands = tuple(
-            command for command_class in command_classes for command in command_class.commands
-        )
-        results = []
-        for command in all_commands:
-            run_command(command)
-            try:
-                command.parse(command)
-            except Exception as exc:  # noqa: BLE001
-                command.errors = command.errors + [str(exc)]
-            results.append(command)
-        return results
-
-    def run_multi_process(self, command_classes):
-        """Run commands with multiple processes.
+    def run_multi_thread(self, command_classes):
+        """Run commands with multiple threads.
 
         Workers are started to read from pending queue.
         Exit when the number of results is equal to the number
         of commands needing to be run.
 
         :param command_classes: All command classes to be run
         :returns: The results from running all commands
         """
         if self._completed_queue is None:
-            self._completed_queue = multiprocessing.Manager().Queue()
+            self._completed_queue = Queue()
         if self._pending_queue is None:
-            self._pending_queue = multiprocessing.Manager().Queue()
+            self._pending_queue = Queue()
         results = {}
         all_commands = tuple(
             command for command_class in command_classes for command in command_class.commands
         )
         self.start_workers(all_commands)
         results = []
         while len(results) != len(all_commands):
@@ -121,18 +103,18 @@
         return results
 
     def start_workers(self, jobs):
         """Start workers and submit jobs to pending queue.
 
         :param jobs: The jobs to be run
         """
-        worker_count = min(len(jobs), PROCESSES)
+        worker_count = len(jobs)
         processes = []
         for _proc in range(worker_count):
-            proc = multiprocessing.Process(
+            proc = threading.Thread(
                 target=worker,
                 args=(self._pending_queue, self._completed_queue),
             )
             processes.append(proc)
             proc.start()
         for job in jobs:
             self._pending_queue.put(job)
@@ -159,41 +141,59 @@
         """Partition a string using a regular expression.
 
         :param content: The content to partition
         :param separator: The separator to use for the partitioning
         :returns: The first partition, separator, and final partition
         """
         separator_match = re.search(separator, content)
-        if not separator_match:
-            return content, "", ""
-        matched_separator = separator_match.group(0)
-        parts = re.split(matched_separator, content, 1)
-        return parts[0], matched_separator, parts[1]
+        if not separator_match or content.startswith(" "):
+            return "", "", content
+        delim = separator_match.group(0)
+        key, content = re.split(delim, content, maxsplit=1)
+        return key, delim, content
 
-    def splitter(self, lines, delimiter):
+    def splitter(self, lines, line_split, section_delim=None):
         """Split lines given a delimiter.
 
         :param lines: The lines to split
-        :param delimiter: The delimiter to use for splitting
+        :param line_split: The delimiter use for splitting each line
+        :param section_delim: The separator between different packages
         :returns: All lines split on the delimiter
         """
         results = []
         result = {}
+        current_key = ""
         while lines:
-            line = lines.pop()
-            left, delim, right = self.re_partition(line, delimiter)
-            right = self._strip(right)
-            if not delim:
-                if result:
-                    results.append(result)
-                    result = {}
+            line = lines.pop(0)
+            key, delim, content = self.re_partition(line, line_split)
+            content = self._strip(content)
+            if section_delim and line == section_delim:
+                results.append(result)
+                result = {}
                 continue
-            key = left.lower().replace("_", "-").strip()
-            value = right
-            result[key] = value
+            if not delim and current_key:
+                result[current_key] += f" {content}"
+                continue
+            current_key = key.lower().replace("_", "-").strip()
+            # system_packages description field needs special handling
+            if current_key == "description":
+                description = []
+                while lines:
+                    line = lines.pop(0)
+                    if line == section_delim:
+                        break
+                    description.append(line)
+                if description:
+                    result[current_key] = " ".join(description)
+                else:
+                    result[current_key] = "No description available"
+                results.append(result)
+                return result
+            result[current_key] = content
+
         if result:
             results.append(result)
         return results
 
 
 class AnsibleCollections(CmdParser):
     """Available ansible collections collector."""
@@ -289,15 +289,15 @@
         ]
 
     def parse(self, command):
         """Parse the output of the pip command.
 
         :param command: The result of running the command
         """
-        parsed = self.splitter(command.stdout.splitlines(), ":")
+        parsed = self.splitter(command.stdout.splitlines(), line_split=":", section_delim="---")
         for pkg in parsed:
             for entry in ["required-by", "requires"]:
                 if pkg[entry]:
                     pkg[entry] = [p.strip() for p in pkg[entry].split(",")]
                 else:
                     pkg[entry] = []
         command.details = parsed
@@ -358,63 +358,51 @@
             else:
                 package.append(line)
         if package:
             packages.append(package)
 
         parsed = []
         for package in packages:
-            entry = {}
-            while package:
-                line = package.pop(0)
-                left, _delim, right = self.re_partition(line, ":")
-                key = left.lower().replace("_", "-").strip()
-
-                # Description is at the end of the package section
-                # read until package is empty
-                if key == "description":
-                    description = []
-                    while package:
-                        description.append(package.pop(0))
-                    # Normalize the data, in the case description is totally empty
-                    if description:
-                        entry[key] = "\n".join(description)
-                    else:
-                        entry[key] = "No description available"
-                    parsed.append(entry)
-                # other package details are 1 line each
-                else:
-                    value = self._strip(right)
-                    entry[key] = value
+            result = self.splitter(package, line_split=":")
+            parsed.append(result)
 
         command.details = parsed
 
 
-def main():
-    """Enter the image introspection process."""
-    response = {"errors": []}
+def main(serialize: bool = True) -> dict[str, JSONTypes] | None:
+    """Enter the image introspection process.
+
+    :param serialize: Whether to serialize the results
+    :returns: The collected data or none if serialize is False
+    """
+    response: dict = {"errors": []}
     response["python_version"] = {"details": {"version": " ".join(sys.version.splitlines())}}
+    response["environment_variables"] = {"details": dict(os.environ)}
     try:
         command_runner = CommandRunner()
         commands = [
             AnsibleCollections(),
             AnsibleVersion(),
             OsRelease(),
             RedhatRelease(),
             PythonPackages(),
             SystemPackages(),
         ]
-        results = command_runner.run_multi_process(commands)
+        results = command_runner.run_multi_thread(commands)
         for result in results:
             result_as_dict = vars(result)
             result_as_dict.pop("parse")
             for key in list(result_as_dict.keys()):
                 if key not in ["details", "errors"]:
                     result_as_dict[f"__{key}"] = result_as_dict[key]
                     result_as_dict.pop(key)
             response[result_as_dict["__id_"]] = result_as_dict
     except Exception as exc:  # noqa: BLE001
         response["errors"].append(str(exc))
-    print(json.dumps(response))
+    if serialize:
+        print(json.dumps(response))
+        return None
+    return response
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/settings-sample.template.yml` & `ansible-navigator-3.4.1/src/ansible_navigator/data/settings-sample.template.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/settings-schema.partial.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/settings-schema.partial.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/themes/dark_vs.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/themes/dark_vs.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/themes/terminal_colors.json` & `ansible-navigator-3.4.1/src/ansible_navigator/data/themes/terminal_colors.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/data/welcome.md` & `ansible-navigator-3.4.1/src/ansible_navigator/data/welcome.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/diagnostics.py` & `ansible-navigator-3.4.1/src/ansible_navigator/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from .command_runner import Command
 from .command_runner import CommandRunner
 from .configuration_subsystem import Constants
 from .configuration_subsystem import to_effective
 from .configuration_subsystem import to_sources
 from .configuration_subsystem.definitions import ApplicationConfiguration
-from .image_manager import introspect
+from .data import image_introspect
 from .image_manager import introspector
 from .utils import ansi
 from .utils.compatibility import importlib_metadata
 from .utils.definitions import ExitMessage
 from .utils.definitions import LogMessage
 from .utils.functions import now_iso
 from .utils.functions import shlex_join
@@ -340,15 +340,15 @@
     @register(Collector(name="local system"))
     def _local_system(self) -> dict[str, JSONTypes]:
         """Add local system information.
 
         :raises FailedCollectionError: If the collection process fails
         :returns: The local system information
         """
-        results = introspect.main(serialize=False)
+        results = image_introspect.main(serialize=False)
         if not results:
             raise FailedCollectionError(results)
         if results.get("errors"):
             raise FailedCollectionError(results["errors"])
         return {"details": results}
 
     @diagnostic_runner
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/image_manager/inspector.py` & `ansible-navigator-3.4.1/src/ansible_navigator/image_manager/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/image_manager/introspector.py` & `ansible-navigator-3.4.1/src/ansible_navigator/image_manager/introspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 import inspect
 import json
 import logging
 import tempfile
 
 from pathlib import Path
 
+from ansible_navigator.data import image_introspect
 from ansible_navigator.runner import Command
 
-from . import introspect
-
 
 logger = logging.getLogger(__name__)
 
 
 def run(image_name: str, container_engine: str) -> tuple[dict, list[str], int]:
     """Run runner to collect image details.
 
@@ -23,16 +22,16 @@
     :param container_engine: The container engine to use
     :returns: Output, errors and the return code
     """
     errors = []
     python_exec_path = "python3"
 
     with tempfile.TemporaryDirectory() as tmp_dir_name:
-        introspect_source = inspect.getsource(introspect)
-        file = Path(tmp_dir_name) / "introspect.py"
+        introspect_source = inspect.getsource(image_introspect)
+        file = Path(tmp_dir_name) / "image_introspect.py"
         file.write_text(introspect_source)
 
         _runner = Command(
             cmdline=[str(file)],
             container_engine=container_engine,
             container_volume_mounts=[f"{tmp_dir_name}:{tmp_dir_name}"],
             executable_cmd=python_exec_path,
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/image_manager/puller.py` & `ansible-navigator-3.4.1/src/ansible_navigator/image_manager/puller.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/initialization.py` & `ansible-navigator-3.4.1/src/ansible_navigator/initialization.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/logger.py` & `ansible-navigator-3.4.1/src/ansible_navigator/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/runner/ansible_config.py` & `ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/runner/ansible_doc.py` & `ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/runner/ansible_inventory.py` & `ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/runner/base.py` & `ansible-navigator-3.4.1/src/ansible_navigator/runner/base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/runner/command.py` & `ansible-navigator-3.4.1/src/ansible_navigator/runner/command.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/runner/command_async.py` & `ansible-navigator-3.4.1/src/ansible_navigator/runner/command_async.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/runner/command_base.py` & `ansible-navigator-3.4.1/src/ansible_navigator/runner/command_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/steps.py` & `ansible-navigator-3.4.1/src/ansible_navigator/steps.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/LICENSE` & `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/compiler.py` & `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/compiler.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/grammars.py` & `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/grammars.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/reg.py` & `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/reg.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/rules.py` & `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/rules.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/state.py` & `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/state.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/tm_tokenize/tokenize.py` & `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/tokenize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/__init__.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/colorize.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/colorize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/curses_defs.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/curses_window.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_window.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_button.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_checks.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_curses_information.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_curses_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_information.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_option.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_option.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_radio.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_radio.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_text.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/field_working.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_button.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_information.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_options.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_options.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_text.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_handler_working.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/form_utils.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/menu_builder.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/menu_builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/sentinels.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/sentinels.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/ui.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/ui_config.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/ui_constants.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/utils.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/ui_framework/validators.py` & `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/validators.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/ansi.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/definitions.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,23 +128,20 @@
         message = textwrap.fill(
             self.message,
             width=width,
             break_on_hyphens=False,
             initial_indent=str(self.prefix) if with_prefix else indent,
             subsequent_indent=indent,
         )
-        printable = []
         lines = message.splitlines()
 
         start_color = self.color if color else ""
         end_color = Color.END if color else ""
 
-        for line in lines:
-            printable.append(f"{start_color}{line}{end_color}")
-
+        printable = [f"{start_color}{line}{end_color}" for line in lines]
         return printable
 
 
 @dataclass
 class ExitMessages:
     """A mechanism to store multiple exit messages."""
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/dict_merge.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/dict_merge.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/dot_paths.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/dot_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/functions.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/functions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/json_schema.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/key_value_store.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/key_value_store.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/packaged_data.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/packaged_data.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/print.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/print.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/serialize.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/definitions.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/migrate.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/migrate.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/settings_file.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py` & `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator.egg-info/PKG-INFO` & `ansible-navigator-3.4.1/src/ansible_navigator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.4.0
+Version: 3.4.1
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.4.0/src/ansible_navigator.egg-info/SOURCES.txt` & `ansible-navigator-3.4.1/src/ansible_navigator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 .github/chronographer.yml
 .github/dependabot.yml
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/documentation_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/security_bug_report.md
+.github/images/test_tree_view.png
 .github/workflows/ack.yml
 .github/workflows/push.yml
 .github/workflows/release.yml
 .github/workflows/tox.yml
 .vscode/launch.json
 .vscode/settings.json
 docs/faq.md
@@ -151,15 +152,14 @@
 src/ansible_navigator/data/grammar/text.html.markdown.json
 src/ansible_navigator/data/grammar/text.log.json
 src/ansible_navigator/data/grammar/yaml.tmLanguage.json
 src/ansible_navigator/data/themes/dark_vs.json
 src/ansible_navigator/data/themes/terminal_colors.json
 src/ansible_navigator/image_manager/__init__.py
 src/ansible_navigator/image_manager/inspector.py
-src/ansible_navigator/image_manager/introspect.py
 src/ansible_navigator/image_manager/introspector.py
 src/ansible_navigator/image_manager/puller.py
 src/ansible_navigator/runner/__init__.py
 src/ansible_navigator/runner/ansible_config.py
 src/ansible_navigator/runner/ansible_doc.py
 src/ansible_navigator/runner/ansible_inventory.py
 src/ansible_navigator/runner/base.py
```

### Comparing `ansible-navigator-3.4.0/tox.ini` & `ansible-navigator-3.4.1/tox.ini`

 * *Files identical despite different names*

