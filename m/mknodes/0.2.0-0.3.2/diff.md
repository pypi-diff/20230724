# Comparing `tmp/mknodes-0.2.0.tar.gz` & `tmp/mknodes-0.3.2.tar.gz`

## Comparing `mknodes-0.2.0.tar` & `mknodes-0.3.2.tar`

### file list

```diff
@@ -1,67 +1,82 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mknodes-0.2.0/.editorconfig
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mknodes-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 mknodes-0.2.0/Makefile
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 mknodes-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mknodes-0.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 mknodes-0.2.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mknodes-0.2.0/docs/gen_pages.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 mknodes-0.2.0/docs/gen_qt.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/__init__.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/classhelpers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/connectionbuilder.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mermaid.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkadmonition.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkbaseclasstable.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkclasspage.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkclasstable.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkcode.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkcritic.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkdiagram.py
--rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkimage.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mklink.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mklist.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkmodulepage.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkmoduletable.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mknav.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mknode.py
--rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkpage.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkshields.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mktable.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mktabs.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mktext.py
--rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/node.py
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/noderesolver.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/__init__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_add.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_admonition.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_classdiagram.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_docstrings.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_image.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_list.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_manual.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_markdownnode.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_mkpage.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_modulepage.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_tabblock.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_text.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 mknodes-0.2.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mknodes-0.2.0/LICENSE
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mknodes-0.2.0/README.md
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 mknodes-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 mknodes-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.3.2/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.3.2/Makefile
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 mknodes-0.3.2/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.3.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.3.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mknodes-0.3.2/docs/gen_pages.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mknodes-0.3.2/docs/gen_qt.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkblock.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10465 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkimage.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mklink.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mklist.py
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mknav.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mknode.py
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkshields.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktable.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktabs.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkbaseclasstable.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_admonition.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_image.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_list.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_modulepage.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_nav.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_page.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_tabblock.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_text.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.3.2/README.md
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 mknodes-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 mknodes-0.3.2/PKG-INFO
```

