# Comparing `tmp/sphinx_toolbox-3.4.0.tar.gz` & `tmp/sphinx_toolbox-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_toolbox-3.4.0.tar", last modified: Mon Jan 23 23:33:00 2023, max compression
+gzip compressed data, was "sphinx_toolbox-3.5.0.tar", last modified: Mon Jul 24 00:24:33 2023, max compression
```

## Comparing `sphinx_toolbox-3.4.0.tar` & `sphinx_toolbox-3.5.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0 runner    (1001) docker     (122)     7973 2023-01-23 23:33:00.440891 sphinx_toolbox-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-01-23 23:33:00.432891 sphinx_toolbox-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6109 2023-01-23 23:33:00.440891 sphinx_toolbox-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-01-23 23:33:00.440891 sphinx_toolbox-3.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-01-23 23:33:00.440891 sphinx_toolbox-3.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5535 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/sidebar_links.py
--rw-r--r--   0 runner    (1001) docker     (122)    27824 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/testing.py
--rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4911 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/source.py
--rw-r--r--   0 runner    (1001) docker     (122)     7233 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/changeset.py
--rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/code.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    10566 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3396 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/assets.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/_css.py
--rw-r--r--   0 runner    (1001) docker     (122)     4780 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/_data_documenter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4645 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     6019 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/confval.py
--rw-r--r--   0 runner    (1001) docker     (122)     4100 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/flake8.py
--rw-r--r--   0 runner    (1001) docker     (122)     5397 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/collapse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/rest_example.py
--rw-r--r--   0 runner    (1001) docker     (122)     6415 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/documentation_summary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5789 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/formatting.py
--rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23655 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/shields.py
--rw-r--r--   0 runner    (1001) docker     (122)     4059 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/issues.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)    20756 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    22342 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/installation.py
--rw-r--r--   0 runner    (1001) docker     (122)    27056 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/regex.py
--rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/augment_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)    10872 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/typevars.py
--rw-r--r--   0 runner    (1001) docker     (122)    16560 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/autonamedtuple.py
--rw-r--r--   0 runner    (1001) docker     (122)    13121 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/autotypeddict.py
--rw-r--r--   0 runner    (1001) docker     (122)    20878 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/sourcelink.py
--rw-r--r--   0 runner    (1001) docker     (122)     5754 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27915 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/typehints.py
--rw-r--r--   0 runner    (1001) docker     (122)    14660 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/overloads.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/genericalias.py
--rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/no_docstring.py
--rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/generic_bases.py
--rw-r--r--   0 runner    (1001) docker     (122)    11620 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/autoprotocol.py
--rw-r--r--   0 runner    (1001) docker     (122)     7758 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/github/repos_and_users.py
--rw-r--r--   0 runner    (1001) docker     (122)    10784 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/github/issues.py
--rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/latex_layout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2333 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/latex_toc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/revert_footnote_style.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5469 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/param_dash.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/tabsize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/sphinx_panels_tabs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-01-23 23:32:33.744756 sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/footnote_symbols.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/latex/succinct_seealso.py
--rw-r--r--   0 runner    (1001) docker     (122)     7205 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/latex/layout.py
--rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/latex/toc.py
--rw-r--r--   0 runner    (1001) docker     (122)    18221 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22600 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autosummary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9011 2023-01-23 23:32:33.740756 sphinx_toolbox-3.4.0/sphinx_toolbox/more_autosummary/column_widths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-24 00:24:33.239348 sphinx_toolbox-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-24 00:24:33.247348 sphinx_toolbox-3.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-07-24 00:24:33.247348 sphinx_toolbox-3.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-07-24 00:24:33.251348 sphinx_toolbox-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6102 2023-07-24 00:24:33.247348 sphinx_toolbox-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/_css.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/code.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4645 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5535 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/sidebar_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6019 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/confval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3396 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23655 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/shields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5789 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    27824 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4059 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/issues.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5397 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10566 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4780 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/_data_documenter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/rest_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22342 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/installation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6415 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/documentation_summary.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20756 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6896 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/assets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4100 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/flake8.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/source.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4911 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7233 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/changeset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22600 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autosummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9011 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autosummary/column_widths.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18221 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/latex/succinct_seealso.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7205 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/latex/layout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/latex/toc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7758 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10784 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/github/issues.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/github/repos_and_users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/no_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5754 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10872 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/typevars.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14350 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/autotypeddict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16561 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/autonamedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/genericalias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/sourcelink.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27915 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/typehints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27056 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/regex.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11645 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/autoprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20878 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/augment_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/generic_bases.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14660 2023-07-24 00:23:51.163011 sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/overloads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2333 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/latex_toc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/revert_footnote_style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/footnote_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/tabsize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/sphinx_panels_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/latex_layout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5469 2023-07-24 00:23:51.167011 sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/param_dash.py
```

### Comparing `sphinx_toolbox-3.4.0/PKG-INFO` & `sphinx_toolbox-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-toolbox
-Version: 3.4.0
+Version: 3.5.0
 Summary: Box of handy tools for Sphinx 🧰 📔
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: documentation,sphinx,sphinx-extension
 Home-page: https://github.com/sphinx-toolbox/sphinx-toolbox
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/sphinx-toolbox/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/sphinx-toolbox
@@ -31,20 +31,20 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: apeye>=0.4.0
 Requires-Dist: autodocsumm>=0.2.0
 Requires-Dist: beautifulsoup4>=4.9.1
