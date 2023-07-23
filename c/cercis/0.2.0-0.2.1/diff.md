# Comparing `tmp/cercis-0.2.0.tar.gz` & `tmp/cercis-0.2.1.tar.gz`

## Comparing `cercis-0.2.0.tar` & `cercis-0.2.1.tar`

### file list

```diff
@@ -1,385 +1,385 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.2.0/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.2.0/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.2.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.2.0/.gitattributes
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 cercis-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.2.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.2.0/.prettierrc.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 cercis-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    51880 2020-02-02 00:00:00.000000 cercis-0.2.0/CHANGES.md
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 cercis-0.2.0/CITATION.cff
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.2.0/Dockerfile
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cercis-0.2.0/HOW_TO_REBASE.md
--rw-r--r--   0        0        0    24909 2020-02-02 00:00:00.000000 cercis-0.2.0/README.md
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 cercis-0.2.0/action.yml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.2.0/mypy.ini
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.0/test_requirements.txt
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 cercis-0.2.0/tox.ini
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/ISSUE_TEMPLATE/docs-issue.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/ISSUE_TEMPLATE/style_issue.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/check-changelog.yml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/diff_shades_comment.yml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/upload_binary.yml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.2.0/.github/workflows/version-check.yml
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 cercis-0.2.0/action/main.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.2.0/autoload/black.vim
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.2.0/gallery/Dockerfile
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.2.0/gallery/README.md
--rwxr-xr-x   0        0        0     9163 2020-02-02 00:00:00.000000 cercis-0.2.0/gallery/gallery.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.2.0/plugin/black.vim
--rw-r--r--   0        0        0   933114 2020-02-02 00:00:00.000000 cercis-0.2.0/screenshots/how_to_rebase/1.png
--rw-r--r--   0        0        0    95589 2020-02-02 00:00:00.000000 cercis-0.2.0/screenshots/how_to_rebase/2.png
--rw-r--r--   0        0        0    93329 2020-02-02 00:00:00.000000 cercis-0.2.0/screenshots/how_to_rebase/3.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/check_version_and_changelog.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/check_version_in_basics_example.py
--rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/diff_shades_gha_helper.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/fuzz.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/make_width_table.py
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.2.0/scripts/migrate-black.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.2.0/src/_cercis_version.py
--rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blackd/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blackd/__main__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blackd/middlewares.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/Grammar.txt
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/PatternGrammar.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/README
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/__init__.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pygram.py
--rw-r--r--   0        0        0    32574 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pytree.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/__init__.py
--rw-r--r--   0        0        0     9587 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/conv.py
--rw-r--r--   0        0        0    10605 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/driver.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/grammar.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/literals.py
--rw-r--r--   0        0        0    14816 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/parse.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/pgen.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/token.py
--rw-r--r--   0        0        0    23007 2020-02-02 00:00:00.000000 cercis-0.2.0/src/blib2to3/pgen2/tokenize.py
--rw-r--r--   0        0        0    51721 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/__main__.py
--rw-r--r--   0        0        0    10761 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/_width_table.py
--rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/brackets.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/cache.py
--rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/comments.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/concurrency.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/const.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/debug.py
--rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/files.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/handle_ipynb_magics.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/indent.py
--rw-r--r--   0        0        0    65200 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/linegen.py
--rw-r--r--   0        0        0    41008 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/lines.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/mode.py
--rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/numerics.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/output.py
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/py.typed
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/rusty.py
--rw-r--r--   0        0        0    14204 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/strings.py
--rw-r--r--   0        0        0    91799 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/trans.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/utils_line_wrapping.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.2.0/src/cercis/utils_linegen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/optional.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test.toml
--rw-r--r--   0        0        0   102206 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test_black.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test_blackd.py
--rw-r--r--   0        0        0    16897 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test_format.py
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test_ipynb.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test_trans.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/test_utils_line_wrapping.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_comments/case_False_False.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_comments/case_False_True.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_comments/case_True_False.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_comments/case_True_True.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/edge_cases.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
--rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/playground/playground.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Black_default.py
--rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Black_default_2.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Cercis_default.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/single_quote/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/single_quote/docstring_preview.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/single_quote/more_quotes.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/single_quote/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/configurable_cases/single_quote/torture.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/no_blank_line_before_docstring.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_312/type_aliases.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_312/type_params.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/ignore_pyi.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/multiline_consecutive_open_parentheses_ignore.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/pep_604.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.2.0/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.2.0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.2.0/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.2.0/LICENSE_ORIGINAL
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 cercis-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    29180 2020-02-02 00:00:00.000000 cercis-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.2.1/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.2.1/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.2.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.2.1/.gitattributes
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 cercis-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.2.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.2.1/.prettierrc.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 cercis-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0    51957 2020-02-02 00:00:00.000000 cercis-0.2.1/CHANGES.md
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 cercis-0.2.1/CITATION.cff
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.2.1/Dockerfile
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cercis-0.2.1/HOW_TO_REBASE.md
+-rw-r--r--   0        0        0    24909 2020-02-02 00:00:00.000000 cercis-0.2.1/README.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 cercis-0.2.1/action.yml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.2.1/mypy.ini
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.1/test_requirements.txt
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 cercis-0.2.1/tox.ini
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/ISSUE_TEMPLATE/docs-issue.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/ISSUE_TEMPLATE/style_issue.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/check-changelog.yml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/diff_shades_comment.yml
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/upload_binary.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.2.1/.github/workflows/version-check.yml
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 cercis-0.2.1/action/main.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.2.1/autoload/black.vim
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.2.1/gallery/Dockerfile
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.2.1/gallery/README.md
+-rwxr-xr-x   0        0        0     9163 2020-02-02 00:00:00.000000 cercis-0.2.1/gallery/gallery.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.2.1/plugin/black.vim
+-rw-r--r--   0        0        0   933114 2020-02-02 00:00:00.000000 cercis-0.2.1/screenshots/how_to_rebase/1.png
+-rw-r--r--   0        0        0    95589 2020-02-02 00:00:00.000000 cercis-0.2.1/screenshots/how_to_rebase/2.png
+-rw-r--r--   0        0        0    93329 2020-02-02 00:00:00.000000 cercis-0.2.1/screenshots/how_to_rebase/3.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/check_version_and_changelog.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/check_version_in_basics_example.py
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/fuzz.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.2.1/scripts/migrate-black.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.2.1/src/_cercis_version.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blackd/middlewares.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/Grammar.txt
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/PatternGrammar.txt
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/README
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32651 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9587 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    23081 2020-02-02 00:00:00.000000 cercis-0.2.1/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0    51718 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/__main__.py
+-rw-r--r--   0        0        0    10761 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/_width_table.py
+-rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/brackets.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/cache.py
+-rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/comments.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/concurrency.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/const.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/debug.py
+-rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/files.py
+-rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/handle_ipynb_magics.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/indent.py
+-rw-r--r--   0        0        0    65200 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/linegen.py
+-rw-r--r--   0        0        0    41067 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/lines.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/mode.py
+-rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/numerics.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/output.py
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/py.typed
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/rusty.py
+-rw-r--r--   0        0        0    14204 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/strings.py
+-rw-r--r--   0        0        0    91799 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/trans.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/utils_line_wrapping.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.2.1/src/cercis/utils_linegen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/optional.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test.toml
+-rw-r--r--   0        0        0   102206 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test_black.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test_blackd.py
+-rw-r--r--   0        0        0    16897 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test_format.py
+-rw-r--r--   0        0        0    16196 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test_trans.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/test_utils_line_wrapping.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_comments/case_False_False.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_comments/case_False_True.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_comments/case_True_False.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_comments/case_True_True.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/edge_cases.py
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
+-rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/playground/playground.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Black_default.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Black_default_2.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Cercis_default.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/single_quote/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/single_quote/docstring_preview.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/single_quote/more_quotes.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/single_quote/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/configurable_cases/single_quote/torture.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/no_blank_line_before_docstring.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_312/type_aliases.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_312/type_params.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/ignore_pyi.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/multiline_consecutive_open_parentheses_ignore.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/pep_604.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.2.1/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.2.1/LICENSE_ORIGINAL
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 cercis-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    29500 2020-02-02 00:00:00.000000 cercis-0.2.1/PKG-INFO
```