### Comparing `mknodes-0.2.0/.pre-commit-config.yaml` & `mknodes-0.3.2/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-default_language_version:
-    python: python3.10
-default_stages: [commit]
-repos:
-- repo: local
-  hooks:
-    - id: pytest-check
-      name: pytest-check
-      entry: hatch run test
-      language: system
-      # stages: [push]
-      types: [python]
-      pass_filenames: false
-      always_run: true
-- repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
-  hooks:
-    # - id: trailing-whitespace
-    # - id: check-ast
-    - id: check-case-conflict
-    - id: check-docstring-first
-    - id: check-merge-conflict
-    # - id: check-yaml
-    - id: check-toml
-    - id: check-json
-    - id: detect-private-key
-    - id: forbid-new-submodules
-    # - id: check-added-large-files
-# https://pre-commit.com/hooks.html
-- repo: https://github.com/ambv/black
-  rev: 23.7.0
-  hooks:
-    - id: black
-      args: [--preview]
-
-- repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.4.1
-  hooks:
-    - id: mypy
-      # args: [--ignore-missing-imports]
-      additional_dependencies: [types-typed-ast]
-
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.278
-  hooks:
-    - id: ruff
-
-- repo: https://github.com/commitizen-tools/commitizen
-  rev: 3.5.2
-  hooks:
-    - id: commitizen
-      stages: [commit-msg]
-      additional_dependencies: [typing-extensions]
+default_language_version:
+    python: python3.10
+default_stages: [commit]
+repos:
+- repo: local
+  hooks:
+    - id: pytest-check
+      name: pytest-check
+      entry: hatch run test
+      language: system
+      # stages: [push]
+      types: [python]
+      pass_filenames: false
+      always_run: true
+- repo: https://github.com/pre-commit/pre-commit-hooks
+  rev: v4.4.0
+  hooks:
+    # - id: trailing-whitespace
+    # - id: check-ast
+    - id: check-case-conflict
+    - id: check-docstring-first
+    - id: check-merge-conflict
+    # - id: check-yaml
+    - id: check-toml
+    - id: check-json
+    - id: detect-private-key
+    - id: forbid-new-submodules
+    # - id: check-added-large-files
+# https://pre-commit.com/hooks.html
+- repo: https://github.com/ambv/black
+  rev: 23.7.0
+  hooks:
+    - id: black
+      args: [--preview]
+
+- repo: https://github.com/pre-commit/mirrors-mypy
+  rev: v1.4.1
+  hooks:
+    - id: mypy
+      # args: [--ignore-missing-imports]
+      additional_dependencies: [types-typed-ast]
+
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: v0.0.280
+  hooks:
+    - id: ruff
+
+- repo: https://github.com/commitizen-tools/commitizen
+  rev: 3.5.3
+  hooks:
+    - id: commitizen
+      stages: [commit-msg]
+      additional_dependencies: [typing-extensions]
```

### Comparing `mknodes-0.2.0/mkdocs.yml` & `mknodes-0.3.2/mkdocs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,133 @@
-site_name: MkNodes
-site_description: "Generate docs with ease."
-repo_url: "https://github.com/phil65/mknodes"
-site_url: https://phil65.github.io/MkNodes/
-watch: [mkdocs.yml, README.md, mknodes/]
-copyright: Copyright &copy; 2023 Philipp Temminghoff
-
-theme:
-  name: material
-  palette:
-  # Palette toggle for light mode
-  - media: "(prefers-color-scheme: light)"
-    scheme: default
-    primary: orange
-    toggle:
-      icon: material/brightness-7
-      name: Switch to dark mode
-
-  # Palette toggle for dark mode
-  - media: "(prefers-color-scheme: dark)"
-    scheme: slate
-    primary: orange
-    toggle:
-      icon: material/brightness-4
-      name: Switch to light mode
-  features:
-  - content.code.copy
-  - content.code.select
-  - content.code.annotate
-  # - content.tooltips  # for insiders..
-  - navigation.instant # make things faster
-  - navigation.tracking # update URL based on current item in TOC
-  - navigation.path  # shows breadcrumbs
-  - navigation.tabs # make top level tabs
-  # - navigation.expand # expand all subsections in left sidebar by defuault
-  - navigation.indexes # documents can be directly attached to sections (overview pages)
-  - navigation.footer # next/previous page buttons in footer
-  # - navigation.tabs.sticky # and make them sticky
-  - toc.follow  # makes toc follow scrolling
-  # - toc.integrate  # integrates toc into left menu
-  - navigation.top  # adds back-to-top button
-  # - navigation.sections # top-level sections are rendered as groups
-plugins:
-- search
-# - social  # this one has dependency which is not on pypi for windows. (cairocffi)
-- tags
-- section-index  # clickable sections leading to index page (https://github.com/oprypin/mkdocs-section-index)
-- glightbox  # better image support
-- macros
-- include-markdown  # include content of other markdown files
-- literate-nav:  # move nav out of mkdocs.yml
-    nav_file: SUMMARY.md
-    # implicit_index: true
-# - autorefs  # allows linking to any header
-- linkreplacer  # allows linking to any markdown page
-- gen-files: # https://github.com/oprypin/mkdocs-gen-files
-    scripts:
-      - docs/gen_pages.py  # or any other name or path
-- mkdocstrings:
-    default_handler: python
-    handlers:
-      python:
-        import:
-        - url: https://docs.python.org/3/objects.inv
-          domains: [std, py]
-        options:
-          # https://mkdocstrings.github.io/python/usage/
-          show_docstring_returns: false
-          show_source: true
-          show_signature_annotations: true
-          show_symbol_type_toc: true
-          show_symbol_type_heading: true
-          # merge_init_into_class: true
-          # ignore_init_summary: true
-          # show_if_no_docstring: true
-          inherited_members: false
-          signature_crossrefs: true
-          # separate_signature: true
-          line_length: 90
-markdown_extensions:
-- codehilite
-- admonition
-- def_list
-- attr_list
-- abbr
-- md_in_html
-- tables
-- footnotes
-- pymdownx.critic
-- pymdownx.caret
-- pymdownx.keys
-- pymdownx.mark
-- pymdownx.tilde
-- pymdownx.magiclink # auto-convert links
-- pymdownx.blocks.tab # new-style tabs
-# - pymdownx.saneheaders # require a whitespace after header #
-- pymdownx.tasklist:
-    custom_checkbox: true
-- pymdownx.highlight:  # syntax highlighting
-    anchor_linenums: true
-    line_spans: __span
-    pygments_lang_class: true
-    # linenums: true
-- pymdownx.inlinehilite  # syntax highlighting inside line (`#!py mycode`)
-- pymdownx.snippets  # syntax highlighting
-- pymdownx.details
-- pymdownx.superfences:  # syntax highlighting
-    custom_fences:
-    - name: mermaid
-      class: mermaid
-      format: !!python/name:pymdownx.superfences.fence_code_format
-- pymdownx.tabbed:
-    alternate_style: true
-- md_in_html
-- toc:
-    toc_depth: 2
-use_directory_urls: false
-
-extra:
-  social:
-  - icon: fontawesome/brands/github
-    link: https://github.com/phil65
-  - icon: fontawesome/brands/gitter
-    link: https://matrix.to/#/#mknodes:gitter.im
-  - icon: fontawesome/brands/python
-    link: https://pypi.org/project/mknodes/
-  # generator: false disable "made with Material"
-  # version:  # multiple doc versions
-  #   provider: mike
+site_name: MkNodes
+site_description: "Generate docs with ease."
+repo_url: "https://github.com/phil65/mknodes"
+site_url: https://phil65.github.io/MkNodes/
+watch: [mkdocs.yml, README.md, mknodes/]
+copyright: Copyright &copy; 2023 Philipp Temminghoff
+
+theme:
+  name: material
+  palette:
+  # Palette toggle for light mode
+  - media: "(prefers-color-scheme: light)"
+    scheme: default
+    primary: orange
+    toggle:
+      icon: material/brightness-7
+      name: Switch to dark mode
+
+  # Palette toggle for dark mode
+  - media: "(prefers-color-scheme: dark)"
+    scheme: slate
+    primary: orange
+    toggle:
+      icon: material/brightness-4
+      name: Switch to light mode
+  features:
+  - content.code.copy
+  - content.code.select
+  - content.code.annotate
+  # - content.tooltips  # for insiders..
+  - navigation.instant # make things faster
+  - navigation.tracking # update URL based on current item in TOC
+  - navigation.path  # shows breadcrumbs
+  - navigation.tabs # make top level tabs
+  # - navigation.expand # expand all subsections in left sidebar by defuault
+  - navigation.indexes # documents can be directly attached to sections (overview pages)
+  - navigation.footer # next/previous page buttons in footer
+  # - navigation.tabs.sticky # and make them sticky
+  - toc.follow  # makes toc follow scrolling
+  # - toc.integrate  # integrates toc into left menu
+  - navigation.top  # adds back-to-top button
+  # - navigation.sections # top-level sections are rendered as groups
+plugins:
+- search
+# - social  # this one has dependency which is not on pypi for windows. (cairocffi)
+- tags
+- section-index  # clickable sections leading to index page (https://github.com/oprypin/mkdocs-section-index)
+- glightbox  # better image support
+- macros
+- include-markdown  # include content of other markdown files
+- literate-nav:  # move nav out of mkdocs.yml
+    nav_file: SUMMARY.md
+    # implicit_index: true
+# - autorefs  # allows linking to any header
+- linkreplacer  # allows linking to any markdown page
+- gen-files: # https://github.com/oprypin/mkdocs-gen-files
+    scripts:
+      - docs/gen_pages.py  # or any other name or path
+- mkdocstrings:
+    default_handler: python
+    handlers:
+      python:
+        import:
+        - url: https://docs.python.org/3/objects.inv
+          domains: [std, py]
+        options:
+          # https://mkdocstrings.github.io/python/usage/
+          show_docstring_returns: false
+          show_source: true
+          show_signature_annotations: true
+          show_symbol_type_toc: true
+          show_symbol_type_heading: true
+          # merge_init_into_class: true
+          # ignore_init_summary: true
+          # show_if_no_docstring: true
+          inherited_members: false
+          signature_crossrefs: true
+          # separate_signature: true
+          line_length: 90
+markdown_extensions:
+- codehilite
+- admonition
+- def_list
+- attr_list
+- abbr
+- md_in_html
+- tables
+- footnotes
+- pymdownx.critic
+- pymdownx.caret
+- pymdownx.keys
+- pymdownx.mark
+- pymdownx.tilde
+- pymdownx.magiclink # auto-convert links
+- pymdownx.blocks.tab # new-style tabs
+- pymdownx.blocks.admonition # new-style admonition
+- pymdownx.blocks.definition # new-style definition
+- pymdownx.blocks.details # new-style details
+- pymdownx.blocks.html # new-style html
+# - pymdownx.saneheaders # require a whitespace after header #
+- pymdownx.tasklist:
+    custom_checkbox: true
+- pymdownx.highlight:  # syntax highlighting
+    anchor_linenums: true
+    line_spans: __span
+    pygments_lang_class: true
+    # linenums: true
+- pymdownx.inlinehilite  # syntax highlighting inside line (`#!py mycode`)
+- pymdownx.snippets  # syntax highlighting
+- pymdownx.details
+- pymdownx.superfences:  # syntax highlighting
+    custom_fences:
+    - name: mermaid
+      class: mermaid
+      format: !!python/name:pymdownx.superfences.fence_code_format
+- pymdownx.tabbed:
+    alternate_style: true
+- md_in_html
+- toc:
+    toc_depth: 2
+use_directory_urls: false
+
+extra:
+  social:
+  - icon: fontawesome/brands/github
+    link: https://github.com/phil65
+  - icon: fontawesome/brands/gitter
+    link: https://matrix.to/#/#mknodes:gitter.im
+  - icon: fontawesome/brands/python
+    link: https://pypi.org/project/mknodes/
+  # generator: false disable "made with Material"
+  # version:  # multiple doc versions
+  #   provider: mike
```

### Comparing `mknodes-0.2.0/.github/workflows/build.yml` & `mknodes-0.3.2/.github/workflows/build.yml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-name: Build
-
-on: [push, pull_request]
-
-jobs:
-  test:
-
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python_version: ['3.10', '3.11']
-
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python_version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install hatch
-        hatch env create
-    - name: Lint and typecheck
-      run: |
-        hatch run lint-check
-    - name: Test
-      run: |
-        hatch run test-cov-xml
-    - uses: codecov/codecov-action@v3
-      with:
-        token: ${{ secrets.CODECOV_TOKEN }}
-        fail_ci_if_error: true
-        verbose: true
-
-  release:
-    runs-on: ubuntu-latest
-    needs: test
-    if: startsWith(github.ref, 'refs/tags/')
-
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-    - name: Install dependencies
-      shell: bash
-      run: |
-        python -m pip install --upgrade pip
-        pip install hatch
-    - name: Build and publish on PyPI
-      env:
-        HATCH_INDEX_USER: ${{ secrets.HATCH_INDEX_USER }}
-        HATCH_INDEX_AUTH: ${{ secrets.HATCH_INDEX_AUTH }}
-      run: |
-        hatch build
-        hatch publish
-    - name: Create release
-      uses: ncipollo/release-action@v1
-      with:
-        draft: true
-        body: ${{ github.event.head_commit.message }}
-        artifacts: dist/*.whl,dist/*.tar.gz
-        token: ${{ secrets.GITHUB_TOKEN }}
+name: Build
+
+on: [push, pull_request]
+
+jobs:
+  test:
+
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python_version: ['3.10', '3.11']
+
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: ${{ matrix.python_version }}
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install hatch
+        hatch env create
+    - name: Lint and typecheck
+      run: |
+        hatch run lint-check
+    - name: Test
+      run: |
+        hatch run test-cov-xml
+    - uses: codecov/codecov-action@v3
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
+        fail_ci_if_error: true
+        verbose: true
+
+  release:
+    runs-on: ubuntu-latest
+    needs: test
+    if: startsWith(github.ref, 'refs/tags/')
+
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: '3.11'
+    - name: Install dependencies
+      shell: bash
+      run: |
+        python -m pip install --upgrade pip
+        pip install hatch
+    - name: Build and publish on PyPI
+      env:
+        HATCH_INDEX_USER: ${{ secrets.HATCH_INDEX_USER }}
+        HATCH_INDEX_AUTH: ${{ secrets.HATCH_INDEX_AUTH }}
+      run: |
+        hatch build
+        hatch publish
+    - name: Create release
+      uses: ncipollo/release-action@v1
+      with:
+        draft: true
+        body: ${{ github.event.head_commit.message }}
+        artifacts: dist/*.whl,dist/*.tar.gz
+        token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `mknodes-0.2.0/.github/workflows/documentation.yml` & `mknodes-0.3.2/.github/workflows/documentation.yml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-name: Build documentation
-
-on:
-  push:
-    branches:
-      - main
-
-# Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
-permissions:
-  contents: read
-  pages: write
-  id-token: write
-
-# Allow one concurrent deployment
-concurrency:
-  group: "pages"
-  cancel-in-progress: true
-
-# Default to bash
-defaults:
-  run:
-    shell: bash
-
-jobs:
-  build:
-
-    runs-on: ubuntu-latest
-
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install hatch
-        hatch env create
-    - name: Build
-      run: hatch run docs-build
-    - name: Upload artifact
-      uses: actions/upload-pages-artifact@v1
-      with:
-        path: ./site
-
-  deploy:
-    environment:
-      name: github-pages
-      url: ${{ steps.deployment.outputs.page_url }}
-    runs-on: ubuntu-latest
-    needs: build
-    steps:
-      - name: Deploy to GitHub Pages
-        id: deployment
-        uses: actions/deploy-pages@v1
+name: Build documentation
+
+on:
+  push:
+    branches:
+      - main
+
+# Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
+permissions:
+  contents: read
+  pages: write
+  id-token: write
+
+# Allow one concurrent deployment
+concurrency:
+  group: "pages"
+  cancel-in-progress: true
+
+# Default to bash
+defaults:
+  run:
+    shell: bash
+
+jobs:
+  build:
+
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: '3.11'
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install hatch
+        hatch env create
+    - name: Build
+      run: hatch run docs-build
+    - name: Upload artifact
+      uses: actions/upload-pages-artifact@v1
+      with:
+        path: ./site
+
+  deploy:
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+    runs-on: ubuntu-latest
+    needs: build
+    steps:
+      - name: Deploy to GitHub Pages
+        id: deployment
+        uses: actions/deploy-pages@v1
```

### Comparing `mknodes-0.2.0/docs/gen_pages.py` & `mknodes-0.3.2/docs/gen_pages.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""Generate the code reference pages and navigation."""
-
-from __future__ import annotations
-
-import pathlib
-
-import mknodes
-from mknodes import manual
-
-
-HEADER = "Don't write docs. Code them."
-WARNING = "This is all very alpha and subject to change."
-FOOTER = """Thats it. We created a website without touching any .md file
-and without having to care about file paths at at all.
-Now check out what we have created!
-"""
-
-# this Nav object is basically the root of everything. It corresponds tou your root
-# SUMMARY.md.
-
-root_nav = mknodes.MkNav()
-
-# Let's begin with the start page. This is your index.md file.
-page = root_nav.add_index_page(hide_toc=True, hide_nav=True)
-
-# The next 6 lines are generating the page you are looking at right now.
-page.add_header(HEADER, level=3)
-page.add_admonition(WARNING, typ="danger", title="Warning!")
-page += "This is the source code for building this website:"
-code = pathlib.Path(__file__).read_text()
-page.add_code(code)
-page += FOOTER
-
-# now we will create the nav section and its pages one by one.
-manual.create_page_1(root_nav)
-manual.create_page_2(root_nav)
-manual.create_page_3(root_nav)
-
-
-# This call will write everything we have done to a virtual folder
-# (powered by mkgen-pages)
-root_nav.write()
+"""Generate the code reference pages and navigation."""
+
+from __future__ import annotations
+
+import pathlib
+
+import mknodes
+from mknodes import manual
+
+
+HEADER = "Don't write docs. Code them."
+WARNING = "This is all very alpha and subject to change."
+FOOTER = """Thats it. We created a website without touching any .md file
+and without having to care about file paths at at all.
+Now check out what we have created!
+"""
+
+# this Nav object is basically the root of everything. It corresponds tou your root
+# SUMMARY.md.
+
+root_nav = mknodes.MkNav()
+
+# Let's begin with the start page. This is your index.md file.
+page = root_nav.add_index_page(hide_toc=True, hide_nav=True)
+
+# The next 6 lines are generating the page you are looking at right now.
+page.add_header(HEADER, level=3)
+page.add_admonition(WARNING, typ="danger", title="Warning!")
+page += "This is the source code for building this website:"
+code = pathlib.Path(__file__).read_text()
+page.add_code(code)
+page += FOOTER
+
+# now we will create the nav section and its pages one by one.
+manual.create_page_1(root_nav)
+manual.create_page_2(root_nav)
+manual.create_page_3(root_nav)
+
+
+# This call will write everything we have done to a virtual folder
+# (powered by mkgen-pages)
+root_nav.write()
```

### Comparing `mknodes-0.2.0/docs/gen_qt.py` & `mknodes-0.3.2/docs/gen_qt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""Generate the code reference pages and navigation."""
-
-from __future__ import annotations
-
-import prettyqt
-import mknodes
-
-prettyqt.import_all()
-
-QT_MODULE_ATTR = "QT_MODULE"
-
-root_nav = mknodes.MkNav()
-page = mknodes.MkPage(path="index.md", hide_toc=True, hide_nav=True)
-page.add_header("Not in the mood to write documentation? Let´s code it then!", level=3)
-page.write()
-
-qt_docs = root_nav.add_documentation(prettyqt, section_name="Qt modules")
-extra_docs = root_nav.add_documentation(prettyqt, section_name="Additional modules")
-
-for submod in qt_docs.iter_modules(predicate=lambda x: hasattr(x, QT_MODULE_ATTR)):
-    subdoc = qt_docs.add_documentation(submod)
-    subdoc.add_module_overview()
-    for klass in subdoc.iter_classes():
-        subdoc.add_class_page(klass=klass, flatten=True)
-for submod in extra_docs.iter_modules(predicate=lambda x: not hasattr(x, QT_MODULE_ATTR)):
-    subdoc = extra_docs.add_documentation(submod)
-    subdoc.add_module_overview()
-    for klass in subdoc.iter_classes():
-        subdoc.add_class_page(klass=klass, flatten=True)
-
-
-# root_nav.pretty_print()
-root_nav.write()  # Finally, we write the whole tree.
+"""Generate the code reference pages and navigation."""
+
+from __future__ import annotations
+
+import prettyqt
+import mknodes
+
+prettyqt.import_all()
+
+QT_MODULE_ATTR = "QT_MODULE"
+
+root_nav = mknodes.MkNav()
+page = root_nav.add_index_page(hide_toc=True, hide_nav=True)
+page.add_header("Not in the mood to write documentation? Let´s code it then!", level=3)
+
+qt_docs = root_nav.add_doc(prettyqt, section_name="Qt modules")
+extra_docs = root_nav.add_doc(prettyqt, section_name="Additional modules")
+
+for submod in qt_docs.iter_modules(predicate=lambda x: hasattr(x, QT_MODULE_ATTR)):
+    subdoc = qt_docs.add_doc(submod)
+    subdoc.add_module_overview()
+    for klass in subdoc.iter_classes():
+        subdoc.add_class_page(klass=klass, flatten=True)
+for submod in extra_docs.iter_modules(predicate=lambda x: not hasattr(x, QT_MODULE_ATTR)):
+    subdoc = extra_docs.add_doc(submod)
+    subdoc.add_module_overview()
+    for klass in subdoc.iter_classes():
+        subdoc.add_class_page(klass=klass, flatten=True)
+
+
+# root_nav.pretty_print()
+root_nav.write()  # Finally, we write the whole tree.
```

### Comparing `mknodes-0.2.0/mknodes/__init__.py` & `mknodes-0.3.2/mknodes/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-from __future__ import annotations
-
-from .mkadmonition import MkAdmonition
-from .mknode import MkNode
-from .mktext import MkText
-from .mkcontainer import MkContainer
-from .mkcode import MkCode
-from .mkdocstrings import MkDocStrings
-from .mkimage import MkImage
-from .mkbinaryimage import MkBinaryImage
-from .mklist import MkList
-from .mkdiagram import MkDiagram
-from .mktable import MkTable
-from .mktabs import MkTabBlock, MkTabbed
-from .mksnippet import MkSnippet
-from .mkcritic import MkCritic
-from .mksourceandresult import MkSourceAndResult
-from .mkshields import MkShields
-from .mkpageinclude import MkPageInclude
-
-from .mkclassdiagram import MkClassDiagram
-
-from .mkbaseclasstable import MkBaseClassTable
-from .mkclasstable import MkClassTable
-from .mkmoduletable import MkModuleTable
-
-from .mkpage import MkPage
-from .mkclasspage import MkClassPage
-from .mkmodulepage import MkModulePage
-
-from .mknav import MkNav
-from .mkdoc import MkDoc
-
-
-__all__ = [
-    "MkNode",
-    "MkContainer",
-    "MkNav",
-    "MkDocStrings",
-    "MkText",
-    "MkCode",
-    "MkImage",
-    "MkBinaryImage",
-    "MkPage",
-    "MkAdmonition",
-    "MkDiagram",
-    "MkClassDiagram",
-    "ConnectionBuilder",
-    "MkTable",
-    "MkBaseClassTable",
-    "MkClassTable",
-    "MkList",
-    "MkClassPage",
-    "MkModulePage",
-    "MkModuleTable",
-    "MkDoc",
-    "MkTabBlock",
-    "MkTabbed",
-    "MkSourceAndResult",
-    "MkSnippet",
-    "MkShields",
-    "MkPageInclude",
-    "MkCritic",
-]
-
-__version__ = "0.2.0"
+from __future__ import annotations
+
+from .mkblock import MkBlock
+from .mkadmonition import MkAdmonition
+from .mknode import MkNode
+from .mktext import MkText
+from .mkcontainer import MkContainer
+from .mkcode import MkCode
+from .mkdocstrings import MkDocStrings
+from .mkimage import MkImage
+from .mkbinaryimage import MkBinaryImage
+from .mklist import MkList
+from .mkdiagram import MkDiagram
+from .mktable import MkTable
+from .mktabcontainer import MkTabBlock, MkTabbed
+from .mksnippet import MkSnippet
+from .mkcritic import MkCritic
+from .mksourceandresult import MkSourceAndResult
+from .mkshields import MkShields
+from .mkpage import MkPage
+from .mkpageinclude import MkPageInclude
+
+from .classnodes.mkclassdiagram import MkClassDiagram
+from .classnodes.mkbaseclasstable import MkBaseClassTable
+from .classnodes.mkclasstable import MkClassTable
+from .classnodes.mkclasspage import MkClassPage
+
+from .modulenodes.mkmoduletable import MkModuleTable
+from .modulenodes.mkmodulepage import MkModulePage
+
+
+from .mknav import MkNav
+from .mkdoc import MkDoc
+
+
+__all__ = [
+    "MkNode",
+    "MkBlock",
+    "MkContainer",
+    "MkNav",
+    "MkDocStrings",
+    "MkText",
+    "MkCode",
+    "MkImage",
+    "MkBinaryImage",
+    "MkPage",
+    "MkAdmonition",
+    "MkDiagram",
+    "MkClassDiagram",
+    "ConnectionBuilder",
+    "MkTable",
+    "MkBaseClassTable",
+    "MkClassTable",
+    "MkList",
+    "MkClassPage",
+    "MkModulePage",
+    "MkModuleTable",
+    "MkDoc",
+    "MkTabBlock",
+    "MkTabbed",
+    "MkSourceAndResult",
+    "MkSnippet",
+    "MkShields",
+    "MkPageInclude",
+    "MkCritic",
+]
+
+__version__ = "0.3.2"
```

### Comparing `mknodes-0.2.0/mknodes/classhelpers.py` & `mknodes-0.3.2/mknodes/utils/classhelpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,185 @@
-from __future__ import annotations
-
-from collections.abc import Iterator, Sequence
-import contextlib
-import importlib
-import inspect
-import logging
-import pathlib
-import types
-import typing
-
-
-T = typing.TypeVar("T", bound=type)
-
-
-logger = logging.getLogger(__name__)
-
-
-def get_subclasses(klass: type, include_abstract: bool = False) -> typing.Iterator[type]:
-    """Recursively iter all subclasses of given klass.
-
-    Arguments:
-        klass: class to get subclasses from
-        include_abstract: whether abstract base classes should be included.
-    """
-    if getattr(klass.__subclasses__, "__self__", None) is None:
-        return
-    for i in klass.__subclasses__():
-        yield from get_subclasses(i)
-        if include_abstract or not inspect.isabstract(i):
-            yield i
-
-
-def to_module(
-    module: str | Sequence[str] | types.ModuleType,
-    return_none: bool = True,
-) -> types.ModuleType | None:
-    """Returns a module for given module path. If module is given, just return it.
-
-    Arguments:
-        module: A ModuleType, str or sequence.
-        return_none: In case module cant get imported, return None.
-                     If False, Exception is thrown.
-    """
-    match module:
-        case (str(), *_) | str():
-            module_path = module if isinstance(module, str) else ".".join(module)
-            try:
-                return importlib.import_module(module_path)
-            except (ImportError, AttributeError) as e:
-                logger.warning(f"Could not import {module_path!r}")
-                if return_none:
-                    return None
-                raise ImportError from e
-        case types.ModuleType():
-            return module
-        case _:
-            raise TypeError(module)
-
-
-def to_class(klass: type | str | tuple[str, ...] | list[str]):
-    match klass:
-        case type():
-            return klass
-        case str():
-            parts = klass.split(".")
-            mod = importlib.import_module(".".join(parts[:-1]))
-            return getattr(mod, parts[-1])
-        case tuple() | list():
-            mod = importlib.import_module(".".join(klass[:-1]))
-            return getattr(mod, klass[-1])
-        case _:
-            raise TypeError(klass)
-
-
-def to_module_parts(  # type: ignore
-    module: Sequence[str] | str | types.ModuleType,
-) -> tuple[str, ...]:
-    """Returns a tuple describing the module path.
-
-    Result is of form ("module", "submodule", "subsubmodule")
-
-    Arguments:
-        module: A ModuleType, str or sequence.
-    """
-    match module:
-        case (str(), *_):
-            return tuple(module)
-        case str():
-            return tuple(module.split("."))
-        case types.ModuleType():
-            return tuple(module.__name__.split("."))
-        case pathlib.Path() if not module.is_absolute():
-            return module.parts
-        case _:
-            raise TypeError(module)
-
-
-def iter_classes(
-    module: types.ModuleType | str | tuple[str],
-    *,
-    type_filter: type | None | types.UnionType = None,
-    module_filter: str | None = None,
-    filter_by___all__: bool = False,
-    recursive: bool = False,
-) -> Iterator[type]:
-    """Yield classes from given module.
-
-    Arguments:
-        module: either a module or a path to a module in form of str or
-                tuple of strings.
-        type_filter: only yield classes which are subclasses of given type.
-        module_filter: filter by a module prefix.
-        filter_by___all__: Whether to filter based on whats defined in __all__.
-        recursive: import all submodules recursively and also yield their classes.
-    """
-    mod = to_module(module)
-    if not mod:
-        return []
-    if recursive:
-        for _name, submod in inspect.getmembers(mod, inspect.ismodule):
-            if submod.__name__.startswith(module_filter or ""):
-                yield from iter_classes(
-                    submod,
-                    type_filter=type_filter,
-                    module_filter=submod.__name__,
-                    filter_by___all__=filter_by___all__,
-                    recursive=True,
-                )
-    for klass_name, kls in inspect.getmembers(mod, inspect.isclass):
-        has_all = hasattr(mod, "__all__")
-        if filter_by___all__ and (not has_all or klass_name not in mod.__all__):
-            continue
-        if type_filter is not None and not issubclass(kls, type_filter):
-            continue
-        if module_filter is not None and not kls.__module__.startswith(module_filter):
-            continue
-        yield kls
-
-
-def get_topmost_module_path(obj: type | types.FunctionType | types.MethodType) -> str:
-    """Return path of topmost module containing given class.
-
-    If a class is imported in any of its parent modules, return that "shorter" path.
-
-    So for a class "submodule.classmodule.Class", it could return "submodule.Class"
-
-    Arguments:
-        obj: Klass to get the path for.
-    """
-    path = obj.__module__
-    match obj:
-        case type():
-            fn = inspect.isclass
-        case types.MethodType():
-            fn = inspect.ismethod
-        case types.FunctionType():
-            fn = inspect.isfunction
-    parts = path.split(".")
-    while parts:
-        with contextlib.suppress(TypeError):
-            new_path = ".".join(parts)
-            mod = importlib.import_module(new_path)
-            objs = [i for _i_name, i in inspect.getmembers(mod, fn)]
-            if obj in objs:
-                path = new_path
-        parts = parts[:-1]
-    return path
-
-
-if __name__ == "__main__":
-    from prettyqt import widgets
-
-    path = iter_classes(widgets, recursive=False)
-    print(len(list(path)))
+from __future__ import annotations
+
+from collections.abc import Iterator, Sequence
+import contextlib
+import importlib
+import inspect
+import logging
+import pathlib
+import types
+import typing
+
+
+T = typing.TypeVar("T", bound=type)
+
+
+logger = logging.getLogger(__name__)
+
+
+def get_subclasses(klass: type, include_abstract: bool = False) -> typing.Iterator[type]:
+    """Recursively iter all subclasses of given klass.
+
+    Arguments:
+        klass: class to get subclasses from
+        include_abstract: whether abstract base classes should be included.
+    """
+    if getattr(klass.__subclasses__, "__self__", None) is None:
+        return
+    for i in klass.__subclasses__():
+        yield from get_subclasses(i)
+        if include_abstract or not inspect.isabstract(i):
+            yield i
+
+
+@typing.overload
+def to_module(module, return_none: typing.Literal[False] = ...) -> types.ModuleType:
+    ...
+
+
+@typing.overload
+def to_module(module, return_none: typing.Literal[True] = ...) -> types.ModuleType | None:
+    ...
+
+
+def to_module(
+    module: str | Sequence[str] | types.ModuleType,
+    return_none: bool = True,
+) -> types.ModuleType | None:
+    """Returns a module for given module path. If module is given, just return it.
+
+    Arguments:
+        module: A ModuleType, str or sequence.
+        return_none: In case module cant get imported, return None.
+                     If False, Exception is thrown.
+    """
+    match module:
+        case (str(), *_) | str():
+            module_path = module if isinstance(module, str) else ".".join(module)
+            try:
+                return importlib.import_module(module_path)
+            except (ImportError, AttributeError) as e:
+                logger.warning("Could not import %s", module_path)
+                if return_none:
+                    return None
+                raise ImportError from e
+        case types.ModuleType():
+            return module
+        case _:
+            raise TypeError(module)
+
+
+def to_class(klass: type | str | tuple[str, ...] | list[str]):
+    match klass:
+        case type():
+            return klass
+        case str():
+            parts = klass.split(".")
+            mod = importlib.import_module(".".join(parts[:-1]))
+            return getattr(mod, parts[-1])
+        case tuple() | list():
+            mod = importlib.import_module(".".join(klass[:-1]))
+            return getattr(mod, klass[-1])
+        case _:
+            raise TypeError(klass)
+
+
+def to_module_parts(  # type: ignore
+    module: Sequence[str] | str | types.ModuleType,
+) -> tuple[str, ...]:
+    """Returns a tuple describing the module path.
+
+    Result is of form ("module", "submodule", "subsubmodule")
+
+    Arguments:
+        module: A ModuleType, str or sequence.
+    """
+    match module:
+        case (str(), *_):
+            return tuple(module)
+        case str():
+            return tuple(module.split("."))
+        case types.ModuleType():
+            return tuple(module.__name__.split("."))
+        case pathlib.Path() if not module.is_absolute():
+            return module.parts
+        case _:
+            raise TypeError(module)
+
+
+def iter_classes(
+    module: types.ModuleType | str | tuple[str],
+    *,
+    type_filter: type | None | types.UnionType = None,
+    module_filter: str | None = None,
+    filter_by___all__: bool = False,
+    recursive: bool = False,
+) -> Iterator[type]:
+    """Yield classes from given module.
+
+    Arguments:
+        module: either a module or a path to a module in form of str or
+                tuple of strings.
+        type_filter: only yield classes which are subclasses of given type.
+        module_filter: filter by a module prefix.
+        filter_by___all__: Whether to filter based on whats defined in __all__.
+        recursive: import all submodules recursively and also yield their classes.
+    """
+    mod = to_module(module)
+    if not mod:
+        return []
+    if recursive:
+        for _name, submod in inspect.getmembers(mod, inspect.ismodule):
+            if submod.__name__.startswith(module_filter or ""):
+                yield from iter_classes(
+                    submod,
+                    type_filter=type_filter,
+                    module_filter=submod.__name__,
+                    filter_by___all__=filter_by___all__,
+                    recursive=True,
+                )
+    for klass_name, kls in inspect.getmembers(mod, inspect.isclass):
+        has_all = hasattr(mod, "__all__")
+        if filter_by___all__ and (not has_all or klass_name not in mod.__all__):
+            continue
+        if type_filter is not None and not issubclass(kls, type_filter):
+            continue
+        if module_filter is not None and not kls.__module__.startswith(module_filter):
+            continue
+        yield kls
+
+
+def get_topmost_module_path(obj: type | types.FunctionType | types.MethodType) -> str:
+    """Return path of topmost module containing given class.
+
+    If a class is imported in any of its parent modules, return that "shorter" path.
+
+    So for a class "submodule.classmodule.Class", it could return "submodule.Class"
+
+    Arguments:
+        obj: Klass to get the path for.
+    """
+    path = obj.__module__
+    match obj:
+        case type():
+            fn = inspect.isclass
+        case types.MethodType():
+            fn = inspect.ismethod
+        case types.FunctionType():
+            fn = inspect.isfunction
+    parts = path.split(".")
+    while parts:
+        with contextlib.suppress(TypeError):
+            new_path = ".".join(parts)
+            mod = importlib.import_module(new_path)
+            objs = [i for _i_name, i in inspect.getmembers(mod, fn)]
+            if obj in objs:
+                path = new_path
+        parts = parts[:-1]
+    return path
+
+
+if __name__ == "__main__":
+    from prettyqt import widgets
+
+    path = iter_classes(widgets, recursive=False)
+    print(len(list(path)))
```

### Comparing `mknodes-0.2.0/mknodes/connectionbuilder.py` & `mknodes-0.3.2/mknodes/utils/connectionbuilder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from __future__ import annotations
-
-import logging
-import textwrap
-
-
-logger = logging.getLogger(__name__)
-
-
-class ConnectionBuilder:
-    def __init__(self, objects):
-        if not isinstance(objects, list | tuple):
-            objects = [objects]
-        self.item_dict = {}
-        self.connections = []
-        self._connect(objects)
-
-    def _connect(self, objects):
-        def add_connections(item):
-            identifier = self.get_id(item)
-            if identifier not in self.item_dict:
-                # if item.__module__.startswith(base_module):
-                self.item_dict[identifier] = self.get_title(item)
-                for base in self.get_children(item):
-                    self.connections.append((self.get_id(base), identifier))
-                    add_connections(base)
-
-        for obj in objects:
-            add_connections(obj)
-
-    @property
-    def items(self):
-        return list(self.item_dict.keys())
-
-    @property
-    def titles(self):
-        return list(self.item_dict.values())
-
-    def get_children(self, item):
-        """This should return a list of children for the tree node."""
-        return NotImplemented
-
-    def get_id(self, item):
-        """This needs to return a unique identifier for an item."""
-        return item
-
-    def get_attributes(self, item):
-        return None
-
-    def get_title(self, item):
-        """This can be overridden for a nicer label."""
-        return self.get_id(item)
-
-    def get_graph_connection_text(self):
-        lines = [
-            f'{identifier}["{title}"]'
-            for identifier, title in zip(self.items, self.titles)
-        ]
-        lines += [f"{a} --> {b}" for a, b in self.connections]
-        return textwrap.indent("\n".join(lines), "  ")
-
-
-if __name__ == "__main__":
-
-    class Test(ConnectionBuilder):
-        def get_children(self, item):
-            return item.__bases__
-
-    test = Test(ConnectionBuilder).get_graph_connection_text()
-    print(test)
+from __future__ import annotations
+
+import logging
+import textwrap
+
+
+logger = logging.getLogger(__name__)
+
+
+class ConnectionBuilder:
+    def __init__(self, objects):
+        if not isinstance(objects, list | tuple):
+            objects = [objects]
+        self.item_dict = {}
+        self.connections = []
+        self._connect(objects)
+
+    def _connect(self, objects):
+        def add_connections(item):
+            identifier = self.get_id(item)
+            if identifier not in self.item_dict:
+                # if item.__module__.startswith(base_module):
+                self.item_dict[identifier] = self.get_title(item)
+                for base in self.get_children(item):
+                    self.connections.append((self.get_id(base), identifier))
+                    add_connections(base)
+
+        for obj in objects:
+            add_connections(obj)
+
+    @property
+    def items(self):
+        return list(self.item_dict.keys())
+
+    @property
+    def titles(self):
+        return list(self.item_dict.values())
+
+    def get_children(self, item) -> list | tuple:
+        """This should return a list of children for the tree node."""
+        return NotImplemented
+
+    def get_id(self, item):
+        """This needs to return a unique identifier for an item."""
+        return item
+
+    def get_attributes(self, item):
+        return None
+
+    def get_title(self, item):
+        """This can be overridden for a nicer label."""
+        return self.get_id(item)
+
+    def get_graph_connection_text(self):
+        lines = [
+            f'{identifier}["{title}"]'
+            for identifier, title in zip(self.items, self.titles)
+        ]
+        lines += [f"{a} --> {b}" for a, b in self.connections]
+        return textwrap.indent("\n".join(lines), "  ")
+
+
+if __name__ == "__main__":
+
+    class Test(ConnectionBuilder):
+        def get_children(self, item):
+            return item.__bases__
+
+    test = Test(ConnectionBuilder).get_graph_connection_text()
+    print(test)
```

### Comparing `mknodes-0.2.0/mknodes/mermaid.py` & `mknodes-0.3.2/mknodes/utils/mermaid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from __future__ import annotations
-
-import dataclasses
-import logging
-
-
-logger = logging.getLogger(__name__)
-
-# Link are created following the documentation here :
-# https://mermaid.js.org/syntax/flowchart.html#links-between-nodes
-LINK_SHAPES = {"normal": "---", "dotted": "-.-", "thick": "==="}
-
-LINK_HEADS = {"none": "", "arrow": ">", "left-arrow": "<", "bullet": "o", "cross": "x"}
-
-
-@dataclasses.dataclass
-class NodeShape:
-    start: str
-    end: str
-
-
-# Shapes are created following the documentation here :
-# https://mermaid.js.org/syntax/flowchart.html#node-shapes
-
-
-NODE_SHAPES = {
-    "normal": NodeShape("[", "]"),
-    "round-edge": NodeShape("(", ")"),
-    "stadium-shape": NodeShape("([", "])"),
-    "subroutine-shape": NodeShape("[[", "]]"),
-    "cylindrical": NodeShape("[(", ")]"),
-    "circle": NodeShape("((", "))"),
-    "label-shape": NodeShape(">", "]"),
-    "rhombus": NodeShape("{", ")"),
-    "hexagon": NodeShape("{{", ")}"),
-    "parallelogram": NodeShape("[/", "/]"),
-    "parallelogram-alt": NodeShape("[\\", "\\]"),
-    "trapezoid": NodeShape("[/", "\\]"),
-    "trapezoid-alt": NodeShape("[\\", "/]"),
-    "double-circle": NodeShape("(((", ")))"),
-}
-
-
-class Node:
-    def __init__(
-        self,
-        identifier: str,
-        content: str = "",
-        shape: str = "normal",
-        sub_nodes: list = None,
-    ):
-        sub_nodes = sub_nodes or []
-        self.id = identifier  # helpers.to_snake(identifier)
-        self.content = content if content else self.id
-        self.shape = NODE_SHAPES[shape]
-        self.sub_nodes = sub_nodes
-
-        # TODO: verify that content match a working string pattern
-
-    def add_sub_nodes(self, new_nodes: list[Node] = None):
-        if new_nodes is None:
-            new_nodes = []
-        self.sub_nodes = self.sub_nodes + new_nodes
-
-    def __repr__(self):
-        return f"{self.id}['{self.content}'] Nb_children:{len(self.sub_nodes)}"
-
-    def __str__(self):
-        return "" + (
-            "\n".join(
-                [
-                    f'subgraph {self.id} ["{self.content}"]',
-                    "\n".join([str(node) for node in self.sub_nodes]),
-                    "end",
-                ]
-            )
-            if len(self.sub_nodes)
-            else "".join([self.id, self.shape.start, f'"{self.content}"', self.shape.end])
-        )
-
-
-class Link:
-    def __init__(
-        self,
-        origin: Node,
-        end: Node,
-        shape: str = "normal",
-        head_left: str = "none",
-        head_right: str = "arrow",
-        message: str = "",
-    ):
-        self.origin = origin
-        self.end = end
-        self.head_left = LINK_HEADS[head_left]
-        self.head_right = LINK_HEADS[head_right]
-        self.shape = LINK_SHAPES[shape]
-        self.message = message
-
-    def __str__(self):
-        elements = [
-            f"{self.origin.id} ",
-            self.head_left,
-            self.shape,
-            self.head_right,
-            f"|{self.message}|" if self.message else "",
-            f" {self.end.id}",
-        ]
-        return "".join(elements)
-
-
-if __name__ == "__main__":
-    pass
+from __future__ import annotations
+
+import dataclasses
+import logging
+
+
+logger = logging.getLogger(__name__)
+
+# Link are created following the documentation here :
+# https://mermaid.js.org/syntax/flowchart.html#links-between-nodes
+LINK_SHAPES = {"normal": "---", "dotted": "-.-", "thick": "==="}
+
+LINK_HEADS = {"none": "", "arrow": ">", "left-arrow": "<", "bullet": "o", "cross": "x"}
+
+
+@dataclasses.dataclass
+class NodeShape:
+    start: str
+    end: str
+
+
+# Shapes are created following the documentation here :
+# https://mermaid.js.org/syntax/flowchart.html#node-shapes
+
+
+NODE_SHAPES = {
+    "normal": NodeShape("[", "]"),
+    "round-edge": NodeShape("(", ")"),
+    "stadium-shape": NodeShape("([", "])"),
+    "subroutine-shape": NodeShape("[[", "]]"),
+    "cylindrical": NodeShape("[(", ")]"),
+    "circle": NodeShape("((", "))"),
+    "label-shape": NodeShape(">", "]"),
+    "rhombus": NodeShape("{", ")"),
+    "hexagon": NodeShape("{{", ")}"),
+    "parallelogram": NodeShape("[/", "/]"),
+    "parallelogram-alt": NodeShape("[\\", "\\]"),
+    "trapezoid": NodeShape("[/", "\\]"),
+    "trapezoid-alt": NodeShape("[\\", "/]"),
+    "double-circle": NodeShape("(((", ")))"),
+}
+
+
+class Node:
+    def __init__(
+        self,
+        identifier: str,
+        content: str = "",
+        shape: str = "normal",
+        sub_nodes: list = None,
+    ):
+        sub_nodes = sub_nodes or []
+        self.id = identifier  # helpers.to_snake(identifier)
+        self.content = content if content else self.id
+        self.shape = NODE_SHAPES[shape]
+        self.sub_nodes = sub_nodes
+
+        # TODO: verify that content match a working string pattern
+
+    def add_sub_nodes(self, new_nodes: list[Node] = None):
+        if new_nodes is None:
+            new_nodes = []
+        self.sub_nodes = self.sub_nodes + new_nodes
+
+    def __repr__(self):
+        return f"{self.id}['{self.content}'] Nb_children:{len(self.sub_nodes)}"
+
+    def __str__(self):
+        return "" + (
+            "\n".join(
+                [
+                    f'subgraph {self.id} ["{self.content}"]',
+                    "\n".join([str(node) for node in self.sub_nodes]),
+                    "end",
+                ],
+            )
+            if len(self.sub_nodes)
+            else "".join([self.id, self.shape.start, f'"{self.content}"', self.shape.end])
+        )
+
+
+class Link:
+    def __init__(
+        self,
+        origin: Node,
+        end: Node,
+        shape: str = "normal",
+        head_left: str = "none",
+        head_right: str = "arrow",
+        message: str = "",
+    ):
+        self.origin = origin
+        self.end = end
+        self.head_left = LINK_HEADS[head_left]
+        self.head_right = LINK_HEADS[head_right]
+        self.shape = LINK_SHAPES[shape]
+        self.message = message
+
+    def __str__(self):
+        elements = [
+            f"{self.origin.id} ",
+            self.head_left,
+            self.shape,
+            self.head_right,
+            f"|{self.message}|" if self.message else "",
+            f" {self.end.id}",
+        ]
+        return "".join(elements)
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `mknodes-0.2.0/mknodes/mkadmonition.py` & `mknodes-0.3.2/mknodes/mkadmonition.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from __future__ import annotations
-
-import logging
-import textwrap
-
-from typing import Literal
-
-from mknodes import mktext
-
-
-logger = logging.getLogger(__name__)
-
-AdmonitionTypeStr = Literal[
-    "node",
-    "abstract",
-    "info",
-    "tip",
-    "success",
-    "question",
-    "warning",
-    "failure",
-    "danger",
-    "bug",
-    "example",
-    "quote",
-]
-
-
-class MkAdmonition(mktext.MkText):
-    """Admonition info box."""
-
-    def __init__(
-        self,
-        text: str,
-        typ: AdmonitionTypeStr = "info",
-        *,
-        title: str | None = None,
-        collapsible: bool = False,
-        **kwargs,
-    ):
-        super().__init__(text=text, **kwargs)
-        self.typ = typ
-        self.title = title
-        self.collapsible = collapsible
-
-    def _to_markdown(self) -> str:
-        if not self.text:
-            return ""
-        block_start = "???" if self.collapsible else "!!!"
-        title = f'" {self.title}"' if self.title else ""
-        text = textwrap.indent(str(self.text), "    ")
-        return f"{block_start} {self.typ}{title}\n{text}\n"
-
-    @staticmethod
-    def examples():
-        for typ in [
-            "node",
-            "abstract",
-            "info",
-            "tip",
-            "success",
-            "question",
-            "warning",
-            "failure",
-            "danger",
-            "bug",
-            "example",
-            "quote",
-        ]:
-            yield dict(typ=typ, text=f"This is type {typ}", title=typ)
-        yield dict(typ="info", text="This is a collapsible menu", collapsible=True)
-
-
-if __name__ == "__main__":
-    admonition = MkAdmonition("")
-    print(admonition)
+from __future__ import annotations
+
+import logging
+import textwrap
+
+from typing import Literal
+
+from mknodes import mktext
+
+
+logger = logging.getLogger(__name__)
+
+AdmonitionTypeStr = Literal[
+    "node",
+    "abstract",
+    "info",
+    "tip",
+    "success",
+    "question",
+    "warning",
+    "failure",
+    "danger",
+    "bug",
+    "example",
+    "quote",
+]
+
+
+class MkAdmonition(mktext.MkText):
+    """Admonition info box."""
+
+    def __init__(
+        self,
+        text: str,
+        typ: AdmonitionTypeStr = "info",
+        *,
+        title: str | None = None,
+        collapsible: bool = False,
+        **kwargs,
+    ):
+        super().__init__(text=text, **kwargs)
+        self.typ = typ
+        self.title = title
+        self.collapsible = collapsible
+
+    def _to_markdown(self) -> str:
+        if not self.text:
+            return ""
+        block_start = "???" if self.collapsible else "!!!"
+        title = f' "{self.title}"' if self.title else ""
+        text = textwrap.indent(str(self.text), "    ")
+        return f"{block_start} {self.typ}{title}\n{text}\n"
+
+    @staticmethod
+    def examples():
+        for typ in [
+            "node",
+            "abstract",
+            "info",
+            "tip",
+            "success",
+            "question",
+            "warning",
+            "failure",
+            "danger",
+            "bug",
+            "example",
+            "quote",
+        ]:
+            yield dict(typ=typ, text=f"This is type {typ}", title=typ)
+        yield dict(typ="info", text="This is a collapsible menu", collapsible=True)
+
+
+if __name__ == "__main__":
+    admonition = MkAdmonition("")
+    print(admonition)
```

### Comparing `mknodes-0.2.0/mknodes/mkbaseclasstable.py` & `mknodes-0.3.2/mknodes/classnodes/mkbaseclasstable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,99 @@
-from __future__ import annotations
-
-from collections.abc import Callable
-import logging
-
-from typing import Literal
-
-from mknodes import mktable, utils
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkBaseClassTable(mktable.MkTable):
-    """Table showing info for a list of classes."""
-
-    def __init__(
-        self,
-        klasses: list[type],
-        *,
-        layout: Literal["compact", "extended"] = "extended",
-        filter_fn: Callable | None = None,
-        **kwargs,
-    ):
-        self.klasses = klasses
-        if filter_fn is None:
-
-            def always_true(_):
-                return True
-
-            self.filter_fn = always_true
-        else:
-            self.filter_fn = filter_fn
-        # STRIP_CODE = r"```[^\S\r\n]*[a-z]*\n.*?\n```"
-        # docs = [re.sub(STRIP_CODE, '', k.__module__, 0, re.DOTALL) for k in klasses]
-        match layout:
-            case "compact":
-                data = [self.default_row_for_klass(kls) for kls in klasses]
-            case "extended":
-                data = [self.extended_row_for_klass(kls) for kls in klasses]
-            case _:
-                raise ValueError(layout)
-
-        super().__init__(data=data, **kwargs)
-
-    def __repr__(self):
-        return utils.get_repr(self, klasses=self.klasses)
-
-    @staticmethod
-    def examples():
-        from mknodes import mknav
-
-        yield dict(klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav])
-        yield dict(
-            klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav], layout="extended"
-        )
-
-    def default_row_for_klass(self, kls: type) -> dict[str, str]:
-        return dict(
-            Class=utils.link_for_class(kls),
-            Module=kls.__module__,
-            Description=utils.get_first_doc_line(kls),
-        )
-
-    def extended_row_for_klass(
-        self, kls: type, shorten_lists_after: int = 10
-    ) -> dict[str, str]:
-        """Return a table row for given class.
-
-        Includes columns for child and parent classes including links.
-        """
-        subclasses = [subkls for subkls in kls.__subclasses__() if self.filter_fn(subkls)]
-        subclass_links = [utils.link_for_class(sub) for sub in subclasses]
-        subclass_str = utils.to_html_list(
-            subclass_links, shorten_after=shorten_lists_after
-        )
-        parents = kls.__bases__
-        parent_links = [utils.link_for_class(parent) for parent in parents]
-        parent_str = utils.to_html_list(parent_links, shorten_after=shorten_lists_after)
-        desc = utils.get_first_doc_line(kls, escape=True)
-        name = utils.link_for_class(kls, size=4, bold=True)
-        module = utils.styled(kls.__module__, size=1, recursive=True)
-        return dict(
-            Name=f"{name}<br>{module}<br>{desc}",
-            # Module=kls.__module__,
-            Children=subclass_str,
-            Inherits=parent_str,
-            # Description=desc,
-        )
-
-
-if __name__ == "__main__":
-    table = MkBaseClassTable(klasses=[mktable.MkTable], layout="extended")
-    print(table)
+from __future__ import annotations
+
+from collections.abc import Callable
+import logging
+
+from typing import Literal
+
+from mknodes import mktable
+from mknodes.utils import helpers
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkBaseClassTable(mktable.MkTable):
+    """Table showing info for a list of classes."""
+
+    def __init__(
+        self,
+        klasses: list[type],
+        *,
+        layout: Literal["compact", "extended"] = "extended",
+        filter_fn: Callable | None = None,
+        **kwargs,
+    ):
+        self.klasses = klasses
+        if filter_fn is None:
+
+            def always_true(_):
+                return True
+
+            self.filter_fn = always_true
+        else:
+            self.filter_fn = filter_fn
+        # STRIP_CODE = r"```[^\S\r\n]*[a-z]*\n.*?\n```"
+        # docs = [re.sub(STRIP_CODE, '', k.__module__, 0, re.DOTALL) for k in klasses]
+        match layout:
+            case "compact":
+                data = [self.default_row_for_klass(kls) for kls in klasses]
+            case "extended":
+                data = [self.extended_row_for_klass(kls) for kls in klasses]
+            case _:
+                raise ValueError(layout)
+
+        super().__init__(data=data, **kwargs)
+
+    def __repr__(self):
+        return helpers.get_repr(self, klasses=self.klasses)
+
+    @staticmethod
+    def examples():
+        from mknodes import mknav
+
+        yield dict(klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav])
+        yield dict(
+            klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav],
+            layout="extended",
+        )
+
+    def default_row_for_klass(self, kls: type) -> dict[str, str]:
+        return dict(
+            Class=helpers.link_for_class(kls),
+            Module=kls.__module__,
+            Description=helpers.get_first_doc_line(kls),
+        )
+
+    def extended_row_for_klass(
+        self,
+        kls: type,
+        shorten_lists_after: int = 10,
+    ) -> dict[str, str]:
+        """Return a table row for given class.
+
+        Includes columns for child and parent classes including links.
+        """
+        subclasses = [subkls for subkls in kls.__subclasses__() if self.filter_fn(subkls)]
+        subclass_links = [helpers.link_for_class(sub) for sub in subclasses]
+        subclass_str = helpers.to_html_list(
+            subclass_links,
+            shorten_after=shorten_lists_after,
+        )
+        parents = kls.__bases__
+        parent_links = [helpers.link_for_class(parent) for parent in parents]
+        parent_str = helpers.to_html_list(parent_links, shorten_after=shorten_lists_after)
+        desc = helpers.get_first_doc_line(kls, escape=True)
+        name = helpers.link_for_class(kls, size=4, bold=True)
+        module = helpers.styled(kls.__module__, size=1, recursive=True)
+        return dict(
+            Name=f"{name}<br>{module}<br>{desc}",
+            # Module=kls.__module__,
+            Children=subclass_str,
+            Inherits=parent_str,
+            # Description=desc,
+        )
+
+
+if __name__ == "__main__":
+    table = MkBaseClassTable(klasses=[mktable.MkTable], layout="extended")
+    print(table)
```

### Comparing `mknodes-0.2.0/mknodes/mkclassdiagram.py` & `mknodes-0.3.2/mknodes/classnodes/mkclassdiagram.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,115 @@
-from __future__ import annotations
-
-import itertools
-
-from typing import Literal
-
-from mknodes import connectionbuilder, mkdiagram, utils
-
-
-DiagramModeStr = Literal["parent_tree", "subclass_tree", "mro"]
-
-
-class BaseClassConnectionBuilder(connectionbuilder.ConnectionBuilder):
-    def __init__(
-        self,
-        objects,
-        *,
-        title_style: Literal["package.classname", "qualname"] = "package.classname",
-    ):
-        self.title_style = title_style
-        # self.object = objects[0]
-        super().__init__(objects)
-
-    def get_id(self, item: type) -> int:
-        return id(item)
-
-    def get_title(self, item: type) -> str:
-        return (
-            utils.label_for_class(item)
-            if self.title_style == "package.classname"
-            else item.__qualname__
-        )
-        # if item.__module__.split(".")[0] == self.object.__module__.split(".")[0]:
-        #     return f"**{text}**"
-        # else:
-        #     return text
-
-    def get_attributes(self, item) -> list[str]:
-        return [i for i in dir(item) if not i.startswith("__")]
-
-
-class SubclassConnectionBuilder(BaseClassConnectionBuilder):
-    def _connect(self, objects):
-        super()._connect(objects)
-        self.connections = [(i[1], i[0]) for i in self.connections]
-
-    def get_children(self, item: type) -> list[type]:
-        return item.__subclasses__()
-
-
-class ParentClassConnectionBuilder(BaseClassConnectionBuilder):
-    def get_children(self, item: type) -> tuple[type, ...]:
-        return item.__bases__
-
-
-class MroConnectionBuilder(BaseClassConnectionBuilder):
-    def _connect(self, objects):
-        mro = list(objects[0].mro())
-        self.item_dict = {self.get_id(kls): self.get_title(kls) for kls in mro}
-        self.connections = [
-            (self.get_id(i), self.get_id(j)) for i, j in itertools.pairwise(mro)
-        ]
-
-
-class MkClassDiagram(mkdiagram.MkDiagram):
-    """Class diagram with several modes."""
-
-    def __init__(
-        self,
-        klass: type,
-        mode: DiagramModeStr = "parent_tree",
-        **kwargs,
-    ):
-        self.klass = klass
-        self.mode = mode
-        super().__init__(graph_type="flow", **kwargs)
-
-    def __repr__(self):
-        return utils.get_repr(
-            self,
-            klass=self.klass,
-            mode=self.mode,
-            orientation=self.orientation,
-        )
-
-    @staticmethod
-    def examples():
-        yield dict(klass=MkClassDiagram)
-
-    def _to_markdown(self) -> str:
-        match self.mode:
-            case "subclass_tree":
-                builder = SubclassConnectionBuilder(self.klass)
-                item_str = builder.get_graph_connection_text()
-            case "parent_tree":
-                builder = ParentClassConnectionBuilder(self.klass)
-                item_str = builder.get_graph_connection_text()
-            case "mro":
-                builder = MroConnectionBuilder(self.klass)
-                item_str = builder.get_graph_connection_text()
-            case _:
-                raise ValueError(self.mode)
-        text = f"{self.graph_type} {self.orientation}\n{item_str}"
-        return f"```mermaid\n{text}\n```"
-
-
-if __name__ == "__main__":
-    diagram = MkClassDiagram(MkClassDiagram, mode="mro")
-    print(diagram)
+from __future__ import annotations
+
+import itertools
+
+from typing import Literal
+
+from mknodes import mkdiagram
+from mknodes.utils import connectionbuilder, helpers
+
+
+DiagramModeStr = Literal["parent_tree", "subclass_tree", "mro"]
+
+
+class BaseClassConnectionBuilder(connectionbuilder.ConnectionBuilder):
+    def __init__(
+        self,
+        objects,
+        *,
+        title_style: Literal["package.classname", "qualname"] = "package.classname",
+    ):
+        self.title_style = title_style
+        # self.object = objects[0]
+        super().__init__(objects)
+
+    def get_id(self, item: type) -> int:
+        return id(item)
+
+    def get_title(self, item: type) -> str:
+        return (
+            helpers.label_for_class(item)
+            if self.title_style == "package.classname"
+            else item.__qualname__
+        )
+        # if item.__module__.split(".")[0] == self.object.__module__.split(".")[0]:
+        #     return f"**{text}**"
+        # else:
+        #     return text
+
+    def get_attributes(self, item) -> list[str]:
+        return [i for i in dir(item) if not i.startswith("__")]
+
+
+class SubclassConnectionBuilder(BaseClassConnectionBuilder):
+    def _connect(self, objects):
+        super()._connect(objects)
+        self.connections = [(i[1], i[0]) for i in self.connections]
+
+    def get_children(self, item: type) -> list[type]:
+        return item.__subclasses__()
+
+
+class ParentClassConnectionBuilder(BaseClassConnectionBuilder):
+    def get_children(self, item: type) -> tuple[type, ...]:
+        return item.__bases__
+
+
+class MroConnectionBuilder(BaseClassConnectionBuilder):
+    def _connect(self, objects):
+        mro = list(objects[0].mro())
+        self.item_dict = {self.get_id(kls): self.get_title(kls) for kls in mro}
+        self.connections = [
+            (self.get_id(i), self.get_id(j)) for i, j in itertools.pairwise(mro)
+        ]
+
+
+class MkClassDiagram(mkdiagram.MkDiagram):
+    """Class diagram with several modes."""
+
+    def __init__(
+        self,
+        klass: type,
+        mode: DiagramModeStr = "parent_tree",
+        orientation: Literal["TD", "DT", "LR", "RL"] = "TD",
+        header: str = "",
+    ):
+        self.klass = klass
+        self.mode = mode
+        super().__init__(
+            graph_type="flow",
+            orientation=orientation,
+            header=header,
+        )
+
+    def __repr__(self):
+        return helpers.get_repr(
+            self,
+            klass=self.klass,
+            mode=self.mode,
+            orientation=self.orientation,
+        )
+
+    @staticmethod
+    def examples():
+        yield dict(klass=MkClassDiagram)
+
+    def _to_markdown(self) -> str:
+        match self.mode:
+            case "subclass_tree":
+                builder = SubclassConnectionBuilder(self.klass)
+                item_str = builder.get_graph_connection_text()
+            case "parent_tree":
+                builder = ParentClassConnectionBuilder(self.klass)
+                item_str = builder.get_graph_connection_text()
+            case "mro":
+                builder = MroConnectionBuilder(self.klass)
+                item_str = builder.get_graph_connection_text()
+            case _:
+                raise ValueError(self.mode)
+        text = f"{self.graph_type} {self.orientation}\n{item_str}"
+        return f"```mermaid\n{text}\n```"
+
+
+if __name__ == "__main__":
+    diagram = MkClassDiagram(MkClassDiagram, mode="mro")
+    print(diagram)
```

### Comparing `mknodes-0.2.0/mknodes/mkclasspage.py` & `mknodes-0.3.2/mknodes/classnodes/mkclasspage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,84 @@
-from __future__ import annotations
-
-import logging
-import os
-import pathlib
-
-from typing import Any
-
-from mknodes import (
-    classhelpers,
-    mkclassdiagram,
-    mkclasstable,
-    mkdocstrings,
-    mkpage,
-    utils,
-)
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkClassPage(mkpage.MkPage):
-    """Page showing information about a class.
-
-    Arguments:
-        klass: class to show info for
-        module_path: If given, overrides module returned by class.__module__
-                     This can be useful if you want to link to an aliased class
-                     (for example a class imported to __init__.py)
-        path: some path for the file.
-        kwargs: keyword arguments passed to base class
-    """
-
-    def __init__(
-        self,
-        klass: type,
-        *,
-        module_path: tuple[str, ...] | str | None = None,
-        hide_toc: bool = False,
-        hide_nav: bool = False,
-        hide_path: bool = False,
-        path: str | os.PathLike = "",
-        **kwargs: Any,
-    ):
-        # TODO: should path be settable?
-        path = pathlib.Path(f"{klass.__name__}.md")
-        super().__init__(
-            path=path,
-            hide_toc=hide_toc,
-            hide_nav=hide_nav,
-            hide_path=hide_path,
-            **kwargs,
-        )
-        self.klass = klass
-        match module_path:
-            case None:
-                self.parts = klass.__module__.split(".")
-            case _:
-                self.parts = classhelpers.to_module_parts(module_path)
-        self._build()
-
-    def __repr__(self):
-        return utils.get_repr(self, klass=self.klass, path=str(self.path))
-
-    @staticmethod
-    def examples():
-        yield dict(klass=MkClassPage)
-
-    def add_class_diagram(self, mode: mkclassdiagram.DiagramModeStr = "parent_tree"):
-        diagram = mkclassdiagram.MkClassDiagram(self.klass, mode=mode)
-        self.append(diagram)
-        return diagram
-
-    def _build(self):
-        module_path = ".".join(self.parts).rstrip(".")
-        path = f"{module_path}.{self.klass.__name__}"
-        item = mkdocstrings.MkDocStrings(path, header="DocStrings")
-        self.append(item)
-        if tbl := mkclasstable.MkClassTable(self.klass):
-            self.append(tbl)
-        item = mkclassdiagram.MkClassDiagram(self.klass, header="Inheritance diagram")
-        self.append(item)
-
-
-if __name__ == "__main__":
-    doc = MkClassPage(MkClassPage)
-    doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
-    print(doc)
-    # print(doc.children)
+from __future__ import annotations
+
+import logging
+import os
+import pathlib
+
+from typing import Any
+
+from mknodes import mkdocstrings, mkpage
+from mknodes.classnodes import mkclassdiagram, mkclasstable
+from mknodes.utils import classhelpers, helpers
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkClassPage(mkpage.MkPage):
+    """Page showing information about a class.
+
+    Arguments:
+        klass: class to show info for
+        module_path: If given, overrides module returned by class.__module__
+                     This can be useful if you want to link to an aliased class
+                     (for example a class imported to __init__.py)
+        path: some path for the file.
+        kwargs: keyword arguments passed to base class
+    """
+
+    def __init__(
+        self,
+        klass: type,
+        *,
+        module_path: tuple[str, ...] | str | None = None,
+        hide_toc: bool = False,
+        hide_nav: bool = False,
+        hide_path: bool = False,
+        path: str | os.PathLike = "",
+        **kwargs: Any,
+    ):
+        # TODO: should path be settable?
+        path = pathlib.Path(f"{klass.__name__}.md")
+        super().__init__(
+            path=path,
+            hide_toc=hide_toc,
+            hide_nav=hide_nav,
+            hide_path=hide_path,
+            **kwargs,
+        )
+        self.klass = klass
+        match module_path:
+            case None:
+                self.parts = klass.__module__.split(".")
+            case _:
+                self.parts = classhelpers.to_module_parts(module_path)
+        self._build()
+
+    def __repr__(self):
+        return helpers.get_repr(self, klass=self.klass, path=str(self.path))
+
+    @staticmethod
+    def examples():
+        yield dict(klass=MkClassPage)
+
+    def add_class_diagram(self, mode: mkclassdiagram.DiagramModeStr = "parent_tree"):
+        diagram = mkclassdiagram.MkClassDiagram(self.klass, mode=mode)
+        self.append(diagram)
+        return diagram
+
+    def _build(self):
+        module_path = ".".join(self.parts).rstrip(".")
+        path = f"{module_path}.{self.klass.__name__}"
+        item = mkdocstrings.MkDocStrings(path, header="DocStrings")
+        self.append(item)
+        if tbl := mkclasstable.MkClassTable(self.klass):
+            self.append(tbl)
+        item = mkclassdiagram.MkClassDiagram(self.klass, header="Inheritance diagram")
+        self.append(item)
+
+
+if __name__ == "__main__":
+    doc = MkClassPage(MkClassPage)
+    doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
+    print(doc)
+    # print(doc.children)
```

### Comparing `mknodes-0.2.0/mknodes/mkcode.py` & `mknodes-0.3.2/mknodes/mkcode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,87 @@
-from __future__ import annotations
-
-from collections.abc import Callable
-import inspect
-import logging
-import textwrap
-import types
-
-from typing import Any
-
-from typing_extensions import Self
-
-from mknodes import mknode, mktext, utils
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkCode(mktext.MkText):
-    """Class representing a Code block."""
-
-    REQUIRED_EXTENSIONS = [
-        "pymdownx.highlight",
-        "pymdownx.inlinehilite",
-        "pymdownx.snippets",
-        "pymdownx.superfences",
-    ]
-
-    def __init__(
-        self,
-        code: str | mknode.MkNode = "",
-        language: str = "py",
-        *,
-        title: str = "",
-        header: str = "",
-        linenums: int | None = None,
-        highlight_lines: list[int] | None = None,
-        parent=None,
-    ):
-        if isinstance(code, MkCode):
-            code = textwrap.indent(str(code), "    ")
-        super().__init__(code, header=header, parent=parent)
-        self.language = language
-        self.title = title
-        self.linenums = linenums
-        self.highlight_lines = highlight_lines
-
-    def _to_markdown(self) -> str:
-        title = f" title={self.title!r}" if self.title else ""
-        return f"``` {self.language}{title}\n{self.text}\n```"
-
-    @staticmethod
-    def examples():
-        yield dict(language="python", code="a = 1 + 2")
-        yield dict(language="js", code="var z = x + y;", title="JavaScript")
-
-    @classmethod
-    def for_object(
-        cls,
-        obj: types.ModuleType
-        | type
-        | types.MethodType
-        | types.FunctionType
-        | types.TracebackType
-        | types.FrameType
-        | types.CodeType
-        | Callable[..., Any],
-        *,
-        dedent: bool = True,
-        extract_body: bool = False,
-        header: str = "",
-    ) -> Self:
-        if extract_body and isinstance(obj, type | types.FunctionType | types.MethodType):
-            code = utils.get_function_body(obj)
-        elif extract_body:
-            raise TypeError("Can only extract body from Functions, Methods and classes")
-        else:
-            code = inspect.getsource(obj)
-        code = textwrap.dedent(code) if dedent else code
-        return cls(code=code, header=header)
-
-
-if __name__ == "__main__":
-    code = MkCode.for_object(MkCode, extract_body=True)
-    print(code)
+from __future__ import annotations
+
+from collections.abc import Callable
+import inspect
+import logging
+import textwrap
+import types
+
+from typing import Any
+
+from typing_extensions import Self
+
+from mknodes import mknode, mktext
+from mknodes.utils import helpers
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkCode(mktext.MkText):
+    """Class representing a Code block."""
+
+    REQUIRED_EXTENSIONS = [
+        "pymdownx.highlight",
+        "pymdownx.inlinehilite",
+        "pymdownx.snippets",
+        "pymdownx.superfences",
+    ]
+
+    def __init__(
+        self,
+        code: str | mknode.MkNode = "",
+        language: str = "py",
+        *,
+        title: str = "",
+        header: str = "",
+        linenums: int | None = None,
+        highlight_lines: list[int] | None = None,
+        parent=None,
+    ):
+        if isinstance(code, MkCode):
+            code = textwrap.indent(str(code), "    ")
+        super().__init__(code, header=header, parent=parent)
+        self.language = language
+        self.title = title
+        self.linenums = linenums
+        self.highlight_lines = highlight_lines
+
+    def _to_markdown(self) -> str:
+        title = f" title={self.title!r}" if self.title else ""
+        return f"``` {self.language}{title}\n{self.text}\n```"
+
+    @staticmethod
+    def examples():
+        yield dict(language="python", code="a = 1 + 2")
+        yield dict(language="js", code="var z = x + y;", title="JavaScript")
+
+    @classmethod
+    def for_object(
+        cls,
+        obj: types.ModuleType
+        | type
+        | types.MethodType
+        | types.FunctionType
+        | types.TracebackType
+        | types.FrameType
+        | types.CodeType
+        | Callable[..., Any],
+        *,
+        dedent: bool = True,
+        extract_body: bool = False,
+        header: str = "",
+    ) -> Self:
+        if extract_body and isinstance(obj, type | types.FunctionType | types.MethodType):
+            code = helpers.get_function_body(obj)
+        elif extract_body:
+            msg = "Can only extract body from Functions, Methods and classes"
+            raise TypeError(msg)
+        else:
+            code = inspect.getsource(obj)
+        code = textwrap.dedent(code) if dedent else code
+        return cls(code=code, header=header)
+
+
+if __name__ == "__main__":
+    code = MkCode.for_object(MkCode, extract_body=True)
+    print(code)
```

### Comparing `mknodes-0.2.0/mknodes/mkcritic.py` & `mknodes-0.3.2/mknodes/mkcritic.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from __future__ import annotations
-
-import logging
-
-from typing import Literal
-
-from mknodes import mktext
-
-
-logger = logging.getLogger(__name__)
-
-CriticMarkStr = Literal["addition", "deletion", "substitution", "comment", "highlight"]
-
-
-class MkCritic(mktext.MkText):
-    """MkCritic block."""
-
-    def __init__(
-        self,
-        text: str,
-        mark: CriticMarkStr = "addition",
-        **kwargs,
-    ):
-        super().__init__(text=text, **kwargs)
-        self.mark = mark
-
-    def _to_markdown(self) -> str:
-        match self.mark:
-            case "addition":
-                left, right = ("++", "++")
-            case "deletion":
-                left, right = ("--", "--")
-            case "highlight":
-                left, right = ("==", "==")
-            case "comment":
-                left, right = (">>", "<<")
-            case _:
-                raise TypeError(self.mark)
-        return f"{{{left}\n\n{self.text}\n\n{right}}}"
-
-    @staticmethod
-    def examples():
-        for typ in ["addition", "deletion", "comment", "highlight"]:
-            yield dict(mark=typ, text=f"This is type {typ}")
-
-
-if __name__ == "__main__":
-    mkcritic = MkCritic("hello")
-    print(mkcritic)
+from __future__ import annotations
+
+import logging
+
+from typing import Literal
+
+from mknodes import mktext
+
+
+logger = logging.getLogger(__name__)
+
+CriticMarkStr = Literal["addition", "deletion", "substitution", "comment", "highlight"]
+
+
+class MkCritic(mktext.MkText):
+    """MkCritic block."""
+
+    def __init__(
+        self,
+        text: str,
+        mark: CriticMarkStr = "addition",
+        **kwargs,
+    ):
+        super().__init__(text=text, **kwargs)
+        self.mark = mark
+
+    def _to_markdown(self) -> str:
+        match self.mark:
+            case "addition":
+                left, right = ("++", "++")
+            case "deletion":
+                left, right = ("--", "--")
+            case "highlight":
+                left, right = ("==", "==")
+            case "comment":
+                left, right = (">>", "<<")
+            case _:
+                raise TypeError(self.mark)
+        return f"{{{left}\n\n{self.text}\n\n{right}}}"
+
+    @staticmethod
+    def examples():
+        for typ in ["addition", "deletion", "comment", "highlight"]:
+            yield dict(mark=typ, text=f"This is type {typ}")
+
+
+if __name__ == "__main__":
+    mkcritic = MkCritic("hello")
+    print(mkcritic)
```

### Comparing `mknodes-0.2.0/mknodes/mkdoc.py` & `mknodes-0.3.2/mknodes/mkdoc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,257 +1,297 @@
-from __future__ import annotations
-
-from collections.abc import Callable, Iterator, Sequence
-
-# import contextlib
-# import importlib
-import inspect
-import logging
-import pathlib
-import types
-
-from typing import Any
-
-from mknodes import classhelpers, mkclasspage, mkmodulepage, mknav, utils
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkDoc(mknav.MkNav):
-    """Nav for showing a module documenation.
-
-    Arguments:
-        module: Module to document
-        filter_by___all__: Whether to filter stuff according to "__all__"
-        exclude_modules: List of modules to exclude
-        section_name: Optional section name override
-    """
-
-    def __init__(
-        self,
-        module: types.ModuleType | Sequence[str] | str,
-        *,
-        filter_by___all__: bool = False,
-        exclude_modules: list[str] | None = None,
-        section_name: str | None = None,
-        class_page=mkclasspage.MkClassPage,
-        **kwargs,
-    ):
-        self.module = classhelpers.to_module(module)
-        self.ClassPage = class_page
-        if self.module is None:
-            raise RuntimeError(f"Couldnt load module {module!r}")
-        self.is_package = hasattr(self.module, "__path__")
-        self.filter_by___all__ = filter_by___all__
-        self.module_name = self.module.__name__.split(".")[-1]
-        self.module_path = self.module.__name__
-        self.file_path = self.module.__file__
-        super().__init__(section=section_name or self.module_name, **kwargs)
-        self._exclude = exclude_modules or []
-        self.root_path = pathlib.Path(f"./{self.module_name}")
-
-    def __repr__(self):
-        return utils.get_repr(
-            self,
-            module=self.module_name,
-            section=self.section or "<root>",
-            filename=self.filename,
-        )
-
-    def iter_files(self, glob: str = "*/*.py") -> Iterator[pathlib.Path]:
-        """Iter through files based on glob.
-
-        Arguments:
-            glob: glob to use for filtering
-        """
-        for path in sorted(self.root_path.rglob(glob)):
-            if (
-                all(i not in path.parts for i in self._exclude)
-                and not any(i.startswith("__") for i in path.parent.parts)
-                and not path.is_dir()
-            ):
-                yield path.relative_to(self.root_path)
-
-    def iter_classes(
-        self,
-        submodule: types.ModuleType | str | tuple | list | None = None,
-        *,
-        recursive: bool = False,
-        predicate: Callable | None = None,
-        _seen: set | None = None,
-    ) -> Iterator[type]:
-        """Iterate over all classes of the module.
-
-        Arguments:
-            submodule: filter based on a submodule
-            recursive: whether to only iterate over members of current module
-                       or whether it should also include classes from submodules.
-            predicate: filter classes based on a predicate.
-        """
-        mod = classhelpers.to_module(submodule) if submodule else self.module
-        if mod is None:
-            return
-        if recursive:
-            seen = _seen or set()
-            for _submod_name, submod in inspect.getmembers(mod, inspect.ismodule):
-                if submod.__name__.startswith(self.module_name) and submod not in seen:
-                    seen.add(submod)
-                    yield from self.iter_classes(
-                        submod,
-                        recursive=True,
-                        predicate=predicate,
-                        _seen=seen,
-                    )
-        for klass_name, klass in inspect.getmembers(mod, inspect.isclass):
-            if self.filter_by___all__ and (
-                not hasattr(mod, "__all__") or klass_name not in mod.__all__
-            ):
-                continue
-            if predicate and not predicate(klass):
-                continue
-            # if klass.__module__.startswith(self.module_name):
-            if self.module_name in klass.__module__.split("."):
-                yield klass
-
-    def iter_modules(
-        self,
-        *,
-        submodule: types.ModuleType | str | tuple | list | None = None,
-        recursive: bool = False,
-        predicate: Callable | None = None,
-        _seen: set | None = None,
-    ) -> Iterator[types.ModuleType]:
-        """Iterate over all submodules of the module.
-
-        Arguments:
-            submodule: filter based on a submodule
-            recursive: whether to only iterate over members of current module
-                       or whether it should also include modules from submodules.
-            predicate: filter modules based on a predicate.
-        """
-        mod = classhelpers.to_module(submodule) if submodule else self.module
-        seen = _seen or set()
-        if mod is None:
-            return
-        for submod_name, submod in inspect.getmembers(mod, inspect.ismodule):
-            not_in_all = hasattr(mod, "__all__") and submod_name not in mod.__all__
-            filtered_by_all = self.filter_by___all__ and not_in_all
-            not_filtered_by_pred = predicate(submod) if predicate else True
-            # if self.module_name in mod.__name__.split(".")
-            if not filtered_by_all and not_filtered_by_pred:
-                yield submod
-            if recursive and submod not in seen:
-                seen.add(submod)
-                yield from self.iter_modules(
-                    submodule=submod,
-                    recursive=True,
-                    predicate=predicate,
-                    _seen=seen,
-                )
-
-    def add_class_page(
-        self,
-        klass: type,
-        *,
-        find_topmost: bool = True,
-        flatten: bool = False,
-        **kwargs: Any,
-    ) -> mkclasspage.MkClassPage:
-        """Add a page showing information about a class.
-
-        Arguments:
-            klass: klass to build a page for
-            find_topmost: Whether to use a module path from a parent package if available
-            flatten: Put page into top level nav if nested.
-            kwargs: keyword arguments passed to CLassPage
-        """
-        if find_topmost:
-            parts = classhelpers.get_topmost_module_path(klass).split(".")
-        else:
-            parts = klass.__module__.split(".")
-        # parts = klass.__module__.split(".")
-        path = pathlib.Path(f"{klass.__name__}.md")
-        page = self.ClassPage(
-            klass=klass,
-            module_path=tuple(parts),
-            path=path,
-            parent=self,
-            **kwargs,
-        )
-        section = (klass.__name__,) if flatten else (*parts[1:], klass.__name__)
-        self.nav[section] = page
-        return page
-
-    # def add_overview_page(self, predicate: Callable | None = None):
-    #     page = mkpage.MkPage(
-    #         hide_toc=True,
-    #         path=pathlib.Path("index.md"),
-    #         # parent=self,
-    #     )
-    #     page += mknodes.ModuleTable(self.module_name, predicate=predicate)
-    #     return page
-
-    def add_module_overview(
-        self,
-        title: str | None = None,
-        **kwargs: Any,
-    ) -> mkmodulepage.MkModulePage:
-        """Add a page showing all submodules.
-
-        Arguments:
-            title: Override title for the section.
-            kwargs: kwargs passed to MkModulePage.
-        """
-        # TODO: slugify?
-        path = pathlib.Path("index.md" if title is None else f"{title}.md")
-        # parts = path.parts[:-1]
-        page = mkmodulepage.MkModulePage(
-            hide_toc=True,
-            module=self.module,  # type: ignore
-            path=path,
-            parent=self,
-            **kwargs,
-        )
-        self.nav[title or self.module_name] = page
-        return page
-
-    # def iter_modules_for_glob(self, glob="*/*.py"):
-    #     for path in self.iter_files(glob):
-    #         module_path = path.with_suffix("")
-    #         parts = tuple(module_path.parts)
-    #         complete_module_path = f"{self.module_name}." + ".".join(parts)
-    #         with contextlib.suppress(ImportError, AttributeError):
-    #             yield importlib.import_module(complete_module_path)
-
-    # def iter_classes_for_glob(
-    #     self,
-    #     glob: str = "*/*.py",
-    #     *,
-    #     recursive: bool = False,
-    #     avoid_duplicates: bool = True,
-    # ) -> Iterator[tuple[type, pathlib.Path]]:
-    #     """Yields (class, path) tuples.
-
-    #     Arguments:
-    #         glob: glob to use for module file selection.
-    #         recursive: Whether to search recursively.
-    #         avoid_duplicates:
-
-    #     """
-    #     seen = set()
-    #     for path in self.iter_files(glob):
-    #         module_path = path.with_suffix("")
-    #         parts = tuple(self.module_name, *module_path.parts)
-    #         module = classhelpers.to_module(parts)
-    #         if not module:
-    #             return
-    #         for klass in self.iter_classes(module, recursive=recursive):
-    #             if (klass, path) not in seen or not avoid_duplicates:
-    #                 seen.add((klass, path))
-    #                 yield klass, path
-
-
-if __name__ == "__main__":
-    doc = MkDoc(module="mkdocs")
-    page = doc.add_class_page(MkDoc)
-    print(page)
+from __future__ import annotations
+
+from collections.abc import Callable, Iterator, Sequence
+
+# import contextlib
+# import importlib
+import inspect
+import logging
+import pathlib
+import types
+
+from typing import Any
+
+from mknodes import mknav
+from mknodes.classnodes import mkclasspage
+from mknodes.modulenodes import mkmodulepage
+from mknodes.utils import classhelpers, helpers
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkDoc(mknav.MkNav):
+    """Nav for showing a module documenation.
+
+    Arguments:
+        module: Module to document
+        filter_by___all__: Whether to filter stuff according to "__all__"
+        exclude_modules: List of modules to exclude
+        section_name: Optional section name override
+    """
+
+    def __init__(
+        self,
+        module: types.ModuleType | Sequence[str] | str,
+        *,
+        filter_by___all__: bool = False,
+        exclude_modules: list[str] | None = None,
+        section_name: str | None = None,
+        class_page: type[mkclasspage.MkClassPage] | None = None,
+        flatten_nav: bool = False,
+        **kwargs,
+    ):
+        self.module = classhelpers.to_module(module, return_none=False)
+        self.is_package = hasattr(self.module, "__path__")
+        self.module_name = self.module.__name__.split(".")[-1]
+        self.module_path = self.module.__name__
+        self.file_path = self.module.__file__
+
+        self.ClassPage = class_page or mkclasspage.MkClassPage
+        self.flatten_nav = flatten_nav
+        self.klasses: set[type] = set()
+        self.submodules: set[types.ModuleType] = set()
+        self.filter_by___all__ = filter_by___all__
+        self._exclude = exclude_modules or []
+        # self.root_path = pathlib.Path(f"./{self.module_name}")
+        super().__init__(section=section_name or self.module_name, **kwargs)
+
+    def __repr__(self):
+        return helpers.get_repr(
+            self,
+            module=self.module_name,
+            section=self.section or "<root>",
+            filename=self.filename,
+        )
+
+    def to_markdown(self) -> str:
+        for klass in self.klasses:
+            self.add_class_page(klass=klass, flatten=self.flatten_nav)
+        for submod in self.submodules:
+            self.add_doc(submod, class_page=self.ClassPage, flatten_nav=self.flatten_nav)
+        return super().to_markdown()
+
+    def collect_classes(
+        self,
+        *,
+        recursive: bool = False,
+        predicate: Callable | None = None,
+        submodule: types.ModuleType | str | tuple | list | None = None,
+    ):
+        for klass in self.iter_classes(
+            recursive=recursive,
+            predicate=predicate,
+            submodule=submodule,
+        ):
+            self.klasses.add(klass)
+
+    def iter_classes(
+        self,
+        submodule: types.ModuleType | str | tuple | list | None = None,
+        *,
+        recursive: bool = False,
+        predicate: Callable | None = None,
+        _seen: set | None = None,
+    ) -> Iterator[type]:
+        """Iterate over all classes of the module.
+
+        Arguments:
+            submodule: filter based on a submodule
+            recursive: whether to only iterate over members of current module
+                       or whether it should also include classes from submodules.
+            predicate: filter classes based on a predicate.
+        """
+        mod = classhelpers.to_module(submodule) if submodule else self.module
+        if mod is None:
+            return
+        if recursive:
+            seen = _seen or set()
+            for _submod_name, submod in inspect.getmembers(mod, inspect.ismodule):
+                if submod.__name__.startswith(self.module_name) and submod not in seen:
+                    seen.add(submod)
+                    yield from self.iter_classes(
+                        submod,
+                        recursive=True,
+                        predicate=predicate,
+                        _seen=seen,
+                    )
+        for klass_name, klass in inspect.getmembers(mod, inspect.isclass):
+            if self.filter_by___all__ and (
+                not hasattr(mod, "__all__") or klass_name not in mod.__all__
+            ):
+                continue
+            if predicate and not predicate(klass):
+                continue
+            # if klass.__module__.startswith(self.module_name):
+            if self.module_name in klass.__module__.split("."):
+                yield klass
+
+    def collect_modules(
+        self,
+        *,
+        recursive: bool = False,
+        predicate: Callable | None = None,
+        submodule: types.ModuleType | str | tuple | list | None = None,
+    ):
+        for module in self.iter_modules(
+            recursive=recursive,
+            predicate=predicate,
+            submodule=submodule,
+        ):
+            self.submodules.add(module)
+
+    def iter_modules(
+        self,
+        *,
+        submodule: types.ModuleType | str | tuple | list | None = None,
+        recursive: bool = False,
+        predicate: Callable | None = None,
+        _seen: set | None = None,
+    ) -> Iterator[types.ModuleType]:
+        """Iterate over all submodules of the module.
+
+        Arguments:
+            submodule: filter based on a submodule
+            recursive: whether to only iterate over members of current module
+                       or whether it should also include modules from submodules.
+            predicate: filter modules based on a predicate.
+        """
+        mod = classhelpers.to_module(submodule) if submodule else self.module
+        seen = _seen or set()
+        if mod is None:
+            return
+        for submod_name, submod in inspect.getmembers(mod, inspect.ismodule):
+            not_in_all = hasattr(mod, "__all__") and submod_name not in mod.__all__
+            filtered_by_all = self.filter_by___all__ and not_in_all
+            not_filtered_by_pred = predicate(submod) if predicate else True
+            # if self.module_name in mod.__name__.split(".")
+            if not filtered_by_all and not_filtered_by_pred:
+                yield submod
+            if recursive and submod not in seen:
+                seen.add(submod)
+                yield from self.iter_modules(
+                    submodule=submod,
+                    recursive=True,
+                    predicate=predicate,
+                    _seen=seen,
+                )
+
+    def add_class_page(
+        self,
+        klass: type,
+        *,
+        find_topmost: bool = True,
+        flatten: bool = False,
+        **kwargs: Any,
+    ) -> mkclasspage.MkClassPage:
+        """Add a page showing information about a class.
+
+        Arguments:
+            klass: klass to build a page for
+            find_topmost: Whether to use a module path from a parent package if available
+            flatten: Put page into top level nav if nested.
+            kwargs: keyword arguments passed to CLassPage
+        """
+        if find_topmost:
+            parts = classhelpers.get_topmost_module_path(klass).split(".")
+        else:
+            parts = klass.__module__.split(".")
+        # parts = klass.__module__.split(".")
+        page = self.ClassPage(
+            klass=klass,
+            module_path=tuple(parts),
+            path=pathlib.Path(f"{klass.__name__}.md"),
+            parent=self,
+            **kwargs,
+        )
+        section = (klass.__name__,) if flatten else (*parts[1:], klass.__name__)
+        self.nav[section] = page
+        return page
+
+    # def add_overview_page(self, predicate: Callable | None = None):
+    #     page = mkpage.MkPage(
+    #         hide_toc=True,
+    #         path=pathlib.Path("index.md"),
+    #         # parent=self,
+    #     )
+    #     page += mknodes.ModuleTable(self.module_name, predicate=predicate)
+    #     return page
+
+    def add_module_overview(
+        self,
+        title: str | None = None,
+        **kwargs: Any,
+    ) -> mkmodulepage.MkModulePage:
+        """Add a page showing all submodules.
+
+        Arguments:
+            title: Override title for the section.
+            kwargs: kwargs passed to MkModulePage.
+        """
+        # TODO: slugify?
+        path = pathlib.Path("index.md" if title is None else f"{title}.md")
+        # parts = path.parts[:-1]
+        page = mkmodulepage.MkModulePage(
+            hide_toc=True,
+            module=self.module,
+            path=path,
+            parent=self,
+            **kwargs,
+        )
+        self.nav[title or self.module_name] = page
+        return page
+
+    # def iter_files(self, glob: str = "*/*.py") -> Iterator[pathlib.Path]:
+    #     """Iter through files based on glob.
+
+    #     Arguments:
+    #         glob: glob to use for filtering
+    #     """
+    #     for path in sorted(self.root_path.rglob(glob)):
+    #         if (
+    #             all(i not in path.parts for i in self._exclude)
+    #             and not any(i.startswith("__") for i in path.parent.parts)
+    #             and not path.is_dir()
+    #         ):
+    #             yield path.relative_to(self.root_path)
+
+    # def iter_modules_for_glob(self, glob="*/*.py"):
+    #     for path in self.iter_files(glob):
+    #         module_path = path.with_suffix("")
+    #         parts = tuple(module_path.parts)
+    #         complete_module_path = f"{self.module_name}." + ".".join(parts)
+    #         with contextlib.suppress(ImportError, AttributeError):
+    #             yield importlib.import_module(complete_module_path)
+
+    # def iter_classes_for_glob(
+    #     self,
+    #     glob: str = "*/*.py",
+    #     *,
+    #     recursive: bool = False,
+    #     avoid_duplicates: bool = True,
+    # ) -> Iterator[tuple[type, pathlib.Path]]:
+    #     """Yields (class, path) tuples.
+
+    #     Arguments:
+    #         glob: glob to use for module file selection.
+    #         recursive: Whether to search recursively.
+    #         avoid_duplicates:
+
+    #     """
+    #     seen = set()
+    #     for path in self.iter_files(glob):
+    #         module_path = path.with_suffix("")
+    #         parts = tuple(self.module_name, *module_path.parts)
+    #         module = classhelpers.to_module(parts)
+    #         if not module:
+    #             return
+    #         for klass in self.iter_classes(module, recursive=recursive):
+    #             if (klass, path) not in seen or not avoid_duplicates:
+    #                 seen.add((klass, path))
+    #                 yield klass, path
+
+
+if __name__ == "__main__":
+    doc = MkDoc(module="mkdocs")
+    page = doc.add_class_page(MkDoc)
+    print(page)
```

### Comparing `mknodes-0.2.0/mknodes/mkdocstrings.py` & `mknodes-0.3.2/mknodes/mkdocstrings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,184 +1,185 @@
-from __future__ import annotations
-
-import importlib
-import logging
-import os
-import types
-
-from typing import Any, Literal
-
-from mknodes import classhelpers, mktext, utils
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkDocStrings(mktext.MkText):
-    """Docstring section (powered by mkdocstrings)."""
-
-    REQUIRED_PLUGINS = "mkdocstrings"
-    OPTIONS_DEFAULT: dict[str, Any] = {}
-
-    def __init__(
-        self,
-        obj: types.ModuleType
-        | str
-        | os.PathLike
-        | type
-        | types.FunctionType
-        | types.MethodType,
-        for_topmost: bool = False,
-        allow_inspection: bool | None = None,
-        show_bases: bool | None = None,
-        show_source: bool | None = None,
-        preload_modules: list[str] | None = None,
-        heading_level: int | None = None,
-        show_root_heading: bool | None = None,
-        show_root_toc_entry: bool | None = None,
-        show_root_full_path: bool | None = None,
-        show_root_members_full_path: bool | None = None,
-        show_object_full_path: bool | None = None,
-        show_category_heading: bool | None = None,
-        show_symbol_type_heading: bool | None = None,
-        show_symbol_type_toc: bool | None = None,
-        inherited_members: bool | None = None,
-        members: list[str] | None = None,
-        members_order: Literal["alphabetical", "source"] | None = None,
-        filters: list[str] | None = None,
-        group_by_category: bool | None = None,
-        show_submodules: bool | None = None,
-        docstring_section_style: Literal["table", "list", "spacy"] | None = None,
-        merge_init_into_class: bool | None = None,
-        show_if_no_docstring: bool | None = None,
-        annotations_path: Literal["brief", "source"] | None = None,
-        line_length: int | None = None,
-        show_signature: bool | None = None,
-        show_signature_annotations: bool | None = None,
-        signature_crossrefs: bool | None = None,
-        separate_signature: bool | None = None,
-        **kwargs: Any,
-    ):
-        """Docstring section.
-
-        Global options for DocStrings can be overridden by setting the keyword arguments
-        to not-None.
-
-        Arguments:
-            obj: What to show DocStrings for.
-            for_topmost: If True, try to find the "shortest" path to given object by
-                         checking whether it can also be found in a parent module.
-            allow_inspection: Whether to allow inspecting modules when visiting
-                              them is not possible
-            show_bases: Show the base classes of a class.
-            show_source: Show the source code of this object.
-            preload_modules: List of modules to pre-load.
-            heading_level: The initial heading level to use.
-            show_root_heading: Show the heading of the object at the root of the
-                               documentation tree (i.e. the object referenced by
-                               the identifier after :::).
-            show_root_toc_entry: If the root heading is not shown, at least
-                                 add a ToC entry for it.
-            show_root_full_path: Show the full Python path for the root
-                                 object heading.
-            show_root_members_full_path: Show the full Python path of the
-                                         root members.
-            show_object_full_path: Show the full Python path of every object.
-            show_category_heading: When grouped by categories, show a heading
-                                   for each category.
-            show_symbol_type_heading: Show the symbol type in headings (e.g. mod,
-                                      class, func and attr).
-            show_symbol_type_toc: Show the symbol type in the Table of
-                                  Contents (e.g. mod, class, func and attr).
-            inherited_members: Also show inherited members.
-            members: An explicit list of members to render.
-            members_order: The members ordering to use.
-            filters: A list of filters applied to filter objects based on their name.
-                     A filter starting with ! will exclude matching objects instead of
-                     including them. The members option takes precedence over filters
-                     (filters will still be applied recursively to lower members in the
-                     hierarchy).
-            group_by_category: Group the object's children by categories:
-                               attributes, classes, functions, and modules.
-            show_submodules: When rendering a module, show its submodules recursively.
-            docstring_section_style: The style used to render docstring sections.
-            merge_init_into_class: Whether to merge the __init__ method into
-                                   the class' signature and docstring.
-            show_if_no_docstring: Show the object heading even if it has no
-                                  docstring or children with docstrings.
-            annotations_path: The verbosity for annotations path
-            line_length: Maximum line length when formatting code/signatures.
-            show_signature: Show methods and functions signatures.
-            show_signature_annotations: Show the type annotations in methods
-                                        and functions signatures.
-            signature_crossrefs: Whether to render cross-references for type
-                                 annotations in signatures.
-            separate_signature: Whether to put the whole signature in a code
-                                block below the heading. If Black is installed,
-                                the signature is also formatted using it.
-            kwargs: Keyword arguments passed to super.
-        """
-        super().__init__(**kwargs)
-        self.obj = obj
-        match obj:
-            case types.ModuleType():
-                self.obj_path = obj.__name__
-            case type() | types.FunctionType() | types.MethodType():
-                if for_topmost:
-                    topmost_path = classhelpers.get_topmost_module_path(obj)
-                    self.obj_path = f"{topmost_path}.{obj.__qualname__}"
-                else:
-                    self.obj_path = f"{obj.__module__}.{obj.__qualname__}"
-            case str():
-                self.obj_path = obj  # for setting a manual path
-            case tuple() | list():
-                self.obj_path = ".".join(obj)
-            case os.PathLike():
-                mod = importlib.import_module(os.fspath(obj))
-                self.obj_path = mod.__name__
-            case _:
-                raise TypeError(obj)
-        self.options = self.OPTIONS_DEFAULT.copy()
-        self.options["allow_inspection"] = allow_inspection
-        self.options["show_bases"] = show_bases
-        self.options["show_source"] = show_source
-        self.options["preload_modules"] = preload_modules
-        self.options["heading_level"] = heading_level
-        self.options["show_root_heading"] = show_root_heading
-        self.options["show_root_toc_entry"] = show_root_toc_entry
-        self.options["show_root_full_path"] = show_root_full_path
-        self.options["show_root_members_full_path"] = show_root_members_full_path
-        self.options["show_object_full_path"] = show_object_full_path
-        self.options["show_category_heading"] = show_category_heading
-        self.options["show_symbol_type_heading"] = show_symbol_type_heading
-        self.options["show_symbol_type_toc"] = show_symbol_type_toc
-        self.options["inherited_members"] = inherited_members
-        self.options["members"] = members
-        self.options["members_order"] = members_order
-        self.options["filters"] = filters
-        self.options["group_by_category"] = group_by_category
-        self.options["show_submodules"] = show_submodules
-        self.options["docstring_section_style"] = docstring_section_style
-        self.options["merge_init_into_class"] = merge_init_into_class
-        self.options["show_if_no_docstring"] = show_if_no_docstring
-        self.options["annotations_path"] = annotations_path
-        self.options["line_length"] = line_length
-        self.options["show_signature"] = show_signature
-        self.options["show_signature_annotations"] = show_signature_annotations
-        self.options["signature_crossrefs"] = signature_crossrefs
-        self.options["separate_signature"] = separate_signature
-        self.options = {k: v for k, v in self.options.items() if v is not None}
-
-    def __repr__(self):
-        return utils.get_repr(self, obj=self.obj)
-
-    def _to_markdown(self) -> str:
-        md = f"::: {self.obj_path}\n"
-        if self.options:
-            options = "\n".join(f"      {k}: {v!r}" for k, v in self.options.items())
-            md = f"{md}    options:\n{options}\n"
-        return md
-
-
-if __name__ == "__main__":
-    docstrings = MkDocStrings("a.b", show_submodules=True)
-    print(docstrings)
+from __future__ import annotations
+
+import importlib
+import logging
+import os
+import types
+
+from typing import Any, Literal
+
+from mknodes import mktext
+from mknodes.utils import classhelpers, helpers
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkDocStrings(mktext.MkText):
+    """Docstring section (powered by mkdocstrings)."""
+
+    REQUIRED_PLUGINS = "mkdocstrings"
+    OPTIONS_DEFAULT: dict[str, Any] = {}
+
+    def __init__(
+        self,
+        obj: types.ModuleType
+        | str
+        | os.PathLike
+        | type
+        | types.FunctionType
+        | types.MethodType,
+        for_topmost: bool = False,
+        allow_inspection: bool | None = None,
+        show_bases: bool | None = None,
+        show_source: bool | None = None,
+        preload_modules: list[str] | None = None,
+        heading_level: int | None = None,
+        show_root_heading: bool | None = None,
+        show_root_toc_entry: bool | None = None,
+        show_root_full_path: bool | None = None,
+        show_root_members_full_path: bool | None = None,
+        show_object_full_path: bool | None = None,
+        show_category_heading: bool | None = None,
+        show_symbol_type_heading: bool | None = None,
+        show_symbol_type_toc: bool | None = None,
+        inherited_members: bool | None = None,
+        members: list[str] | None = None,
+        members_order: Literal["alphabetical", "source"] | None = None,
+        filters: list[str] | None = None,
+        group_by_category: bool | None = None,
+        show_submodules: bool | None = None,
+        docstring_section_style: Literal["table", "list", "spacy"] | None = None,
+        merge_init_into_class: bool | None = None,
+        show_if_no_docstring: bool | None = None,
+        annotations_path: Literal["brief", "source"] | None = None,
+        line_length: int | None = None,
+        show_signature: bool | None = None,
+        show_signature_annotations: bool | None = None,
+        signature_crossrefs: bool | None = None,
+        separate_signature: bool | None = None,
+        **kwargs: Any,
+    ):
+        """Docstring section.
+
+        Global options for DocStrings can be overridden by setting the keyword arguments
+        to not-None.
+
+        Arguments:
+            obj: What to show DocStrings for.
+            for_topmost: If True, try to find the "shortest" path to given object by
+                         checking whether it can also be found in a parent module.
+            allow_inspection: Whether to allow inspecting modules when visiting
+                              them is not possible
+            show_bases: Show the base classes of a class.
+            show_source: Show the source code of this object.
+            preload_modules: List of modules to pre-load.
+            heading_level: The initial heading level to use.
+            show_root_heading: Show the heading of the object at the root of the
+                               documentation tree (i.e. the object referenced by
+                               the identifier after :::).
+            show_root_toc_entry: If the root heading is not shown, at least
+                                 add a ToC entry for it.
+            show_root_full_path: Show the full Python path for the root
+                                 object heading.
+            show_root_members_full_path: Show the full Python path of the
+                                         root members.
+            show_object_full_path: Show the full Python path of every object.
+            show_category_heading: When grouped by categories, show a heading
+                                   for each category.
+            show_symbol_type_heading: Show the symbol type in headings (e.g. mod,
+                                      class, func and attr).
+            show_symbol_type_toc: Show the symbol type in the Table of
+                                  Contents (e.g. mod, class, func and attr).
+            inherited_members: Also show inherited members.
+            members: An explicit list of members to render.
+            members_order: The members ordering to use.
+            filters: A list of filters applied to filter objects based on their name.
+                     A filter starting with ! will exclude matching objects instead of
+                     including them. The members option takes precedence over filters
+                     (filters will still be applied recursively to lower members in the
+                     hierarchy).
+            group_by_category: Group the object's children by categories:
+                               attributes, classes, functions, and modules.
+            show_submodules: When rendering a module, show its submodules recursively.
+            docstring_section_style: The style used to render docstring sections.
+            merge_init_into_class: Whether to merge the __init__ method into
+                                   the class' signature and docstring.
+            show_if_no_docstring: Show the object heading even if it has no
+                                  docstring or children with docstrings.
+            annotations_path: The verbosity for annotations path
+            line_length: Maximum line length when formatting code/signatures.
+            show_signature: Show methods and functions signatures.
+            show_signature_annotations: Show the type annotations in methods
+                                        and functions signatures.
+            signature_crossrefs: Whether to render cross-references for type
+                                 annotations in signatures.
+            separate_signature: Whether to put the whole signature in a code
+                                block below the heading. If Black is installed,
+                                the signature is also formatted using it.
+            kwargs: Keyword arguments passed to super.
+        """
+        super().__init__(**kwargs)
+        self.obj = obj
+        match obj:
+            case types.ModuleType():
+                self.obj_path = obj.__name__
+            case type() | types.FunctionType() | types.MethodType():
+                if for_topmost:
+                    topmost_path = classhelpers.get_topmost_module_path(obj)
+                    self.obj_path = f"{topmost_path}.{obj.__qualname__}"
+                else:
+                    self.obj_path = f"{obj.__module__}.{obj.__qualname__}"
+            case str():
+                self.obj_path = obj  # for setting a manual path
+            case tuple() | list():
+                self.obj_path = ".".join(obj)
+            case os.PathLike():
+                mod = importlib.import_module(os.fspath(obj))
+                self.obj_path = mod.__name__
+            case _:
+                raise TypeError(obj)
+        self.options = self.OPTIONS_DEFAULT.copy()
+        self.options["allow_inspection"] = allow_inspection
+        self.options["show_bases"] = show_bases
+        self.options["show_source"] = show_source
+        self.options["preload_modules"] = preload_modules
+        self.options["heading_level"] = heading_level
+        self.options["show_root_heading"] = show_root_heading
+        self.options["show_root_toc_entry"] = show_root_toc_entry
+        self.options["show_root_full_path"] = show_root_full_path
+        self.options["show_root_members_full_path"] = show_root_members_full_path
+        self.options["show_object_full_path"] = show_object_full_path
+        self.options["show_category_heading"] = show_category_heading
+        self.options["show_symbol_type_heading"] = show_symbol_type_heading
+        self.options["show_symbol_type_toc"] = show_symbol_type_toc
+        self.options["inherited_members"] = inherited_members
+        self.options["members"] = members
+        self.options["members_order"] = members_order
+        self.options["filters"] = filters
+        self.options["group_by_category"] = group_by_category
+        self.options["show_submodules"] = show_submodules
+        self.options["docstring_section_style"] = docstring_section_style
+        self.options["merge_init_into_class"] = merge_init_into_class
+        self.options["show_if_no_docstring"] = show_if_no_docstring
+        self.options["annotations_path"] = annotations_path
+        self.options["line_length"] = line_length
+        self.options["show_signature"] = show_signature
+        self.options["show_signature_annotations"] = show_signature_annotations
+        self.options["signature_crossrefs"] = signature_crossrefs
+        self.options["separate_signature"] = separate_signature
+        self.options = {k: v for k, v in self.options.items() if v is not None}
+
+    def __repr__(self):
+        return helpers.get_repr(self, obj=self.obj)
+
+    def _to_markdown(self) -> str:
+        md = f"::: {self.obj_path}\n"
+        if self.options:
+            options = "\n".join(f"      {k}: {v!r}" for k, v in self.options.items())
+            md = f"{md}    options:\n{options}\n"
+        return md
+
+
+if __name__ == "__main__":
+    docstrings = MkDocStrings("a.b", show_submodules=True)
+    print(docstrings)
```

### Comparing `mknodes-0.2.0/mknodes/mkmoduletable.py` & `mknodes-0.3.2/mknodes/modulenodes/mkmoduletable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-from __future__ import annotations
-
-from collections.abc import Callable
-import inspect
-import logging
-import types
-
-from mknodes import classhelpers, mktable, utils
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkModuleTable(mktable.MkTable):
-    """Class representing a formatted table containing information a module."""
-
-    def __init__(
-        self,
-        module: types.ModuleType | str | tuple[str, ...],
-        *,
-        predicate: Callable | None = None,
-        **kwargs,
-    ):
-        self.module = classhelpers.to_module(module, return_none=False)
-        dicts = [
-            self.get_row_for_module(submod)
-            for _, submod in inspect.getmembers(self.module, inspect.ismodule)
-            if (predicate is None or predicate(submod)) and "__" not in submod.__name__
-        ]
-        super().__init__(dicts, **kwargs)
-
-    def get_row_for_module(self, module: types.ModuleType) -> dict[str, str]:
-        return dict(
-            Name=module.__name__,
-            # utils.link_for_class(submod, size=4, bold=True),
-            Information=utils.get_first_doc_line(
-                module, fallback="*No docstrings defined.*"
-            ),
-            Members=(
-                utils.to_html_list(module.__all__, make_link=True)
-                if hasattr(module, "__all__")
-                else ""
-            ),
-        )
-
-    # def __repr__(self):
-    #     return utils.get_repr(self, module=self.module)
-
-    @staticmethod
-    def examples():
-        import mknodes
-
-        yield dict(module=mknodes)
-
-
-if __name__ == "__main__":
-    table = MkModuleTable(module=utils)
-    print(table)
+from __future__ import annotations
+
+from collections.abc import Callable
+import inspect
+import logging
+import types
+
+from mknodes import mktable
+from mknodes.utils import classhelpers, helpers
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkModuleTable(mktable.MkTable):
+    """Class representing a formatted table containing information a module."""
+
+    def __init__(
+        self,
+        module: types.ModuleType | str | tuple[str, ...],
+        *,
+        predicate: Callable | None = None,
+        **kwargs,
+    ):
+        self.module = classhelpers.to_module(module, return_none=False)
+        dicts = [
+            self.get_row_for_module(submod)
+            for _, submod in inspect.getmembers(self.module, inspect.ismodule)
+            if (predicate is None or predicate(submod)) and "__" not in submod.__name__
+        ]
+        super().__init__(dicts, **kwargs)
+
+    def get_row_for_module(self, module: types.ModuleType) -> dict[str, str]:
+        return dict(
+            Name=module.__name__,
+            # helpers.link_for_class(submod, size=4, bold=True),
+            Information=helpers.get_first_doc_line(
+                module,
+                fallback="*No docstrings defined.*",
+            ),
+            Members=(
+                helpers.to_html_list(module.__all__, make_link=True)
+                if hasattr(module, "__all__")
+                else ""
+            ),
+        )
+
+    # def __repr__(self):
+    #     return helpers.get_repr(self, module=self.module)
+
+    @staticmethod
+    def examples():
+        import mknodes
+
+        yield dict(module=mknodes)
+
+
+if __name__ == "__main__":
+    table = MkModuleTable(module=helpers)
+    print(table)
```

### Comparing `mknodes-0.2.0/mknodes/mknode.py` & `mknodes-0.3.2/mknodes/mknode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,136 +1,139 @@
-from __future__ import annotations
-
-import logging
-import textwrap
-
-import mkdocs_gen_files
-
-from mknodes import connectionbuilder, node
-
-
-logger = logging.getLogger(__name__)
-
-
-class NodeConnectionBuilder(connectionbuilder.ConnectionBuilder):
-    def get_children(self, item):
-        return item.children
-
-    def get_id(self, item):
-        # id() would be enough, but name is sometimes useful for debugging.
-        return f"{type(item).__name__}_{id(item)}"
-
-    def get_title(self, item) -> str:
-        return f"{type(item).__name__}"
-
-
-class MkNode(node.Node):
-    """Base class for everything which can be expressed as Markup.
-
-    The class inherits from Node. The idea is that starting from the
-    root nav (aka Docs) down to nested Markup blocks, the whole project can be represented
-    by one tree.
-
-    Arguments:
-        header: Optional header for contained Markup
-        indent: Indentation of given Markup (unused ATM)
-        parent: Parent for building the tree
-    """
-
-    def __init__(self, header: str = "", indent: str = "", parent: MkNode | None = None):
-        super().__init__(parent=parent)
-        self.header = header
-        self.indent = indent
-
-    def __str__(self):
-        return self.to_markdown()
-
-    # @staticmethod
-    # def examples():
-    #     yield from ()
-
-    def _to_markdown(self) -> str:
-        return NotImplemented
-
-    def to_markdown(self) -> str:
-        """Outputs markdown for self and all children."""
-        text = self._to_markdown()
-        if self.indent:
-            text = textwrap.indent(text, self.indent)
-        return f"## {self.header}\n\n{text}" if self.header else text
-
-    @property
-    def resolved_parts(self) -> tuple[str, ...]:
-        """Returns a tuple containing all section names."""
-        from mknodes import mknav
-
-        parent = self
-        parts = [self.section] if isinstance(self, mknav.MkNav) and self.section else []
-        while parent := parent.parent_item:
-            if isinstance(parent, mknav.MkNav) and parent.section:
-                parts.append(parent.section)
-        return tuple(reversed(parts))
-
-    @property
-    def resolved_file_path(self) -> str:
-        """Returns the resulting section/subsection/../filename.xyz path."""
-        filename = str(self.path) if hasattr(self, "path") else ""
-        path = "/".join(self.resolved_parts) + "/" + filename
-        return path
-
-    def virtual_files(self):
-        """Returns a dict containing the virtual files attached to this tree element.
-
-        This can be overridden by nodes if they want files to be included in the build.
-        """
-        return {}
-
-    def all_virtual_files(self, only_children: bool = False) -> dict[str, str | bytes]:
-        """Return a dictionary containing all virtual files of itself and all children.
-
-        Dict key contains the filename, dict value contains the file content.
-
-        The resulting filepath is determined based on the tree hierarchy.
-        """
-        from mknodes import mknav
-
-        dct: dict[str, str | bytes] = {}
-        for des in self.descendants:
-            sections = [i.section for i in des.ancestors if isinstance(i, mknav.MkNav)]
-            section = "/".join(i for i in reversed(sections) if i is not None)
-            if section:
-                section += "/"
-            files_for_item = {f"{section}{k}": v for k, v in des.virtual_files().items()}
-            dct |= files_for_item
-        if not only_children:
-            dct |= self.virtual_files()
-        return dct
-
-    def write(self, only_children: bool = False):
-        # path = pathlib.Path(self.path)
-        # path.parent.mkdir(parents=True, exist_ok=True)
-        for k, v in self.all_virtual_files(only_children=only_children).items():
-            logger.info(f"Written file to {k}")
-            mode = "w" if isinstance(v, str) else "wb"
-            with mkdocs_gen_files.open(k, mode) as file:
-                file.write(v)
-
-    def pretty_print(self, _indent: int = 0):
-        """PrettyPrint node and its children."""
-        text = _indent * "    " + repr(self) + "->" + self.resolved_file_path
-        logger.info(text)
-        for child_item in self.children:
-            child_item.pretty_print(_indent + 1)
-
-    def to_tree_graph(self, orientation: str = "TD") -> str:
-        """Returns markdown to display a tree graph of this node and all subnodes.
-
-        Arguments:
-            orientation: Orientation of resulting graph
-        """
-        item_str = NodeConnectionBuilder([self]).get_graph_connection_text()
-        text = f"graph {orientation}\n{item_str}"
-        return f"```mermaid\n{text}\n```"
-
-
-if __name__ == "__main__":
-    section = MkNode(header="fff")
+from __future__ import annotations
+
+import logging
+import textwrap
+
+import mkdocs_gen_files
+
+from mknodes import node
+from mknodes.utils import connectionbuilder
+
+
+logger = logging.getLogger(__name__)
+
+
+class NodeConnectionBuilder(connectionbuilder.ConnectionBuilder):
+    def get_children(self, item):
+        return item.children
+
+    def get_id(self, item):
+        # id() would be enough, but name is sometimes useful for debugging.
+        return f"{type(item).__name__}_{id(item)}"
+
+    def get_title(self, item) -> str:
+        return f"{type(item).__name__}"
+
+
+class MkNode(node.Node):
+    """Base class for everything which can be expressed as Markup.
+
+    The class inherits from Node. The idea is that starting from the
+    root nav (aka Docs) down to nested Markup blocks, the whole project can be represented
+    by one tree.
+
+    Arguments:
+        header: Optional header for contained Markup
+        indent: Indentation of given Markup (unused ATM)
+        parent: Parent for building the tree
+    """
+
+    def __init__(self, header: str = "", indent: str = "", parent: MkNode | None = None):
+        super().__init__(parent=parent)
+        self.header = header
+        self.indent = indent
+
+    def __str__(self):
+        return self.to_markdown()
+
+    # @staticmethod
+    # def examples():
+    #     yield from ()
+
+    def _to_markdown(self) -> str:
+        return NotImplemented
+
+    def to_markdown(self) -> str:
+        """Outputs markdown for self and all children."""
+        text = self._to_markdown()
+        if self.indent:
+            text = textwrap.indent(text, self.indent)
+        return f"## {self.header}\n\n{text}" if self.header else text
+
+    @property
+    def resolved_parts(self) -> tuple[str, ...]:
+        """Returns a tuple containing all section names."""
+        from mknodes import mknav
+
+        parent = self
+        parts = [self.section] if isinstance(self, mknav.MkNav) and self.section else []
+        while parent := parent.parent_item:
+            if isinstance(parent, mknav.MkNav) and parent.section:
+                parts.append(parent.section)
+        return tuple(reversed(parts))
+
+    @property
+    def resolved_file_path(self) -> str:
+        """Returns the resulting section/subsection/../filename.xyz path."""
+        filename = str(self.path) if hasattr(self, "path") else ""
+        return "/".join(self.resolved_parts) + "/" + filename
+
+    def virtual_files(self):
+        """Returns a dict containing the virtual files attached to this tree element.
+
+        This can be overridden by nodes if they want files to be included in the build.
+        """
+        return {}
+
+    @property
+    def resolved_virtual_files(self) -> dict[str, str | bytes]:
+        from mknodes import mknav
+
+        sections = [i.section for i in self.ancestors if isinstance(i, mknav.MkNav)]
+        section = "/".join(i for i in reversed(sections) if i is not None)
+        if section:
+            section += "/"
+        return {f"{section}{k}": v for k, v in self.virtual_files().items()}
+
+    def all_virtual_files(self, only_children: bool = False) -> dict[str, str | bytes]:
+        """Return a dictionary containing all virtual files of itself and all children.
+
+        Dict key contains the filename, dict value contains the file content.
+
+        The resulting filepath is determined based on the tree hierarchy.
+        """
+        all_files: dict[str, str | bytes] = {}
+        for des in self.descendants:
+            all_files |= des.resolved_virtual_files
+        if not only_children:
+            all_files |= self.resolved_virtual_files
+        return all_files
+
+    def write(self, only_children: bool = False):
+        # path = pathlib.Path(self.path)
+        # path.parent.mkdir(parents=True, exist_ok=True)
+        for k, v in self.all_virtual_files(only_children=only_children).items():
+            logger.info("Written file to %s", k)
+            mode = "w" if isinstance(v, str) else "wb"
+            with mkdocs_gen_files.open(k, mode) as file:
+                file.write(v)
+
+    def pretty_print(self, _indent: int = 0):
+        """PrettyPrint node and its children."""
+        text = _indent * "    " + repr(self) + "->" + self.resolved_file_path
+        logger.info(text)
+        for child_item in self.children:
+            child_item.pretty_print(_indent + 1)
+
+    def to_tree_graph(self, orientation: str = "TD") -> str:
+        """Returns markdown to display a tree graph of this node and all subnodes.
+
+        Arguments:
+            orientation: Orientation of resulting graph
+        """
+        item_str = NodeConnectionBuilder([self]).get_graph_connection_text()
+        text = f"graph {orientation}\n{item_str}"
+        return f"```mermaid\n{text}\n```"
+
+
+if __name__ == "__main__":
+    section = MkNode(header="fff")
```

### Comparing `mknodes-0.2.0/mknodes/mkpage.py` & `mknodes-0.3.2/mknodes/mkpage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,320 +1,321 @@
-from __future__ import annotations
-
-from collections.abc import Mapping
-import logging
-import os
-import types
-
-from typing import Any, Literal
-
-from mknodes import (
-    mkadmonition,
-    mkcode,
-    mkcontainer,
-    mkdocstrings,
-    mklink,
-    mknav,
-    mknode,
-    mktabs,
-    utils,
-)
-
-
-logger = logging.getLogger(__name__)
-
-HEADER = "---\n{options}\n---\n\n"
-
-
-class MkPage(mkcontainer.MkContainer):
-    """A node container representing a Markdown page.
-
-    A page contains a list of other Markdown nodes, has a virtual Markdown file
-    associated, and can have metadata (added as header)
-    """
-
-    def __init__(
-        self,
-        path: str | os.PathLike = "",
-        *,
-        hide_toc: bool = False,
-        hide_nav: bool = False,
-        hide_path: bool = False,
-        parent: mknav.MkNav | None = None,
-        **kwargs: Any,
-    ):
-        super().__init__(parent=parent, **kwargs)
-        self.path = path
-        self.header_options: dict[str, Any] = {}
-        if hide_toc:
-            self.header_options.setdefault("hide", []).append("toc")
-        if hide_nav:
-            self.header_options.setdefault("hide", []).append("navigation")
-        if hide_path:
-            self.header_options.setdefault("hide", []).append("path")
-
-    def __repr__(self):
-        return utils.get_repr(self, path=str(self.path))
-
-    def __str__(self):
-        return self.to_markdown()
-
-    def virtual_files(self):
-        return {self.path: self.to_markdown()}
-
-    def to_markdown(self) -> str:
-        header = self.formatted_header()
-        content_str = self._to_markdown()
-        return header + content_str if header else content_str
-
-    def formatted_header(self) -> str:
-        """Return the formatted header (containing metadata) for the page."""
-        lines = []
-        keys = self.header_options.keys()
-        if not keys:
-            return ""
-        for option in keys:
-            lines.append(f"{option}:")
-            lines.extend(f"  - {area}" for area in self.header_options[option])
-        return HEADER.format(options="\n".join(lines))
-
-    def add_newlines(self, num: int):
-        """Add line separators to the page.
-
-        Arguments:
-            num: Amount of newlines to add.
-        """
-        self.append("<br>" * num)
-
-    def add_link(
-        self,
-        url: str,
-        title: str = "",
-    ) -> mklink.MkLink:
-        """Add a Link to the page.
-
-        Arguments:
-            url: URL to link to.
-            title: Text to display for the link
-        """
-        item = mklink.MkLink(url)
-        self.append(item)
-        return item
-
-    def add_header(self, text: str, level: int = 2):
-        """Add line separators to the page.
-
-        Arguments:
-            text: header text
-            level: header level
-        """
-        prefix = "#" * level
-        self.append(f"{prefix} {text}")
-
-    def add_admonition(
-        self,
-        text: str,
-        typ: mkadmonition.AdmonitionTypeStr = "info",
-        *,
-        title: str | None = None,
-        collapsible: bool = False,
-    ) -> mkadmonition.MkAdmonition:
-        """Add a Admonition info box to the page.
-
-        Arguments:
-            text: Text to display inside the box
-            typ: the admonition type
-            title: The title of the box
-            collapsible: whether the box should be collapsible by the user.
-        """
-        item = mkadmonition.MkAdmonition(
-            text=text,
-            typ=typ,
-            title=title,
-            collapsible=collapsible,
-        )
-        self.append(item)
-        return item
-
-    def add_mkdocstrings(
-        self,
-        obj: types.ModuleType | str | os.PathLike | type,
-        *,
-        header: str = "",
-        for_topmost: bool = False,
-        allow_inspection: bool | None = None,
-        show_bases: bool | None = None,
-        show_source: bool | None = None,
-        preload_modules: list[str] | None = None,
-        heading_level: int | None = None,
-        show_root_heading: bool | None = None,
-        show_root_toc_entry: bool | None = None,
-        show_root_full_path: bool | None = None,
-        show_root_members_full_path: bool | None = None,
-        show_object_full_path: bool | None = None,
-        show_category_heading: bool | None = None,
-        show_symbol_type_heading: bool | None = None,
-        show_symbol_type_toc: bool | None = None,
-        members: list[str] | None = None,
-        members_order: Literal["alphabetical", "source"] | None = None,
-        filters: list[str] | None = None,
-        group_by_category: bool | None = None,
-        show_submodules: bool | None = None,
-        docstring_section_style: Literal["table", "list", "spacy"] | None = None,
-        merge_init_into_class: bool | None = None,
-        show_if_no_docstring: bool | None = None,
-        annotations_path: Literal["brief", "source"] | None = None,
-        line_length: int | None = None,
-        show_signature: bool | None = None,
-        show_signature_annotations: bool | None = None,
-        signature_crossrefs: bool | None = None,
-        separate_signature: bool | None = None,
-    ) -> mkdocstrings.MkDocStrings:
-        """Add a DocStrings section to the page.
-
-        Arguments:
-            obj: What to show Docstrings for
-            header: Section header
-            for_topmost: whether to try to find the most topmost module path for given
-                         object
-            allow_inspection: Whether to allow inspecting modules when visiting
-                              them is not possible
-            show_bases: Show the base classes of a class.
-            show_source: Show the source code of this object.
-            preload_modules: List of modules to pre-load.
-            heading_level: The initial heading level to use.
-            show_root_heading: Show the heading of the object at the root of the
-                               documentation tree (i.e. the object referenced by
-                               the identifier after :::).
-            show_root_toc_entry: If the root heading is not shown, at least
-                                 add a ToC entry for it.
-            show_root_full_path: Show the full Python path for the root
-                                 object heading.
-            show_root_members_full_path: Show the full Python path of the
-                                         root members.
-            show_object_full_path: Show the full Python path of every object.
-            show_category_heading: When grouped by categories, show a heading
-                                   for each category.
-            show_symbol_type_heading: Show the symbol type in headings (e.g. mod,
-                                      class, func and attr).
-            show_symbol_type_toc: Show the symbol type in the Table of
-                                  Contents (e.g. mod, class, func and attr).
-            members: An explicit list of members to render.
-            members_order: The members ordering to use.
-            filters: A list of filters applied to filter objects based on their name.
-                     A filter starting with ! will exclude matching objects instead of
-                     including them. The members option takes precedence over filters
-                     (filters will still be applied recursively to lower members in the
-                     hierarchy).
-            group_by_category: Group the object's children by categories:
-                               attributes, classes, functions, and modules.
-            show_submodules: When rendering a module, show its submodules recursively.
-            docstring_section_style: The style used to render docstring sections.
-            merge_init_into_class: Whether to merge the __init__ method into
-                                   the class' signature and docstring.
-            show_if_no_docstring: Show the object heading even if it has no
-                                  docstring or children with docstrings.
-            annotations_path: The verbosity for annotations path
-            line_length: Maximum line length when formatting code/signatures.
-            show_signature: Show methods and functions signatures.
-            show_signature_annotations: Show the type annotations in methods
-                                        and functions signatures.
-            signature_crossrefs: Whether to render cross-references for type
-                                 annotations in signatures.
-            separate_signature: Whether to put the whole signature in a code
-                                block below the heading. If Black is installed,
-                                the signature is also formatted using it.
-        """
-        item = mkdocstrings.MkDocStrings(
-            obj=obj,
-            header=header,
-            for_topmost=for_topmost,
-            allow_inspection=allow_inspection,
-            show_bases=show_bases,
-            show_source=show_source,
-            preload_modules=preload_modules,
-            heading_level=heading_level,
-            show_root_heading=show_root_heading,
-            show_root_toc_entry=show_root_toc_entry,
-            show_root_full_path=show_root_full_path,
-            show_root_members_full_path=show_root_members_full_path,
-            show_object_full_path=show_object_full_path,
-            show_category_heading=show_category_heading,
-            show_symbol_type_heading=show_symbol_type_heading,
-            show_symbol_type_toc=show_symbol_type_toc,
-            members=members,
-            members_order=members_order,
-            filters=filters,
-            group_by_category=group_by_category,
-            show_submodules=show_submodules,
-            docstring_section_style=docstring_section_style,
-            merge_init_into_class=merge_init_into_class,
-            show_if_no_docstring=show_if_no_docstring,
-            annotations_path=annotations_path,
-            line_length=line_length,
-            show_signature=show_signature,
-            show_signature_annotations=show_signature_annotations,
-            signature_crossrefs=signature_crossrefs,
-            separate_signature=separate_signature,
-        )
-        self.append(item)
-        return item
-
-    def add_code(
-        self,
-        code: str | mknode.MkNode,
-        language: str = "py",
-        *,
-        title: str = "",
-        header: str = "",
-        linenums: int | None = None,
-        highlight_lines: list[int] | None = None,
-    ) -> mkcode.MkCode:
-        """Add code block to the page.
-
-        Arguments:
-            code: Code
-            language: language for syntax highlighting
-            title: Optional title for the code block
-            header: Optional header for the code block
-            linenums: Optional start line number for the code block
-            highlight_lines: Optional highlighting of a line range.
-        """
-        item = mkcode.MkCode(
-            code=code,
-            language=language,
-            title=title,
-            header=header,
-            linenums=linenums,
-            highlight_lines=highlight_lines,
-            parent=self,
-        )
-        self.append(item)
-        return item
-
-    def add_tabs(
-        self,
-        data: Mapping[str, str | mknode.MkNode],
-        style: Literal["tabbed", "tabblock"] = "tabbed",
-        **kwargs: Any,
-    ):
-        """Add tabs to the page.
-
-        Arguments:
-            data: tab data
-            style: Whether to use new-style (tabblock) or old-style (tabbed) tabs.
-            kwargs: Keyword arguments passed to Tabs
-        """
-        if style == "tabbed":
-            tabblock = mktabs.MkTabbed(data, parent=self, **kwargs)
-        else:
-            tabblock = mktabs.MkTabBlock(data, parent=self, **kwargs)
-        self.append(tabblock)
-        return tabblock
-
-
-if __name__ == "__main__":
-    doc = MkPage()
-    doc.add_link("test")
-    doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
-    print(doc)
-    # print(doc.children)
+from __future__ import annotations
+
+from collections.abc import Mapping
+import logging
+import os
+import types
+
+from typing import Any, Literal
+
+from mknodes import (
+    mkadmonition,
+    mkcode,
+    mkcontainer,
+    mkdocstrings,
+    mklink,
+    mknav,
+    mknode,
+    mktabcontainer,
+)
+from mknodes.utils import helpers
+
+
+logger = logging.getLogger(__name__)
+
+HEADER = "---\n{options}\n---\n\n"
+
+
+class MkPage(mkcontainer.MkContainer):
+    """A node container representing a Markdown page.
+
+    A page contains a list of other Markdown nodes, has a virtual Markdown file
+    associated, and can have metadata (added as header)
+    """
+
+    def __init__(
+        self,
+        path: str | os.PathLike = "",
+        *,
+        hide_toc: bool = False,
+        hide_nav: bool = False,
+        hide_path: bool = False,
+        parent: mknav.MkNav | None = None,
+        **kwargs: Any,
+    ):
+        super().__init__(parent=parent, **kwargs)
+        self.path = str(path)
+        self.header_options: dict[str, Any] = {}
+        if hide_toc:
+            self.header_options.setdefault("hide", []).append("toc")
+        if hide_nav:
+            self.header_options.setdefault("hide", []).append("navigation")
+        if hide_path:
+            self.header_options.setdefault("hide", []).append("path")
+
+    def __repr__(self):
+        return helpers.get_repr(self, path=str(self.path))
+
+    def __str__(self):
+        return self.to_markdown()
+
+    def virtual_files(self) -> dict[str, str]:
+        return {self.path: self.to_markdown()}
+
+    def to_markdown(self) -> str:
+        header = self.formatted_header()
+        content_str = self._to_markdown()
+        return header + content_str if header else content_str
+
+    def formatted_header(self) -> str:
+        """Return the formatted header (containing metadata) for the page."""
+        lines = []
+        keys = self.header_options.keys()
+        if not keys:
+            return ""
+        for option in keys:
+            lines.append(f"{option}:")
+            lines.extend(f"  - {area}" for area in self.header_options[option])
+        return HEADER.format(options="\n".join(lines))
+
+    def add_newlines(self, num: int):
+        """Add line separators to the page.
+
+        Arguments:
+            num: Amount of newlines to add.
+        """
+        self.append("<br>" * num)
+
+    def add_link(
+        self,
+        url: str,
+        title: str = "",
+    ) -> mklink.MkLink:
+        """Add a Link to the page.
+
+        Arguments:
+            url: URL to link to.
+            title: Text to display for the link
+        """
+        item = mklink.MkLink(url)
+        self.append(item)
+        return item
+
+    def add_header(self, text: str, level: int = 2):
+        """Add line separators to the page.
+
+        Arguments:
+            text: header text
+            level: header level
+        """
+        prefix = "#" * level
+        self.append(f"{prefix} {text}")
+
+    def add_admonition(
+        self,
+        text: str,
+        typ: mkadmonition.AdmonitionTypeStr = "info",
+        *,
+        title: str | None = None,
+        collapsible: bool = False,
+    ) -> mkadmonition.MkAdmonition:
+        """Add a Admonition info box to the page.
+
+        Arguments:
+            text: Text to display inside the box
+            typ: the admonition type
+            title: The title of the box
+            collapsible: whether the box should be collapsible by the user.
+        """
+        item = mkadmonition.MkAdmonition(
+            text=text,
+            typ=typ,
+            title=title,
+            collapsible=collapsible,
+        )
+        self.append(item)
+        return item
+
+    def add_mkdocstrings(
+        self,
+        obj: types.ModuleType | str | os.PathLike | type,
+        *,
+        header: str = "",
+        for_topmost: bool = False,
+        allow_inspection: bool | None = None,
+        show_bases: bool | None = None,
+        show_source: bool | None = None,
+        preload_modules: list[str] | None = None,
+        heading_level: int | None = None,
+        show_root_heading: bool | None = None,
+        show_root_toc_entry: bool | None = None,
+        show_root_full_path: bool | None = None,
+        show_root_members_full_path: bool | None = None,
+        show_object_full_path: bool | None = None,
+        show_category_heading: bool | None = None,
+        show_symbol_type_heading: bool | None = None,
+        show_symbol_type_toc: bool | None = None,
+        members: list[str] | None = None,
+        members_order: Literal["alphabetical", "source"] | None = None,
+        filters: list[str] | None = None,
+        group_by_category: bool | None = None,
+        show_submodules: bool | None = None,
+        docstring_section_style: Literal["table", "list", "spacy"] | None = None,
+        merge_init_into_class: bool | None = None,
+        show_if_no_docstring: bool | None = None,
+        annotations_path: Literal["brief", "source"] | None = None,
+        line_length: int | None = None,
+        show_signature: bool | None = None,
+        show_signature_annotations: bool | None = None,
+        signature_crossrefs: bool | None = None,
+        separate_signature: bool | None = None,
+    ) -> mkdocstrings.MkDocStrings:
+        """Add a DocStrings section to the page.
+
+        Arguments:
+            obj: What to show Docstrings for
+            header: Section header
+            for_topmost: whether to try to find the most topmost module path for given
+                         object
+            allow_inspection: Whether to allow inspecting modules when visiting
+                              them is not possible
+            show_bases: Show the base classes of a class.
+            show_source: Show the source code of this object.
+            preload_modules: List of modules to pre-load.
+            heading_level: The initial heading level to use.
+            show_root_heading: Show the heading of the object at the root of the
+                               documentation tree (i.e. the object referenced by
+                               the identifier after :::).
+            show_root_toc_entry: If the root heading is not shown, at least
+                                 add a ToC entry for it.
+            show_root_full_path: Show the full Python path for the root
+                                 object heading.
+            show_root_members_full_path: Show the full Python path of the
+                                         root members.
+            show_object_full_path: Show the full Python path of every object.
+            show_category_heading: When grouped by categories, show a heading
+                                   for each category.
+            show_symbol_type_heading: Show the symbol type in headings (e.g. mod,
+                                      class, func and attr).
+            show_symbol_type_toc: Show the symbol type in the Table of
+                                  Contents (e.g. mod, class, func and attr).
+            members: An explicit list of members to render.
+            members_order: The members ordering to use.
+            filters: A list of filters applied to filter objects based on their name.
+                     A filter starting with ! will exclude matching objects instead of
+                     including them. The members option takes precedence over filters
+                     (filters will still be applied recursively to lower members in the
+                     hierarchy).
+            group_by_category: Group the object's children by categories:
+                               attributes, classes, functions, and modules.
+            show_submodules: When rendering a module, show its submodules recursively.
+            docstring_section_style: The style used to render docstring sections.
+            merge_init_into_class: Whether to merge the __init__ method into
+                                   the class' signature and docstring.
+            show_if_no_docstring: Show the object heading even if it has no
+                                  docstring or children with docstrings.
+            annotations_path: The verbosity for annotations path
+            line_length: Maximum line length when formatting code/signatures.
+            show_signature: Show methods and functions signatures.
+            show_signature_annotations: Show the type annotations in methods
+                                        and functions signatures.
+            signature_crossrefs: Whether to render cross-references for type
+                                 annotations in signatures.
+            separate_signature: Whether to put the whole signature in a code
+                                block below the heading. If Black is installed,
+                                the signature is also formatted using it.
+        """
+        item = mkdocstrings.MkDocStrings(
+            obj=obj,
+            header=header,
+            for_topmost=for_topmost,
+            allow_inspection=allow_inspection,
+            show_bases=show_bases,
+            show_source=show_source,
+            preload_modules=preload_modules,
+            heading_level=heading_level,
+            show_root_heading=show_root_heading,
+            show_root_toc_entry=show_root_toc_entry,
+            show_root_full_path=show_root_full_path,
+            show_root_members_full_path=show_root_members_full_path,
+            show_object_full_path=show_object_full_path,
+            show_category_heading=show_category_heading,
+            show_symbol_type_heading=show_symbol_type_heading,
+            show_symbol_type_toc=show_symbol_type_toc,
+            members=members,
+            members_order=members_order,
+            filters=filters,
+            group_by_category=group_by_category,
+            show_submodules=show_submodules,
+            docstring_section_style=docstring_section_style,
+            merge_init_into_class=merge_init_into_class,
+            show_if_no_docstring=show_if_no_docstring,
+            annotations_path=annotations_path,
+            line_length=line_length,
+            show_signature=show_signature,
+            show_signature_annotations=show_signature_annotations,
+            signature_crossrefs=signature_crossrefs,
+            separate_signature=separate_signature,
+        )
+        self.append(item)
+        return item
+
+    def add_code(
+        self,
+        code: str | mknode.MkNode,
+        language: str = "py",
+        *,
+        title: str = "",
+        header: str = "",
+        linenums: int | None = None,
+        highlight_lines: list[int] | None = None,
+    ) -> mkcode.MkCode:
+        """Add code block to the page.
+
+        Arguments:
+            code: Code
+            language: language for syntax highlighting
+            title: Optional title for the code block
+            header: Optional header for the code block
+            linenums: Optional start line number for the code block
+            highlight_lines: Optional highlighting of a line range.
+        """
+        item = mkcode.MkCode(
+            code=code,
+            language=language,
+            title=title,
+            header=header,
+            linenums=linenums,
+            highlight_lines=highlight_lines,
+            parent=self,
+        )
+        self.append(item)
+        return item
+
+    def add_tabs(
+        self,
+        data: Mapping[str, str | mknode.MkNode],
+        *,
+        style: Literal["tabbed", "tabblock"] = "tabbed",
+        **kwargs: Any,
+    ):
+        """Add tabs to the page.
+
+        Arguments:
+            data: tab data
+            style: Whether to use new-style (tabblock) or old-style (tabbed) tabs.
+            kwargs: Keyword arguments passed to Tabs
+        """
+        if style == "tabbed":
+            tabblock = mktabcontainer.MkTabbed(data, parent=self, **kwargs)
+        else:
+            tabblock = mktabcontainer.MkTabBlock(data, parent=self, **kwargs)
+        self.append(tabblock)
+        return tabblock
+
+
+if __name__ == "__main__":
+    doc = MkPage()
+    doc.add_link("test")
+    doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
+    print(doc)
+    # print(doc.children)
```

### Comparing `mknodes-0.2.0/mknodes/mkpageinclude.py` & `mknodes-0.3.2/mknodes/mkpageinclude.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-from __future__ import annotations
-
-import logging
-import os
-import pathlib
-
-from typing import Literal
-
-from mknodes import mknode, mkpage
-
-
-logger = logging.getLogger(__name__)
-
-CriticMarkStr = Literal["addition", "deletion", "substitution", "comment", "highlight"]
-
-
-class MkPageInclude(mknode.MkNode):
-    """MkCritic block."""
-
-    def __init__(
-        self,
-        page: str | os.PathLike | mkpage.MkPage,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.page = page
-
-    def _to_markdown(self) -> str:
-        match self.page:
-            case os.PathLike() | str():
-                left, right = "{%", "%}"
-                text = pathlib.Path(self.page).read_text()
-                return f"{{{left}\n\n{text}\n\n{right}}}"
-            case mkpage.MkPage():
-                return str(self.page)
-            case _:
-                raise TypeError(self.page)
-
-    @staticmethod
-    def examples():
-        yield dict(page=mkpage.MkPage(items=["test"]))
-
-
-if __name__ == "__main__":
-    mkcritic = MkPageInclude(page=mkpage.MkPage(items=["test"]))
-    print(mkcritic)
+from __future__ import annotations
+
+import logging
+import os
+import pathlib
+
+from typing import Literal
+
+from mknodes import mknode, mkpage
+
+
+logger = logging.getLogger(__name__)
+
+CriticMarkStr = Literal["addition", "deletion", "substitution", "comment", "highlight"]
+
+
+class MkPageInclude(mknode.MkNode):
+    """MkCritic block."""
+
+    def __init__(
+        self,
+        page: str | os.PathLike | mkpage.MkPage,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.page = page
+
+    def _to_markdown(self) -> str:
+        match self.page:
+            # case os.PathLike() | str():
+            #     left, right = "{%", "%}"
+            #     text = pathlib.Path(self.page).read_text()
+            #     return f"{left}\n\n{text}\n\n{right}"
+            case os.PathLike() | str():
+                return pathlib.Path(self.page).read_text()
+            case mkpage.MkPage():
+                return str(self.page)
+            case _:
+                raise TypeError(self.page)
+
+    @staticmethod
+    def examples():
+        yield dict(page=mkpage.MkPage(items=["test"]))
+
+
+if __name__ == "__main__":
+    page = mkpage.MkPage(items=["test"])
+    include = MkPageInclude(page=__file__)
+    print(include)
```

### Comparing `mknodes-0.2.0/mknodes/mksnippet.py` & `mknodes-0.3.2/mknodes/mksnippet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from __future__ import annotations
-
-import logging
-import os
-
-from mknodes import mknode, utils
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkSnippet(mknode.MkNode):
-    """Snippet to include markdown from another file.
-
-    [More info](https://facelessuser.github.io/pymdown-extensions/extensions/snippets/)
-    """
-
-    REQUIRED_EXTENSIONS = "pymdownx.snippets"
-
-    def __init__(self, path: str | os.PathLike, header: str = ""):
-        super().__init__(header)
-        self.path = path
-
-    def __str__(self):
-        return self.to_markdown()
-
-    def __repr__(self):
-        return utils.get_repr(self, path=str(self.path))
-
-    def _to_markdown(self) -> str:
-        return f"--8<--\n{self.path}\n--8<--\n"
-
-
-if __name__ == "__main__":
-    section = MkSnippet("test.md", header="test")
-    print(section.to_markdown())
+from __future__ import annotations
+
+import logging
+import os
+
+from mknodes import mknode
+from mknodes.utils import helpers
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkSnippet(mknode.MkNode):
+    """Snippet to include markdown from another file.
+
+    [More info](https://facelessuser.github.io/pymdown-extensions/extensions/snippets/)
+    """
+
+    REQUIRED_EXTENSIONS = "pymdownx.snippets"
+
+    def __init__(self, path: str | os.PathLike, header: str = ""):
+        super().__init__(header)
+        self.path = path
+
+    def __str__(self):
+        return self.to_markdown()
+
+    def __repr__(self):
+        return helpers.get_repr(self, path=str(self.path))
+
+    def _to_markdown(self) -> str:
+        return f"--8<--\n{self.path}\n--8<--\n"
+
+
+if __name__ == "__main__":
+    section = MkSnippet("test.md", header="test")
+    print(section.to_markdown())
```

### Comparing `mknodes-0.2.0/mknodes/mktable.py` & `mknodes-0.3.2/mknodes/mktable.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from __future__ import annotations
-
-from collections.abc import Callable, Mapping, Sequence
-import logging
-
-from mknodes import mknode
-
-
-logger = logging.getLogger(__name__)
-
-
-class MkTable(mknode.MkNode):
-    """Class representing a formatted table."""
-
-    REQUIRED_EXTENSIONS = "tables"
-
-    def __init__(
-        self,
-        data: Sequence[Sequence[str]] | Sequence[dict] | dict[str, list] | None = None,
-        columns: Sequence[str] | None = None,
-        *,
-        column_modifiers: dict[str, Callable[[str], str]] | None = None,
-        header: str = "",
-        **kwargs,
-    ):
-        super().__init__(header=header, **kwargs)
-        column_modifiers = column_modifiers or {}
-        match data:
-            case None:
-                self.data = {}
-            case Mapping():
-                self.data = {str(k): [str(i) for i in v] for k, v in data.items()}
-            case ((str(), *_), *_):
-                h = columns or [str(i) for i in range(len(data))]
-                self.data = {}
-                for i, col in enumerate(data):
-                    self.data[h[i]] = [str(j) for j in col]
-            case (dict(), *_):
-                self.data = {k: [dic[k] for dic in data] for k in data[0]}  # type: ignore
-            case ():
-                self.data = {}
-            case _:
-                raise TypeError(data)
-        for k, v in column_modifiers.items():
-            self.data[k] = [v(i) for i in self.data[k]]
-
-    def _to_markdown(self) -> str:
-        if not any(self.data[k] for k in self.data.keys()):
-            return ""
-        formatters = [f"{{:<{self.width_for_column(c)}}}" for c in self.data.keys()]
-        headers = [formatters[i].format(k) for i, k in enumerate(self.data.keys())]
-        divider = [self.width_for_column(c) * "-" for c in self.data.keys()]
-        data = [
-            [formatters[i].format(k) for i, k in enumerate(row)]
-            for row in self._iter_rows()
-        ]
-        header_txt = "| " + " | ".join(headers) + " |"
-        divider_text = "| " + " | ".join(divider) + " |"
-        data_txt = ["| " + " | ".join(line) + " |" for line in data]
-        return "\n".join([header_txt, divider_text, *data_txt])
-
-    @staticmethod
-    def examples():
-        yield dict(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
-        dicts = [{"col 1": "abc", "col 2": "cde"}, {"col 1": "fgh", "col 2": "ijk"}]
-        yield dict(data=dicts)
-
-    def _iter_rows(self):
-        length = min(len(i) for i in self.data.values())
-        for j, _ in enumerate(range(length)):
-            yield [self.data[k][j] or "" for k in self.data.keys()]
-
-    def width_for_column(self, column: str | int):
-        """Returns the minimum width needed for given column.
-
-        Arguments:
-            column: Name or index of the column
-        """
-        if isinstance(column, int):
-            column = list(self.data.keys())[column]
-        max_len = max((len(str(i)) for i in self.data[column]), default=0)
-        return max(len(column), max_len)
-
-    @classmethod
-    def for_items(cls, items, columns: dict[str, Callable]):
-        ls = [{k: v(item) for k, v in columns.items()} for item in items]
-        return cls(ls)
-
-
-if __name__ == "__main__":
-    table = MkTable(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
-    print(table)
+from __future__ import annotations
+
+from collections.abc import Callable, Mapping, Sequence
+import logging
+
+from mknodes import mknode
+
+
+logger = logging.getLogger(__name__)
+
+
+class MkTable(mknode.MkNode):
+    """Class representing a formatted table."""
+
+    REQUIRED_EXTENSIONS = "tables"
+
+    def __init__(
+        self,
+        data: Sequence[Sequence[str]] | Sequence[dict] | dict[str, list] | None = None,
+        columns: Sequence[str] | None = None,
+        *,
+        column_modifiers: dict[str, Callable[[str], str]] | None = None,
+        header: str = "",
+        **kwargs,
+    ):
+        super().__init__(header=header, **kwargs)
+        column_modifiers = column_modifiers or {}
+        match data:
+            case None:
+                self.data = {}
+            case Mapping():
+                self.data = {str(k): [str(i) for i in v] for k, v in data.items()}
+            case ((str(), *_), *_):
+                h = columns or [str(i) for i in range(len(data))]
+                self.data = {}
+                for i, col in enumerate(data):
+                    self.data[h[i]] = [str(j) for j in col]
+            case (dict(), *_):
+                self.data = {k: [dic[k] for dic in data] for k in data[0]}  # type: ignore
+            case ():
+                self.data = {}
+            case _:
+                raise TypeError(data)
+        for k, v in column_modifiers.items():
+            self.data[k] = [v(i) for i in self.data[k]]
+
+    def _to_markdown(self) -> str:
+        if not any(self.data[k] for k in self.data):
+            return ""
+        formatters = [f"{{:<{self.width_for_column(c)}}}" for c in self.data]
+        headers = [formatters[i].format(k) for i, k in enumerate(self.data.keys())]
+        divider = [self.width_for_column(c) * "-" for c in self.data]
+        data = [
+            [formatters[i].format(k) for i, k in enumerate(row)]
+            for row in self._iter_rows()
+        ]
+        header_txt = "| " + " | ".join(headers) + " |"
+        divider_text = "| " + " | ".join(divider) + " |"
+        data_txt = ["| " + " | ".join(line) + " |" for line in data]
+        return "\n".join([header_txt, divider_text, *data_txt])
+
+    @staticmethod
+    def examples():
+        yield dict(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
+        dicts = [{"col 1": "abc", "col 2": "cde"}, {"col 1": "fgh", "col 2": "ijk"}]
+        yield dict(data=dicts)
+
+    def _iter_rows(self):
+        length = min(len(i) for i in self.data.values())
+        for j, _ in enumerate(range(length)):
+            yield [self.data[k][j] or "" for k in self.data]
+
+    def width_for_column(self, column: str | int):
+        """Returns the minimum width needed for given column.
+
+        Arguments:
+            column: Name or index of the column
+        """
+        if isinstance(column, int):
+            column = list(self.data.keys())[column]
+        max_len = max((len(str(i)) for i in self.data[column]), default=0)
+        return max(len(column), max_len)
+
+    @classmethod
+    def for_items(cls, items, columns: dict[str, Callable]):
+        ls = [{k: v(item) for k, v in columns.items()} for item in items]
+        return cls(ls)
+
+
+if __name__ == "__main__":
+    table = MkTable(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
+    print(table)
```

### Comparing `mknodes-0.2.0/mknodes/noderesolver.py` & `mknodes-0.3.2/mknodes/utils/noderesolver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,346 +1,345 @@
-from __future__ import annotations
-
-import logging
-import re
-
-from typing import Any
-
-
-_MAXCACHE = 20
-
-logger = logging.getLogger(__name__)
-
-
-# based on anyTree resolver, credits to them.
-
-
-class BaseResolver:
-    _match_cache: dict[tuple[str, bool], re.Pattern] = {}
-
-    def __init__(self, ignore_case: bool = False):
-        """Base resolver. Subclass to get glob functionality.
-
-        Keyword Args:
-            name (str): Name of the node attribute to be used for resolving
-            ignore_case (bool): Enable case insensisitve handling.
-        """
-        super().__init__()
-        self.ignore_case = ignore_case
-
-    def get_parent(self, node):
-        return NotImplemented
-
-    def get_children(self, node):
-        return NotImplemented
-
-    def get_attribute(self, node):
-        return NotImplemented
-
-    def get_root(self, node):
-        prev = node
-        while node:
-            node = self.get_parent(node)
-            prev = node
-        return prev
-
-    def get_separator(self, node) -> str:
-        return "/"
-
-    def get(self, path: str, root_node):
-        """Return instance at `path`.
-
-        An example module tree:
-
-        >>> top = Node("top", parent=None)
-        >>> sub0 = Node("sub0", parent=top)
-        >>> sub0sub0 = Node("sub0sub0", parent=sub0)
-        >>> sub0sub1 = Node("sub0sub1", parent=sub0)
-        >>> sub1 = Node("sub1", parent=top)
-
-        A resolver using the `name` attribute:
-
-        >>> r = Resolver('name')
-
-        Relative paths:
-
-        >>> r.get(top, "sub0/sub0sub0")
-        Node('/top/sub0/sub0sub0')
-        >>> r.get(sub1, "..")
-        Node('/top')
-        >>> r.get(sub1, "../sub0/sub0sub1")
-        Node('/top/sub0/sub0sub1')
-        >>> r.get(sub1, ".")
-        Node('/top/sub1')
-        >>> r.get(sub1, "")
-        Node('/top/sub1')
-        >>> r.get(top, "sub2")
-        Traceback (most recent call last):
-          ...
-        ChildResolverError: Node('/top') has no child sub2.
-        Children are: 'sub0', 'sub1'.
-
-        Absolute paths:
-
-        >>> r.get(sub0sub0, "/top")
-        Node('/top')
-        >>> r.get(sub0sub0, "/top/sub0")
-        Node('/top/sub0')
-        >>> r.get(sub0sub0, "/")
-        Traceback (most recent call last):
-          ...
-        ResolverError: root node missing. root is '/top'.
-        >>> r.get(sub0sub0, "/bar")
-        Traceback (most recent call last):
-          ...
-        ResolverError: unknown root node '/bar'. root is '/top'.
-
-        Going above the root node raises a :any:`RootResolverError`:
-
-        >>> r.get(top, "..")
-        Traceback (most recent call last):
-            ...
-        RootResolverError: Cannot go above root node Node('/top')
-
-        Case insensitive matching:
-
-        >>> r.get(top, '/TOP')
-        Traceback (most recent call last):
-            ...
-        ResolverError: unknown root node '/TOP'. root is '/top'.
-
-        >>> r = Resolver('name', ignore_case=True)
-        >>> r.get(top, '/TOp')
-        Node('/top')
-        """
-        node, parts = self._start(root_node, path, self.__cmp)
-        for part in parts:
-            if part == "..":
-                parent = self.get_parent(node)
-                if parent is None:
-                    raise RootResolverError(node)
-                node = parent
-            elif part not in ("", "."):
-                node = self.__get(node, part)
-        return node
-
-    def __get(self, node, name):
-        for child in self.get_children(node):
-            if self.__cmp(self.get_attribute(child), str(name)):
-                return child
-        names = [repr(self.get_attribute(c)) for c in self.get_children(node)]
-        raise ChildResolverError(node, name, names)
-
-    def glob(self, path: str, root_node):
-        """Return instances at `path` supporting wildcards.
-
-        Behaves identical to :any:`get`, but accepts wildcards and returns
-        a list of found nodes.
-
-        * `*` matches any characters, except '/'.
-        * `?` matches a single character, except '/'.
-
-        An example module tree:
-
-        >>> top = Node("top", parent=None)
-        >>> sub0 = Node("sub0", parent=top)
-        >>> sub0sub0 = Node("sub0", parent=sub0)
-        >>> sub0sub1 = Node("sub1", parent=sub0)
-        >>> sub1 = Node("sub1", parent=top)
-        >>> sub1sub0 = Node("sub0", parent=sub1)
-
-        A resolver using the `name` attribute:
-
-        >>> r = Resolver('name')
-
-        Relative paths:
-
-        >>> r.glob(top, "sub0/sub?")
-        [Node('/top/sub0/sub0'), Node('/top/sub0/sub1')]
-        >>> r.glob(sub1, ".././*")
-        [Node('/top/sub0'), Node('/top/sub1')]
-        >>> r.glob(top, "*/*")
-        [Node('/top/sub0/sub0'), Node('/top/sub0/sub1'), Node('/top/sub1/sub0')]
-        >>> r.glob(top, "*/sub0")
-        [Node('/top/sub0/sub0'), Node('/top/sub1/sub0')]
-        >>> r.glob(top, "sub1/sub1")
-        Traceback (most recent call last):
-            ...
-        ChildResolverError: Node('/top/sub1') has no child sub1.
-        Children are: 'sub0'.
-
-        Non-matching wildcards are no error:
-
-        >>> r.glob(top, "bar*")
-        []
-        >>> r.glob(top, "sub2")
-        Traceback (most recent call last):
-          ...
-        ChildResolverError: Node('/top') has no child sub2.
-        Children are: 'sub0', 'sub1'.
-
-        Absolute paths:
-
-        >>> r.glob(sub0sub0, "/top/*")
-        [Node('/top/sub0'), Node('/top/sub1')]
-        >>> r.glob(sub0sub0, "/")
-        Traceback (most recent call last):
-          ...
-        ResolverError: root node missing. root is '/top'.
-        >>> r.glob(sub0sub0, "/bar")
-        Traceback (most recent call last):
-          ...
-        ResolverError: unknown root node '/bar'. root is '/top'.
-
-        Going above the root node raises a :any:`RootResolverError`:
-
-        >>> r.glob(top, "..")
-        Traceback (most recent call last):
-            ...
-        RootResolverError: Cannot go above root node Node('/top')
-        """
-        node, parts = self._start(root_node, path, self.__match)
-        return self._glob(node, parts)
-
-    def _start(self, node, path: str, cmp_) -> tuple[Any, list[str]]:
-        sep = self.get_separator(node)
-        parts = path.split(sep)
-        # resolve root
-        if path.startswith(sep):
-            node = self.get_root(node)
-            rootpart = self.get_attribute(node)
-            parts.pop(0)
-            if not parts[0]:
-                msg = f"root node missing. root is '{sep}{rootpart}'."
-                raise ResolverError(node, "", msg)
-            if not cmp_(rootpart, parts[0]):
-                msg = f"unknown root node '{sep}{parts[0]}'. root is '{sep}{rootpart}'."
-                raise ResolverError(node, "", msg)
-            parts.pop(0)
-        return node, parts
-
-    def _glob(self, node, parts):
-        assert node is not None
-        nodes = []
-        if parts:
-            name = parts[0]
-            remainder = parts[1:]
-            # handle relative
-            if name == "..":
-                parent = self.get_parent(node)
-                if parent is None:
-                    raise RootResolverError(node)
-                else:
-                    nodes += self._glob(parent, remainder)
-            elif name in ("", "."):
-                nodes += self._glob(node, remainder)
-            elif matches := self._find(node, name, remainder):
-                nodes += matches
-            elif self.is_wildcard(name):
-                nodes += matches
-            else:
-                names = [repr(self.get_attribute(c)) for c in self.get_children(node)]
-                raise ChildResolverError(node, name, names)
-        else:
-            nodes = [node]
-        return nodes
-
-    def _find(self, node, pat: str, remainder) -> list:
-        matches = []
-        for child in self.get_children(node):
-            name = self.get_attribute(child)
-            try:
-                if self.__match(name, pat):
-                    if remainder:
-                        matches += self._glob(child, remainder)
-                    else:
-                        matches.append(child)
-            except ResolverError as exc:  # noqa: PERF203
-                if not self.is_wildcard(pat):
-                    raise exc
-        return matches
-
-    @staticmethod
-    def is_wildcard(path: str) -> bool:
-        """Return `True` is a wildcard."""
-        return "?" in path or "*" in path
-
-    def __match(self, name: str, pat: str) -> bool:
-        k = (pat, self.ignore_case)
-        try:
-            re_pat = self._match_cache[k]
-        except KeyError:
-            res = self.__translate(pat)
-            if len(self._match_cache) >= _MAXCACHE:
-                self._match_cache.clear()
-            flags = 0
-            if self.ignore_case:
-                flags |= re.IGNORECASE
-            self._match_cache[k] = re_pat = re.compile(res, flags=flags)
-        return re_pat.match(name) is not None
-
-    def __cmp(self, name, pat):
-        return name.upper() == pat.upper() if self.ignore_case else name == pat
-
-    @staticmethod
-    def __translate(pat: str) -> str:
-        re_pat = ""
-        for char in pat:
-            if char == "*":
-                re_pat += ".*"
-            elif char == "?":
-                re_pat += "."
-            else:
-                re_pat += re.escape(char)
-        return f"(?ms){re_pat}" + r"\Z"  # noqa: ISC003
-
-
-class ResolverError(RuntimeError):
-    def __init__(self, node, child, msg):
-        """Resolve Error at `node` handling `child`."""
-        super().__init__(msg)
-        self.node = node
-        self.child = child
-
-
-class RootResolverError(ResolverError):
-    def __init__(self, root):
-        """Root Resolve Error, cannot go above root node."""
-        msg = f"Cannot go above root node {root!r}"
-        super().__init__(root, None, msg)
-
-
-class ChildResolverError(ResolverError):
-    def __init__(self, node, child, names):
-        """Child Resolve Error at `node` handling `child`."""
-        msg = "{!r} has no child {}. Children are: {}.".format(
-            node, child, ", ".join(names)
-        )
-        super().__init__(node, child, msg)
-
-
-class NodeResolver(BaseResolver):
-    def __init__(self, path_attr: str = "obj", ignore_case: bool = False):
-        """Resolve any `Node` paths using attribute `path_attr`.
-
-        Arguments:
-            path_attr: Name of the node attribute to be used for resolving
-            ignore_case: Enable case insensisitve handling.
-        """
-        super().__init__(ignore_case=ignore_case)
-        self.path_attr = path_attr
-
-    def get_parent(self, node):
-        return node.parent
-
-    def get_children(self, node):
-        return node.children
-
-    def get_root(self, node):
-        return node.root
-
-    def get_attribute(self, node):
-        return getattr(node, self.path_attr)
-
-
-if __name__ == "__main__":
-    resolver = NodeResolver()
+from __future__ import annotations
+
+import logging
+import re
+
+from typing import Any
+
+
+_MAXCACHE = 20
+
+logger = logging.getLogger(__name__)
+
+
+# based on anyTree resolver, credits to them.
+
+
+class BaseResolver:
+    _match_cache: dict[tuple[str, bool], re.Pattern] = {}
+
+    def __init__(self, ignore_case: bool = False):
+        """Base resolver. Subclass to get glob functionality.
+
+        Keyword Args:
+            name (str): Name of the node attribute to be used for resolving
+            ignore_case (bool): Enable case insensisitve handling.
+        """
+        super().__init__()
+        self.ignore_case = ignore_case
+
+    def get_parent(self, node):
+        return NotImplemented
+
+    def get_children(self, node):
+        return NotImplemented
+
+    def get_attribute(self, node):
+        return NotImplemented
+
+    def get_root(self, node):
+        prev = node
+        while node:
+            node = self.get_parent(node)
+            prev = node
+        return prev
+
+    def get_separator(self, node) -> str:
+        return "/"
+
+    def get(self, path: str, root_node):
+        """Return instance at `path`.
+
+        An example module tree:
+
+        >>> top = Node("top", parent=None)
+        >>> sub0 = Node("sub0", parent=top)
+        >>> sub0sub0 = Node("sub0sub0", parent=sub0)
+        >>> sub0sub1 = Node("sub0sub1", parent=sub0)
+        >>> sub1 = Node("sub1", parent=top)
+
+        A resolver using the `name` attribute:
+
+        >>> r = Resolver('name')
+
+        Relative paths:
+
+        >>> r.get(top, "sub0/sub0sub0")
+        Node('/top/sub0/sub0sub0')
+        >>> r.get(sub1, "..")
+        Node('/top')
+        >>> r.get(sub1, "../sub0/sub0sub1")
+        Node('/top/sub0/sub0sub1')
+        >>> r.get(sub1, ".")
+        Node('/top/sub1')
+        >>> r.get(sub1, "")
+        Node('/top/sub1')
+        >>> r.get(top, "sub2")
+        Traceback (most recent call last):
+          ...
+        ChildResolverError: Node('/top') has no child sub2.
+        Children are: 'sub0', 'sub1'.
+
+        Absolute paths:
+
+        >>> r.get(sub0sub0, "/top")
+        Node('/top')
+        >>> r.get(sub0sub0, "/top/sub0")
+        Node('/top/sub0')
+        >>> r.get(sub0sub0, "/")
+        Traceback (most recent call last):
+          ...
+        ResolverError: root node missing. root is '/top'.
+        >>> r.get(sub0sub0, "/bar")
+        Traceback (most recent call last):
+          ...
+        ResolverError: unknown root node '/bar'. root is '/top'.
+
+        Going above the root node raises a :any:`RootResolverError`:
+
+        >>> r.get(top, "..")
+        Traceback (most recent call last):
+            ...
+        RootResolverError: Cannot go above root node Node('/top')
+
+        Case insensitive matching:
+
+        >>> r.get(top, '/TOP')
+        Traceback (most recent call last):
+            ...
+        ResolverError: unknown root node '/TOP'. root is '/top'.
+
+        >>> r = Resolver('name', ignore_case=True)
+        >>> r.get(top, '/TOp')
+        Node('/top')
+        """
+        node, parts = self._start(root_node, path, self.__cmp)
+        for part in parts:
+            if part == "..":
+                parent = self.get_parent(node)
+                if parent is None:
+                    raise RootResolverError(node)
+                node = parent
+            elif part not in ("", "."):
+                node = self.__get(node, part)
+        return node
+
+    def __get(self, node, name):
+        for child in self.get_children(node):
+            if self.__cmp(self.get_attribute(child), str(name)):
+                return child
+        names = [repr(self.get_attribute(c)) for c in self.get_children(node)]
+        raise ChildResolverError(node, name, names)
+
+    def glob(self, path: str, root_node):
+        """Return instances at `path` supporting wildcards.
+
+        Behaves identical to :any:`get`, but accepts wildcards and returns
+        a list of found nodes.
+
+        * `*` matches any characters, except '/'.
+        * `?` matches a single character, except '/'.
+
+        An example module tree:
+
+        >>> top = Node("top", parent=None)
+        >>> sub0 = Node("sub0", parent=top)
+        >>> sub0sub0 = Node("sub0", parent=sub0)
+        >>> sub0sub1 = Node("sub1", parent=sub0)
+        >>> sub1 = Node("sub1", parent=top)
+        >>> sub1sub0 = Node("sub0", parent=sub1)
+
+        A resolver using the `name` attribute:
+
+        >>> r = Resolver('name')
+
+        Relative paths:
+
+        >>> r.glob(top, "sub0/sub?")
+        [Node('/top/sub0/sub0'), Node('/top/sub0/sub1')]
+        >>> r.glob(sub1, ".././*")
+        [Node('/top/sub0'), Node('/top/sub1')]
+        >>> r.glob(top, "*/*")
+        [Node('/top/sub0/sub0'), Node('/top/sub0/sub1'), Node('/top/sub1/sub0')]
+        >>> r.glob(top, "*/sub0")
+        [Node('/top/sub0/sub0'), Node('/top/sub1/sub0')]
+        >>> r.glob(top, "sub1/sub1")
+        Traceback (most recent call last):
+            ...
+        ChildResolverError: Node('/top/sub1') has no child sub1.
+        Children are: 'sub0'.
+
+        Non-matching wildcards are no error:
+
+        >>> r.glob(top, "bar*")
+        []
+        >>> r.glob(top, "sub2")
+        Traceback (most recent call last):
+          ...
+        ChildResolverError: Node('/top') has no child sub2.
+        Children are: 'sub0', 'sub1'.
+
+        Absolute paths:
+
+        >>> r.glob(sub0sub0, "/top/*")
+        [Node('/top/sub0'), Node('/top/sub1')]
+        >>> r.glob(sub0sub0, "/")
+        Traceback (most recent call last):
+          ...
+        ResolverError: root node missing. root is '/top'.
+        >>> r.glob(sub0sub0, "/bar")
+        Traceback (most recent call last):
+          ...
+        ResolverError: unknown root node '/bar'. root is '/top'.
+
+        Going above the root node raises a :any:`RootResolverError`:
+
+        >>> r.glob(top, "..")
+        Traceback (most recent call last):
+            ...
+        RootResolverError: Cannot go above root node Node('/top')
+        """
+        node, parts = self._start(root_node, path, self.__match)
+        return self._glob(node, parts)
+
+    def _start(self, node, path: str, cmp_) -> tuple[Any, list[str]]:
+        sep = self.get_separator(node)
+        parts = path.split(sep)
+        # resolve root
+        if path.startswith(sep):
+            node = self.get_root(node)
+            rootpart = self.get_attribute(node)
+            parts.pop(0)
+            if not parts[0]:
+                msg = f"root node missing. root is '{sep}{rootpart}'."
+                raise ResolverError(node, "", msg)
+            if not cmp_(rootpart, parts[0]):
+                msg = f"unknown root node '{sep}{parts[0]}'. root is '{sep}{rootpart}'."
+                raise ResolverError(node, "", msg)
+            parts.pop(0)
+        return node, parts
+
+    def _glob(self, node, parts):
+        assert node is not None
+        nodes = []
+        if parts:
+            name = parts[0]
+            remainder = parts[1:]
+            # handle relative
+            if name == "..":
+                parent = self.get_parent(node)
+                if parent is None:
+                    raise RootResolverError(node)
+                nodes += self._glob(parent, remainder)
+            elif name in ("", "."):
+                nodes += self._glob(node, remainder)
+            elif (matches := self._find(node, name, remainder)) or self.is_wildcard(name):
+                nodes += matches
+            else:
+                names = [repr(self.get_attribute(c)) for c in self.get_children(node)]
+                raise ChildResolverError(node, name, names)
+        else:
+            nodes = [node]
+        return nodes
+
+    def _find(self, node, pat: str, remainder) -> list:
+        matches = []
+        for child in self.get_children(node):
+            name = self.get_attribute(child)
+            try:
+                if self.__match(name, pat):
+                    if remainder:
+                        matches += self._glob(child, remainder)
+                    else:
+                        matches.append(child)
+            except ResolverError:  # noqa: PERF203
+                if not self.is_wildcard(pat):
+                    raise
+        return matches
+
+    @staticmethod
+    def is_wildcard(path: str) -> bool:
+        """Return `True` is a wildcard."""
+        return "?" in path or "*" in path
+
+    def __match(self, name: str, pat: str) -> bool:
+        k = (pat, self.ignore_case)
+        try:
+            re_pat = self._match_cache[k]
+        except KeyError:
+            res = self.__translate(pat)
+            if len(self._match_cache) >= _MAXCACHE:
+                self._match_cache.clear()
+            flags = 0
+            if self.ignore_case:
+                flags |= re.IGNORECASE
+            self._match_cache[k] = re_pat = re.compile(res, flags=flags)
+        return re_pat.match(name) is not None
+
+    def __cmp(self, name, pat):
+        return name.upper() == pat.upper() if self.ignore_case else name == pat
+
+    @staticmethod
+    def __translate(pat: str) -> str:
+        re_pat = ""
+        for char in pat:
+            if char == "*":
+                re_pat += ".*"
+            elif char == "?":
+                re_pat += "."
+            else:
+                re_pat += re.escape(char)
+        return f"(?ms){re_pat}" + r"\Z"  # noqa: ISC003
+
+
+class ResolverError(RuntimeError):
+    def __init__(self, node, child, msg):
+        """Resolve Error at `node` handling `child`."""
+        super().__init__(msg)
+        self.node = node
+        self.child = child
+
+
+class RootResolverError(ResolverError):
+    def __init__(self, root):
+        """Root Resolve Error, cannot go above root node."""
+        msg = f"Cannot go above root node {root!r}"
+        super().__init__(root, None, msg)
+
+
+class ChildResolverError(ResolverError):
+    def __init__(self, node, child, names):
+        """Child Resolve Error at `node` handling `child`."""
+        msg = "{!r} has no child {}. Children are: {}.".format(
+            node,
+            child,
+            ", ".join(names),
+        )
+        super().__init__(node, child, msg)
+
+
+class NodeResolver(BaseResolver):
+    def __init__(self, path_attr: str = "obj", ignore_case: bool = False):
+        """Resolve any `Node` paths using attribute `path_attr`.
+
+        Arguments:
+            path_attr: Name of the node attribute to be used for resolving
+            ignore_case: Enable case insensisitve handling.
+        """
+        super().__init__(ignore_case=ignore_case)
+        self.path_attr = path_attr
+
+    def get_parent(self, node):
+        return node.parent
+
+    def get_children(self, node):
+        return node.children
+
+    def get_root(self, node):
+        return node.root
+
+    def get_attribute(self, node):
+        return getattr(node, self.path_attr)
+
+
+if __name__ == "__main__":
+    resolver = NodeResolver()
```

### Comparing `mknodes-0.2.0/mknodes/utils.py` & `mknodes-0.3.2/mknodes/utils/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,220 +1,211 @@
-from __future__ import annotations
-
-from collections.abc import Callable
-from importlib import metadata
-import inspect
-import itertools
-import logging
-import re
-import reprlib
-import sys
-import types
-
-from typing import Any
-
-
-logger = logging.getLogger(__name__)
-
-BASE_URL = "https://doc.qt.io/qtforpython-6/PySide6/"
-BUILTIN_URL = "https://docs.python.org/3/library/{mod}.html#{name}"
-
-
-class LengthLimitRepr(reprlib.Repr):
-    pass
-
-
-limit_repr = LengthLimitRepr()
-limit_repr.maxlist = 10
-limit_repr.maxstring = 80
-
-
-def get_repr(_obj: Any, *args: Any, _shorten: bool = True, **kwargs: Any) -> str:
-    """Get a suitable __repr__ string for an object.
-
-    Args:
-        _obj: The object to get a repr for.
-        _shorten: Whether to shorten the repr.
-        *args: Arguments for the repr
-        **kwargs: Keyword arguments for the repr
-    """
-    my_repr = limit_repr.repr if _shorten else repr
-    classname = type(_obj).__name__
-    parts = [my_repr(val) for val in args]
-    kw_parts = []
-    for k, v in kwargs.items():
-        if isinstance(v, type | types.ModuleType | types.MethodType | types.FunctionType):
-            name = v.__name__
-        else:
-            name = my_repr(v)
-        kw_parts.append(f"{k}={name}")
-    sig = ", ".join(parts + kw_parts)
-    return f"{classname}({sig})"
-
-
-def escaped(text: str, entity_type: str | None = None) -> str:
-    """Helper function to escape telegram markup symbols.
-
-    Args:
-        text: The text.
-        entity_type: For the entity types ``PRE``, ``CODE`` and the link
-                     part of ``TEXT_LINKS``, only certain characters need to be escaped.
-    """
-    if entity_type in ["pre", "code"]:
-        escape_chars = r"\`"
-    elif entity_type == "text_link":
-        escape_chars = r"\)"
-    else:
-        escape_chars = r"_*[]()~`>#+-=|{}.!"
-
-    return re.sub(f"([{re.escape(escape_chars)}])", r"\\\1", text)
-
-
-def slugify(text: str) -> str:
-    text = text.lower()
-    text = re.sub("[^0-9a-zA-Z_.]", "_", text)
-    text = re.sub("^[^a-zA-Z_#]+", "", text)
-    return text
-
-
-def groupby(data, keyfunc: Callable | None = None) -> dict[str, list]:
-    data = sorted(data, key=keyfunc or (lambda x: x))
-    return {k: list(g) for k, g in itertools.groupby(data, keyfunc)}
-
-
-def groupby_first_letter(data, keyfunc: Callable | None = None) -> dict[str, list]:
-    data = sorted(data, key=keyfunc or (lambda x: x))
-
-    def first_letter(x):
-        return keyfunc(x)[0] if keyfunc else x[0]
-
-    return {k: list(g) for k, g in itertools.groupby(data, first_letter)}
-
-
-# import pathlib
-# from mkdocstrings import inventory
-
-# path = pathlib.Path(__file__, "../qt6.inv")
-# with path.open("rb") as file:
-#     inv = inventory.Inventory.parse_sphinx(file)
-
-#     logger.warning(inv.values())
-
-
-def linked(identifier: str, title: str | None = None) -> str:
-    suffix = (
-        ""
-        if identifier.startswith(("http:", "https:", "www."))
-        or identifier.endswith(".md")
-        else ".md"
-    )
-    return f"[{identifier if title is None else title}]({identifier}{suffix})"
-
-
-def styled(
-    text: str,
-    size: int | None = None,
-    bold: bool = False,
-    recursive: bool = False,
-    code: bool = False,
-) -> str:
-    if size:
-        text = f"<font size='{size}'>{text}</font>"
-    if bold:
-        text = f"**{text}**"
-    if recursive:
-        text = f"*{text}*"
-    if code:
-        text = f"`{text}`"
-    return text
-
-
-def link_for_class(kls: type, **kwargs) -> str:
-    if kls.__module__ == "builtins":
-        url = BUILTIN_URL.format(mod="functions", name=kls.__name__)
-        link = linked(url, title=kls.__name__)
-    elif kls.__module__ in sys.stdlib_module_names:
-        mod = kls.__module__
-        url = BUILTIN_URL.format(mod=mod, name=f"{mod}.{kls.__name__}")
-        link = linked(url, title=kls.__name__)
-    elif kls.__module__.startswith(("PyQt", "PySide")):
-        mod = kls.__module__.replace("PySide6.", "").replace("PyQt6.", "")
-        url = f"{BASE_URL}{mod}/{kls.__qualname__.replace('.', '/')}.html"
-        link = linked(url, title=kls.__name__)
-    elif kls.__module__.startswith("prettyqt"):
-        link = linked(kls.__qualname__)
-    else:
-        try:
-            dist = metadata.distribution(kls.__module__.split(".")[0])
-        except metadata.PackageNotFoundError:
-            link = linked(kls.__qualname__)
-        else:
-            if url := dist.metadata["Home-Page"]:
-                link = linked(url, title=kls.__qualname__)
-            else:
-                link = linked(kls.__qualname__)
-    return styled(link, **kwargs)
-
-
-def label_for_class(klass: type) -> str:
-    if klass.__module__.startswith("prettyqt."):
-        parts = klass.__module__.split(".")
-        return f"{parts[1]}.{klass.__name__}"
-    return f"{klass.__module__.split('.')[-1]}.{klass.__name__}"
-
-
-def to_html_list(
-    ls: list[str], shorten_after: int | None = None, make_link: bool = False
-) -> str:
-    if not ls:
-        return ""
-    item_str = "".join(
-        f"<li>{linked(i)}</li>" if make_link else f"<li>{i}</li>"
-        for i in ls[:shorten_after]
-    )
-    if shorten_after and len(ls) > shorten_after:
-        item_str += "<li>...</li>"
-    return f"<ul>{item_str}</ul>"
-
-
-def format_kwargs(kwargs: dict[str, Any]) -> str:
-    if not kwargs:
-        return ""
-    kw_parts = []
-    for k, v in kwargs.items():
-        if isinstance(v, type | types.ModuleType | types.MethodType | types.FunctionType):
-            name = v.__name__
-        else:
-            name = repr(v)
-        kw_parts.append(f"{k}={name}")
-    return ", ".join(kw_parts)
-
-
-def get_function_body(func: types.MethodType | types.FunctionType | type) -> str:
-    # see https://stackoverflow.com/questions/38050649
-    source_lines = inspect.getsourcelines(func)[0]
-    source_lines = itertools.dropwhile(lambda x: x.startswith("@"), source_lines)
-    line = next(source_lines).strip()  # type: ignore
-    if not line.startswith(("def ", "class ")):
-        return line.rsplit(":")[-1].strip()
-    elif not line.endswith(":"):
-        for line in source_lines:
-            line = line.strip()
-            if line.endswith(":"):
-                break
-    return "".join(source_lines)
-
-
-def get_deprecated_message(obj) -> str | None:
-    return obj.__deprecated__ if hasattr(obj, "__deprecated__") else None
-
-
-def get_first_doc_line(obj, escape: bool = False, fallback: str = "") -> str:
-    doc = obj.__doc__.split("\n")[0] if isinstance(obj.__doc__, str) else fallback
-    if escape:
-        doc = escaped(doc)
-    return doc
-
-
-if __name__ == "__main__":
-    strings = groupby_first_letter([str(i) for i in range(1000)])
-    print(limit_repr.repr(strings))
+from __future__ import annotations
+
+from collections.abc import Callable
+from importlib import metadata
+import inspect
+import itertools
+import logging
+import re
+import reprlib
+import sys
+import types
+
+from typing import Any
+
+
+logger = logging.getLogger(__name__)
+
+BASE_URL = "https://doc.qt.io/qtforpython-6/PySide6/"
+BUILTIN_URL = "https://docs.python.org/3/library/{mod}.html#{name}"
+
+
+class LengthLimitRepr(reprlib.Repr):
+    pass
+
+
+limit_repr = LengthLimitRepr()
+limit_repr.maxlist = 10
+limit_repr.maxstring = 80
+
+
+def get_repr(_obj: Any, *args: Any, _shorten: bool = True, **kwargs: Any) -> str:
+    """Get a suitable __repr__ string for an object.
+
+    Args:
+        _obj: The object to get a repr for.
+        _shorten: Whether to shorten the repr.
+        *args: Arguments for the repr
+        **kwargs: Keyword arguments for the repr
+    """
+    my_repr = limit_repr.repr if _shorten else repr
+    classname = type(_obj).__name__
+    parts = [my_repr(val) for val in args]
+    kw_parts = []
+    for k, v in kwargs.items():
+        if isinstance(v, type | types.ModuleType | types.MethodType | types.FunctionType):
+            name = v.__name__
+        else:
+            name = my_repr(v)
+        kw_parts.append(f"{k}={name}")
+    sig = ", ".join(parts + kw_parts)
+    return f"{classname}({sig})"
+
+
+def escaped(text: str, entity_type: str | None = None) -> str:
+    """Helper function to escape telegram markup symbols.
+
+    Args:
+        text: The text.
+        entity_type: For the entity types ``PRE``, ``CODE`` and the link
+                     part of ``TEXT_LINKS``, only certain characters need to be escaped.
+    """
+    if entity_type in ["pre", "code"]:
+        escape_chars = r"\`"
+    elif entity_type == "text_link":
+        escape_chars = r"\)"
+    else:
+        escape_chars = r"_*[]()~`>#+-=|{}.!"
+
+    return re.sub(f"([{re.escape(escape_chars)}])", r"\\\1", text)
+
+
+def slugify(text: str) -> str:
+    text = text.lower()
+    text = re.sub("[^0-9a-zA-Z_.]", "_", text)
+    return re.sub("^[^a-zA-Z_#]+", "", text)
+
+
+def groupby(data, keyfunc: Callable | None = None) -> dict[str, list]:
+    data = sorted(data, key=keyfunc or (lambda x: x))
+    return {k: list(g) for k, g in itertools.groupby(data, keyfunc)}
+
+
+def groupby_first_letter(data, keyfunc: Callable | None = None) -> dict[str, list]:
+    data = sorted(data, key=keyfunc or (lambda x: x))
+
+    def first_letter(x):
+        return keyfunc(x)[0] if keyfunc else x[0]
+
+    return {k: list(g) for k, g in itertools.groupby(data, first_letter)}
+
+
+def linked(identifier: str, title: str | None = None) -> str:
+    suffix = (
+        ""
+        if identifier.startswith(("http:", "https:", "www."))
+        or identifier.endswith(".md")
+        else ".md"
+    )
+    return f"[{identifier if title is None else title}]({identifier}{suffix})"
+
+
+def styled(
+    text: str,
+    size: int | None = None,
+    bold: bool = False,
+    recursive: bool = False,
+    code: bool = False,
+) -> str:
+    if size:
+        text = f"<font size='{size}'>{text}</font>"
+    if bold:
+        text = f"**{text}**"
+    if recursive:
+        text = f"*{text}*"
+    if code:
+        text = f"`{text}`"
+    return text
+
+
+def link_for_class(kls: type, **kwargs) -> str:
+    if kls.__module__ == "builtins":
+        url = BUILTIN_URL.format(mod="functions", name=kls.__name__)
+        link = linked(url, title=kls.__name__)
+    elif kls.__module__ in sys.stdlib_module_names:
+        mod = kls.__module__
+        url = BUILTIN_URL.format(mod=mod, name=f"{mod}.{kls.__name__}")
+        link = linked(url, title=kls.__name__)
+    elif kls.__module__.startswith(("PyQt", "PySide")):
+        mod = kls.__module__.replace("PySide6.", "").replace("PyQt6.", "")
+        url = f"{BASE_URL}{mod}/{kls.__qualname__.replace('.', '/')}.html"
+        link = linked(url, title=kls.__name__)
+    elif kls.__module__.startswith("prettyqt"):
+        link = linked(kls.__qualname__)
+    else:
+        try:
+            dist = metadata.distribution(kls.__module__.split(".")[0])
+        except metadata.PackageNotFoundError:
+            link = linked(kls.__qualname__)
+        else:
+            if url := dist.metadata["Home-Page"]:
+                link = linked(url, title=kls.__qualname__)
+            else:
+                link = linked(kls.__qualname__)
+    return styled(link, **kwargs)
+
+
+def label_for_class(klass: type) -> str:
+    if klass.__module__.startswith("prettyqt."):
+        parts = klass.__module__.split(".")
+        return f"{parts[1]}.{klass.__name__}"
+    return f"{klass.__module__.split('.')[-1]}.{klass.__name__}"
+
+
+def to_html_list(
+    ls: list[str],
+    shorten_after: int | None = None,
+    make_link: bool = False,
+) -> str:
+    if not ls:
+        return ""
+    item_str = "".join(
+        f"<li>{linked(i)}</li>" if make_link else f"<li>{i}</li>"
+        for i in ls[:shorten_after]
+    )
+    if shorten_after and len(ls) > shorten_after:
+        item_str += "<li>...</li>"
+    return f"<ul>{item_str}</ul>"
+
+
+def format_kwargs(kwargs: dict[str, Any]) -> str:
+    if not kwargs:
+        return ""
+    kw_parts = []
+    for k, v in kwargs.items():
+        if isinstance(v, type | types.ModuleType | types.MethodType | types.FunctionType):
+            name = v.__name__
+        else:
+            name = repr(v)
+        kw_parts.append(f"{k}={name}")
+    return ", ".join(kw_parts)
+
+
+def get_function_body(func: types.MethodType | types.FunctionType | type) -> str:
+    # see https://stackoverflow.com/questions/38050649
+    source_lines = inspect.getsourcelines(func)[0]
+    source_lines = itertools.dropwhile(lambda x: x.startswith("@"), source_lines)
+    line = next(source_lines).strip()  # type: ignore
+    if not line.startswith(("def ", "class ")):
+        return line.rsplit(":")[-1].strip()
+    if not line.endswith(":"):
+        for line in source_lines:
+            line = line.strip()
+            if line.endswith(":"):
+                break
+    return "".join(source_lines)
+
+
+def get_deprecated_message(obj) -> str | None:
+    return obj.__deprecated__ if hasattr(obj, "__deprecated__") else None
+
+
+def get_first_doc_line(obj, escape: bool = False, fallback: str = "") -> str:
+    doc = obj.__doc__.split("\n")[0] if isinstance(obj.__doc__, str) else fallback
+    if escape:
+        doc = escaped(doc)
+    return doc
+
+
+if __name__ == "__main__":
+    strings = groupby_first_letter([str(i) for i in range(1000)])
+    print(limit_repr.repr(strings))
```

### Comparing `mknodes-0.2.0/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.3.2/mknodes/__linkreplacer/linkreplacer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,75 @@
-from __future__ import annotations
-
-import collections
-import logging
-import os
-import pathlib
-import re
-import urllib.parse
-
-from mkdocs.plugins import BasePlugin
-import mkdocs.utils
-
-
-logger = logging.getLogger(f"mkdocs.plugins.{__name__}")
-logger.addFilter(mkdocs.utils.warning_filter)
-
-# For Regex, match groups are:
-#       0: Whole markdown link e.g. [Alt-text](url)
-#       1: Alt text
-#       2: Full URL e.g. url + hash anchor
-#       3: Filename e.g. filename.md
-#       4: File extension e.g. .md, .png, etc.
-#       5. hash anchor e.g. #my-sub-heading-link
-AUTOLINK_RE = r"\[([^\]]+)\]\((([^)/]+\.(md|png|jpg))(#.*)*)\)"
-
-
-class AutoLinkReplacerPlugin:
-    def __init__(self, base_docs_url, page_url, mapping):
-        self.mapping = mapping
-        self.page_url = page_url
-        self.base_docs_url = pathlib.Path(base_docs_url)
-        # Absolute URL of the linker
-        self.linker_url = os.path.dirname(self.base_docs_url / page_url)  # noqa: PTH120
-
-    def __call__(self, match):
-        # Name of the markdown file
-        filename = urllib.parse.unquote(match.group(3).strip())
-        if filename not in self.mapping:
-            return f"`{match.group(3).replace('.md', '')}`"
-        filenames = self.mapping[filename]
-        # if len(filenames) > 1:
-        #     logger.warning(
-        #         f"{self.page_url}: {match.group(3)} has multiple targets: {filenames}"
-        #     )
-        abs_link_url = (self.base_docs_url / filenames[0]).parent
-        # need os.replath here bc pathlib.relative_to throws an exception
-        # when linking across drives
-        rel_path = os.path.relpath(abs_link_url, self.linker_url)
-        # html_filename = filename.replace(".md", ".html")
-        rel_link_url = os.path.join(rel_path, filename)  # noqa: PTH118
-        new_text = (
-            match.group(0).replace(match.group(2), rel_link_url)
-            if match.group(5) is None
-            else match.group(0).replace(match.group(2), rel_link_url + match.group(5))
-        )
-        new_text = new_text.replace("\\", "/")
-        logger.debug(
-            f"LinkReplacer: {self.page_url}: {match.group(3)=} -> {rel_link_url=}"
-        )
-        return new_text
-
-
-class LinkReplacerPlugin(BasePlugin):
-    def on_page_markdown(self, markdown, page, config, files, **kwargs):
-        base_docs_url = config["docs_dir"]
-        page_url = page.file.src_path
-        mapping = collections.defaultdict(list)
-        for file_ in files:
-            filename = os.path.basename(file_.abs_src_path)  # noqa: PTH119
-            mapping[filename].append(file_.url)
-        plugin = AutoLinkReplacerPlugin(base_docs_url, page_url, mapping)
-        markdown = re.sub(AUTOLINK_RE, plugin, markdown)
-        return markdown
+from __future__ import annotations
+
+import collections
+import logging
+import os
+import pathlib
+import re
+import urllib.parse
+
+from mkdocs.plugins import BasePlugin
+import mkdocs.utils
+
+
+logger = logging.getLogger(f"mkdocs.plugins.{__name__}")
+logger.addFilter(mkdocs.utils.warning_filter)
+
+# For Regex, match groups are:
+#       0: Whole markdown link e.g. [Alt-text](url)
+#       1: Alt text
+#       2: Full URL e.g. url + hash anchor
+#       3: Filename e.g. filename.md
+#       4: File extension e.g. .md, .png, etc.
+#       5. hash anchor e.g. #my-sub-heading-link
+AUTOLINK_RE = r"\[([^\]]+)\]\((([^)/]+\.(md|png|jpg))(#.*)*)\)"
+
+
+class AutoLinkReplacerPlugin:
+    def __init__(self, base_docs_url, page_url, mapping):
+        self.mapping = mapping
+        self.page_url = page_url
+        self.base_docs_url = pathlib.Path(base_docs_url)
+        # Absolute URL of the linker
+        self.linker_url = os.path.dirname(self.base_docs_url / page_url)  # noqa: PTH120
+
+    def __call__(self, match):
+        # Name of the markdown file
+        filename = urllib.parse.unquote(match.group(3).strip())
+        if filename not in self.mapping:
+            return f"`{match.group(3).replace('.md', '')}`"
+        filenames = self.mapping[filename]
+        # if len(filenames) > 1:
+        #     logger.warning(
+        #         f"{self.page_url}: {match.group(3)} has multiple targets: {filenames}"
+        #     )
+        abs_link_url = (self.base_docs_url / filenames[0]).parent
+        # need os.replath here bc pathlib.relative_to throws an exception
+        # when linking across drives
+        rel_path = os.path.relpath(abs_link_url, self.linker_url)
+        # html_filename = filename.replace(".md", ".html")
+        rel_link_url = os.path.join(rel_path, filename)  # noqa: PTH118
+        new_text = (
+            match.group(0).replace(match.group(2), rel_link_url)
+            if match.group(5) is None
+            else match.group(0).replace(match.group(2), rel_link_url + match.group(5))
+        )
+        new_text = new_text.replace("\\", "/")
+        logger.debug(
+            "LinkReplacer: %s: %s -> %s",
+            self.page_url,
+            match.group(3),
+            rel_link_url,
+        )
+        return new_text
+
+
+class LinkReplacerPlugin(BasePlugin):
+    def on_page_markdown(self, markdown, page, config, files, **kwargs):
+        base_docs_url = config["docs_dir"]
+        page_url = page.file.src_path
+        mapping = collections.defaultdict(list)
+        for file_ in files:
+            filename = os.path.basename(file_.abs_src_path)  # noqa: PTH119
+            mapping[filename].append(file_.url)
+        plugin = AutoLinkReplacerPlugin(base_docs_url, page_url, mapping)
+        return re.sub(AUTOLINK_RE, plugin, markdown)
```

### Comparing `mknodes-0.2.0/mknodes/manual/page_1.py` & `mknodes-0.3.2/mknodes/manual/page_1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,73 @@
-from __future__ import annotations
-
-import inspect
-
-import mknodes
-
-from mknodes import classhelpers, utils
-
-
-INTRO_TEXT = """
-Basically everything interesting in this library inherits from MkNode.
-It`s the base class for all tree nodes we are building. The tree goes from the root nav
-down to single markup elements. We can show the subclass tree by using
-the MkClassDiagram Node.
-"""
-
-
-def create_page_1(root_nav: mknodes.MkNav):
-    # Basic structure: Theres one root nav, navs can contain pages and other navs,
-    # pages contain more atomic markup nodes, like text, tables, and diagrams.
-    # These markup nodes in some cases can contain other Markup nodes.
-    # It`s all one big tree.
-
-    home_nav = root_nav.add_nav("User guide")
-    overview = home_nav.add_page("Overview", hide_toc=True)
-
-    # this here is what you are reading right now.
-    overview.add_code(inspect.getsource(create_page_1))
-    nodes_nav = home_nav.add_nav("Nodes")
-
-    # for convenience, we can add strings directly to pages.
-    # they will get converted to a mknodes.Text node.
-    overview += INTRO_TEXT
-
-    # Lets take a look at the relations of the included nodes.
-    # It`s easy to show different diagrams for classes.
-    subcls_page = home_nav.add_page("Subclass tree", hide_toc=True)
-    subcls_page += mknodes.MkClassDiagram(
-        mknodes.MkNode, mode="subclass_tree", orientation="LR"
-    )
-    # let`s take a look at some of the mentioned Markup nodes.
-    # Some of them have a `examples` classmethod which yields some example signatures
-    #  to show the functionality.
-    for kls in classhelpers.get_subclasses(mknodes.MkNode):
-        # get_subclasses just calls __subclasses__ recursively.
-        subpage = nodes_nav.add_page(kls.__name__)
-        if hasattr(kls, "examples"):
-            subpage += mknodes.MkCode.for_object(kls.examples, header="Signatures:")
-            for i, sig in enumerate(kls.examples(), start=1):
-                subpage.add_header(f"Trying signature {i}", level=2)
-                sig_txt = utils.format_kwargs(sig)
-                text = f"node = mknodes.{kls.__name__}({sig_txt})\nstr(node)"
-                subpage.add_code(code=text, title=f"example_{i}.py")
-                node = kls(**sig)
-                code = mknodes.MkCode(language="md", code=node, title=f"result_{i}.md")
-                subpage.add_tabs({"Preview": str(node), "Generated markdown": str(code)})
-                subpage.add_newlines(3)
-        subpage.add_mkdocstrings(kls)
+from __future__ import annotations
+
+import inspect
+
+import mknodes
+
+from mknodes.utils import classhelpers, helpers
+
+
+INTRO_TEXT = """
+Basically everything interesting in this library inherits from MkNode.
+It`s the base class for all tree nodes we are building. The tree goes from the root nav
+down to single markup elements. We can show the subclass tree by using
+the MkClassDiagram Node.
+"""
+
+
+def create_page_1(root_nav: mknodes.MkNav):
+    # Basic structure: Theres one root nav, navs can contain pages and other navs,
+    # pages contain more atomic markup nodes, like text, tables, and diagrams.
+    # These markup nodes in some cases can contain other Markup nodes.
+    # It`s all one big tree.
+
+    home_nav = root_nav.add_nav("User guide")
+    overview = home_nav.add_page("Overview", hide_toc=True)
+
+    # this here is what you are reading right now.
+    overview.add_code(inspect.getsource(create_page_1))
+    nodes_nav = home_nav.add_nav("Nodes")
+
+    # for convenience, we can add strings directly to pages.
+    # they will get converted to a mknodes.Text node.
+    overview += INTRO_TEXT
+
+    # Lets take a look at the relations of the included nodes.
+    # It`s easy to show different diagrams for classes.
+    subcls_page = home_nav.add_page("Subclass tree", hide_toc=True)
+    subcls_page += mknodes.MkClassDiagram(
+        mknodes.MkNode,
+        mode="subclass_tree",
+        orientation="LR",
+    )
+    # let`s take a look at some of the mentioned Markup nodes.
+    # Some of them have a `examples` classmethod which yields some example signatures
+    #  to show the functionality.
+    for kls in classhelpers.get_subclasses(mknodes.MkNode):
+        # get_subclasses just calls __subclasses__ recursively.
+        subpage = nodes_nav.add_page(kls.__name__)
+        if hasattr(kls, "examples"):
+            subpage += mknodes.MkCode.for_object(
+                kls.examples,
+                header="Example signatures",
+            )
+            for i, sig in enumerate(kls.examples(), start=1):
+                subpage.add_header(f"Example {i}", level=2)
+                sig_txt = helpers.format_kwargs(sig)
+                text = f"node = mknodes.{kls.__name__}({sig_txt})\nstr(node)"
+                subpage.add_code(code=text, title=f"example_{i}.py")
+                node = kls(**sig)
+                subpage += mknodes.MkText(str(node), header="Preview")
+                subpage += mknodes.MkCode(
+                    language="md",
+                    code=node,
+                    title="Resulting markdown",
+                )
+                subpage.add_newlines(3)
+        subpage.add_mkdocstrings(kls)
+
+
+if __name__ == "__main__":
+    nav = mknodes.MkNav()
+    create_page_1(nav)
+    print(nav.children[0])
```

### Comparing `mknodes-0.2.0/mknodes/manual/page_3.py` & `mknodes-0.3.2/mknodes/manual/page_3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-from __future__ import annotations
-
-import inspect
-import pprint
-
-import mknodes
-
-
-INTRO_TEXT = """Lets show some info about the tree we built.
-The tree starts from the root nav down to the Markup elements.
-"""
-
-
-def create_page_3(root_nav: mknodes.MkNav):
-    internals_nav = root_nav.add_nav("Internals")
-
-    overview = internals_nav.add_page("Overview", hide_toc=True)
-    overview += INTRO_TEXT
-
-    # we are here right now.
-    overview.add_code(inspect.getsource(create_page_3))
-
-    # the "Tree" section in the left sidebar shows what we have done up to now.
-    # we create a new page and add a formatted represenation of our Tree.
-
-    tree_page = internals_nav.add_page("Tree", hide_toc=True)
-    tree_page.add_header("This is the tree we built up to now.", level=3)
-    lines = [f"{level * '    '} {node!r}" for level, node in root_nav.iter_nodes()]
-    tree_page += mknodes.MkCode("\n".join(lines))
-
-    # Each tree item can carry virtual files. Lets dispay all files which are currently
-    # attached to the tree:
-    files_page = internals_nav.add_page("File map", hide_toc=True, hide_nav=True)
-    files_page.add_header("These are the 'virtual' files attached to the tree:", level=3)
-    virtual_files = root_nav.all_virtual_files()
-    file_txt = pprint.pformat(list(virtual_files.keys()))
-    files_page += mknodes.MkCode(file_txt)
-    # print(nodes_nav.to_tree_graph())
+from __future__ import annotations
+
+import inspect
+import pprint
+
+import mknodes
+
+
+INTRO_TEXT = """Lets show some info about the tree we built.
+The tree starts from the root nav down to the Markup elements.
+"""
+
+
+def create_page_3(root_nav: mknodes.MkNav):
+    internals_nav = root_nav.add_nav("Internals")
+
+    overview = internals_nav.add_page("Overview", hide_toc=True)
+    overview += INTRO_TEXT
+
+    # we are here right now.
+    overview.add_code(inspect.getsource(create_page_3))
+
+    # the "Tree" section in the left sidebar shows what we have done up to now.
+    # we create a new page and add a formatted represenation of our Tree.
+
+    tree_page = internals_nav.add_page("Tree", hide_toc=True)
+    tree_page.add_header("This is the tree we built up to now.", level=3)
+    lines = [f"{level * '    '} {node!r}" for level, node in root_nav.iter_nodes()]
+    tree_page += mknodes.MkCode("\n".join(lines))
+
+    # Each tree item can carry virtual files. Lets dispay all files which are currently
+    # attached to the tree:
+    files_page = internals_nav.add_page("File map", hide_toc=True)
+    files_page.add_header("These are the 'virtual' files attached to the tree:", level=3)
+    virtual_files = root_nav.all_virtual_files()
+    file_txt = pprint.pformat(list(virtual_files.keys()))
+    files_page += mknodes.MkCode(file_txt)
+    # print(nodes_nav.to_tree_graph())
+
+
+if __name__ == "__main__":
+    nav = mknodes.MkNav()
+    create_page_3(nav)
+    print(nav.children[0])
```

### Comparing `mknodes-0.2.0/LICENSE` & `mknodes-0.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Philipp Temminghoff
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Philipp Temminghoff
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `mknodes-0.2.0/PKG-INFO` & `mknodes-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.2.0
+Version: 0.3.2
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.2.0 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.3.2 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.10 Requires-Dist: mkdocs Requires-Dist: mkdocs-
 gen-files Requires-Dist: typing-extensions Description-Content-Type: text/
 markdown # MkNodes
                            Generate docs with ease.
```

