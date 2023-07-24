# Comparing `tmp/autodoc_pydantic-1.9.0.tar.gz` & `tmp/autodoc_pydantic-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodoc_pydantic-1.9.0.tar", max compression
+gzip compressed data, was "autodoc_pydantic-2.0.0.tar", max compression
```

## Comparing `autodoc_pydantic-1.9.0.tar` & `autodoc_pydantic-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1071 2023-07-03 19:04:23.280982 autodoc_pydantic-1.9.0/LICENSE
--rw-r--r--   0        0        0    16402 2023-07-03 19:04:23.280982 autodoc_pydantic-1.9.0/README.md
--rw-r--r--   0        0        0     1830 2023-07-03 19:04:23.292982 autodoc_pydantic-1.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/__init__.py
--rw-r--r--   0        0        0     6258 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/__init__.py
--rw-r--r--   0        0        0      181 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css
--rw-r--r--   0        0        0        0 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/__init__.py
--rw-r--r--   0        0        0    31842 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py
--rw-r--r--   0        0        0     9252 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/directives.py
--rw-r--r--   0        0        0        0 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/__init__.py
--rw-r--r--   0        0        0     9253 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py
--rw-r--r--   0        0        0     3764 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py
--rw-r--r--   0        0        0      452 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/enums.py
--rw-r--r--   0        0        0     1814 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py
--rw-r--r--   0        0        0      838 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/templates.py
--rw-r--r--   0        0        0     1302 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/utility.py
--rw-r--r--   0        0        0     1140 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/events.py
--rw-r--r--   0        0        0    16648 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/inspection.py
--rw-r--r--   0        0        0     1736 2023-07-03 19:04:23.296982 autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/utility.py
--rw-r--r--   0        0        0    18173 1970-01-01 00:00:00.000000 autodoc_pydantic-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 20:07:57.450222 autodoc_pydantic-2.0.0/LICENSE
+-rw-r--r--   0        0        0    17990 2023-07-24 20:07:57.450222 autodoc_pydantic-2.0.0/README.md
+-rw-r--r--   0        0        0     1944 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/__init__.py
+-rw-r--r--   0        0        0     6075 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css
+-rw-r--r--   0        0        0        0 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/__init__.py
+-rw-r--r--   0        0        0    30118 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py
+-rw-r--r--   0        0        0     8884 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/directives.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/__init__.py
+-rw-r--r--   0        0        0     9253 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py
+-rw-r--r--   0        0        0     3484 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py
+-rw-r--r--   0        0        0      452 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/enums.py
+-rw-r--r--   0        0        0     1814 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py
+-rw-r--r--   0        0        0      838 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/templates.py
+-rw-r--r--   0        0        0     1957 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/utility.py
+-rw-r--r--   0        0        0      946 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/events.py
+-rw-r--r--   0        0        0    17697 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/inspection.py
+-rw-r--r--   0        0        0     1736 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/utility.py
+-rw-r--r--   0        0        0    19874 1970-01-01 00:00:00.000000 autodoc_pydantic-2.0.0/PKG-INFO
```

### Comparing `autodoc_pydantic-1.9.0/LICENSE` & `autodoc_pydantic-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-1.9.0/README.md` & `autodoc_pydantic-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI version](https://img.shields.io/pypi/v/autodoc_pydantic?style=for-the-badge)](https://pypi.org/project/autodoc-pydantic/)
 ![Python](https://img.shields.io/badge/python-3.7+-blue.svg?style=for-the-badge)
 
 [![Master](https://img.shields.io/github/actions/workflow/status/mansenfranzen/autodoc_pydantic/tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/autodoc_pydantic/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic)
 
 [![Downloads](https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-badge)](https://pypistats.org/packages/autodoc-pydantic)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-31-orange.svg?style=for-the-badge)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-34-orange.svg?style=for-the-badge)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 You love [pydantic](https://pydantic-docs.helpmanual.io/) ❤ and you want to
 document your models and configuration settings with [sphinx](https://www.sphinx-doc.org/en/master/)?
 
 Perfect, let's go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html)
@@ -24,32 +24,33 @@
 - 💬 provides default values, alias and constraints for model fields
 - 🔗 adds hyperlinks between validators and corresponding fields
 - 📃 includes collapsable model json schema
 - 🏄 natively integrates with autodoc and autosummary extensions
 - 📎 defines explicit pydantic prefixes for models, settings, fields, validators and model config
 - 📋 shows summary section for model configuration, fields and validators
 - 👀 hides overloaded and redundant model class signature
-- 📚 sorts fields, validators and model config within models by type
-- 🍀 Supports `pydantic >= 1.5.0` and `sphinx >= 3.4.0`
-
-### Comparison between autodoc sphinx and autodoc pydantic
-
-[![Comparison](https://raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/main/docs/source/material/example_comparison_v1.0.0.gif)](https://autodoc-pydantic.readthedocs.io/en/latest/examples.html#default-configuration)
-
-To see those features in action, jump over to the [example documentation](https://autodoc-pydantic.readthedocs.io/en/stable/users/examples.html#default-configuration) to compare
-the appearance of standard sphinx autodoc with *autodoc_pydantic*.
+- 🔱 visualizes entity-relationship-diagrams for class hierarchies
+- 🍀 Supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0`
 
 ## Documentation
 
 For more details, please visit the official [documentation](https://autodoc-pydantic.readthedocs.io/en/stable/):
 
 - [Installation](https://autodoc-pydantic.readthedocs.io/en/stable/users/installation.html)
 - [Configuration](https://autodoc-pydantic.readthedocs.io/en/stable/users/configuration.html)
 - [Usage](https://autodoc-pydantic.readthedocs.io/en/stable/users/usage.html)
 - [Examples](https://autodoc-pydantic.readthedocs.io/en/stable/users/examples.html)
+- [Developer Guide](https://autodoc-pydantic.readthedocs.io/en/stable/developers/setup.html)
+
+## Comparison between autodoc sphinx and autodoc pydantic
+
+[![Comparison](https://raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/main/docs/source/material/example_comparison_v1.0.0.gif)](https://autodoc-pydantic.readthedocs.io/en/latest/examples.html#default-configuration)
+
+To see those features in action, jump over to the [example documentation](https://autodoc-pydantic.readthedocs.io/en/stable/users/examples.html#default-configuration) to compare
+the appearance of standard sphinx autodoc with *autodoc_pydantic*.
 
 ## Acknowledgements
 
 Thanks to great open source projects [sphinx](https://www.sphinx-doc.org/en/master/),
 [pydantic](https://pydantic-docs.helpmanual.io/) and
 [poetry](https://python-poetry.org/) (and so many more) ❤ in addition to the following contributors:
 
@@ -94,14 +95,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://t.me/pipeknight"><img src="https://avatars.githubusercontent.com/u/34810566?v=4?s=100" width="100px;" alt="Evgeniy Lupashin"/><br /><sub><b>Evgeniy Lupashin</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3APipeKnight" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://janhendrikewers.uk/"><img src="https://avatars.githubusercontent.com/u/12383029?v=4?s=100" width="100px;" alt="Jan-Hendrik Ewers"/><br /><sub><b>Jan-Hendrik Ewers</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Aiwishiwasaneagle" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://jon-e.net"><img src="https://avatars.githubusercontent.com/u/12961499?v=4?s=100" width="100px;" alt="Jonny Saunders"/><br /><sub><b>Jonny Saunders</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Asneakers-the-rat" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://charlie.machalow.com"><img src="https://avatars.githubusercontent.com/u/5749838?v=4?s=100" width="100px;" alt="Charles Machalow"/><br /><sub><b>Charles Machalow</b></sub></a><br /><a href="#question-csm10495" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tkaraouzene"><img src="https://avatars.githubusercontent.com/u/20064077?v=4?s=100" width="100px;" alt="Thomas Karaouzene"/><br /><sub><b>Thomas Karaouzene</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Atkaraouzene" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/caseyzak24"><img src="https://avatars.githubusercontent.com/u/29411281?v=4?s=100" width="100px;" alt="caseyzak24"/><br /><sub><b>caseyzak24</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=caseyzak24" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/PriOliveira"><img src="https://avatars.githubusercontent.com/u/13801839?v=4?s=100" width="100px;" alt="Priscila Oliveira"/><br /><sub><b>Priscila Oliveira</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3APriOliveira" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-PriOliveira" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/awoimbee"><img src="https://avatars.githubusercontent.com/u/22431493?v=4?s=100" width="100px;" alt="Arthur Woimbée"/><br /><sub><b>Arthur Woimbée</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Aawoimbee" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-awoimbee" title="User Testing">📓</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Tests">⚠️</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -6,65 +6,60 @@
 github/actions/workflow/status/mansenfranzen/autodoc_pydantic/
 tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/
 autodoc_pydantic/actions/workflows/tests.yml) [![Coverage](https://
 img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-
 badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic) [![Downloads]
 (https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-
 badge)](https://pypistats.org/packages/autodoc-pydantic) [![All Contributors]
-(https://img.shields.io/badge/all_contributors-31-orange.svg?style=for-the-
+(https://img.shields.io/badge/all_contributors-34-orange.svg?style=for-the-
 badge)](#contributors)  You love [pydantic](https://pydantic-
 docs.helpmanual.io/) â¤ and you want to document your models and configuration
 settings with [sphinx](https://www.sphinx-doc.org/en/master/)? Perfect, let's
 go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/
 extensions/autodoc.html) does not integrate too well with pydantic models ð.
 Don't worry - just `pip install autodoc_pydantic` âº. ## Features - ð¬
 provides default values, alias and constraints for model fields - ð adds
 hyperlinks between validators and corresponding fields - ð includes
 collapsable model json schema - ð natively integrates with autodoc and
 autosummary extensions - ð defines explicit pydantic prefixes for models,
 settings, fields, validators and model config - ð shows summary section for
 model configuration, fields and validators - ð hides overloaded and
-redundant model class signature - ð sorts fields, validators and model
-config within models by type - ð Supports `pydantic >= 1.5.0` and `sphinx >=
-3.4.0` ### Comparison between autodoc sphinx and autodoc pydantic [!
-[Comparison](https://raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/
-main/docs/source/material/example_comparison_v1.0.0.gif)](https://autodoc-
+redundant model class signature - ð± visualizes entity-relationship-diagrams
+for class hierarchies - ð Supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0`
+## Documentation For more details, please visit the official [documentation]
+(https://autodoc-pydantic.readthedocs.io/en/stable/): - [Installation](https://
+autodoc-pydantic.readthedocs.io/en/stable/users/installation.html) -
+[Configuration](https://autodoc-pydantic.readthedocs.io/en/stable/users/
+configuration.html) - [Usage](https://autodoc-pydantic.readthedocs.io/en/
+stable/users/usage.html) - [Examples](https://autodoc-pydantic.readthedocs.io/
+en/stable/users/examples.html) - [Developer Guide](https://autodoc-
+pydantic.readthedocs.io/en/stable/developers/setup.html) ## Comparison between
+autodoc sphinx and autodoc pydantic [![Comparison](https://
+raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/main/docs/source/
+material/example_comparison_v1.0.0.gif)](https://autodoc-
 pydantic.readthedocs.io/en/latest/examples.html#default-configuration) To see
 those features in action, jump over to the [example documentation](https://
 autodoc-pydantic.readthedocs.io/en/stable/users/examples.html#default-
 configuration) to compare the appearance of standard sphinx autodoc with
-*autodoc_pydantic*. ## Documentation For more details, please visit the
-official [documentation](https://autodoc-pydantic.readthedocs.io/en/stable/): -
-[Installation](https://autodoc-pydantic.readthedocs.io/en/stable/users/
-installation.html) - [Configuration](https://autodoc-pydantic.readthedocs.io/
-en/stable/users/configuration.html) - [Usage](https://autodoc-
-pydantic.readthedocs.io/en/stable/users/usage.html) - [Examples](https://
-autodoc-pydantic.readthedocs.io/en/stable/users/examples.html) ##
-Acknowledgements Thanks to great open source projects [sphinx](https://
-www.sphinx-doc.org/en/master/), [pydantic](https://pydantic-docs.helpmanual.io/
-) and [poetry](https://python-poetry.org/) (and so many more) â¤ in addition
-to the following contributors:
-          [Franz_WÃ¶llert]                  [Yves_Renier]               [TheBeardedBerserkr]     [Jan_VlÄinskÃ½]      [antvig]          [Hugo_O    [yura_bondarenko]
-           Franz_WÃ¶llert                    Yves_Renier                 TheBeardedBerserkr       Jan_VlÄinskÃ½        antvig           Rivera]     yura_bondarenko
-        ð§ ð â ï¸       ð â ï¸ ð           ð¤              ð¡ï¸       ð ð�   Hugo_O        ð ð
-                                                                                                                                                Rivera
-                                                                                                                                                 ð¤
-              [Trevor_Howard]                  [thomas-pedot]                [Mat_Utter]            [David_C_Hall]      [Josh_A._Mitchell]    [Roderick      [Lily_Wang]
-               Trevor_Howard                    thomas-pedot                  Mat_Utter              David_C_Hall        Josh_A._Mitchell        Go]          Lily_Wang
-                 ð ð               ð ð            ð ð        ð¤ ð�     ð¤ â ïRoderick_Go      ð ð
-                                                                                                                                                â ï¸
-             [j-carson]                     [Jakob_Lykke_Andersen]   [Juan_Luis_Cano_RodrÃ­guez   [Mikalai_Chaly]       [Stig_Korsnes]        [Ilia     [Grzegorz_Bokota]
-              j-carson                       Jakob_Lykke_Andersen     Juan_Luis_Cano_RodrÃ­guez    Mikalai_Chaly         Stig_Korsnes       Kurenkov]    Grzegorz_Bokota
-          ð ð» â ï¸             ð»                   ð              ð â ï      ð ð¤�    Ilia           ð
-                                                                                                                                               Kurenkov
-                                                                                                                                                 ð
-                   [jgunstone]                      [iwyrkore]           [spacemanspiff2007]           [Luke_Hsiao]        [Daniel_Walker]     [Evgeniy     [Jan-Hendrik
-                    jgunstone                        iwyrkore             spacemanspiff2007             Luke_Hsiao          Daniel_Walker     Lupashin]        Ewers]
-                      ð                         ð»               ð ð¤            ð             ð       Evgeniy    Jan-Hendrik_Ewers
-                                                                                                                                               Lupashin         ð
-                                                                                                                                                 ð
-               [Jonny_Saunders]                [Charles_Machalow]          [Thomas_Karaouzene]
-                Jonny_Saunders                  Charles_Machalow            Thomas_Karaouzene
-                     ð                         ð¬                    ð
+*autodoc_pydantic*. ## Acknowledgements Thanks to great open source projects
+[sphinx](https://www.sphinx-doc.org/en/master/), [pydantic](https://pydantic-
+docs.helpmanual.io/) and [poetry](https://python-poetry.org/) (and so many
+more) â¤ in addition to the following contributors:
+          [Franz_WÃ¶llert]                  [Yves_Renier]               [TheBeardedBerserkr]     [Jan_VlÄinskÃ½]      [antvig]                        [Hugo_O_Rivera]       [yura_bondarenko]
+           Franz_WÃ¶llert                    Yves_Renier                 TheBeardedBerserkr       Jan_VlÄinskÃ½        antvig                          Hugo_O_Rivera         yura_bondarenko
+        ð§ ð â ï¸       ð â ï¸ ð           ð¤              ð¡ï¸       ð ð                    ð¤             ð ð
+              [Trevor_Howard]                  [thomas-pedot]                [Mat_Utter]            [David_C_Hall]      [Josh_A._Mitchell]                    [Roderick_Go]           [Lily_Wang]
+               Trevor_Howard                    thomas-pedot                  Mat_Utter              David_C_Hall        Josh_A._Mitchell                      Roderick_Go             Lily_Wang
+                 ð ð               ð ð            ð ð        ð¤ ð�     ð¤ â ï¸                â ï¸          ð ð
+             [j-carson]                     [Jakob_Lykke_Andersen]   [Juan_Luis_Cano_RodrÃ­guez   [Mikalai_Chaly]       [Stig_Korsnes]                     [Ilia_Kurenkov]       [Grzegorz_Bokota]
+              j-carson                       Jakob_Lykke_Andersen     Juan_Luis_Cano_RodrÃ­guez    Mikalai_Chaly         Stig_Korsnes                       Ilia_Kurenkov         Grzegorz_Bokota
+          ð ð» â ï¸             ð»                   ð              ð â ï      ð ð¤                    ð               ð
+                   [jgunstone]                      [iwyrkore]           [spacemanspiff2007]           [Luke_Hsiao]        [Daniel_Walker]                 [Evgeniy_Lupashin]        [Jan-Hendrik
+                    jgunstone                        iwyrkore             spacemanspiff2007             Luke_Hsiao          Daniel_Walker                   Evgeniy_Lupashin            Ewers]
+                      ð                         ð»               ð ð¤            ð             ð                          ð         Jan-Hendrik_Ewers
+                                                                                                                                                                                         ð
+               [Jonny_Saunders]                [Charles_Machalow]          [Thomas_Karaouzene]         [caseyzak24]     [Priscila_Oliveira]            [Arthur_WoimbÃ©e]
+                Jonny_Saunders                  Charles_Machalow            Thomas_Karaouzene           caseyzak24       Priscila_Oliveira              Arthur_WoimbÃ©e
+                     ð                         ð¬                    ð                 ð          ð ð�        ð ð ð» â ï¸
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `autodoc_pydantic-1.9.0/pyproject.toml` & `autodoc_pydantic-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autodoc_pydantic"
-version = "1.9.0"
+version = "2.0.0"
 description = "Seamlessly integrate pydantic models in your Sphinx documentation."
 authors = ["mansenfranzen <franz.woellert@gmail.com>"]
 packages = [{ include = "sphinxcontrib" }]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mansenfranzen/autodoc_pydantic"
 repository = "https://github.com/mansenfranzen/autodoc_pydantic"
@@ -15,26 +15,29 @@
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development :: Documentation"
 ]
 include = ["sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css"]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<4.0.0"
-Sphinx = ">=3.4"
-pydantic = ">=1.5,<2.0.0"
+Sphinx = ">=4.0"
+pydantic = ">=2.0,<3.0.0"
+pydantic-settings = ">=2.0,<3.0.0"
+
+importlib-metadata = { version = ">1", markers = "python_version <= '3.8'" }
 
 sphinx-rtd-theme = { version = "^1.0", optional = true }
 sphinx-tabs = { version = "^3", optional = true }
 sphinx-copybutton = { version = "^0.4", optional = true }
 sphinxcontrib-mermaid = { version = "^0.7", optional = true }
 pytest = {version = "^7", optional = true }
 coverage = { version ="^7", optional = true }
 flake8 = { version = "^3", optional = true }
 tox = { version ="^3", optional = true }
-erdantic= { version ="^0.5", optional = true }
+erdantic = { version ="^0.6", optional = true }
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 
 [tool.poetry.extras]
 docs = ["sphinx-rtd-theme",
         "sphinx-tabs",
```

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/__init__.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """Contains the extension setup.
 
 """
 
 from pathlib import Path
 from typing import Dict, Any
 
+try:
+    from importlib.metadata import version
+except ModuleNotFoundError:
+    from importlib_metadata import version
+
 from sphinx.domains import ObjType
 from sphinx.application import Sphinx
 
 from sphinxcontrib.autodoc_pydantic.directives.autodocumenters import (
     PydanticValidatorDocumenter,
     PydanticModelDocumenter,
-    PydanticConfigClassDocumenter,
     PydanticFieldDocumenter,
     PydanticSettingsDocumenter
 )
 from sphinxcontrib.autodoc_pydantic.directives.options.enums import \
     OptionsJsonErrorStrategy, OptionsFieldDocPolicy, OptionsSummaryListOrder
 
 from sphinxcontrib.autodoc_pydantic.directives.directives import (
     PydanticField,
-    PydanticConfigClass,
     PydanticValidator,
     PydanticModel,
     PydanticSettings
 )
 
-__version__ = "1.8.0"
+__version__ = version("autodoc_pydantic")
 
 from sphinxcontrib.autodoc_pydantic.events import add_fallback_css_class
 
 
 def add_css_file(app: Sphinx, exception: Exception):
     """Adds custom css to HTML output.
 
@@ -75,30 +78,28 @@
     summary_list_order = OptionsSummaryListOrder.ALPHABETICAL
 
     add(f'{stem}config_signature_prefix', "model", True, str)
     add(f'{stem}config_members', True, True, bool)
 
     add(f'{stem}settings_show_json', True, True, bool)
     add(f'{stem}settings_show_json_error_strategy', json_strategy, True, str)
-    add(f'{stem}settings_show_config_member', False, True, bool)
     add(f'{stem}settings_show_config_summary', True, True, bool)
     add(f'{stem}settings_show_validator_members', True, True, bool)
     add(f'{stem}settings_show_validator_summary', True, True, bool)
     add(f'{stem}settings_show_field_summary', True, True, bool)
     add(f'{stem}settings_summary_list_order', summary_list_order, True, str)
     add(f'{stem}settings_hide_paramlist', True, True, bool)
     add(f'{stem}settings_hide_reused_validator', True, True, bool)
     add(f'{stem}settings_undoc_members', True, True, bool)
     add(f'{stem}settings_members', True, True, bool)
     add(f'{stem}settings_member_order', 'groupwise', True, str)
     add(f'{stem}settings_signature_prefix', "pydantic settings", True, str)
 
     add(f'{stem}model_show_json', True, True, bool)
     add(f'{stem}model_show_json_error_strategy', json_strategy, True, str)
-    add(f'{stem}model_show_config_member', False, True, bool)
     add(f'{stem}model_show_config_summary', True, True, bool)
     add(f'{stem}model_show_validator_members', True, True, bool)
     add(f'{stem}model_show_validator_summary', True, True, bool)
     add(f'{stem}model_show_field_summary', True, True, bool)
     add(f'{stem}model_summary_list_order', summary_list_order, True, str)
     add(f'{stem}model_hide_paramlist', True, True, bool)
     add(f'{stem}model_hide_reused_validator', True, True, bool)
@@ -131,23 +132,21 @@
     application.
 
     """
 
     app.add_directive_to_domain("py", "pydantic_field", PydanticField)
     app.add_directive_to_domain("py", "pydantic_model", PydanticModel)
     app.add_directive_to_domain("py", "pydantic_settings", PydanticSettings)
-    app.add_directive_to_domain("py", "pydantic_config", PydanticConfigClass)
     app.add_directive_to_domain("py", "pydantic_validator", PydanticValidator)
 
     app.setup_extension('sphinx.ext.autodoc')
     app.add_autodocumenter(PydanticFieldDocumenter)
     app.add_autodocumenter(PydanticModelDocumenter)
     app.add_autodocumenter(PydanticSettingsDocumenter)
     app.add_autodocumenter(PydanticValidatorDocumenter)
-    app.add_autodocumenter(PydanticConfigClassDocumenter)
 
     app.connect('object-description-transform', add_fallback_css_class)
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     add_configuration_values(app)
     add_directives_and_autodocumenters(app)
```

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 
 import json
 from typing import Any, Optional, Dict, List, Iterable, Callable, Set
 
 import sphinx
 from docutils.statemachine import StringList
-from pydantic import BaseSettings, BaseModel
+from pydantic import BaseModel
+from pydantic_settings import BaseSettings
 from sphinx.ext.autodoc import (
     MethodDocumenter,
     ClassDocumenter,
     AttributeDocumenter,
     Documenter
 )
 from sphinx.util.docstrings import prepare_docstring
@@ -25,24 +26,25 @@
     OptionsSummaryListOrder
 )
 from sphinxcontrib.autodoc_pydantic.directives.options.definition import (
     OPTIONS_MODEL,
     OPTIONS_SETTINGS,
     OPTIONS_FIELD,
     OPTIONS_VALIDATOR,
-    OPTIONS_CONFIG,
     OPTIONS_MERGED
 )
 from sphinxcontrib.autodoc_pydantic.directives.templates import to_collapsable
 from sphinxcontrib.autodoc_pydantic.inspection import ModelInspector, \
     ValidatorFieldMap
 from sphinxcontrib.autodoc_pydantic.directives.options.composites import (
     AutoDocOptions
 )
-from sphinxcontrib.autodoc_pydantic.directives.utility import NONE
+from sphinxcontrib.autodoc_pydantic.directives.utility import NONE, \
+    intercept_type_annotations_py_gt_39
+
 try:
     import erdantic as erd
 except ImportError:
     erd = None
 
 
 class PydanticAutoDoc:
@@ -202,14 +204,17 @@
         is_val = super().can_document_member(member, membername, isattr,
                                              parent)
         is_model = ModelInspector.static.is_pydantic_model(member)
         return is_val and is_model
 
     def __init__(self, *args: Any) -> None:
         super().__init__(*args)
+        exclude_members = self.options.setdefault("exclude-members", set())
+        exclude_members.add("model_fields")
+        exclude_members.add("model_config")
         self.pydantic = PydanticAutoDoc(self, is_child=False)
 
     def document_members(self, *args, **kwargs):
         """Modify member options before starting to document members.
 
         """
 
@@ -229,42 +234,35 @@
         super().document_members(*args, **kwargs)
 
     def hide_config_member(self):
         """Add `Config` to `exclude_members` option.
 
         """
 
-        if "exclude-members" not in self.options:
-            self.options["exclude-members"] = {"Config"}
-        else:
-            self.options["exclude-members"].add("Config")
+        exclude_members = self.options["exclude-members"]
+        exclude_members.add("Config")  # deprecated since pydantic v2
+        exclude_members.add("model_config")
 
     def hide_validator_members(self):
         """Add validator names to `exclude_members`.
 
         """
-
         validators = self.pydantic.inspect.validators.names
-        if "exclude-members" not in self.options:
-            self.options["exclude-members"] = validators
-        else:
-            self.options["exclude-members"].update(validators)
+        exclude_members = self.options["exclude-members"]
+        exclude_members.update(validators)
 
     def hide_reused_validators(self):
         """Add reused validators to `exclude_members` option.
 
         """
 
         validators = self.pydantic.inspect.validators
-        reused_validators = validators.get_reused_validator_method_names()
-
-        if "exclude-members" not in self.options:
-            self.options["exclude-members"] = set(reused_validators)
-        else:
-            self.options["exclude-members"].update(reused_validators)
+        reused_validators = validators.get_reused_validators_names()
+        exclude_members = self.options["exclude-members"]
+        exclude_members.update(reused_validators)
 
     def format_signature(self, **kwargs) -> str:
         """If parameter list is to be hidden, return only empty signature.
 
         """
 
         if self.pydantic.options.is_true("hide-paramlist", True):
@@ -301,15 +299,14 @@
             self.add_validators_summary()
 
     def add_collapsable_schema(self):
         """Adds collapse code block containing JSON schema.
 
         """
 
-        schema = self.pydantic.inspect.schema.sanitized
         non_serializable = self.pydantic.inspect.fields.non_json_serializable
 
         # handle non serializable fields
         strategy = self.pydantic.options.get_value("show-json-error-strategy")
         if non_serializable:
             error_msg = (
                 f"JSON schema can't be generated for '{self.fullname}' "
@@ -324,31 +321,33 @@
                 raise sphinx.errors.ExtensionError(error_msg)
             elif strategy != OptionsJsonErrorStrategy.COERCE:
                 raise sphinx.errors.ExtensionError(
                     f"Invalid option provided for 'show-json-error-strategy'. "
                     f"Allowed values are f{OptionsJsonErrorStrategy.values()}"
                 )
 
+        schema = self.pydantic.inspect.schema.sanitized
         schema_rest = self._convert_json_schema_to_rest(schema)
         source_name = self.get_sourcename()
         for line in schema_rest:
             self.add_line(line, source_name)
 
     def add_erdantic_figure(self):
         """Adds an erdantic entity relation diagram to the doc of an
         pydantic model.
 
         """
         source_name = self.get_sourcename()
         if erd is None:
-            error_msg = 'erdantic is not installed, you need to install ' \
-                'it before creating an Entity Relationship Diagram for ' \
-                'f{self.fullname}. See ' \
-                'https://autodoc-pydantic.readthedocs.io/' \
-                'en/stable/users/installation.html'
+            error_msg = (
+                'erdantic is not installed, you need to install it before '
+                'creating an Entity Relationship Diagram for '
+                'f{self.fullname}. See '
+                'https://autodoc-pydantic.readthedocs.io/'
+                'en/stable/users/installation.html')
             raise RuntimeError(error_msg)
 
         # Graphviz [DOT language](https://graphviz.org/doc/info/lang.html)
         figure_dot = erd.to_dot(self.object).replace('\t', '   ').split('\n')
         lines_dot = ['   ' + line for line in figure_dot]
         lines = [".. graphviz::", ""] + lines_dot + [""]
 
@@ -444,15 +443,14 @@
         """Adds summary section describing all validators with corresponding
         fields.
 
         """
 
         if not self.pydantic.inspect.validators:
             return
-
         sorted_references = self._get_validator_summary_references()
 
         source_name = self.get_sourcename()
         self.add_line(":Validators:", source_name)
         for ref in sorted_references:
             line = self._build_validator_summary_rest_line(ref)
             self.add_line(line, source_name)
@@ -534,15 +532,14 @@
         return stringify(annotations.get(field_name, ""))
 
     @staticmethod
     def _convert_json_schema_to_rest(schema: Dict) -> List[str]:
         """Convert model's schema dict into reST.
 
         """
-
         schema = json.dumps(schema, default=str, indent=3)
         lines = [f"   {line}" for line in schema.split("\n")]
         lines = ['.. code-block:: json', ''] + lines
         lines = to_collapsable(
             lines,
             "Show JSON schema",
             "autodoc_pydantic_collapsable_json"
@@ -646,15 +643,14 @@
 
         return self.objpath[-1]
 
     def add_directive_header(self, sig: str) -> None:
         """Delegate header options.
 
         """
-
         super().add_directive_header(sig)
 
         self.add_default_value_or_marker()
         self.add_alias()
 
     @property
     def needs_required_marker(self) -> bool:
@@ -712,23 +708,23 @@
     def add_alias(self):
         """Adds alias directive option.
 
         """
 
         field_name = self.pydantic_field_name
         field = self.pydantic.inspect.fields.get(field_name)
-        alias_given = field.alias != field_name
+        alias_given = field.alias and field.alias != field_name
 
         show_alias = self.pydantic.options.is_true("field-show-alias")
         swap = self.pydantic.options.is_true("field-swap-name-and-alias")
         alias_required = show_alias or swap
 
         if alias_given and alias_required:
             sourcename = self.get_sourcename()
-            self.add_line('   :alias: ' + field.alias, sourcename)
+            self.add_line(f'   :alias: {field.alias}', sourcename)
 
     def add_content(self,
                     more_content: Optional[StringList],
                     **kwargs,
                     ) -> None:
         """Delegate additional content creation.
 
@@ -804,14 +800,23 @@
             resolver = self.pydantic.resolve_inherited_validator_reference
             ref = resolver(reference.validator_ref)
             line = f"   - :py:obj:`{reference.validator_name} <{ref}>`"
             self.add_line(line, source_name)
 
         self.add_line("", source_name)
 
+    def add_line(self, line: str, source: str, *lineno: int) -> None:
+        """Intercept added rst lines to handle edge cases such as correct
+        string representation for annotated types in python < 3.9.
+
+        """
+
+        line = intercept_type_annotations_py_gt_39(line)
+        super().add_line(line, source, *lineno)
+
 
 class PydanticValidatorDocumenter(MethodDocumenter):
     """Represents specialized Documenter subclass for pydantic validators.
 
     """
 
     objtype = 'pydantic_validator'
@@ -899,68 +904,7 @@
         self.add_line(":Validates:", source_name)
 
         for reference in references:
             line = self._build_field_list_rest_line(reference)
             self.add_line(line, source_name)
 
         self.add_line("", source_name)
-
-
-class PydanticConfigClassDocumenter(ClassDocumenter):
-    """Represents specialized Documenter subclass for pydantic model
-    configuration.
-
-    """
-
-    objtype = 'pydantic_config'
-    directivetype = 'pydantic_config'
-    option_spec = ClassDocumenter.option_spec.copy()
-    option_spec.update(OPTIONS_CONFIG)
-    member_order = 100
-    priority = 10 + ClassDocumenter.priority
-
-    pyautodoc_pass_to_directive = (
-        "config-signature-prefix",
-    )
-
-    def __init__(self, *args: Any) -> None:
-        super().__init__(*args)
-        self.pydantic = PydanticAutoDoc(self, is_child=True)
-
-    @classmethod
-    def can_document_member(cls,
-                            member: Any,
-                            membername: str,
-                            isattr: bool,
-                            parent: Any) -> bool:
-        """Filter only pydantic model configurations.
-
-        """
-
-        is_val = super().can_document_member(member, membername, isattr,
-                                             parent)
-        is_parent_model = ModelInspector.static.is_pydantic_model(
-            parent.object)
-        is_config = membername == "Config"
-        is_class = isinstance(member, type)
-        return is_val and is_parent_model and is_config and is_class
-
-    def document_members(self, *args, **kwargs):
-        """Modify member options before starting to document members.
-
-        """
-
-        self.pydantic.options.set_members_all()
-        if self.options.get("members"):
-            self.options["undoc-members"] = True
-
-        # handle special case when Config is documented as an attribute
-        # in which case `all_members` defaults to True which has to be
-        # overruled by `autodoc_pydantic_config_members` app cfg
-        app_cfg = self.pydantic.options.get_app_cfg_by_name("members")
-        hide_members = app_cfg is False
-        no_members = bool(self.options.get("members")) is False
-
-        if hide_members and no_members:
-            super().document_members(all_members=False, **kwargs)
-        else:
-            super().document_members(*args, **kwargs)
```

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/directives.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,20 +262,7 @@
 
         fullname, prefix = super().handle_signature(sig, signode)
 
         if self.pyautodoc.get_value("validator-replace-signature"):
             self.replace_return_node(signode)
 
         return fullname, prefix
-
-
-class PydanticConfigClass(PydanticDirectiveBase, PyClasslike):
-    """Specialized directive for pydantic config class.
-
-    """
-
-    option_spec = PyClasslike.option_spec.copy()
-    option_spec.update({"__doc_disable_except__": option_list_like,
-                        "config-signature-prefix": unchanged})
-
-    config_name = "config"
-    default_prefix = "class"
```

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,22 +27,16 @@
                      "validator-list-fields": option_default_true,
                      "validator-signature-prefix": unchanged,
                      "field-swap-name-and-alias": option_default_true,
                      "__doc_disable_except__": option_list_like}
 """Represents added directive options for :class:`PydanticValidatorDocumenter`.
 """
 
-OPTIONS_CONFIG = {"members": option_members,
-                  "config-signature-prefix": unchanged,
-                  "__doc_disable_except__": option_list_like}
-"""Represents added directive options for :class:`PydanticConfigDocumenter`."""
-
 OPTIONS_MERGED = {**OPTIONS_FIELD,
-                  **OPTIONS_VALIDATOR,
-                  **OPTIONS_CONFIG}
+                  **OPTIONS_VALIDATOR}
 
 OPTIONS_MODEL = {
     "model-show-json": option_default_true,
     "model-show-json-error-strategy": option_one_of_factory(
         OptionsJsonErrorStrategy.values()
     ),
     "model-hide-paramlist": option_default_true,
```

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/directives/templates.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/templates.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/events.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/events.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import sphinx
 from sphinx.addnodes import desc_content
 from sphinx.application import Sphinx
 
 OBJTYPES_CSS_FALLBACKS = {"pydantic_model": "class",
                           "pydantic_settings": "class",
                           "pydantic_validator": "method",
-                          "pydantic_field": "attribute",
-                          "pydantic_config": "class"}
+                          "pydantic_field": "attribute"}
 
 
 def add_fallback_css_class(app: Sphinx,
                            domain: str,
                            objtype: str,
                            contentnode: desc_content):
     """Used as `object-description-transform` sphinx event to add default css
@@ -19,17 +17,13 @@
     """
 
     if objtype not in OBJTYPES_CSS_FALLBACKS:
         return
 
     classes = contentnode.parent.attributes["classes"]
 
-    # for older sphinx versions, add objtype explicitly
-    if sphinx.version_info < (3, 6):
-        classes.append(objtype)
-
     if not app.env.config["autodoc_pydantic_add_fallback_css_class"]:
         return
 
     idx = classes.index(objtype)
     fallback = OBJTYPES_CSS_FALLBACKS[objtype]
     classes.insert(idx, fallback)
```

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/inspection.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/inspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,31 @@
 import itertools
 import pydoc
 import warnings
 from collections import defaultdict
 from typing import NamedTuple, List, Dict, Any, Set, TypeVar, Type, Callable, \
     Optional
 
-import pydantic
-from pydantic import BaseModel, create_model
-from pydantic.class_validators import Validator
-from pydantic.fields import ModelField
-from pydantic.schema import get_field_schema_validations
+from pydantic import BaseModel, create_model, ConfigDict, \
+    PydanticInvalidForJsonSchema
+from pydantic.fields import FieldInfo
+from pydantic_settings import BaseSettings
 from sphinx.addnodes import desc_signature
 
 ASTERISK_FIELD_NAME = "all fields"
 
 
-class ValidatorAdapter(BaseModel):
+class ValidatorAdapter(NamedTuple):
     """Provide standardized interface to pydantic's validator objects with
     additional metadata (e.g. root validator) for internal usage in
     autodoc_pydantic.
 
     """
 
     func: Callable
-    root_pre: bool = False
-    root_post: bool = False
 
     @property
     def name(self) -> str:
         """Return the validators function name.
 
         """
         return self.func.__name__
@@ -62,30 +59,14 @@
     def object_path(self) -> str:
         """Return the fully qualified object path of the validators function.
 
         """
 
         return f"{self.func.__module__}.{self.func.__qualname__}"
 
-    def is_member(self, model: Type) -> bool:
-        """Check if `self.func` is a member of provided `model` class or its
-        base classes. This can be used to identify functions that are reused
-        as validators.
-
-        """
-
-        if self.class_name is None:
-            return False
-
-        bases = (f"{x.__module__}.{x.__qualname__}" for x in model.__mro__)
-        return f"{self.module}.{self.class_name}" in bases
-
-    class Config:
-        arbitrary_types_allowed = True
-
     def __hash__(self):
         return id(f"{self}")
 
 
 class ValidatorFieldMap(NamedTuple):
     """Contains single mapping of a pydantic validator and field.
 
@@ -119,26 +100,27 @@
 class FieldInspector(BaseInspectionComposite):
     """Provide namespace for inspection methods for fields of pydantic models.
 
     """
 
     def __init__(self, parent: 'ModelInspector'):
         super().__init__(parent)
-        self.attribute = self.model.__fields__
+        # json schema can reliably be created only at model level
+        self.attribute = self.model.model_fields
 
     @property
     def names(self) -> List[str]:
         """Return field names while keeping ordering.
 
         """
 
         return list(self.attribute.keys())
 
-    def get(self, name: str) -> ModelField:
-        """Get the instance of `ModelField` for given field `name`.
+    def get(self, name: str) -> FieldInfo:
+        """Get the instance of `FieldInfo` for given field `name`.
 
         """
 
         return self.attribute[name]
 
     def get_alias_or_name(self, field_name: str) -> str:
         """Get the alias of a pydantic field if given. Otherwise, return the
@@ -159,41 +141,94 @@
                                      field_name: str,
                                      property_name: str) -> Any:
         """Get specific property value from pydantic's field info.
 
         """
 
         field = self.get(field_name)
-        return getattr(field.field_info, property_name, None)
+        return getattr(field, property_name, None)
+
+    def get_constraint_items(self, field_name: str) -> Dict[str, str]:
+        """Extract all possible constraints along with their default values
+        from a fields meta attribute.
+
+        """
+
+        metadata = self.model.model_fields[field_name].metadata
+        available = [meta for meta in metadata if meta is not None]
+
+        return {key: getattr(meta, key)
+                for meta in available
+                for key, value in self._get_meta_items(meta).items()}
+
+    @staticmethod
+    def _get_meta_items(meta_class: Any) -> Dict[str, str]:
+        """Helper method to extract constraint names and values from different
+        pydantic Metadata objects such as `pydantic.types.Strict`.
+
+        """
+
+        try:
+            return meta_class.__dataclass_fields__
+        except AttributeError:
+            return meta_class.__dict__
+
+    def get_given_constraint_keys(self, field_name: str) -> Set[str]:
+        """Retrieves all schema attribute keys that have been set.
+        This information is relevant to distinguish given values that are
+        equivalent to their default values. Otherwise, there is no chance
+        to determine if a constraint was actually given by the user or set as
+        a default value.
+
+        Note: Accessing private attributes with many levels of nesting is far
+        from being desired but currently there is no proper solution around
+        this. Accessing the `properties` via the `model_schema_json` may fail
+        in cases where fields are not serializable.
+
+        """
+
+        definition = self.model.__pydantic_core_schema__["definitions"][0]
+
+        # account for varying levels of nesting :-(
+        try:
+            field_schemas = definition["schema"]["fields"]
+        except KeyError:
+            field_schemas = definition["schema"]["schema"]["fields"]
+
+        # account for generics and other non-native fields without schema info
+        try:
+            schema = field_schemas[field_name]["schema"]
+        except KeyError:
+            return set()
+
+        # account for yet another level on model-field :-(
+        if "schema" in schema:
+            schema = schema["schema"]
+
+        return set(schema.keys())
 
     def get_constraints(self, field_name: str) -> Dict[str, Any]:
         """Get constraints for given `field_name`.
 
         """
 
-        field = self.get(field_name)
-        constraints = get_field_schema_validations(field)
-        ignore = {"env_names", "env"}
-
-        # ignore additional kwargs from pydantic `Field`, see #110
-        extra_kwargs = self.get_property_from_field_info(field_name=field_name,
-                                                         property_name="extra")
-        if extra_kwargs:
-            ignore = ignore.union(extra_kwargs.keys())
+        constraint_items = self.get_constraint_items(field_name).items()
+        given_constraint_keys = self.get_given_constraint_keys(field_name)
 
-        return {key: value for key, value in constraints.items()
-                if key not in ignore}
+        return {key: value
+                for key, value in constraint_items
+                if key in given_constraint_keys}
 
     def is_required(self, field_name: str) -> bool:
         """Check if a given pydantic field is required/mandatory. Returns True,
         if a value for this field needs to provided upon model creation.
 
         """
 
-        return self.get(field_name).required
+        return self.get(field_name).is_required()
 
     def has_default_factory(self, field_name: str) -> bool:
         """Check if field has a `default_factory` being set. This information
         is used to determine if a pydantic field is optional or not.
 
         """
 
@@ -206,44 +241,37 @@
 
         """
 
         field = self.get(field_name)
         return self._is_json_serializable(field)
 
     @classmethod
-    def _is_json_serializable(cls, field: ModelField):
-        """Ensure JSON serializability for given pydantic `ModelField`.
+    def _is_json_serializable(cls, field: FieldInfo):
+        """Ensure JSON serializability for given pydantic `FieldInfo`.
 
         """
-
-        # check for sub fields in case of `Union` or alike, see #98
-        if field.sub_fields:
-            return all(
-                cls._is_json_serializable(sub_field)
-                for sub_field in field.sub_fields
-            )
-
         # hide user warnings in sphinx output
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             return cls._test_field_serializabiltiy(field)
 
     @staticmethod
-    def _test_field_serializabiltiy(field: ModelField) -> bool:
-        """Test JSON serializability for given pydantic `ModelField`.
+    def _test_field_serializabiltiy(field: FieldInfo) -> bool:
+        """Test JSON serializability for given pydantic `FieldInfo`.
 
         """
 
-        class Cfg:
-            arbitrary_types_allowed = True
+        model_config = ConfigDict(arbitrary_types_allowed=True)
 
         try:
-            field_args = (field.type_, field.default)
-            model = create_model("_", test_field=field_args, Config=Cfg)
-            model.schema()
+            field_args = (field.annotation, field.default)
+            model = create_model("_",
+                                 __config__=model_config,
+                                 test_field=field_args)
+            model.model_json_schema()
             return True
 
         except Exception:
             return False
 
     @property
     def non_json_serializable(self) -> List[str]:
@@ -266,104 +294,91 @@
     """Provide namespace for inspection methods for validators of pydantic
     models.
 
     """
 
     def __init__(self, parent: 'ModelInspector'):
         super().__init__(parent)
-        self.attribute: Dict[str, List[Validator]] = self.model.__validators__
 
     @property
     def values(self) -> Set[ValidatorAdapter]:
         """Returns set of all available validators.
 
         """
 
         all_validators = self._parent.field_validator_mappings.values()
         flattened = itertools.chain.from_iterable(all_validators)
         return set(flattened)
 
-    def get_reused_validator_method_names(self) -> List[str]:
-        """Identify all bound methods names that are used to generate reused
-        validators as placeholders.
-
-        """
-
-        reused_validators = self.get_reused_validators()
-        if not reused_validators:
-            return []
-
-        validator_set = set([x.func for x in reused_validators])
-        bound_methods = {key: value
-                         for key, value in vars(self.model).items()
-                         if inspect.ismethod(getattr(self.model, key))}
-
-        return [key for key, value in bound_methods.items()
-                if value.__func__ in validator_set]
-
-    def get_reused_validators(self) -> List[ValidatorAdapter]:
-        """Identify all reused validators.
+    def get_reused_validators_names(self) -> List[str]:
+        """Identify all reused validators. This is done implicitly by relying
+        on the fact the reused validators are registered as unbound functions
+        instead of bound methods.
 
         """
 
-        return [validator for validator in self.values
-                if not validator.is_member(self.model)]
+        validators = self.model.__pydantic_decorators__.field_validators
+        return [x.cls_var_name
+                for x in validators.values()
+                if inspect.isfunction(x.func)]
 
     @property
     def names(self) -> Set[str]:
         """Return names of all validators of pydantic model.
 
         """
 
         return set([validator.name for validator in self.values])
 
     def __bool__(self):
         """Equals to False if no validators are present.
 
         """
 
-        return bool(self.attribute)
+        return bool(self.values)
 
 
 class ConfigInspector(BaseInspectionComposite):
     """Provide namespace for inspection methods for config class of pydantic
     models.
 
     """
 
     def __init__(self, parent: 'ModelInspector'):
         super().__init__(parent)
-        self.attribute: Dict = self.model.Config
+        self.items = self._get_values_per_type()
 
-    @property
-    def is_configured(self) -> bool:
-        """Check if pydantic model config was explicitly configured. If not,
-        it defaults to the standard configuration provided by pydantic and
-        typically does not required documentation.
+    def _get_values_per_type(self) -> Dict[str, str]:
+        """Get the configuration values from any pydantic model.
+
+        Behavior of configuration values varies between `BaseModel` and
+        BaseSettings`. For `BaseModel`, if no configs are provided, then
+        model_config` is empty. However, for `BaseSettings`, `model_config`
+        contains a predefined set of values. This needs to be handled properly
+        otherwise the `BaseSettings` always show up a lot of irrelevant default
+        values. Hence, the default values are removed.
 
         """
 
-        cfg = self.attribute
+        values = self.model.model_config
 
-        is_main_config = cfg is pydantic.main.BaseConfig
-        is_setting_config = cfg is pydantic.env_settings.BaseSettings.Config
-        is_default_config = is_main_config or is_setting_config
+        if issubclass(self.model, BaseSettings):
+            default = tuple(BaseSettings.model_config.items())
+            available = tuple(values.items())
 
-        return not is_default_config
+            result = [given for given in available if given not in default]
+            values = dict(result)
 
-    @property
-    def items(self) -> Dict:
-        """Return all non private (without leading underscore `_`) items of
-        pydantic configuration class.
+        return values
 
-        """
+    @property
+    def is_configured(self) -> bool:
+        """Check if pydantic model config was explicitly configured."""
 
-        return {key: getattr(self.attribute, key)
-                for key in dir(self.attribute)
-                if not key.startswith("_")}
+        return bool(self.items)
 
 
 class ReferenceInspector(BaseInspectionComposite):
     """Provide namespace for inspection methods for creating references
     mainly between pydantic fields and validators.
 
     Importantly, `mappings` provides the set of all `ValidatorFieldMap`
@@ -444,19 +459,24 @@
         fields will be replaced by TypeVars.
 
         """
 
         try:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
-                return self.model.schema()
+                schema = self.model.model_json_schema()
 
-        except (TypeError, ValueError):
+        except (TypeError, ValueError, PydanticInvalidForJsonSchema):
             new_model = self.create_sanitized_model()
-            return new_model.schema()
+            schema = new_model.model_json_schema()
+
+        keys_order = ["title", "description", "type", "properties"]
+        reordered_schema = {k: schema[k] for k in keys_order if k in schema}
+        reordered_schema.update(schema)
+        return reordered_schema
 
     def create_sanitized_model(self) -> BaseModel:
         """Generates a new pydantic model from the original one while
         substituting invalid fields with typevars.
 
         """
 
@@ -486,15 +506,15 @@
         """Determine if given `field` is a pydantic field.
 
         """
 
         if not cls.is_pydantic_model(parent):
             return False
 
-        return field_name in parent.__fields__
+        return field_name in parent.model_fields
 
     @classmethod
     def is_validator_by_name(cls, name: str, obj: Any) -> bool:
         """Determine if a validator is present under provided `name` for given
         `model`.
 
         """
@@ -528,29 +548,24 @@
 
         Validators are wrapped into `ValidatorAdapters` to provide uniform
         interface within autodoc_pydantic.
 
         """
 
         mapping = defaultdict(list)
+        decorators = self.model.__pydantic_decorators__
 
-        # standard validators
-        for field, validators in self.model.__validators__.items():
-            for validator in validators:
+        # field validators
+        for validator in decorators.field_validators.values():
+            for field in validator.info.fields:
                 mapping[field].append(ValidatorAdapter(func=validator.func))
 
-        # root pre
-        for func in self.model.__pre_root_validators__:
-            mapping["*"].append(ValidatorAdapter(func=func,
-                                                 root_pre=True))
-
-        # root post
-        for _, func in self.model.__post_root_validators__:
-            mapping["*"].append(ValidatorAdapter(func=func,
-                                                 root_post=True))
+        # model validators
+        for validator in decorators.model_validators.values():
+            mapping["*"].append(ValidatorAdapter(func=validator.func))
 
         return mapping
 
     @classmethod
     def from_child_signode(cls, signode: desc_signature) -> "ModelInspector":
         """Create instance from a child `signode` as used within sphinx
         directives.
```

### Comparing `autodoc_pydantic-1.9.0/sphinxcontrib/autodoc_pydantic/utility.py` & `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/utility.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-1.9.0/PKG-INFO` & `autodoc_pydantic-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodoc-pydantic
-Version: 1.9.0
+Version: 2.0.0
 Summary: Seamlessly integrate pydantic models in your Sphinx documentation.
 Home-page: https://github.com/mansenfranzen/autodoc_pydantic
 License: MIT
 Keywords: sphinx,pydantic,autodoc,documentation,extension
 Author: mansenfranzen
 Author-email: franz.woellert@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -17,19 +17,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: erdantic
 Provides-Extra: test
-Requires-Dist: Sphinx (>=3.4)
+Requires-Dist: Sphinx (>=4.0)
 Requires-Dist: coverage (>=7,<8) ; extra == "test" or extra == "dev"
-Requires-Dist: erdantic (>=0.5,<0.6) ; extra == "erdantic"
+Requires-Dist: erdantic (>=0.6,<0.7) ; extra == "erdantic"
 Requires-Dist: flake8 (>=3,<4) ; extra == "dev"
-Requires-Dist: pydantic (>=1.5,<2.0.0)
+Requires-Dist: importlib-metadata (>1) ; python_version <= "3.8"
+Requires-Dist: pydantic (>=2.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0,<3.0.0)
 Requires-Dist: pytest (>=7,<8) ; extra == "test" or extra == "dev"
 Requires-Dist: sphinx-copybutton (>=0.4,<0.5) ; extra == "docs" or extra == "dev"
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs" or extra == "dev"
 Requires-Dist: sphinx-tabs (>=3,<4) ; extra == "docs" or extra == "dev"
 Requires-Dist: sphinxcontrib-mermaid (>=0.7,<0.8) ; extra == "docs" or extra == "dev"
 Requires-Dist: tox (>=3,<4) ; extra == "dev"
 Project-URL: Documentation, https://github.com/mansenfranzen/autodoc_pydantic
@@ -41,15 +43,15 @@
 [![PyPI version](https://img.shields.io/pypi/v/autodoc_pydantic?style=for-the-badge)](https://pypi.org/project/autodoc-pydantic/)
 ![Python](https://img.shields.io/badge/python-3.7+-blue.svg?style=for-the-badge)
 
 [![Master](https://img.shields.io/github/actions/workflow/status/mansenfranzen/autodoc_pydantic/tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/autodoc_pydantic/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic)
 
 [![Downloads](https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-badge)](https://pypistats.org/packages/autodoc-pydantic)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-31-orange.svg?style=for-the-badge)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-34-orange.svg?style=for-the-badge)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 You love [pydantic](https://pydantic-docs.helpmanual.io/) ❤ and you want to
 document your models and configuration settings with [sphinx](https://www.sphinx-doc.org/en/master/)?
 
 Perfect, let's go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html)
@@ -62,32 +64,33 @@
 - 💬 provides default values, alias and constraints for model fields
 - 🔗 adds hyperlinks between validators and corresponding fields
 - 📃 includes collapsable model json schema
 - 🏄 natively integrates with autodoc and autosummary extensions
 - 📎 defines explicit pydantic prefixes for models, settings, fields, validators and model config
 - 📋 shows summary section for model configuration, fields and validators
 - 👀 hides overloaded and redundant model class signature
-- 📚 sorts fields, validators and model config within models by type
-- 🍀 Supports `pydantic >= 1.5.0` and `sphinx >= 3.4.0`
-
-### Comparison between autodoc sphinx and autodoc pydantic
-
-[![Comparison](https://raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/main/docs/source/material/example_comparison_v1.0.0.gif)](https://autodoc-pydantic.readthedocs.io/en/latest/examples.html#default-configuration)
-
-To see those features in action, jump over to the [example documentation](https://autodoc-pydantic.readthedocs.io/en/stable/users/examples.html#default-configuration) to compare
-the appearance of standard sphinx autodoc with *autodoc_pydantic*.
+- 🔱 visualizes entity-relationship-diagrams for class hierarchies
+- 🍀 Supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0`
 
 ## Documentation
 
 For more details, please visit the official [documentation](https://autodoc-pydantic.readthedocs.io/en/stable/):
 
 - [Installation](https://autodoc-pydantic.readthedocs.io/en/stable/users/installation.html)
 - [Configuration](https://autodoc-pydantic.readthedocs.io/en/stable/users/configuration.html)
 - [Usage](https://autodoc-pydantic.readthedocs.io/en/stable/users/usage.html)
 - [Examples](https://autodoc-pydantic.readthedocs.io/en/stable/users/examples.html)
+- [Developer Guide](https://autodoc-pydantic.readthedocs.io/en/stable/developers/setup.html)
+
+## Comparison between autodoc sphinx and autodoc pydantic
+
+[![Comparison](https://raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/main/docs/source/material/example_comparison_v1.0.0.gif)](https://autodoc-pydantic.readthedocs.io/en/latest/examples.html#default-configuration)
+
+To see those features in action, jump over to the [example documentation](https://autodoc-pydantic.readthedocs.io/en/stable/users/examples.html#default-configuration) to compare
+the appearance of standard sphinx autodoc with *autodoc_pydantic*.
 
 ## Acknowledgements
 
 Thanks to great open source projects [sphinx](https://www.sphinx-doc.org/en/master/),
 [pydantic](https://pydantic-docs.helpmanual.io/) and
 [poetry](https://python-poetry.org/) (and so many more) ❤ in addition to the following contributors:
 
@@ -132,14 +135,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://t.me/pipeknight"><img src="https://avatars.githubusercontent.com/u/34810566?v=4?s=100" width="100px;" alt="Evgeniy Lupashin"/><br /><sub><b>Evgeniy Lupashin</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3APipeKnight" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://janhendrikewers.uk/"><img src="https://avatars.githubusercontent.com/u/12383029?v=4?s=100" width="100px;" alt="Jan-Hendrik Ewers"/><br /><sub><b>Jan-Hendrik Ewers</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Aiwishiwasaneagle" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://jon-e.net"><img src="https://avatars.githubusercontent.com/u/12961499?v=4?s=100" width="100px;" alt="Jonny Saunders"/><br /><sub><b>Jonny Saunders</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Asneakers-the-rat" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://charlie.machalow.com"><img src="https://avatars.githubusercontent.com/u/5749838?v=4?s=100" width="100px;" alt="Charles Machalow"/><br /><sub><b>Charles Machalow</b></sub></a><br /><a href="#question-csm10495" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tkaraouzene"><img src="https://avatars.githubusercontent.com/u/20064077?v=4?s=100" width="100px;" alt="Thomas Karaouzene"/><br /><sub><b>Thomas Karaouzene</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Atkaraouzene" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/caseyzak24"><img src="https://avatars.githubusercontent.com/u/29411281?v=4?s=100" width="100px;" alt="caseyzak24"/><br /><sub><b>caseyzak24</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=caseyzak24" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/PriOliveira"><img src="https://avatars.githubusercontent.com/u/13801839?v=4?s=100" width="100px;" alt="Priscila Oliveira"/><br /><sub><b>Priscila Oliveira</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3APriOliveira" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-PriOliveira" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/awoimbee"><img src="https://avatars.githubusercontent.com/u/22431493?v=4?s=100" width="100px;" alt="Arthur Woimbée"/><br /><sub><b>Arthur Woimbée</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Aawoimbee" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-awoimbee" title="User Testing">📓</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Tests">⚠️</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