-Requires-Dist: cachecontrol[filecache]>=0.12.6
+Requires-Dist: cachecontrol[filecache]>=0.13.0
 Requires-Dist: dict2css>=0.2.3
-Requires-Dist: docutils<0.19,>=0.16
+Requires-Dist: docutils>=0.16
 Requires-Dist: domdf-python-tools>=2.9.0
+Requires-Dist: filelock>=3.8.0
 Requires-Dist: html5lib>=1.1
-Requires-Dist: lockfile>=0.12.2
 Requires-Dist: ruamel.yaml>=0.16.12
 Requires-Dist: sphinx>=3.2.0
 Requires-Dist: sphinx-autodoc-typehints>=1.11.1
 Requires-Dist: sphinx-jinja2-compat>=0.1.0
 Requires-Dist: sphinx-prompt>=1.1.0
 Requires-Dist: sphinx-tabs<3.5.0,>=1.2.1
 Requires-Dist: tabulate>=0.8.7
@@ -158,15 +158,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/sphinx-toolbox
 	:target: https://github.com/sphinx-toolbox/sphinx-toolbox/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/sphinx-toolbox
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-toolbox/v3.4.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-toolbox/v3.5.0
 	:target: https://github.com/sphinx-toolbox/sphinx-toolbox/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/sphinx-toolbox
 	:target: https://github.com/sphinx-toolbox/sphinx-toolbox/commit/master
 	:alt: GitHub last commit
