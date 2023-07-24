# Comparing `tmp/angreal-2.0.8.tar.gz` & `tmp/angreal-2.0.9.tar.gz`

## Comparing `angreal-2.0.8.tar` & `angreal-2.0.9.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 angreal-2.0.8/Cargo.toml
--rw-r--r--   0      501       20     1461 2023-07-23 15:44:48.000000 angreal-2.0.8/.angreal/task_run_tests.py
--rw-r--r--   0      501       20      394 2023-07-23 15:44:48.000000 angreal-2.0.8/.angreal/task_setup.py
--rw-r--r--   0      501       20     1778 2023-07-23 15:44:48.000000 angreal-2.0.8/.github/workflows/docs.yaml
--rw-r--r--   0      501       20     7958 2023-07-23 15:44:48.000000 angreal-2.0.8/.github/workflows/release.yaml
--rw-r--r--   0      501       20     3721 2023-07-23 15:44:48.000000 angreal-2.0.8/.github/workflows/test.yaml
--rw-r--r--   0      501       20     5668 2023-07-23 15:44:48.000000 angreal-2.0.8/.gitignore
--rw-r--r--   0      501       20     1176 2023-07-23 15:44:48.000000 angreal-2.0.8/.pre-commit-config.yaml
--rw-r--r--   0      501       20        6 2023-07-23 15:44:48.000000 angreal-2.0.8/.spelling_wordlist.txt
--rw-r--r--   0      501       20      887 2023-07-23 15:44:48.000000 angreal-2.0.8/.yamllint-config.yml
--rw-r--r--   0      501       20     2563 2023-07-23 15:44:48.000000 angreal-2.0.8/README.md
--rw-r--r--   0      501       20      825 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/_draft/how_to/include-jinja-templates.rst.md
--rw-r--r--   0      501       20      365 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/_draft/how_to/use-docker-integration.rst.md
--rw-r--r--   0      501       20      548 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/_draft/how_to/use-git-integration.rst.md
--rw-r--r--   0      501       20      864 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/_draft/how_to/work_with_virtual_environments.rst.md
--rw-r--r--   0      501       20       83 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/archetypes/default.md
--rw-r--r--   0      501       20     2787 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/config.toml
--rw-r--r--   0      501       20     2551 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/_index.md
--rw-r--r--   0      501       20      493 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/api_reference/_index.md
--rw-r--r--   0      501       20       55 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/api_reference/py_angreal/_index.md
--rw-r--r--   0      501       20     2122 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/api_reference/py_angreal/argument_decorator.md
--rw-r--r--   0      501       20      645 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/api_reference/py_angreal/command_decorator.md
--rw-r--r--   0      501       20     1125 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/api_reference/py_angreal/command_group.md
--rw-r--r--   0      501       20      318 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/api_reference/py_angreal/get_root.md
--rw-r--r--   0      501       20      473 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/api_reference/py_angreal/required_version.md
--rw-r--r--   0      501       20       64 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/available_templates/_index.md
--rw-r--r--   0      501       20     3212 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/code_of_conduct/_index.md
--rw-r--r--   0      501       20     1311 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/contributing/_index.md
--rw-r--r--   0      501       20       56 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/discussions/_index.md
--rw-r--r--   0      501       20     1816 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/discussions/angreal_init_behaviour.md
--rw-r--r--   0      501       20       58 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/how-to/_index.md
--rw-r--r--   0      501       20     4380 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/how-to/add_arguments.md
--rw-r--r--   0      501       20      321 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/how-to/create_a_task.md
--rw-r--r--   0      501       20      560 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/how-to/create_task_group.md
--rw-r--r--   0      501       20       63 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/tutorials/_index.md
--rw-r--r--   0      501       20       69 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/tutorials/meeting_notes.files/angreal.toml
--rw-r--r--   0      501       20       62 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/init.py
--rw-r--r--   0      501       20     1254 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py
--rw-r--r--   0      501       20       85 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/tutorials/meeting_notes.files/{{ name }}/README.md
--rw-r--r--   0      501       20     5274 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/tutorials/your-first-angreal.md
--rw-r--r--   0      501       20     5660 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/content/why/_index.md
--rw-r--r--   0      501       20      198 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/layouts/partials/logo.html
--rw-r--r--   0      501       20     6445 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/static/images/wheel.png
--rw-r--r--   0      501       20     1139 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/LICENSE.md
--rw-r--r--   0      501       20      169 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/archetypes/chapter.md
--rw-r--r--   0      501       20       99 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/archetypes/default.md
--rw-r--r--   0      501       20      585 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/ar.toml
--rw-r--r--   0      501       20      507 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/de.toml
--rw-r--r--   0      501       20      487 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/en.toml
--rw-r--r--   0      501       20      484 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/es.toml
--rw-r--r--   0      501       20      531 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/fr.toml
--rw-r--r--   0      501       20      726 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/hi.toml
--rw-r--r--   0      501       20      499 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/id.toml
--rw-r--r--   0      501       20      514 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/ja.toml
--rw-r--r--   0      501       20      499 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/nl.toml
--rw-r--r--   0      501       20      490 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/pt.toml
--rw-r--r--   0      501       20      623 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/ru.toml
--rw-r--r--   0      501       20      495 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/tr.toml
--rw-r--r--   0      501       20      710 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/vn.toml
--rw-r--r--   0      501       20      484 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/zh-cn.toml
--rw-r--r--   0      501       20   284162 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/images/screenshot.png
--rw-r--r--   0      501       20   143335 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/images/tn.png
--rw-r--r--   0      501       20     2263 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/404.html
--rw-r--r--   0      501       20      550 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/_default/list.html
--rw-r--r--   0      501       20      354 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/_default/single.html
--rw-r--r--   0      501       20     1384 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/index.html
--rw-r--r--   0      501       20      429 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/index.json
--rw-r--r--   0      501       20       78 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/custom-comments.html
--rw-r--r--   0      501       20      180 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/custom-footer.html
--rw-r--r--   0      501       20      148 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/custom-header.html
--rw-r--r--   0      501       20       76 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/favicon.html
--rw-r--r--   0      501       20     4539 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/footer.html
--rw-r--r--   0      501       20     5312 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/header.html
--rw-r--r--   0      501       20      137 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/logo.html
--rw-r--r--   0      501       20      193 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/menu-footer.html
--rw-r--r--   0      501       20     6236 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/menu.html
--rw-r--r--   0      501       20      215 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/meta.html
--rw-r--r--   0      501       20      911 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/search.html
--rw-r--r--   0      501       20      172 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/tags.html
--rw-r--r--   0      501       20       90 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/toc.html
--rw-r--r--   0      501       20     1176 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html
--rw-r--r--   0      501       20      452 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/button.html
--rw-r--r--   0      501       20     4463 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html
--rw-r--r--   0      501       20      730 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html
--rw-r--r--   0      501       20      164 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/mermaid.html
--rw-r--r--   0      501       20      151 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/notice.html
--rw-r--r--   0      501       20      441 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/ref.html
--rw-r--r--   0      501       20      441 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/relref.html
--rw-r--r--   0      501       20      191 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/siteparam.html
--rw-r--r--   0      501       20      369 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/tab.html
--rw-r--r--   0      501       20      793 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html
--rw-r--r--   0      501       20     1588 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css
--rw-r--r--   0      501       20      890 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/auto-complete.css
--rw-r--r--   0      501       20     1869 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/featherlight.min.css
--rw-r--r--   0      501       20   101895 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css
--rw-r--r--   0      501       20     4755 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/hugo-theme.css
--rw-r--r--   0      501       20     1342 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/hybrid.css
--rw-r--r--   0      501       20    11887 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/nucleus.css
--rw-r--r--   0      501       20     4629 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css
--rw-r--r--   0      501       20      859 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/tabs.css
--rw-r--r--   0      501       20     1010 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/tags.css
--rw-r--r--   0      501       20     4088 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme-blue.css
--rw-r--r--   0      501       20     4088 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme-green.css
--rw-r--r--   0      501       20     4085 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme-red.css
--rw-r--r--   0      501       20    24719 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme.css
--rw-r--r--   0      501       20    35620 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot
--rw-r--r--   0      501       20    61991 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg
--rw-r--r--   0      501       20    63184 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf
--rw-r--r--   0      501       20    38248 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff
--rw-r--r--   0      501       20    22446 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot
--rw-r--r--   0      501       20    98610 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg
--rw-r--r--   0      501       20    56884 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf
--rw-r--r--   0      501       20    24772 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff
--rw-r--r--   0      501       20    19760 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2
--rw-r--r--   0      501       20    21080 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot
--rw-r--r--   0      501       20    91969 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg
--rw-r--r--   0      501       20    55600 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf
--rw-r--r--   0      501       20    23476 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff
--rw-r--r--   0      501       20    18716 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2
--rw-r--r--   0      501       20    24290 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot
--rw-r--r--   0      501       20    54839 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg
--rw-r--r--   0      501       20    49752 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf
--rw-r--r--   0      501       20    25896 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff
--rw-r--r--   0      501       20    21128 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2
--rw-r--r--   0      501       20    24817 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot
--rw-r--r--   0      501       20    54787 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg
--rw-r--r--   0      501       20    50784 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf
--rw-r--r--   0      501       20    26392 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff
--rw-r--r--   0      501       20    21548 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2
--rw-r--r--   0      501       20    26481 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot
--rw-r--r--   0      501       20    54422 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg
--rw-r--r--   0      501       20    54232 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf
--rw-r--r--   0      501       20    27900 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff
--rw-r--r--   0      501       20    22884 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2
--rw-r--r--   0      501       20      510 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/images/clippy.svg
--rw-r--r--   0      501       20      608 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/images/favicon.png
--rw-r--r--   0      501       20   206249 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg
--rw-r--r--   0      501       20     5328 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/auto-complete.js
--rw-r--r--   0      501       20    10754 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/clipboard.min.js
--rw-r--r--   0      501       20     9296 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/featherlight.min.js
--rw-r--r--   0      501       20    95350 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/highlight.pack.js
--rw-r--r--   0      501       20     2847 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/hugo-learn.js
--rw-r--r--   0      501       20    86927 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js
--rwxr-xr-x   0      501       20    10085 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js
--rw-r--r--   0      501       20    16771 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/learn.js
--rw-r--r--   0      501       20    29528 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/lunr.min.js
--rw-r--r--   0      501       20     7547 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js
--rw-r--r--   0      501       20    25333 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js
--rw-r--r--   0      501       20    25012 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js
--rw-r--r--   0      501       20     3443 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/search.js
--rw-r--r--   0      501       20   832983 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js
--rw-r--r--   0      501       20   134396 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot
--rw-r--r--   0      501       20   739403 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg
--rw-r--r--   0      501       20   186124 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0      501       20    87048 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff
--rw-r--r--   0      501       20   107656 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0      501       20    40308 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot
--rw-r--r--   0      501       20   135805 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg
--rw-r--r--   0      501       20    62320 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0      501       20    18164 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff
--rw-r--r--   0      501       20    25236 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0      501       20   209012 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot
--rw-r--r--   0      501       20   771698 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg
--rw-r--r--   0      501       20   397420 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0      501       20   102224 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff
--rw-r--r--   0      501       20   150516 2023-07-23 15:44:48.000000 angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0      501       20        0 2023-07-23 15:44:48.000000 angreal-2.0.8/py_tests/__init__.py
--rw-r--r--   0      501       20     2053 2023-07-23 15:44:48.000000 angreal-2.0.8/py_tests/integrations/test_docker.py
--rw-r--r--   0      501       20      831 2023-07-23 15:44:48.000000 angreal-2.0.8/py_tests/integrations/test_git.py
--rw-r--r--   0      501       20        6 2023-07-23 15:44:48.000000 angreal-2.0.8/py_tests/integrations/test_r.txt
--rw-r--r--   0      501       20     2385 2023-07-23 15:44:48.000000 angreal-2.0.8/py_tests/integrations/test_venv.py
--rw-r--r--   0      501       20     3547 2023-07-23 15:44:48.000000 angreal-2.0.8/py_tests/test_angreal.py
--rw-r--r--   0      501       20      930 2023-07-23 15:44:48.000000 angreal-2.0.8/pyproject.toml
--rw-r--r--   0      501       20     5041 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/__init__.py
--rw-r--r--   0      501       20       68 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/integrations/docker/__init__.py
--rw-r--r--   0      501       20       85 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/integrations/docker/container.py
--rw-r--r--   0      501       20       74 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/integrations/docker/image.py
--rw-r--r--   0      501       20       80 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/integrations/docker/network.py
--rw-r--r--   0      501       20       77 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/integrations/docker/volume.py
--rw-r--r--   0      501       20     2664 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/integrations/git.py
--rw-r--r--   0      501       20     4782 2023-07-23 15:44:48.000000 angreal-2.0.8/python/angreal/integrations/venv.py
--rw-r--r--   0      501       20       31 2023-07-23 15:44:48.000000 angreal-2.0.8/rust-toolchain.toml
--rw-r--r--   0      501       20     6270 2023-07-23 15:44:48.000000 angreal-2.0.8/src/builder.rs
--rw-r--r--   0      501       20     7183 2023-07-23 15:44:48.000000 angreal-2.0.8/src/git/mod.rs
--rw-r--r--   0      501       20    19080 2023-07-23 15:44:48.000000 angreal-2.0.8/src/init.rs
--rw-r--r--   0      501       20     7817 2023-07-23 15:44:48.000000 angreal-2.0.8/src/lib.rs
--rw-r--r--   0      501       20     1284 2023-07-23 15:44:48.000000 angreal-2.0.8/src/logger.rs
--rw-r--r--   0      501       20     1039 2023-07-23 15:44:48.000000 angreal-2.0.8/src/macros.rs
--rw-r--r--   0      501       20     3290 2023-07-23 15:44:48.000000 angreal-2.0.8/src/py_logger.rs
--rw-r--r--   0      501       20     8423 2023-07-23 15:44:48.000000 angreal-2.0.8/src/task.rs
--rw-r--r--   0      501       20     7510 2023-07-23 15:44:48.000000 angreal-2.0.8/src/utils.rs
--rw-r--r--   0      501       20      672 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/mod.rs
--rw-r--r--   0      501       20       41 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/bad_import_init.py
--rw-r--r--   0      501       20       41 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/bad_import_task.py
--rw-r--r--   0      501       20       34 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/exception_init.py
--rw-r--r--   0      501       20       32 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/exception_task.py
--rw-r--r--   0      501       20        0 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/good_init.py
--rw-r--r--   0      501       20      109 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/good_task.py
--rw-r--r--   0      501       20        0 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/internal_module/__init__.py
--rw-r--r--   0      501       20       30 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/no_func_init.py
--rw-r--r--   0      501       20       30 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/no_func_task.py
--rw-r--r--   0      501       20        0 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/test_template/.wee
--rw-r--r--   0      501       20      116 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/test_template/angreal.toml
--rw-r--r--   0      501       20       21 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/test_template/{{ folder_variable }}/.angreal/init.py
--rw-r--r--   0      501       20       20 2023-07-23 15:44:48.000000 angreal-2.0.8/tests/common/test_assets/test_template/{{ folder_variable }}/README.rst
--rw-r--r--   0      501       20    72292 2023-07-23 15:44:48.000000 angreal-2.0.8/Cargo.lock
--rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 angreal-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 angreal-2.0.9/Cargo.toml
+-rw-r--r--   0      501       20     1461 2023-07-23 23:46:49.000000 angreal-2.0.9/.angreal/task_run_tests.py
+-rw-r--r--   0      501       20      394 2023-07-23 23:46:49.000000 angreal-2.0.9/.angreal/task_setup.py
+-rw-r--r--   0      501       20     1778 2023-07-23 23:46:49.000000 angreal-2.0.9/.github/workflows/docs.yaml
+-rw-r--r--   0      501       20     7958 2023-07-23 23:46:49.000000 angreal-2.0.9/.github/workflows/release.yaml
+-rw-r--r--   0      501       20     3721 2023-07-23 23:46:49.000000 angreal-2.0.9/.github/workflows/test.yaml
+-rw-r--r--   0      501       20     5668 2023-07-23 23:46:49.000000 angreal-2.0.9/.gitignore
+-rw-r--r--   0      501       20     1176 2023-07-23 23:46:49.000000 angreal-2.0.9/.pre-commit-config.yaml
+-rw-r--r--   0      501       20        6 2023-07-23 23:46:49.000000 angreal-2.0.9/.spelling_wordlist.txt
+-rw-r--r--   0      501       20      887 2023-07-23 23:46:49.000000 angreal-2.0.9/.yamllint-config.yml
+-rw-r--r--   0      501       20     2563 2023-07-23 23:46:49.000000 angreal-2.0.9/README.md
+-rw-r--r--   0      501       20      825 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/_draft/how_to/include-jinja-templates.rst.md
+-rw-r--r--   0      501       20      365 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/_draft/how_to/use-docker-integration.rst.md
+-rw-r--r--   0      501       20      548 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/_draft/how_to/use-git-integration.rst.md
+-rw-r--r--   0      501       20      864 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/_draft/how_to/work_with_virtual_environments.rst.md
+-rw-r--r--   0      501       20       83 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/archetypes/default.md
+-rw-r--r--   0      501       20     2787 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/config.toml
+-rw-r--r--   0      501       20     2551 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/_index.md
+-rw-r--r--   0      501       20      493 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/api_reference/_index.md
+-rw-r--r--   0      501       20       55 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/api_reference/py_angreal/_index.md
+-rw-r--r--   0      501       20     2122 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/api_reference/py_angreal/argument_decorator.md
+-rw-r--r--   0      501       20      645 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/api_reference/py_angreal/command_decorator.md
+-rw-r--r--   0      501       20     1125 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/api_reference/py_angreal/command_group.md
+-rw-r--r--   0      501       20      318 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/api_reference/py_angreal/get_root.md
+-rw-r--r--   0      501       20      473 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/api_reference/py_angreal/required_version.md
+-rw-r--r--   0      501       20       64 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/available_templates/_index.md
+-rw-r--r--   0      501       20     3212 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/code_of_conduct/_index.md
+-rw-r--r--   0      501       20     1311 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/contributing/_index.md
+-rw-r--r--   0      501       20       56 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/discussions/_index.md
+-rw-r--r--   0      501       20     1816 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/discussions/angreal_init_behaviour.md
+-rw-r--r--   0      501       20       58 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/how-to/_index.md
+-rw-r--r--   0      501       20     4380 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/how-to/add_arguments.md
+-rw-r--r--   0      501       20      321 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/how-to/create_a_task.md
+-rw-r--r--   0      501       20      560 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/how-to/create_task_group.md
+-rw-r--r--   0      501       20       63 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/tutorials/_index.md
+-rw-r--r--   0      501       20       69 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/tutorials/meeting_notes.files/angreal.toml
+-rw-r--r--   0      501       20       62 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/init.py
+-rw-r--r--   0      501       20     1254 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py
+-rw-r--r--   0      501       20       85 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/tutorials/meeting_notes.files/{{ name }}/README.md
+-rw-r--r--   0      501       20     5274 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/tutorials/your-first-angreal.md
+-rw-r--r--   0      501       20     5660 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/content/why/_index.md
+-rw-r--r--   0      501       20      198 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/layouts/partials/logo.html
+-rw-r--r--   0      501       20     6445 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/static/images/wheel.png
+-rw-r--r--   0      501       20     1139 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/LICENSE.md
+-rw-r--r--   0      501       20      169 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/archetypes/chapter.md
+-rw-r--r--   0      501       20       99 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/archetypes/default.md
+-rw-r--r--   0      501       20      585 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/ar.toml
+-rw-r--r--   0      501       20      507 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/de.toml
+-rw-r--r--   0      501       20      487 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/en.toml
+-rw-r--r--   0      501       20      484 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/es.toml
+-rw-r--r--   0      501       20      531 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/fr.toml
+-rw-r--r--   0      501       20      726 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/hi.toml
+-rw-r--r--   0      501       20      499 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/id.toml
+-rw-r--r--   0      501       20      514 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/ja.toml
+-rw-r--r--   0      501       20      499 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/nl.toml
+-rw-r--r--   0      501       20      490 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/pt.toml
+-rw-r--r--   0      501       20      623 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/ru.toml
+-rw-r--r--   0      501       20      495 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/tr.toml
+-rw-r--r--   0      501       20      710 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/vn.toml
+-rw-r--r--   0      501       20      484 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/zh-cn.toml
+-rw-r--r--   0      501       20   284162 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/images/screenshot.png
+-rw-r--r--   0      501       20   143335 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/images/tn.png
+-rw-r--r--   0      501       20     2263 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/404.html
+-rw-r--r--   0      501       20      550 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/_default/list.html
+-rw-r--r--   0      501       20      354 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/_default/single.html
+-rw-r--r--   0      501       20     1384 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/index.html
+-rw-r--r--   0      501       20      429 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/index.json
+-rw-r--r--   0      501       20       78 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/custom-comments.html
+-rw-r--r--   0      501       20      180 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/custom-footer.html
+-rw-r--r--   0      501       20      148 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/custom-header.html
+-rw-r--r--   0      501       20       76 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/favicon.html
+-rw-r--r--   0      501       20     4539 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/footer.html
+-rw-r--r--   0      501       20     5312 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/header.html
+-rw-r--r--   0      501       20      137 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/logo.html
+-rw-r--r--   0      501       20      193 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/menu-footer.html
+-rw-r--r--   0      501       20     6236 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/menu.html
+-rw-r--r--   0      501       20      215 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/meta.html
+-rw-r--r--   0      501       20      911 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/search.html
+-rw-r--r--   0      501       20      172 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/tags.html
+-rw-r--r--   0      501       20       90 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/toc.html
+-rw-r--r--   0      501       20     1176 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html
+-rw-r--r--   0      501       20      452 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/button.html
+-rw-r--r--   0      501       20     4463 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html
+-rw-r--r--   0      501       20      730 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html
+-rw-r--r--   0      501       20      164 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/mermaid.html
+-rw-r--r--   0      501       20      151 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/notice.html
+-rw-r--r--   0      501       20      441 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/ref.html
+-rw-r--r--   0      501       20      441 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/relref.html
+-rw-r--r--   0      501       20      191 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/siteparam.html
+-rw-r--r--   0      501       20      369 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/tab.html
+-rw-r--r--   0      501       20      793 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html
+-rw-r--r--   0      501       20     1588 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css
+-rw-r--r--   0      501       20      890 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/auto-complete.css
+-rw-r--r--   0      501       20     1869 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/featherlight.min.css
+-rw-r--r--   0      501       20   101895 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css
+-rw-r--r--   0      501       20     4755 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/hugo-theme.css
+-rw-r--r--   0      501       20     1342 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/hybrid.css
+-rw-r--r--   0      501       20    11887 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/nucleus.css
+-rw-r--r--   0      501       20     4629 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css
+-rw-r--r--   0      501       20      859 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/tabs.css
+-rw-r--r--   0      501       20     1010 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/tags.css
+-rw-r--r--   0      501       20     4088 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme-blue.css
+-rw-r--r--   0      501       20     4088 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme-green.css
+-rw-r--r--   0      501       20     4085 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme-red.css
+-rw-r--r--   0      501       20    24719 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme.css
+-rw-r--r--   0      501       20    35620 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot
+-rw-r--r--   0      501       20    61991 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg
+-rw-r--r--   0      501       20    63184 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf
+-rw-r--r--   0      501       20    38248 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff
+-rw-r--r--   0      501       20    22446 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot
+-rw-r--r--   0      501       20    98610 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg
+-rw-r--r--   0      501       20    56884 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf
+-rw-r--r--   0      501       20    24772 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff
+-rw-r--r--   0      501       20    19760 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2
+-rw-r--r--   0      501       20    21080 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot
+-rw-r--r--   0      501       20    91969 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg
+-rw-r--r--   0      501       20    55600 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf
+-rw-r--r--   0      501       20    23476 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff
+-rw-r--r--   0      501       20    18716 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2
+-rw-r--r--   0      501       20    24290 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot
+-rw-r--r--   0      501       20    54839 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg
+-rw-r--r--   0      501       20    49752 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf
+-rw-r--r--   0      501       20    25896 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff
+-rw-r--r--   0      501       20    21128 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2
+-rw-r--r--   0      501       20    24817 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot
+-rw-r--r--   0      501       20    54787 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg
+-rw-r--r--   0      501       20    50784 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf
+-rw-r--r--   0      501       20    26392 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff
+-rw-r--r--   0      501       20    21548 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2
+-rw-r--r--   0      501       20    26481 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot
+-rw-r--r--   0      501       20    54422 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg
+-rw-r--r--   0      501       20    54232 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf
+-rw-r--r--   0      501       20    27900 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff
+-rw-r--r--   0      501       20    22884 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2
+-rw-r--r--   0      501       20      510 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/images/clippy.svg
+-rw-r--r--   0      501       20      608 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/images/favicon.png
+-rw-r--r--   0      501       20   206249 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg
+-rw-r--r--   0      501       20     5328 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/auto-complete.js
+-rw-r--r--   0      501       20    10754 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/clipboard.min.js
+-rw-r--r--   0      501       20     9296 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/featherlight.min.js
+-rw-r--r--   0      501       20    95350 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/highlight.pack.js
+-rw-r--r--   0      501       20     2847 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/hugo-learn.js
+-rw-r--r--   0      501       20    86927 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js
+-rwxr-xr-x   0      501       20    10085 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js
+-rw-r--r--   0      501       20    16771 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/learn.js
+-rw-r--r--   0      501       20    29528 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/lunr.min.js
+-rw-r--r--   0      501       20     7547 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js
+-rw-r--r--   0      501       20    25333 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js
+-rw-r--r--   0      501       20    25012 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js
+-rw-r--r--   0      501       20     3443 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/search.js
+-rw-r--r--   0      501       20   832983 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js
+-rw-r--r--   0      501       20   134396 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot
+-rw-r--r--   0      501       20   739403 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg
+-rw-r--r--   0      501       20   186124 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0      501       20    87048 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff
+-rw-r--r--   0      501       20   107656 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0      501       20    40308 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot
+-rw-r--r--   0      501       20   135805 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg
+-rw-r--r--   0      501       20    62320 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0      501       20    18164 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff
+-rw-r--r--   0      501       20    25236 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0      501       20   209012 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot
+-rw-r--r--   0      501       20   771698 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg
+-rw-r--r--   0      501       20   397420 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0      501       20   102224 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff
+-rw-r--r--   0      501       20   150516 2023-07-23 23:46:49.000000 angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0      501       20        0 2023-07-23 23:46:49.000000 angreal-2.0.9/py_tests/__init__.py
+-rw-r--r--   0      501       20     2053 2023-07-23 23:46:49.000000 angreal-2.0.9/py_tests/integrations/test_docker.py
+-rw-r--r--   0      501       20      831 2023-07-23 23:46:49.000000 angreal-2.0.9/py_tests/integrations/test_git.py
+-rw-r--r--   0      501       20        6 2023-07-23 23:46:49.000000 angreal-2.0.9/py_tests/integrations/test_r.txt
+-rw-r--r--   0      501       20     2385 2023-07-23 23:46:49.000000 angreal-2.0.9/py_tests/integrations/test_venv.py
+-rw-r--r--   0      501       20     3547 2023-07-23 23:46:49.000000 angreal-2.0.9/py_tests/test_angreal.py
+-rw-r--r--   0      501       20      930 2023-07-23 23:46:49.000000 angreal-2.0.9/pyproject.toml
+-rw-r--r--   0      501       20     5041 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/__init__.py
+-rw-r--r--   0      501       20       68 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/integrations/docker/__init__.py
+-rw-r--r--   0      501       20       85 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/integrations/docker/container.py
+-rw-r--r--   0      501       20       74 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/integrations/docker/image.py
+-rw-r--r--   0      501       20       80 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/integrations/docker/network.py
+-rw-r--r--   0      501       20       77 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/integrations/docker/volume.py
+-rw-r--r--   0      501       20     2664 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/integrations/git.py
+-rw-r--r--   0      501       20     4782 2023-07-23 23:46:49.000000 angreal-2.0.9/python/angreal/integrations/venv.py
+-rw-r--r--   0      501       20       31 2023-07-23 23:46:49.000000 angreal-2.0.9/rust-toolchain.toml
+-rw-r--r--   0      501       20     6445 2023-07-23 23:46:49.000000 angreal-2.0.9/src/builder.rs
+-rw-r--r--   0      501       20     7183 2023-07-23 23:46:49.000000 angreal-2.0.9/src/git/mod.rs
+-rw-r--r--   0      501       20    19080 2023-07-23 23:46:49.000000 angreal-2.0.9/src/init.rs
+-rw-r--r--   0      501       20     7817 2023-07-23 23:46:49.000000 angreal-2.0.9/src/lib.rs
+-rw-r--r--   0      501       20     1284 2023-07-23 23:46:49.000000 angreal-2.0.9/src/logger.rs
+-rw-r--r--   0      501       20     1039 2023-07-23 23:46:49.000000 angreal-2.0.9/src/macros.rs
+-rw-r--r--   0      501       20     3290 2023-07-23 23:46:49.000000 angreal-2.0.9/src/py_logger.rs
+-rw-r--r--   0      501       20     8423 2023-07-23 23:46:49.000000 angreal-2.0.9/src/task.rs
+-rw-r--r--   0      501       20     7510 2023-07-23 23:46:49.000000 angreal-2.0.9/src/utils.rs
+-rw-r--r--   0      501       20      672 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/mod.rs
+-rw-r--r--   0      501       20       41 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/bad_import_init.py
+-rw-r--r--   0      501       20       41 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/bad_import_task.py
+-rw-r--r--   0      501       20       34 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/exception_init.py
+-rw-r--r--   0      501       20       32 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/exception_task.py
+-rw-r--r--   0      501       20        0 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/good_init.py
+-rw-r--r--   0      501       20      109 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/good_task.py
+-rw-r--r--   0      501       20        0 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/internal_module/__init__.py
+-rw-r--r--   0      501       20       30 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/no_func_init.py
+-rw-r--r--   0      501       20       30 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/no_func_task.py
+-rw-r--r--   0      501       20        0 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/test_template/.wee
+-rw-r--r--   0      501       20      116 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/test_template/angreal.toml
+-rw-r--r--   0      501       20       21 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/test_template/{{ folder_variable }}/.angreal/init.py
+-rw-r--r--   0      501       20       20 2023-07-23 23:46:49.000000 angreal-2.0.9/tests/common/test_assets/test_template/{{ folder_variable }}/README.rst
+-rw-r--r--   0      501       20    72292 2023-07-23 23:48:18.000000 angreal-2.0.9/Cargo.lock
+-rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 angreal-2.0.9/PKG-INFO
```

### Comparing `angreal-2.0.8/Cargo.toml` & `angreal-2.0.9/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 description = "Angreal is a tool for templating projects and associated processes to provide a consistent developer experience across multiple projects."
 edition = "2021"
 homepage = "https://github.com/angreal/angreal"
 license = "GPL-3.0-only"
 name = "angreal"
 readme = "README.md"
 repository = "https://github.com/angreal/angreal"