### Comparing `cercis-0.2.0/.pre-commit-config.yaml` & `cercis-0.2.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Note: don't use this config for your own repositories. Instead, see
 # "Version control integration" in docs/integrations/source_version_control.md
-exclude: ^(src/blib2to3/|profiling/|tests/data/)
+exclude: ^(profiling/|tests/data/)
 repos:
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pycqa/flake8
@@ -12,24 +12,25 @@
     hooks:
       - id: flake8
         args: [--max-line-length=88]
         additional_dependencies:
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-simplify
+        exclude: ^src/blib2to3/
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
       - id: mypy
         exclude: ^docs/conf.py
         additional_dependencies:
           - types-PyYAML
           - tomli >= 0.2.6, < 2.0.0
-          - click >= 8.1.0, != 8.1.4
+          - click >= 8.1.0, != 8.1.4, != 8.1.5
           - packaging >= 22.0
           - platformdirs >= 2.1.0
           - pytest
           - hypothesis
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0
```

### Comparing `cercis-0.2.0/.pre-commit-hooks.yaml` & `cercis-0.2.1/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/CHANGELOG.md` & `cercis-0.2.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Change Log
 
+## [0.2.1] - 2023-07-23
+
+- Changed
+  - Rebased `Cercis` to be head to head with `Black`
+- Fixed
+  - Fixed a pytest regression where Python warnings are treated as errors
+    (https://github.com/jsh9/cercis/commit/1229b9dd18f861423e26f8de3f4b5e714d72bd9c)
+- Diff
+  - https://github.com/jsh9/cercis/compare/0.2.0...0.2.1
+
 ## [0.2.0] - 2023-07-12
 
 - Changed
   - Rebased `Cercis` to be head to head with `Black`
     [version 23.7.0](https://github.com/psf/black/releases/tag/23.7.0)
 - Diff
   - https://github.com/jsh9/cercis/compare/0.1.7...0.2.0
```

### Comparing `cercis-0.2.0/CHANGES.md` & `cercis-0.2.1/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 <!-- Changes to the parser or to version autodetection -->
 
 ### Performance
 
 <!-- Changes that improve Black's performance. -->
 
+- Avoid importing `IPython` if notebook cells do not contain magics (#3782)
+
 ### Output
 
 <!-- Changes to Black's terminal output and error messages -->
 
 ### _Blackd_
 
 <!-- Changes to blackd -->
```

### Comparing `cercis-0.2.0/CITATION.cff` & `cercis-0.2.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/Dockerfile` & `cercis-0.2.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/HOW_TO_REBASE.md` & `cercis-0.2.1/HOW_TO_REBASE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/README.md` & `cercis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/action.yml` & `cercis-0.2.1/action.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/mypy.ini` & `cercis-0.2.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `cercis-0.2.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/dependabot.yml` & `cercis-0.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `cercis-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/ISSUE_TEMPLATE/config.yml` & `cercis-0.2.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/ISSUE_TEMPLATE/docs-issue.md` & `cercis-0.2.1/.github/ISSUE_TEMPLATE/docs-issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `cercis-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/ISSUE_TEMPLATE/style_issue.md` & `cercis-0.2.1/.github/ISSUE_TEMPLATE/style_issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/check-changelog.yml` & `cercis-0.2.1/.github/workflows/check-changelog.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/diff_shades_comment.yml` & `cercis-0.2.1/.github/workflows/diff_shades_comment.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/docker.yml` & `cercis-0.2.1/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/fuzz.yml` & `cercis-0.2.1/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/lint.yml` & `cercis-0.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/python-package.yml` & `cercis-0.2.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/python-publish.yml` & `cercis-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/test.yml` & `cercis-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/upload_binary.yml` & `cercis-0.2.1/.github/workflows/upload_binary.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/.github/workflows/version-check.yml` & `cercis-0.2.1/.github/workflows/version-check.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/action/main.py` & `cercis-0.2.1/action/main.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/autoload/black.vim` & `cercis-0.2.1/autoload/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/gallery/README.md` & `cercis-0.2.1/gallery/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/gallery/gallery.py` & `cercis-0.2.1/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/plugin/black.vim` & `cercis-0.2.1/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/screenshots/how_to_rebase/1.png` & `cercis-0.2.1/screenshots/how_to_rebase/1.png`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/screenshots/how_to_rebase/2.png` & `cercis-0.2.1/screenshots/how_to_rebase/2.png`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/screenshots/how_to_rebase/3.png` & `cercis-0.2.1/screenshots/how_to_rebase/3.png`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/scripts/check_version_and_changelog.py` & `cercis-0.2.1/scripts/check_version_and_changelog.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/scripts/check_version_in_basics_example.py` & `cercis-0.2.1/scripts/check_version_in_basics_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Check that the rev value in the example from ``the_basics.md`` matches
 the latest version of Black. This saves us from forgetting to update that
 during the release process.
 """
 
-import os
 import sys
 
 import commonmark
 from bs4 import BeautifulSoup
 
 
 def main(changes: str, the_basics: str) -> None:
@@ -36,13 +35,10 @@
                 )
                 sys.exit(1)
 
 
 if __name__ == "__main__":
     with open("CHANGES.md", encoding="utf-8") as fd:
         changes = fd.read()
-    with open(
-        os.path.join("docs", "usage_and_configuration", "the_basics.md"),
-        encoding="utf-8",
-    ) as fd:
-        the_basics = fd.read()
+
+    the_basics = ""
     main(changes, the_basics)
```

### Comparing `cercis-0.2.0/scripts/diff_shades_gha_helper.py` & `cercis-0.2.1/scripts/diff_shades_gha_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 import os
 import platform
 import pprint
 import subprocess
 import sys
 import zipfile
+from base64 import b64encode
 from io import BytesIO
 from pathlib import Path
 from typing import Any
 
 import click
 import urllib3
 from packaging.version import Version
@@ -49,20 +50,24 @@
 
 def set_output(name: str, value: str) -> None:
     if len(value) < 200:
         print(f"[INFO]: setting '{name}' to '{value}'")
     else:
         print(f"[INFO]: setting '{name}' to [{len(value)} chars]")
 
-    # Originally the `set-output` workflow command was used here, now replaced
-    # by setting variables through the `GITHUB_OUTPUT` environment variable
-    # to stay up to date with GitHub's update.
     if "GITHUB_OUTPUT" in os.environ:
+        if "\n" in value:
+            # https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#multiline-strings
+            delimiter = b64encode(os.urandom(16)).decode()
+            value = f"{delimiter}\n{value}\n{delimiter}"
+            command = f"{name}<<{value}"
+        else:
+            command = f"{name}={value}"
         with open(os.environ["GITHUB_OUTPUT"], "a") as f:
-            print(f"{name}={value}", file=f)
+            print(command, file=f)
 
 
 def http_get(url: str, *, is_json: bool = True, **kwargs: Any) -> Any:
     headers = kwargs.get("headers") or {}
     headers["User-Agent"] = USER_AGENT
     if "github" in url:
         if GH_API_TOKEN:
@@ -220,14 +225,12 @@
     set_output("pr-number", str(comment_data["pr-number"]))
     body = comment_data["body"]
     # It's more convenient to fill in these fields after the first workflow is done
     # since this command can access the workflows API (doing it in the main workflow
     # while it's still in progress seems impossible).
     body = body.replace("$workflow-run-url", data["html_url"])
     body = body.replace("$job-diff-url", diff_url)
-    # https://github.community/t/set-output-truncates-multiline-strings/16852/3
-    escaped = body.replace("%", "%25").replace("\n", "%0A").replace("\r", "%0D")
-    set_output("comment-body", escaped)
+    set_output("comment-body", body)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cercis-0.2.0/scripts/fuzz.py` & `cercis-0.2.1/scripts/fuzz.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/scripts/make_width_table.py` & `cercis-0.2.1/scripts/make_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/scripts/migrate-black.py` & `cercis-0.2.1/scripts/migrate-black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blackd/__init__.py` & `cercis-0.2.1/src/blackd/__init__.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blackd/middlewares.py` & `cercis-0.2.1/src/blackd/middlewares.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blib2to3/Grammar.txt` & `cercis-0.2.1/src/blib2to3/Grammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blib2to3/LICENSE` & `cercis-0.2.1/src/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blib2to3/PatternGrammar.txt` & `cercis-0.2.1/src/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blib2to3/README` & `cercis-0.2.1/src/blib2to3/README`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-A subset of lib2to3 taken from Python 3.7.0b2.
-Commit hash: 9c17e3a1987004b8bcfbe423953aad84493a7984
+A subset of lib2to3 taken from Python 3.7.0b2. Commit hash:
+9c17e3a1987004b8bcfbe423953aad84493a7984
 
 Reasons for forking:
+
 - consistent handling of f-strings for users of Python < 3.6.2
-- backport of BPO-33064 that fixes parsing files with trailing commas after
-  *args and **kwargs
-- backport of GH-6143 that restores the ability to reformat legacy usage of
-  `async`
+- backport of BPO-33064 that fixes parsing files with trailing commas after \*args and
+  \*\*kwargs
+- backport of GH-6143 that restores the ability to reformat legacy usage of `async`
 - support all types of string literals
 - better ability to debug (better reprs)
 - INDENT and DEDENT don't hold whitespace and comment prefixes
 - ability to Cythonize
 
 Change Log:
+
 - Changes default logger used by Driver
 - Backported the following upstream parser changes:
   - "bpo-42381: Allow walrus in set literals and set comprehensions (GH-23332)"
     https://github.com/python/cpython/commit/cae60187cf7a7b26281d012e1952fafe4e2e97e9
   - "bpo-42316: Allow unparenthesized walrus operator in indexes (GH-23317)"
     https://github.com/python/cpython/commit/b0aba1fcdc3da952698d99aec2334faa79a8b68c
 - Tweaks to help mypyc compile faster code (including inlining type information,
```

### Comparing `cercis-0.2.0/src/blib2to3/pygram.py` & `cercis-0.2.1/src/blib2to3/pygram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Copyright 2006 Google, Inc. All Rights Reserved.
 # Licensed to PSF under a Contributor Agreement.
 
 """Export the Python grammar and symbols."""
 
 # Python imports
 import os
-
 from typing import Union
 
 # Local imports
 from .pgen2 import driver
-
 from .pgen2.grammar import Grammar
 
 # Moved into initialize because mypyc can't handle __file__ (XXX bug)
 # # The grammar file
 # _GRAMMAR_FILE = os.path.join(os.path.dirname(__file__), "Grammar.txt")
 # _PATTERN_GRAMMAR_FILE = os.path.join(os.path.dirname(__file__),
 #                                      "PatternGrammar.txt")
```

### Comparing `cercis-0.2.0/src/blib2to3/pytree.py` & `cercis-0.2.1/src/blib2to3/pytree.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 """
 
 # mypy: allow-untyped-defs, allow-incomplete-defs
 
 from typing import (
     Any,
     Dict,
+    Iterable,
     Iterator,
     List,
     Optional,
+    Set,
     Tuple,
     TypeVar,
     Union,
-    Set,
-    Iterable,
 )
+
 from blib2to3.pgen2.grammar import Grammar
 
 __author__ = "Guido van Rossum <guido@python.org>"
 
 import sys
 from io import StringIO
 
@@ -54,15 +55,14 @@
 
 NL = Union["Node", "Leaf"]
 Context = Tuple[str, Tuple[int, int]]
 RawNode = Tuple[int, Optional[str], Optional[Context], Optional[List[NL]]]
 
 
 class Base:
-
     """
     Abstract base class for Node and Leaf.
 
     This provides some default functionality and boilerplate using the
     template pattern.
 
     A node may be a subnode of at most one parent.
@@ -233,27 +233,26 @@
         if next_sib is None:
             return ""
         prefix = next_sib.prefix
         return prefix
 
 
 class Node(Base):
-
     """Concrete implementation for interior nodes."""
 
     fixers_applied: Optional[List[Any]]
     used_names: Optional[Set[str]]
 
     def __init__(
-        self,
-        type: int,
-        children: List[NL],
-        context: Optional[Any] = None,
-        prefix: Optional[str] = None,
-        fixers_applied: Optional[List[Any]] = None,
+            self,
+            type: int,
+            children: List[NL],
+            context: Optional[Any] = None,
+            prefix: Optional[str] = None,
+            fixers_applied: Optional[List[Any]] = None,
     ) -> None:
         """
         Initializer.
 
         Takes a type constant (a symbol number >= 256), a sequence of
         child nodes, and an optional context keyword argument.
 
@@ -374,15 +373,14 @@
             _prev[id(current)] = previous
             _next[id(previous)] = current
             previous = current
         _next[id(current)] = None
 
 
 class Leaf(Base):
-
     """Concrete implementation for leaf nodes."""
 
     # Default values for instance variables
     value: str
     fixers_applied: List[Any]
     bracket_depth: int
     # Changed later in brackets.py
@@ -393,22 +391,22 @@
     column: int = 0  # Column where this token starts in the input
     # If not None, this Leaf is created by converting a block of fmt off/skip
     # code, and `fmt_pass_converted_first_leaf` points to the first Leaf in the
     # converted code.
     fmt_pass_converted_first_leaf: Optional["Leaf"] = None
 
     def __init__(
-        self,
-        type: int,
-        value: str,
-        context: Optional[Context] = None,
-        prefix: Optional[str] = None,
-        fixers_applied: List[Any] = [],
-        opening_bracket: Optional["Leaf"] = None,
-        fmt_pass_converted_first_leaf: Optional["Leaf"] = None,
+            self,
+            type: int,
+            value: str,
+            context: Optional[Context] = None,
+            prefix: Optional[str] = None,
+            fixers_applied: List[Any] = [],
+            opening_bracket: Optional["Leaf"] = None,
+            fmt_pass_converted_first_leaf: Optional["Leaf"] = None,
     ) -> None:
         """
         Initializer.
 
         Takes a type constant (a token number < 256), a string value, and an
         optional context keyword argument.
         """
@@ -502,15 +500,14 @@
         return Leaf(type, value or "", context=context)
 
 
 _Results = Dict[str, NL]
 
 
 class BasePattern:
-
     """
     A pattern is a tree matching pattern.
 
     It looks for a specific node type (token or symbol), and
     optionally for a specific content.
 
     This is an abstract base class.  There are three concrete
@@ -595,18 +592,18 @@
         r: _Results = {}
         if nodes and self.match(nodes[0], r):
             yield 1, r
 
 
 class LeafPattern(BasePattern):
     def __init__(
-        self,
-        type: Optional[int] = None,
-        content: Optional[str] = None,
-        name: Optional[str] = None,
+            self,
+            type: Optional[int] = None,
+            content: Optional[str] = None,
+            name: Optional[str] = None,
     ) -> None:
         """
         Initializer.  Takes optional type, content, and name.
 
         The type, if given must be a token type (< 256).  If not given,
         this matches any *leaf* node; the content may still be required.
 
@@ -642,22 +639,21 @@
 
         When returning False, the results dict may still be updated.
         """
         return self.content == node.value
 
 
 class NodePattern(BasePattern):
-
     wildcards: bool = False
 
     def __init__(
-        self,
-        type: Optional[int] = None,
-        content: Optional[Iterable[str]] = None,
-        name: Optional[str] = None,
+            self,
+            type: Optional[int] = None,
+            content: Optional[Iterable[str]] = None,
+            name: Optional[str] = None,
     ) -> None:
         """
         Initializer.  Takes optional type, content, and name.
 
         The type, if given, must be a symbol type (>= 256).  If the
         type is None this matches *any* single node (leaf or not),
         except if content is not None, in which it only matches
@@ -711,15 +707,14 @@
         for subpattern, child in zip(self.content, node.children):
             if not subpattern.match(child, results):
                 return False
         return True
 
 
 class WildcardPattern(BasePattern):
-
     """
     A wildcard pattern can match zero or more nodes.
 
     This has all the flexibility needed to implement patterns like:
 
     .*      .+      .?      .{m,n}
     (a b c | d e | f)
@@ -728,19 +723,19 @@
     except it always uses non-greedy matching.
     """
 
     min: int
     max: int
 
     def __init__(
-        self,
-        content: Optional[str] = None,
-        min: int = 0,
-        max: int = HUGE,
-        name: Optional[str] = None,
+            self,
+            content: Optional[str] = None,
+            min: int = 0,
+            max: int = HUGE,
+            name: Optional[str] = None,
     ) -> None:
         """
         Initializer.
 
         Args:
             content: optional sequence of subsequences of patterns;
                      if absent, matches one node;
@@ -761,17 +756,15 @@
             list of alternatives, e.g. (a b c | d e | f g h)*
         """
         assert 0 <= min <= max <= HUGE, (min, max)
         if content is not None:
             f = lambda s: tuple(s)
             wrapped_content = tuple(map(f, content))  # Protect against alterations
             # Check sanity of alternatives
-            assert len(wrapped_content), repr(
-                wrapped_content
-            )  # Can't have zero alternatives
+            assert len(wrapped_content), repr(wrapped_content)  # Can't have zero alternatives
             for alt in wrapped_content:
                 assert len(alt), repr(alt)  # Can have empty alternatives
         self.content = wrapped_content
         self.min = min
         self.max = max
         self.name = name
 
@@ -955,15 +948,15 @@
             # Return a match if the argument pattern has no matches
             for c, r in self.content.generate_matches(nodes):
                 return
             yield 0, {}
 
 
 def generate_matches(
-    patterns: List[BasePattern], nodes: List[NL]
+        patterns: List[BasePattern], nodes: List[NL]
 ) -> Iterator[Tuple[int, _Results]]:
     """
     Generator yielding matches for a sequence of patterns and nodes.
 
     Args:
         patterns: a sequence of patterns
         nodes: a sequence of nodes
```

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/conv.py` & `cercis-0.2.1/src/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/driver.py` & `cercis-0.2.1/src/blib2to3/pgen2/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,38 +13,29 @@
 
 __author__ = "Guido van Rossum <guido@python.org>"
 
 __all__ = ["Driver", "load_grammar"]
 
 # Python imports
 import io
-import os
 import logging
+import os
 import pkgutil
 import sys
-from typing import (
-    Any,
-    cast,
-    IO,
-    Iterable,
-    List,
-    Optional,
-    Iterator,
-    Tuple,
-    Union,
-)
 from contextlib import contextmanager
 from dataclasses import dataclass, field
-
-# Pgen imports
-from . import grammar, parse, token, tokenize, pgen
 from logging import Logger
-from blib2to3.pytree import NL
+from typing import IO, Any, Iterable, Iterator, List, Optional, Tuple, Union, cast
+
 from blib2to3.pgen2.grammar import Grammar
 from blib2to3.pgen2.tokenize import GoodTokenInfo
+from blib2to3.pytree import NL
+
+# Pgen imports
+from . import grammar, parse, pgen, token, tokenize
 
 Path = Union[str, "os.PathLike[str]"]
 
 
 @dataclass
 class ReleaseRange:
     start: int
@@ -192,15 +183,15 @@
         return self.parse_tokens(tokens, debug)
 
     def parse_stream(self, stream: IO[str], debug: bool = False) -> NL:
         """Parse a stream and return the syntax tree."""
         return self.parse_stream_raw(stream, debug)
 
     def parse_file(
-        self, filename: Path, encoding: Optional[str] = None, debug: bool = False
+            self, filename: Path, encoding: Optional[str] = None, debug: bool = False
     ) -> NL:
         """Parse a file and return the syntax tree."""
         with open(filename, encoding=encoding) as stream:
             return self.parse_stream(stream, debug)
 
     def parse_string(self, text: str, debug: bool = False) -> NL:
         """Parse a string and return the syntax tree."""
@@ -245,19 +236,19 @@
     if cache_dir:
         return os.path.join(cache_dir, os.path.basename(name))
     else:
         return name
 
 
 def load_grammar(
-    gt: str = "Grammar.txt",
-    gp: Optional[str] = None,
-    save: bool = True,
-    force: bool = False,
-    logger: Optional[Logger] = None,
+        gt: str = "Grammar.txt",
+        gp: Optional[str] = None,
+        save: bool = True,
+        force: bool = False,
+        logger: Optional[Logger] = None,
 ) -> Grammar:
     """Load the grammar (maybe from a pickle)."""
     if logger is None:
         logger = logging.getLogger(__name__)
     gp = _generate_pickle_name(gt) if gp is None else gp
     if force or not _newer(gp, gt):
         g: grammar.Grammar = pgen.generate_grammar(gt)
@@ -279,15 +270,15 @@
         return False
     if not os.path.exists(b):
         return True
     return os.path.getmtime(a) >= os.path.getmtime(b)
 
 
 def load_packaged_grammar(
-    package: str, grammar_source: str, cache_dir: Optional[Path] = None
+        package: str, grammar_source: str, cache_dir: Optional[Path] = None
 ) -> grammar.Grammar:
     """Normally, loads a pickled grammar by doing
         pkgutil.get_data(package, pickled_grammar)
     where *pickled_grammar* is computed from *grammar_source* by adding the
     Python version and using a ``.pickle`` extension.
 
     However, if *grammar_source* is an extant file, load_grammar(grammar_source)
```

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/grammar.py` & `cercis-0.2.1/src/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/literals.py` & `cercis-0.2.1/src/blib2to3/pgen2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright 2004-2005 Elemental Security, Inc. All Rights Reserved.
 # Licensed to PSF under a Contributor Agreement.
 
 """Safely evaluate Python string literals without using eval()."""
 
 import re
-
 from typing import Dict, Match
 
-
 simple_escapes: Dict[str, str] = {
     "a": "\a",
     "b": "\b",
     "f": "\f",
     "n": "\n",
     "r": "\r",
     "t": "\t",
```

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/parse.py` & `cercis-0.2.1/src/blib2to3/pgen2/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 The grammar table must be loaded first.
 
 See Parser/parser.c in the Python distribution for additional info on
 how this parsing engine works.
 
 """
 from contextlib import contextmanager
-
-# Local imports
-from . import grammar, token, tokenize
 from typing import (
-    cast,
+    TYPE_CHECKING,
     Any,
-    Optional,
-    Union,
-    Tuple,
+    Callable,
     Dict,
-    List,
     Iterator,
-    Callable,
+    List,
+    Optional,
     Set,
-    TYPE_CHECKING,
+    Tuple,
+    Union,
+    cast,
 )
+
 from blib2to3.pgen2.grammar import Grammar
-from blib2to3.pytree import convert, NL, Context, RawNode, Leaf, Node
+from blib2to3.pytree import NL, Context, Leaf, Node, RawNode, convert
+
+# Local imports
+from . import grammar, token, tokenize
 
 if TYPE_CHECKING:
     from blib2to3.pgen2.driver import TokenProxy
 
 
 Results = Dict[str, NL]
 Convert = Callable[[Grammar, RawNode], Union[Node, Leaf]]
@@ -45,15 +46,15 @@
 
 
 # A placeholder node, used when parser is backtracking.
 DUMMY_NODE = (-1, None, None, None)
 
 
 def stack_copy(
-    stack: List[Tuple[DFAS, int, RawNode]]
+        stack: List[Tuple[DFAS, int, RawNode]]
 ) -> List[Tuple[DFAS, int, RawNode]]:
     """Nodeless stack copy."""
     return [(dfa, label, DUMMY_NODE) for dfa, label, _ in stack]
 
 
 class Recorder:
     def __init__(self, parser: "Parser", ilabels: List[int], context: Context) -> None:
@@ -108,15 +109,17 @@
         for ilabel in self.ilabels:
             with self.switch_to(ilabel):
                 args = [tok_type, tok_val, self.context]
                 if raw:
                     args.insert(0, ilabel)
                 func(*args)
 
-    def determine_route(self, value: Optional[str] = None, force: bool = False) -> Optional[int]:
+    def determine_route(
+            self, value: Optional[str] = None, force: bool = False
+    ) -> Optional[int]:
         alive_ilabels = self.ilabels
         if len(alive_ilabels) == 0:
             *_, most_successful_ilabel = self._dead_ilabels
             raise ParseError("bad input", most_successful_ilabel, value, self.context)
 
         ilabel, *rest = alive_ilabels
         if force or not rest:
@@ -125,15 +128,15 @@
             return None
 
 
 class ParseError(Exception):
     """Exception to signal the parser is stuck."""
 
     def __init__(
-        self, msg: str, type: Optional[int], value: Optional[str], context: Context
+            self, msg: str, type: Optional[int], value: Optional[str], context: Context
     ) -> None:
         Exception.__init__(
             self, f"{msg}: type={type!r}, value={value!r}, context={context!r}"
         )
         self.msg = msg
         self.type = type
         self.value = value
```

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/pgen.py` & `cercis-0.2.1/src/blib2to3/pgen2/pgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # Copyright 2004-2005 Elemental Security, Inc. All Rights Reserved.
 # Licensed to PSF under a Contributor Agreement.
 
-# Pgen imports
-from . import grammar, token, tokenize
-
+import os
 from typing import (
+    IO,
     Any,
     Dict,
-    IO,
     Iterator,
     List,
+    NoReturn,
     Optional,
+    Sequence,
     Tuple,
     Union,
-    Sequence,
-    NoReturn,
 )
-from blib2to3.pgen2 import grammar
-from blib2to3.pgen2.tokenize import GoodTokenInfo
-import os
 
+from blib2to3.pgen2 import grammar, token, tokenize
+from blib2to3.pgen2.tokenize import GoodTokenInfo
 
 Path = Union[str, "os.PathLike[str]"]
 
 
 class PgenGrammar(grammar.Grammar):
     pass
 
@@ -145,15 +142,15 @@
 
     def calcfirst(self, name: str) -> None:
         dfa = self.dfas[name]
         self.first[name] = None  # dummy to detect left recursion
         state = dfa[0]
         totalset: Dict[str, int] = {}
         overlapcheck = {}
-        for label, next in state.arcs.items():
+        for label in state.arcs:
             if label in self.dfas:
                 if label in self.first:
                     fset = self.first[label]
                     if fset is None:
                         raise ValueError("recursion for rule %r" % name)
                 else:
                     self.calcfirst(label)
@@ -186,17 +183,17 @@
             name = self.expect(token.NAME)
             self.expect(token.OP, ":")
             a, z = self.parse_rhs()
             self.expect(token.NEWLINE)
             # self.dump_nfa(name, a, z)
             dfa = self.make_dfa(a, z)
             # self.dump_dfa(name, dfa)
-            oldlen = len(dfa)
+            # oldlen = len(dfa)
             self.simplify_dfa(dfa)
-            newlen = len(dfa)
+            # newlen = len(dfa)
             dfas[name] = dfa
             # print name, oldlen, newlen
             if startsymbol is None:
                 startsymbol = name
         assert startsymbol is not None
         return dfas, startsymbol
 
@@ -342,15 +339,15 @@
             a.addarc(z, self.value)
             self.gettoken()
             return a, z
         else:
             self.raise_error(
                 "expected (...) or NAME or STRING, got %s/%s", self.type, self.value
             )
-            assert False
+            raise AssertionError
 
     def expect(self, type: int, value: Optional[Any] = None) -> str:
         if self.type != type or (value is not None and self.value != value):
             self.raise_error(
                 "expected %s/%s, got %s/%s", type, value, self.type, self.value
             )
         value = self.value
@@ -364,15 +361,15 @@
         self.type, self.value, self.begin, self.end, self.line = tup
         # print token.tok_name[self.type], repr(self.value)
 
     def raise_error(self, msg: str, *args: Any) -> NoReturn:
         if args:
             try:
                 msg = msg % args
-            except:
+            except Exception:
                 msg = " ".join([msg] + list(map(str, args)))
         raise SyntaxError(msg, (self.filename, self.end[0], self.end[1], self.line))
 
 
 class NFAState:
     arcs: List[Tuple[Optional[str], "NFAState"]]
```

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/token.py` & `cercis-0.2.1/src/blib2to3/pgen2/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Token constants (from "token.h")."""
 
-from typing import Dict
-
-from typing import Final
+from typing import Dict, Final
 
 #  Taken from Python (r53757) and modified to include some tokens
 #   originally monkeypatched in by pgen2.tokenize
 
 # --start constants--
 ENDMARKER: Final = 0
 NAME: Final = 1
```

### Comparing `cercis-0.2.0/src/blib2to3/pgen2/tokenize.py` & `cercis-0.2.1/src/blib2to3/pgen2/tokenize.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,36 +26,49 @@
 are the same, except instead of generating tokens, tokeneater is a callback
 function to which the 5 fields described above are passed as 5 arguments,
 each time a new token is found."""
 
 import sys
 from typing import (
     Callable,
+    Final,
     Iterable,
     Iterator,
     List,
     Optional,
+    Pattern,
     Set,
     Tuple,
-    Pattern,
     Union,
     cast,
 )
 
-from typing import Final
-
-from blib2to3.pgen2.token import *
 from blib2to3.pgen2.grammar import Grammar
+from blib2to3.pgen2.token import (
+    ASYNC,
+    AWAIT,
+    COMMENT,
+    DEDENT,
+    ENDMARKER,
+    ERRORTOKEN,
+    INDENT,
+    NAME,
+    NEWLINE,
+    NL,
+    NUMBER,
+    OP,
+    STRING,
+    tok_name,
+)
 
 __author__ = "Ka-Ping Yee <ping@lfw.org>"
 __credits__ = "GvR, ESR, Tim Peters, Thomas Wouters, Fred Drake, Skip Montanaro"
 
 import re
 from codecs import BOM_UTF8, lookup
-from blib2to3.pgen2.token import *
 
 from . import token
 
 __all__ = [x for x in dir(token) if x[0] != "_"] + [
     "tokenize",
     "generate_tokens",
     "untokenize",
@@ -184,15 +197,15 @@
     pass
 
 
 Coord = Tuple[int, int]
 
 
 def printtoken(
-    type: int, token: str, srow_col: Coord, erow_col: Coord, line: str
+        type: int, token: str, srow_col: Coord, erow_col: Coord, line: str
 ) -> None:  # for testing
     (srow, scol) = srow_col
     (erow, ecol) = erow_col
     print(
         "%d,%d-%d,%d:\t%s\t%s" % (srow, scol, erow, ecol, tok_name[type], repr(token))
     )
 
@@ -330,15 +343,15 @@
     encoding = None
     default = "utf-8"
 
     def read_or_stop() -> bytes:
         try:
             return readline()
         except StopIteration:
-            return b''
+            return b""
 
     def find_cookie(line: bytes) -> Optional[str]:
         try:
             line_string = line.decode("ascii")
         except UnicodeDecodeError:
             return None
         match = cookie_re.match(line_string)
@@ -402,15 +415,15 @@
         assert t1 == t2
     """
     ut = Untokenizer()
     return ut.untokenize(iterable)
 
 
 def generate_tokens(
-    readline: Callable[[], str], grammar: Optional[Grammar] = None
+        readline: Callable[[], str], grammar: Optional[Grammar] = None
 ) -> Iterator[GoodTokenInfo]:
     """
     The generate_tokens() generator requires one argument, readline, which
     must be a callable object which provides the same interface as the
     readline() method of built-in file objects. Each call to the function
     should return one line of input as a string.  Alternately, readline
     can be a callable function terminating with StopIteration:
@@ -551,17 +564,15 @@
         while pos < max:
             pseudomatch = pseudoprog.match(line, pos)
             if pseudomatch:  # scan for tokens
                 start, end = pseudomatch.span(1)
                 spos, epos, pos = (lnum, start), (lnum, end), end
                 token, initial = line[start:end], line[start]
 
-                if initial in numchars or (
-                    initial == "." and token != "."
-                ):  # ordinary number
+                if initial in numchars or (initial == "." and token != "."):  # ordinary number
                     yield (NUMBER, token, spos, epos, line)
                 elif initial in "\r\n":
                     newline = NEWLINE
                     if parenlev > 0:
                         newline = NL
                     elif async_def:
                         async_def_nl = True
@@ -672,19 +683,17 @@
                 yield (ERRORTOKEN, line[pos], (lnum, pos), (lnum, pos + 1), line)
                 pos += 1
 
     if stashed:
         yield stashed
         stashed = None
 
-    for indent in indents[1:]:  # pop remaining indent levels
+    for _indent in indents[1:]:  # pop remaining indent levels
         yield (DEDENT, "", (lnum, 0), (lnum, 0), "")
     yield (ENDMARKER, "", (lnum, 0), (lnum, 0), "")
 
 
 if __name__ == "__main__":  # testing
-    import sys
-
     if len(sys.argv) > 1:
         tokenize(open(sys.argv[1]).readline)
     else:
         tokenize(sys.stdin.readline)
```

### Comparing `cercis-0.2.0/src/cercis/__init__.py` & `cercis-0.2.1/src/cercis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -847,15 +847,15 @@
                 report.path_ignored(p, "matches the --force-exclude regular expression")
                 continue
 
             if is_stdin:
                 p = Path(f"{STDIN_PLACEHOLDER}{str(p)}")
 
             if p.suffix == ".ipynb" and not jupyter_dependencies_are_installed(
-                verbose=verbose, quiet=quiet
+                warn=verbose or not quiet
             ):
                 continue
 
             sources.add(p)
         elif p.is_dir():
             p = root / normalize_path_maybe_ignore(p, ctx.obj["root"], report)
             if verbose:
```

### Comparing `cercis-0.2.0/src/cercis/_width_table.py` & `cercis-0.2.1/src/cercis/_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/brackets.py` & `cercis-0.2.1/src/cercis/brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/cache.py` & `cercis-0.2.1/src/cercis/cache.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/comments.py` & `cercis-0.2.1/src/cercis/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/concurrency.py` & `cercis-0.2.1/src/cercis/concurrency.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/const.py` & `cercis-0.2.1/src/cercis/const.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/debug.py` & `cercis-0.2.1/src/cercis/debug.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/files.py` & `cercis-0.2.1/src/cercis/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
                 new_gitignore_dict,
                 verbose=verbose,
                 quiet=quiet,
             )
 
         elif child.is_file():
             if child.suffix == ".ipynb" and not jupyter_dependencies_are_installed(
-                verbose=verbose, quiet=quiet
+                warn=verbose or not quiet
             ):
                 continue
             include_match = include.search(normalized_path) if include else True
             if include_match:
                 yield child
```

### Comparing `cercis-0.2.0/src/cercis/handle_ipynb_magics.py` & `cercis-0.2.1/src/cercis/handle_ipynb_magics.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import ast
 import collections
 import dataclasses
 import secrets
 import sys
 from functools import lru_cache
+from importlib.util import find_spec
 from typing import Dict, List, Optional, Tuple
 
 if sys.version_info >= (3, 10):
     from typing import TypeGuard
 else:
     from typing_extensions import TypeGuard
 
@@ -52,33 +53,25 @@
 @dataclasses.dataclass(frozen=True)
 class Replacement:
     mask: str
     src: str
 
 
 @lru_cache
-def jupyter_dependencies_are_installed(*, verbose: bool, quiet: bool) -> bool:
-    try:
-        # isort: off
-        # tokenize_rt is less commonly installed than IPython
-        # and IPython is expensive to import
-        import tokenize_rt  # noqa:F401
-        import IPython  # noqa:F401
-
-        # isort: on
-    except ModuleNotFoundError:
-        if verbose or not quiet:
-            msg = (
-                "Skipping .ipynb files as Jupyter dependencies are not installed.\n"
-                'You can fix this by running ``pip install "cercis[jupyter]"``'
-            )
-            out(msg)
-        return False
-    else:
-        return True
+def jupyter_dependencies_are_installed(*, warn: bool) -> bool:
+    installed = (
+        find_spec("tokenize_rt") is not None and find_spec("IPython") is not None
+    )
+    if not installed and warn:
+        msg = (
+            "Skipping .ipynb files as Jupyter dependencies are not installed.\n"
+            'You can fix this by running ``pip install "cercis[jupyter]"``'
+        )
+        out(msg)
+    return installed
 
 
 def remove_trailing_semicolon(src: str) -> Tuple[str, bool]:
     """Remove trailing semicolon from Jupyter notebook cell.
 
     For example,
```

### Comparing `cercis-0.2.0/src/cercis/indent.py` & `cercis-0.2.1/src/cercis/indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/linegen.py` & `cercis-0.2.1/src/cercis/linegen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/lines.py` & `cercis-0.2.1/src/cercis/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 _PRAGMA_REGEX = re.compile("( *# (?:pylint|pytype|noqa|type(?=: *ignore)):)")
 
 
 @dataclass
 class Line:
     """Holds leaves and comments. Can be printed with `str(line)`."""
 
-    mode: Mode
+    mode: Mode = field(repr=False)
     depth: Tuple[Indent, ...] = field(default_factory=tuple)
     leaves: List[Leaf] = field(default_factory=list)
     # keys ordered like `leaves`
     comments: Dict[LeafID, List[Leaf]] = field(default_factory=dict)
     bracket_tracker: BracketTracker = field(default_factory=BracketTracker)
     inside_brackets: bool = False
     should_split_rhs: bool = False
@@ -665,36 +665,41 @@
             first_leaf = current_line.leaves[0]
             before = first_leaf.prefix.count("\n")
             before = min(before, max_allowed)
             first_leaf.prefix = ""
         else:
             before = 0
         depth = current_line.depth
-        while self.previous_defs and len(self.previous_defs[-1].depth) >= len(depth):
+
+        previous_def = None
+        while self.previous_defs and self.previous_defs[-1].depth >= depth:
+            previous_def = self.previous_defs.pop()
+
+        if previous_def is not None:
+            assert self.previous_line is not None
             if self.mode.is_pyi:
-                assert self.previous_line is not None
                 if depth and not current_line.is_def and self.previous_line.is_def:
                     # Empty lines between attributes and methods should be preserved.
                     before = min(1, before)
                 elif (
                     Preview.blank_line_after_nested_stub_class in self.mode
-                    and self.previous_defs[-1].is_class
-                    and not self.previous_defs[-1].is_stub_class
+                    and previous_def.is_class
+                    and not previous_def.is_stub_class
                 ):
                     before = 1
                 elif depth:
                     before = 0
                 else:
                     before = 1
             else:
                 if depth:
                     before = 1
                 elif (
                     not depth
-                    and self.previous_defs[-1].depth
+                    and previous_def.depth
                     and current_line.leaves[-1].type == token.COLON
                     and (
                         current_line.leaves[0].value
                         not in ("with", "try", "for", "while", "if", "match")
                     )
                 ):
                     # We shouldn't add two newlines between an indented function and
@@ -703,15 +708,15 @@
                     # and therefore get two trailing newlines, but look weird and
                     # inconsistent when they're followed by elif, else, etc. This is
                     # worse because these functions only get *one* preceding newline
                     # already.
                     before = 1
                 else:
                     before = 2
-            self.previous_defs.pop()
+
         if current_line.is_decorator or current_line.is_def or current_line.is_class:
             return self._maybe_empty_lines_for_class_or_def(current_line, before)
 
         if (
             self.previous_line
             and self.previous_line.is_import
             and not current_line.is_import
```

### Comparing `cercis-0.2.0/src/cercis/mode.py` & `cercis-0.2.1/src/cercis/mode.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/nodes.py` & `cercis-0.2.1/src/cercis/nodes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/numerics.py` & `cercis-0.2.1/src/cercis/numerics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/output.py` & `cercis-0.2.1/src/cercis/output.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/parsing.py` & `cercis-0.2.1/src/cercis/parsing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/report.py` & `cercis-0.2.1/src/cercis/report.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/rusty.py` & `cercis-0.2.1/src/cercis/rusty.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/strings.py` & `cercis-0.2.1/src/cercis/strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/trans.py` & `cercis-0.2.1/src/cercis/trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/utils_line_wrapping.py` & `cercis-0.2.1/src/cercis/utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/src/cercis/utils_linegen.py` & `cercis-0.2.1/src/cercis/utils_linegen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/optional.py` & `cercis-0.2.1/tests/optional.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/test_black.py` & `cercis-0.2.1/tests/test_black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/test_blackd.py` & `cercis-0.2.1/tests/test_blackd.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/test_format.py` & `cercis-0.2.1/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/test_ipynb.py` & `cercis-0.2.1/tests/test_ipynb.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,25 +442,21 @@
         monkeypatch: MonkeyPatch, tmp_path: pathlib.Path
 ) -> None:
     # Check that the cache isn't written to if Jupyter dependencies aren't installed.
     jupyter_dependencies_are_installed.cache_clear()
     nb = get_case_path("jupyter", "notebook_trailing_newline.ipynb")
     tmp_nb = tmp_path / "notebook.ipynb"
     tmp_nb.write_bytes(nb.read_bytes())
-    monkeypatch.setattr(
-        "cercis.jupyter_dependencies_are_installed", lambda verbose, quiet: False
-    )
+    monkeypatch.setattr("cercis.jupyter_dependencies_are_installed", lambda warn: False)
     result = runner.invoke(
         main, [str(tmp_path / "notebook.ipynb"), f"--config={EMPTY_CONFIG}"]
     )
     assert "No Python files are present to be formatted. Nothing to do" in result.output
     jupyter_dependencies_are_installed.cache_clear()
-    monkeypatch.setattr(
-        "cercis.jupyter_dependencies_are_installed", lambda verbose, quiet: True
-    )
+    monkeypatch.setattr("cercis.jupyter_dependencies_are_installed", lambda warn: True)
     result = runner.invoke(
         main, [str(tmp_path / "notebook.ipynb"), f"--config={EMPTY_CONFIG}"]
     )
     assert "reformatted" in result.output
 
 
 def test_cache_isnt_written_if_no_jupyter_deps_dir(
@@ -468,21 +464,21 @@
 ) -> None:
     # Check that the cache isn't written to if Jupyter dependencies aren't installed.
     jupyter_dependencies_are_installed.cache_clear()
     nb = get_case_path("jupyter", "notebook_trailing_newline.ipynb")
     tmp_nb = tmp_path / "notebook.ipynb"
     tmp_nb.write_bytes(nb.read_bytes())
     monkeypatch.setattr(
-        "cercis.files.jupyter_dependencies_are_installed", lambda verbose, quiet: False
+        "cercis.files.jupyter_dependencies_are_installed", lambda warn: False
     )
     result = runner.invoke(main, [str(tmp_path), f"--config={EMPTY_CONFIG}"])
     assert "No Python files are present to be formatted. Nothing to do" in result.output
     jupyter_dependencies_are_installed.cache_clear()
     monkeypatch.setattr(
-        "cercis.files.jupyter_dependencies_are_installed", lambda verbose, quiet: True
+        "cercis.files.jupyter_dependencies_are_installed", lambda warn: True
     )
     result = runner.invoke(main, [str(tmp_path), f"--config={EMPTY_CONFIG}"])
     assert "reformatted" in result.output
 
 
 def test_ipynb_flag(tmp_path: pathlib.Path) -> None:
     nb = get_case_path("jupyter", "notebook_trailing_newline.ipynb")
```

### Comparing `cercis-0.2.0/tests/test_no_ipynb.py` & `cercis-0.2.1/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/test_trans.py` & `cercis-0.2.1/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/test_utils_line_wrapping.py` & `cercis-0.2.1/tests/test_utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/util.py` & `cercis-0.2.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/conditional_expression.py` & `cercis-0.2.1/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py` & `cercis-0.2.1/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py` & `cercis-0.2.1/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py` & `cercis-0.2.1/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py` & `cercis-0.2.1/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py` & `cercis-0.2.1/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py` & `cercis-0.2.1/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py` & `cercis-0.2.1/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/edge_cases.py` & `cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/edge_cases.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py` & `cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py` & `cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py` & `cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py` & `cercis-0.2.1/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py` & `cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py` & `cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py` & `cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py` & `cercis-0.2.1/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Black_default.py` & `cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Black_default_2.py` & `cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Black_default_2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Cercis_default.py` & `cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py` & `cercis-0.2.1/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/single_quote/docstring.py` & `cercis-0.2.1/tests/data/configurable_cases/single_quote/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/single_quote/docstring_preview.py` & `cercis-0.2.1/tests/data/configurable_cases/single_quote/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/single_quote/more_quotes.py` & `cercis-0.2.1/tests/data/configurable_cases/single_quote/more_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/single_quote/string_prefixes.py` & `cercis-0.2.1/tests/data/configurable_cases/single_quote/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/configurable_cases/single_quote/torture.py` & `cercis-0.2.1/tests/data/configurable_cases/single_quote/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `cercis-0.2.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/jupyter/notebook_trailing_newline.ipynb` & `cercis-0.2.1/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/jupyter/notebook_without_changes.ipynb` & `cercis-0.2.1/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/debug_visitor.out` & `cercis-0.2.1/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/debug_visitor.py` & `cercis-0.2.1/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/decorators.py` & `cercis-0.2.1/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/docstring_no_string_normalization.py` & `cercis-0.2.1/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `cercis-0.2.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/force_py36.py` & `cercis-0.2.1/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/force_pyi.py` & `cercis-0.2.1/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/long_strings_flag_disabled.py` & `cercis-0.2.1/tests/data/miscellaneous/long_strings_flag_disabled.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/python2_detection.py` & `cercis-0.2.1/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/string_quotes.py` & `cercis-0.2.1/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/miscellaneous/stub.pyi` & `cercis-0.2.1/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/cantfit.py` & `cercis-0.2.1/tests/data/preview/cantfit.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/comments7.py` & `cercis-0.2.1/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/format_unicode_escape_seq.py` & `cercis-0.2.1/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/long_dict_values.py` & `cercis-0.2.1/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/long_strings.py` & `cercis-0.2.1/tests/data/preview/long_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/long_strings__east_asian_width.py` & `cercis-0.2.1/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/long_strings__edge_case.py` & `cercis-0.2.1/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/long_strings__regression.py` & `cercis-0.2.1/tests/data/preview/long_strings__regression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/long_strings__type_annotations.py` & `cercis-0.2.1/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/multiline_strings.py` & `cercis-0.2.1/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/no_blank_line_before_docstring.py` & `cercis-0.2.1/tests/data/preview/no_blank_line_before_docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/prefer_rhs_split.py` & `cercis-0.2.1/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview/trailing_comma.py` & `cercis-0.2.1/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview_context_managers/targeting_py38.py` & `cercis-0.2.1/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview_context_managers/targeting_py39.py` & `cercis-0.2.1/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `cercis-0.2.1/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_310/parenthesized_context_managers.py` & `cercis-0.2.1/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_310/pattern_matching_complex.py` & `cercis-0.2.1/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_310/pattern_matching_extras.py` & `cercis-0.2.1/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_310/pattern_matching_generic.py` & `cercis-0.2.1/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_310/pattern_matching_simple.py` & `cercis-0.2.1/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_310/pattern_matching_style.py` & `cercis-0.2.1/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_311/pep_646.py` & `cercis-0.2.1/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_311/pep_654.py` & `cercis-0.2.1/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_311/pep_654_style.py` & `cercis-0.2.1/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_312/type_params.py` & `cercis-0.2.1/tests/data/py_312/type_params.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_36/numeric_literals.py` & `cercis-0.2.1/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_37/python37.py` & `cercis-0.2.1/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_38/pep_570.py` & `cercis-0.2.1/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_38/pep_572.py` & `cercis-0.2.1/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_38/pep_572_remove_parens.py` & `cercis-0.2.1/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_38/python38.py` & `cercis-0.2.1/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_39/python39.py` & `cercis-0.2.1/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/py_39/remove_with_brackets.py` & `cercis-0.2.1/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/attribute_access_on_number_literals.py` & `cercis-0.2.1/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/class_blank_parentheses.py` & `cercis-0.2.1/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/class_methods_new_line.py` & `cercis-0.2.1/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/collections.py` & `cercis-0.2.1/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments.py` & `cercis-0.2.1/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments2.py` & `cercis-0.2.1/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments3.py` & `cercis-0.2.1/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments4.py` & `cercis-0.2.1/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments5.py` & `cercis-0.2.1/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments6.py` & `cercis-0.2.1/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments9.py` & `cercis-0.2.1/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/comments_non_breaking_space.py` & `cercis-0.2.1/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/composition.py` & `cercis-0.2.1/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/composition_no_trailing_comma.py` & `cercis-0.2.1/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/docstring.py` & `cercis-0.2.1/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/docstring_preview.py` & `cercis-0.2.1/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/empty_lines.py` & `cercis-0.2.1/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/expression.diff` & `cercis-0.2.1/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/expression.py` & `cercis-0.2.1/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/fmtonoff.py` & `cercis-0.2.1/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/fmtonoff2.py` & `cercis-0.2.1/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/fmtonoff5.py` & `cercis-0.2.1/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/fmtskip2.py` & `cercis-0.2.1/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/fmtskip8.py` & `cercis-0.2.1/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/fstring.py` & `cercis-0.2.1/tests/data/simple_cases/fstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/function.py` & `cercis-0.2.1/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/function2.py` & `cercis-0.2.1/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/function_trailing_comma.py` & `cercis-0.2.1/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/import_spacing.py` & `cercis-0.2.1/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/multiline_consecutive_open_parentheses_ignore.py` & `cercis-0.2.1/tests/data/simple_cases/multiline_consecutive_open_parentheses_ignore.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/one_element_subscript.py` & `cercis-0.2.1/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/pep_604.py` & `cercis-0.2.1/tests/data/simple_cases/pep_604.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/power_op_spacing.py` & `cercis-0.2.1/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `cercis-0.2.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/remove_await_parens.py` & `cercis-0.2.1/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/remove_except_parens.py` & `cercis-0.2.1/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/remove_for_brackets.py` & `cercis-0.2.1/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `cercis-0.2.1/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/remove_parens.py` & `cercis-0.2.1/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/return_annotation_brackets.py` & `cercis-0.2.1/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/skip_magic_trailing_comma.py` & `cercis-0.2.1/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/slices.py` & `cercis-0.2.1/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/string_prefixes.py` & `cercis-0.2.1/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/torture.py` & `cercis-0.2.1/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `cercis-0.2.1/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `cercis-0.2.1/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `cercis-0.2.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/LICENSE` & `cercis-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/LICENSE_ORIGINAL` & `cercis-0.2.1/LICENSE_ORIGINAL`

 * *Files identical despite different names*

### Comparing `cercis-0.2.0/pyproject.toml` & `cercis-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 collapse-nested-brackets = false  # use Black style for easier rebasing
 wrap-pragma-comments = true  # use Black style for easier rebasing
 target-version = ['py37', 'py38']
 include = '\.pyi?$'
 extend-exclude = '''
 /(
   # The following are specific to Black, you probably don't want those.
-  | blib2to3
-  | tests/data
+  tests/data
   | profiling
 )/
 '''
 # We use preview style for formatting Black itself. If you
 # want stable formatting across releases, you should keep
 # this off.
 preview = true
@@ -31,15 +30,15 @@
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cercis"
-version = "0.2.0"
+version = "0.2.1"
 description = "A more configurable Python code formatter"
 license = { text = "MIT" }
 requires-python = ">=3.8"
 authors = [
   { name = "Łukasz Langa", email = "lukasz@langa.pl" },
   { name = "jsh9", email = "" },
 ]
@@ -185,15 +184,15 @@
 AIOHTTP_NO_EXTENSIONS = "1"
 
 [tool.isort]
 atomic = true
 profile = "black"
 line_length = 88
 skip_gitignore = true
-skip_glob = ["src/blib2to3", "tests/data", "profiling"]
+skip_glob = ["tests/data", "profiling"]
 known_first_party = ["cercis", "blib2to3", "blackd", "_cercis_version"]
 
 [tool.pytest.ini_options]
 # Option below requires `tests/optional.py`
 addopts = "--strict-config --strict-markers"
 optional-tests = [
   "no_blackd: run when `d` extra NOT installed",
```

### Comparing `cercis-0.2.0/PKG-INFO` & `cercis-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cercis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A more configurable Python code formatter
 Project-URL: Changelog, https://github.com/jsh9/cercis/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/jsh9/cercis
 Author: jsh9
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 License-File: LICENSE
@@ -789,14 +789,24 @@
 There are 2 files in this repo: [CHANGELOG.md](./CHANGELOG.md) and
 [CHANGES.md](./CHANGES.md).
 
 The former tracks the changes of _Cercis_ (_Black_ does not have this file). The latter
 tracks the changes on _Black_ (it exists in the _Black_ repo as well).
 # Change Log
 
+## [0.2.1] - 2023-07-23
+
+- Changed
+  - Rebased `Cercis` to be head to head with `Black`
+- Fixed
+  - Fixed a pytest regression where Python warnings are treated as errors
+    (https://github.com/jsh9/cercis/commit/1229b9dd18f861423e26f8de3f4b5e714d72bd9c)
+- Diff
+  - https://github.com/jsh9/cercis/compare/0.2.0...0.2.1
+
 ## [0.2.0] - 2023-07-12
 
 - Changed
   - Rebased `Cercis` to be head to head with `Black`
     [version 23.7.0](https://github.com/psf/black/releases/tag/23.7.0)
 - Diff
   - https://github.com/jsh9/cercis/compare/0.1.7...0.2.0
```

