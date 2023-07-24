# Comparing `tmp/render-engine-theme-kjaymiller-2023.7.1a3.tar.gz` & `tmp/render-engine-theme-kjaymiller-2023.7.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render-engine-theme-kjaymiller-2023.7.1a3.tar", last modified: Mon Jul 24 02:52:11 2023, max compression
+gzip compressed data, was "render-engine-theme-kjaymiller-2023.7.1a4.tar", last modified: Mon Jul 24 05:19:24 2023, max compression
```

## Comparing `render-engine-theme-kjaymiller-2023.7.1a3.tar` & `render-engine-theme-kjaymiller-2023.7.1a4.tar`

### file list

```diff
@@ -1,82 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.092208 render-engine-theme-kjaymiller-2023.7.1a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.072208 render-engine-theme-kjaymiller-2023.7.1a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.076208 render-engine-theme-kjaymiller-2023.7.1a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.076208 render-engine-theme-kjaymiller-2023.7.1a3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 02:52:11.092208 render-engine-theme-kjaymiller-2023.7.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:52:11.092208 render-engine-theme-kjaymiller-2023.7.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.072208 render-engine-theme-kjaymiller-2023.7.1a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.076208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.076208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/__pycache__/kjaymiller.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/kjaymiller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.072208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.076208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/css/microblog_archive.css
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/css/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.076208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/files/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/files/cloudanimation.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      261 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/files/search.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.084208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   987560 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Italic Nerd Font Complete.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   971960 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Nerd Font Complete.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   973908 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki Italic Nerd Font Complete.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   967448 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki-Regular Nerd Font Complete.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.084208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)   579310 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/images/social_card_base.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.092208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/YouTube_embed.html
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_archive.html
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_guest_appearances.html
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_podcasts.html
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_projects.html
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_retired_podcasts.html
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/about.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/analytics.html
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/blog.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/blog_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/categories.html
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/conference-talks.html
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/contact.html
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/extended-page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/featured_post.html
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/flex_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/full-jumbotron.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/github_disclaimer.html
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/lg-screen-jumbotron.html
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/menu_dropdown.js
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/microblog_archive.html
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/newsletter.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/noanalytics.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/pod_archive.html
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/podcast_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/podcasts.html
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/projects.html
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/short_bio.html
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/social-cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/tag_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/transistor.html
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/twitch_frame.html
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 02:51:52.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/what_im.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:11.076208 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 02:52:11.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-24 02:52:11.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:52:11.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 02:52:11.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 02:52:11.000000 render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.755438 render-engine-theme-kjaymiller-2023.7.1a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 05:19:24.755438 render-engine-theme-kjaymiller-2023.7.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 05:19:24.755438 render-engine-theme-kjaymiller-2023.7.1a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/kjaymiller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/css/microblog_archive.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/css/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/files/cloudanimation.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      261 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/files/search.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.747438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   987560 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Italic Nerd Font Complete.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   971960 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Nerd Font Complete.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   973908 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki Italic Nerd Font Complete.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   967448 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki-Regular Nerd Font Complete.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.747438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   579310 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/images/social_card_base.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.755438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/YouTube_embed.html
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_archive.html
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_guest_appearances.html
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_podcasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_projects.html
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_retired_podcasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/about.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/analytics.html
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/blog.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/blog_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/categories.html
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/conference-talks.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/contact.html
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/extended-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/featured_post.html
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/flex_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/full-jumbotron.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/github_disclaimer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/lg-screen-jumbotron.html
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/menu_dropdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/microblog_archive.html
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/newsletter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/noanalytics.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/pod_archive.html
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/podcast_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/podcasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/projects.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/short_bio.html
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/social-cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/tag_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/transistor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/twitch_frame.html
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 05:19:09.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/what_im.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:19:24.743438 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 05:19:24.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-24 05:19:24.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:19:24.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 05:19:24.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 05:19:24.000000 render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller.egg-info/top_level.txt
```

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/.github/workflows/publish.yml` & `render-engine-theme-kjaymiller-2023.7.1a4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/.gitignore` & `render-engine-theme-kjaymiller-2023.7.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/pyproject.toml` & `render-engine-theme-kjaymiller-2023.7.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/requirements.txt` & `render-engine-theme-kjaymiller-2023.7.1a4/requirements.txt`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/css/pygments.css` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/files/cloudanimation.svg` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/files/cloudanimation.svg`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Italic Nerd Font Complete.ttf` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Italic Nerd Font Complete.ttf`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Nerd Font Complete.ttf` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Nerd Font Complete.ttf`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki Italic Nerd Font Complete.ttf` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki Italic Nerd Font Complete.ttf`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/fonts/mononoki-Regular Nerd Font Complete.ttf` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/fonts/mononoki-Regular Nerd Font Complete.ttf`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/static/images/social_card_base.jpg` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/static/images/social_card_base.jpg`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_archive.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_archive.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_guest_appearances.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_guest_appearances.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/_podcasts.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/_podcasts.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/base.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/base.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/blog.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/blog.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/conference-talks.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/conference-talks.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/contact.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/contact.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/extended-page.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/extended-page.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/featured_post.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/featured_post.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/footer.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/footer.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/full-jumbotron.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/full-jumbotron.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/header.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/header.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/index.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/index.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/lg-screen-jumbotron.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/lg-screen-jumbotron.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/microblog_archive.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/microblog_archive.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/newsletter.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/newsletter.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/pagination.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/pod_archive.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/pod_archive.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/projects.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/projects.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/search.js` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/search.js`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/short_bio.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/short_bio.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/twitch_frame.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/twitch_frame.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller/templates/what_im.html` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller/templates/what_im.html`

 * *Files identical despite different names*

### Comparing `render-engine-theme-kjaymiller-2023.7.1a3/src/render_engine_theme_kjaymiller.egg-info/SOURCES.txt` & `render-engine-theme-kjaymiller-2023.7.1a4/src/render_engine_theme_kjaymiller.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 src/render_engine_theme_kjaymiller/__init__.py
 src/render_engine_theme_kjaymiller/kjaymiller.py
 src/render_engine_theme_kjaymiller.egg-info/PKG-INFO
 src/render_engine_theme_kjaymiller.egg-info/SOURCES.txt
 src/render_engine_theme_kjaymiller.egg-info/dependency_links.txt
 src/render_engine_theme_kjaymiller.egg-info/requires.txt
 src/render_engine_theme_kjaymiller.egg-info/top_level.txt
-src/render_engine_theme_kjaymiller/__pycache__/__init__.cpython-311.pyc
-src/render_engine_theme_kjaymiller/__pycache__/kjaymiller.cpython-311.pyc
 src/render_engine_theme_kjaymiller/static/css/microblog_archive.css
 src/render_engine_theme_kjaymiller/static/css/pygments.css
 src/render_engine_theme_kjaymiller/static/css/tailwind.css
 src/render_engine_theme_kjaymiller/static/files/cloudanimation.svg
 src/render_engine_theme_kjaymiller/static/files/search.svg
 src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Italic Nerd Font Complete.ttf
 src/render_engine_theme_kjaymiller/static/fonts/mononoki Bold Nerd Font Complete.ttf
```