-version = "2.0.8"
+version = "2.0.9"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib","rlib"]
 doctest = false
 name = "angreal"
```

### Comparing `angreal-2.0.8/.angreal/task_run_tests.py` & `angreal-2.0.9/.angreal/task_run_tests.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/.github/workflows/docs.yaml` & `angreal-2.0.9/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/.github/workflows/release.yaml` & `angreal-2.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/.github/workflows/test.yaml` & `angreal-2.0.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/.gitignore` & `angreal-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/.pre-commit-config.yaml` & `angreal-2.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/.yamllint-config.yml` & `angreal-2.0.9/.yamllint-config.yml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/README.md` & `angreal-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/_draft/how_to/include-jinja-templates.rst.md` & `angreal-2.0.9/docs/_draft/how_to/include-jinja-templates.rst.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/_draft/how_to/use-git-integration.rst.md` & `angreal-2.0.9/docs/_draft/how_to/use-git-integration.rst.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/_draft/how_to/work_with_virtual_environments.rst.md` & `angreal-2.0.9/docs/_draft/how_to/work_with_virtual_environments.rst.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/config.toml` & `angreal-2.0.9/docs/config.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/_index.md` & `angreal-2.0.9/docs/content/_index.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/api_reference/py_angreal/argument_decorator.md` & `angreal-2.0.9/docs/content/api_reference/py_angreal/argument_decorator.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/api_reference/py_angreal/command_decorator.md` & `angreal-2.0.9/docs/content/api_reference/py_angreal/command_decorator.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/api_reference/py_angreal/command_group.md` & `angreal-2.0.9/docs/content/api_reference/py_angreal/command_group.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/code_of_conduct/_index.md` & `angreal-2.0.9/docs/content/code_of_conduct/_index.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/contributing/_index.md` & `angreal-2.0.9/docs/content/contributing/_index.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/discussions/angreal_init_behaviour.md` & `angreal-2.0.9/docs/content/discussions/angreal_init_behaviour.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/how-to/add_arguments.md` & `angreal-2.0.9/docs/content/how-to/add_arguments.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/how-to/create_task_group.md` & `angreal-2.0.9/docs/content/how-to/create_task_group.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py` & `angreal-2.0.9/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/tutorials/your-first-angreal.md` & `angreal-2.0.9/docs/content/tutorials/your-first-angreal.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/content/why/_index.md` & `angreal-2.0.9/docs/content/why/_index.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/static/images/wheel.png` & `angreal-2.0.9/docs/static/images/wheel.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/LICENSE.md` & `angreal-2.0.9/docs/themes/hugo-theme-learn/LICENSE.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/ar.toml` & `angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/ar.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/fr.toml` & `angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/fr.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/hi.toml` & `angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/hi.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/ja.toml` & `angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/ja.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/ru.toml` & `angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/ru.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/i18n/vn.toml` & `angreal-2.0.9/docs/themes/hugo-theme-learn/i18n/vn.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/images/screenshot.png` & `angreal-2.0.9/docs/themes/hugo-theme-learn/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/images/tn.png` & `angreal-2.0.9/docs/themes/hugo-theme-learn/images/tn.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/404.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/404.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/_default/list.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/_default/list.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/index.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/index.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/footer.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/footer.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/header.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/header.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/menu.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/menu.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/partials/search.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/partials/search.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html` & `angreal-2.0.9/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/auto-complete.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/auto-complete.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/featherlight.min.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/featherlight.min.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/hugo-theme.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/hugo-theme.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/hybrid.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/hybrid.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/nucleus.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/nucleus.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/tabs.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/tags.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/tags.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme-blue.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme-blue.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme-green.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme-green.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme-red.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme-red.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/css/theme.css` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/images/favicon.png` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/auto-complete.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/auto-complete.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/clipboard.min.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/featherlight.min.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/featherlight.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/highlight.pack.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/hugo-learn.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/hugo-learn.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/learn.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/learn.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/lunr.min.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/lunr.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/js/search.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/js/search.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2` & `angreal-2.0.9/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/py_tests/integrations/test_docker.py` & `angreal-2.0.9/py_tests/integrations/test_docker.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/py_tests/integrations/test_git.py` & `angreal-2.0.9/py_tests/integrations/test_git.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/py_tests/integrations/test_venv.py` & `angreal-2.0.9/py_tests/integrations/test_venv.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/py_tests/test_angreal.py` & `angreal-2.0.9/py_tests/test_angreal.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/pyproject.toml` & `angreal-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/python/angreal/__init__.py` & `angreal-2.0.9/python/angreal/__init__.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/python/angreal/integrations/git.py` & `angreal-2.0.9/python/angreal/integrations/git.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/python/angreal/integrations/venv.py` & `angreal-2.0.9/python/angreal/integrations/venv.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/builder.rs` & `angreal-2.0.9/src/builder.rs`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 
                 let mut task_parent = groups[task_parent_pos].clone();
                 task_parent = task_parent.subcommand(task);
                 groups.insert(task_parent_pos, task_parent);
 
                 for (pos, e) in c_groups.iter().enumerate().rev() {
                     if pos == 0 {
+                        // register the top level task when we're done building the chain.
                         top_level_groups.push(e.name.clone());
                         break;
                     }
 
                     let this_subcommand_pos = groups
                         .iter()
                         .position(|x| x.get_name() == e.name.as_str())
@@ -128,16 +129,17 @@
                     groups.insert(parent_subcommand_pos, parent_subcommand);
                 }
 
                 // loop groups backwards, register up the chain with a copy
             }
         }
 
-        // Register all "top level commands"
-
+        // sort, de duplicate, and register top level commands
+        top_level_groups.sort();
+        top_level_groups.dedup();
         for top in top_level_groups {
             let top_level = groups
                 .iter()
                 .find(|&x| x.get_name() == top.as_str())
                 .unwrap();
             app = app.subcommand(top_level.clone());
         }
```

### Comparing `angreal-2.0.8/src/git/mod.rs` & `angreal-2.0.9/src/git/mod.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/init.rs` & `angreal-2.0.9/src/init.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/lib.rs` & `angreal-2.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/logger.rs` & `angreal-2.0.9/src/logger.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/macros.rs` & `angreal-2.0.9/src/macros.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/py_logger.rs` & `angreal-2.0.9/src/py_logger.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/task.rs` & `angreal-2.0.9/src/task.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/src/utils.rs` & `angreal-2.0.9/src/utils.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/tests/common/mod.rs` & `angreal-2.0.9/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.8/Cargo.lock` & `angreal-2.0.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "angreal"
-version = "2.0.8"
+version = "2.0.9"
 dependencies = [
  "clap",
  "docker-pyo3",
  "git-url-parse",
  "git2",
  "git2_credentials",
  "glob",
```

### Comparing `angreal-2.0.8/PKG-INFO` & `angreal-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angreal
-Version: 2.0.8
+Version: 2.0.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
```