```

### Comparing `sphinx_toolbox-3.4.0/LICENSE` & `sphinx_toolbox-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/pyproject.toml` & `sphinx_toolbox-3.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "sphinx-toolbox"
-version = "3.4.0"
+version = "3.5.0"
 description = "Box of handy tools for Sphinx 🧰 📔"
 readme = "README.rst"
 keywords = [ "documentation", "sphinx", "sphinx-extension",]
 dynamic = []
 dependencies = [
     "apeye>=0.4.0",
     "autodocsumm>=0.2.0",
     "beautifulsoup4>=4.9.1",
-    "cachecontrol[filecache]>=0.12.6",
+    "cachecontrol[filecache]>=0.13.0",
     "dict2css>=0.2.3",
-    "docutils<0.19,>=0.16",
+    "docutils>=0.16",
     "domdf-python-tools>=2.9.0",
+    "filelock>=3.8.0",
     "html5lib>=1.1",
-    "lockfile>=0.12.2",
     "ruamel.yaml>=0.16.12",
     "sphinx>=3.2.0",
     "sphinx-autodoc-typehints>=1.11.1",
     "sphinx-jinja2-compat>=0.1.0",
     "sphinx-prompt>=1.1.0",
     "sphinx-tabs<3.5.0,>=1.2.1",
     "tabulate>=0.8.7",
@@ -85,15 +85,15 @@
 python-versions = [ "3.7", "3.8", "3.9", "3.10",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "sphinx_toolbox"
 
 [tool.dep_checker]
-allowed_unused = [ "html5lib", "sphinx_prompt", "sphinx_tabs", "lockfile", "cachecontrol", "sphinx_jinja2_compat",]
+allowed_unused = [ "html5lib", "sphinx_prompt", "sphinx_tabs", "filelock", "cachecontrol", "sphinx_jinja2_compat",]
 namespace_packages = [ "ruamel.yaml",]
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 
 [tool.sphinx-pyproject]
```

### Comparing `sphinx_toolbox-3.4.0/README.rst` & `sphinx_toolbox-3.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/sphinx-toolbox
 	:target: https://github.com/sphinx-toolbox/sphinx-toolbox/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/sphinx-toolbox
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-toolbox/v3.4.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-toolbox/v3.5.0
 	:target: https://github.com/sphinx-toolbox/sphinx-toolbox/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/sphinx-toolbox
 	:target: https://github.com/sphinx-toolbox/sphinx-toolbox/commit/master
 	:alt: GitHub last commit
```

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/sidebar_links.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/sidebar_links.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/testing.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/testing.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/config.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/config.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/wikipedia.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/wikipedia.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/source.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/source.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/changeset.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/changeset.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/code.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/code.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/pre_commit.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/pre_commit.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/__init__.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 		wikipedia
 		)
 from sphinx_toolbox.cache import cache  # noqa: F401
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "3.4.0"
+__version__: str = "3.5.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ("setup", )
 
 
 def setup(app: Sphinx) -> "utils.SphinxExtMetadata":
 	"""
```

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/assets.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,17 @@
 
 	assets_out_dir = PathPlus(translator.builder.outdir) / "_assets"
 	assets_out_dir.maybe_make(parents=True)
 
 	source_file = PathPlus(translator.builder.confdir) / node["source_file"]
 
 	source_file_exists = source_file.is_file()
-	source_file_not_seen = source_file not in translator._asset_node_seen_files  # type: ignore[attr-defined]
+	source_file_seen = source_file in translator._asset_node_seen_files  # type: ignore[attr-defined]
 
-	if source_file_not_seen and source_file_exists:
+	if not source_file_seen and source_file_exists:
 		# Avoid unnecessary copies of potentially large files.
 		translator._asset_node_seen_files.append(source_file)  # type: ignore[attr-defined]
 		shutil.copy2(source_file, assets_out_dir)
 	elif not source_file_exists:
 		stderr_writer(
 				f"\x1b[31m{translator.builder.current_docname}: "
 				f"Asset file '{source_file}' not found.\x1b[39m"
```

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/_css.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/_css.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/_data_documenter.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/_data_documenter.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/decorators.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/decorators.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/confval.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/confval.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/flake8.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/flake8.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/collapse.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/collapse.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/rest_example.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/rest_example.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/documentation_summary.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/documentation_summary.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/formatting.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/formatting.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/__main__.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/shields.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/shields.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/issues.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/issues.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/cache.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/cache.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/utils.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/installation.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/installation.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/regex.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/regex.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/augment_defaults.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/augment_defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/typevars.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/typevars.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/autonamedtuple.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/autonamedtuple.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,14 +396,15 @@
 				if field in type_hints:
 					arg_type = format_annotation(type_hints[field])
 
 			self.add_line(f"{a_tab}.. namedtuple-field:: {field}", sourcename)
 			self.add_line('', sourcename)
 			# field_entry = [f"{a_tab}{pos})", "|nbsp|", f"**{field}**"]
 			field_entry = [f"{a_tab}{pos}) \u00A0**{field}**"]
+
 			if arg_type:
 				field_entry.append(f"({arg_type}\\)")
 			field_entry.append("--")
 			field_entry.extend(doc)
 
 			if self.field_alias_re.match(getattr(self.object, field).__doc__ or ''):
 				getattr(self.object, field).__doc__ = ' '.join(doc)
```

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/autotypeddict.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/autotypeddict.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,14 +215,58 @@
 		:rtype:
 
 		.. latex:clearpage::
 		"""
 
 		return ''
 
+	def add_directive_header(self, sig: str) -> None:
+		"""
+		Add the directive header.
+
+		:param sig:
+		"""
+
+		sourcename = self.get_sourcename()
+
+		if self.doc_as_attr:
+			self.directivetype = "attribute"
+
+		Documenter.add_directive_header(self, sig)
+
+		if self.analyzer and '.'.join(self.objpath) in self.analyzer.finals:
+			self.add_line("   :final:", sourcename)
+
+		# add inheritance info, if wanted
+		if not self.doc_as_attr and self.options.show_inheritance:
+			self.add_line('', sourcename)
+
+			def get_bases(obj: Type) -> List[Type]:
+				bases: Tuple[Type, ...] = ()
+				if hasattr(obj, "__orig_bases__") and len(obj.__orig_bases__):
+					# A subclass of generic types
+					# refs: PEP-560 <https://www.python.org/dev/peps/pep-0560/>
+					bases = obj.__orig_bases__
+				elif hasattr(obj, "__bases__") and len(obj.__bases__):
+					# A normal class
+					bases = obj.__bases__
+
+				output = []
+				for base in bases:
+					if base.__name__.startswith('_'):
+						output.extend(get_bases(base))
+					else:
+						output.append(base)
+
+				return output
+
+			bases = [format_annotation(cls) for cls in get_bases(self.object)]
+			self.add_line("   " + _("Bases: %s") % ", ".join(bases), sourcename)
+			self.add_line('', sourcename)
+
 	def add_content(self, more_content: Any, no_docstring: bool = False) -> None:
 		"""
 		Add the autodocumenter content.
 
 		:param more_content:
 		:param no_docstring:
 		"""
```

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/variables.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/variables.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/sourcelink.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/sourcelink.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/__init__.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/typehints.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/typehints.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/overloads.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/overloads.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/genericalias.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/genericalias.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/no_docstring.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/no_docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/generic_bases.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/generic_bases.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autodoc/autoprotocol.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autodoc/autoprotocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,15 @@
 			"__args__",
 			"__dict__",
 			"__weakref__",
 			"__annotations__",
 			"__abstractmethods__",
 			"__class_getitem__",
 			"__init_subclass__",
+			"__protocol_attrs__",
 			}
 
 	def __init__(self, directive: DocumenterBridge, name: str, indent: str = '') -> None:
 		super().__init__(directive, name, indent)
 		self.options = Options(self.options.copy())
 
 	@classmethod
```

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/github/__init__.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/github/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/github/repos_and_users.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/github/repos_and_users.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/github/issues.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/github/issues.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/latex_layout.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/latex_layout.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/latex_toc.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/latex_toc.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/revert_footnote_style.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/revert_footnote_style.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/__init__.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/param_dash.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/param_dash.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/tabsize.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/tabsize.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/sphinx_panels_tabs.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/sphinx_panels_tabs.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/tweaks/footnote_symbols.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/tweaks/footnote_symbols.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/latex/succinct_seealso.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/latex/succinct_seealso.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/latex/layout.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/latex/layout.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/latex/toc.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/latex/toc.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/latex/__init__.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autosummary/__init__.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autosummary/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_toolbox-3.4.0/sphinx_toolbox/more_autosummary/column_widths.py` & `sphinx_toolbox-3.5.0/sphinx_toolbox/more_autosummary/column_widths.py`

 * *Files identical despite different names*

