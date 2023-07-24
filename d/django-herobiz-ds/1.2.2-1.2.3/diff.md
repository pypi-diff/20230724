# Comparing `tmp/django-herobiz_ds-1.2.2.tar.gz` & `tmp/django-herobiz_ds-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-herobiz_ds-1.2.2.tar", last modified: Tue May  9 01:21:14 2023, max compression
+gzip compressed data, was "django-herobiz_ds-1.2.3.tar", last modified: Mon Jul 24 06:44:39 2023, max compression
```

## Comparing `django-herobiz_ds-1.2.2.tar` & `django-herobiz_ds-1.2.3.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.923284 django-herobiz_ds-1.2.2/
--rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      270 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3123 2023-05-09 01:21:14.923284 django-herobiz_ds-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.802342 django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/
--rw-rw-rw-   0        0        0     3123 2023-05-09 01:21:13.000000 django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11723 2023-05-09 01:21:13.000000 django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 01:21:13.000000 django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-05-09 01:21:13.000000 django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-09 01:21:13.000000 django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.845713 django-herobiz_ds-1.2.2/herobiz/
--rw-rw-rw-   0        0        0        0 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/__init__.py
--rw-rw-rw-   0        0        0      515 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/admin.py
--rw-rw-rw-   0        0        0      152 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/apps.py
--rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/forms.py
--rw-rw-rw-   0        0        0     1234 2023-02-13 00:17:54.000000 django-herobiz_ds-1.2.2/herobiz/models.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.749627 django-herobiz_ds-1.2.2/herobiz/static/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.754659 django-herobiz_ds-1.2.2/herobiz/static/herobiz/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.885626 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/
--rw-rw-rw-   0        0        0    64471 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/main.css
--rw-rw-rw-   0        0        0     7622 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-blue.css
--rw-rw-rw-   0        0        0     7619 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-green.css
--rw-rw-rw-   0        0        0     7622 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-orange.css
--rw-rw-rw-   0        0        0     7624 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-pink.css
--rw-rw-rw-   0        0        0     7624 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-purple.css
--rw-rw-rw-   0        0        0     7616 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-red.css
--rw-rw-rw-   0        0        0     7615 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables.css
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.003622 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/
--rw-rw-rw-   0        0        0      766 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/about-bg.png
--rw-rw-rw-   0        0        0    71291 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/about.jpg
--rw-rw-rw-   0        0        0     1738 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/apple-touch-icon.png
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.102084 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/
--rw-rw-rw-   0        0        0    70413 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-1.jpg
--rw-rw-rw-   0        0        0   124803 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-2.jpg
--rw-rw-rw-   0        0        0    90577 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-3.jpg
--rw-rw-rw-   0        0        0    90549 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-4.jpg
--rw-rw-rw-   0        0        0   121809 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-5.jpg
--rw-rw-rw-   0        0        0    72443 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-6.jpg
--rw-rw-rw-   0        0        0    64790 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-author.jpg
--rw-rw-rw-   0        0        0    85335 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-inside-post.jpg
--rw-rw-rw-   0        0        0    83411 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-1.jpg
--rw-rw-rw-   0        0        0    78239 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-2.jpg
--rw-rw-rw-   0        0        0    71055 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-3.jpg
--rw-rw-rw-   0        0        0   115012 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-4.jpg
--rw-rw-rw-   0        0        0    93369 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-5.jpg
--rw-rw-rw-   0        0        0    17444 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-1.jpg
--rw-rw-rw-   0        0        0    15407 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-2.jpg
--rw-rw-rw-   0        0        0    17041 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-3.jpg
--rw-rw-rw-   0        0        0    17774 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-4.jpg
--rw-rw-rw-   0        0        0    10855 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-5.jpg
--rw-rw-rw-   0        0        0    14253 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-6.jpg
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.151952 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/
--rw-rw-rw-   0        0        0    10383 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/aaid.png
--rw-rw-rw-   0        0        0    78067 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/amc.png
--rw-rw-rw-   0        0        0    68489 2023-02-08 02:57:18.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/ao.png
--rw-rw-rw-   0        0        0    58360 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/cmc.png
--rw-rw-rw-   0        0        0     8251 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/eao.png
--rw-rw-rw-   0        0        0    10453 2023-02-08 02:53:49.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kamprs.png
--rw-rw-rw-   0        0        0    18244 2023-02-08 02:43:47.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kaomi.png
--rw-rw-rw-   0        0        0    72990 2023-02-08 02:47:31.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kaoms.png
--rw-rw-rw-   0        0        0    88587 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/khmc.png
--rw-rw-rw-   0        0        0    25920 2023-02-08 02:58:04.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kugh.png
--rw-rw-rw-   0        0        0    27504 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/pnuh.png
--rw-rw-rw-   0        0        0   302776 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/sev.png
--rw-rw-rw-   0        0        0     5709 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/smc.png
--rw-rw-rw-   0        0        0   150139 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/snuh.png
--rw-rw-rw-   0        0        0        0 2023-02-08 02:32:05.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/가로세로3대1정도png로.txt
--rw-rw-rw-   0        0        0    63230 2023-02-05 23:21:12.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/cta.jpg
--rw-rw-rw-   0        0        0    95604 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/faq.jpg
--rw-rw-rw-   0        0        0      491 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/favicon.png
--rw-rw-rw-   0        0        0     9582 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-1.svg
--rw-rw-rw-   0        0        0    20971 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-2.svg
--rw-rw-rw-   0        0        0    16706 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-3.svg
--rw-rw-rw-   0        0        0    18350 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-4.svg
--rw-rw-rw-   0        0        0    21346 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-5.svg
--rw-rw-rw-   0        0        0    25920 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-6.svg
--rw-rw-rw-   0        0        0    13287 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-bg.png
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.173241 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-carousel/
--rw-rw-rw-   0        0        0    16021 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-carousel/hero-carousel-1.svg
--rw-rw-rw-   0        0        0    44883 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-carousel/hero-carousel-2.svg
--rw-rw-rw-   0        0        0    17290 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-carousel/hero-carousel-3.svg
--rw-rw-rw-   0        0        0   208099 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-fullscreen-bg.jpg
--rw-rw-rw-   0        0        0    13081 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/onfocus-content-bg.jpg
--rw-rw-rw-   0        0        0    87953 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/onfocus-video-bg.jpg
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.240570 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/
--rw-rw-rw-   0        0        0    67064 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/app-1.jpg
--rw-rw-rw-   0        0        0    73871 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/app-2.jpg
--rw-rw-rw-   0        0        0    42308 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/app-3.jpg
--rw-rw-rw-   0        0        0    80146 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/books-1.jpg
--rw-rw-rw-   0        0        0    60824 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/books-2.jpg
--rw-rw-rw-   0        0        0    91462 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/books-3.jpg
--rw-rw-rw-   0        0        0    25514 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/branding-1.jpg
--rw-rw-rw-   0        0        0    52305 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/branding-2.jpg
--rw-rw-rw-   0        0        0    77892 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/branding-3.jpg
--rw-rw-rw-   0        0        0    62035 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/product-1.jpg
--rw-rw-rw-   0        0        0    89298 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/product-2.jpg
--rw-rw-rw-   0        0        0    20090 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/product-3.jpg
--rw-rw-rw-   0        0        0    61855 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/pricing-bg.jpg
--rw-rw-rw-   0        0        0    79550 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-1.jpg
--rw-rw-rw-   0        0        0    50649 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-2.jpg
--rw-rw-rw-   0        0        0    55307 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-3.jpg
--rw-rw-rw-   0        0        0    65283 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-4.jpg
--rw-rw-rw-   0        0        0    81737 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-5.jpg
--rw-rw-rw-   0        0        0   111917 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-6.jpg
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.258783 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/team/
--rw-rw-rw-   0        0        0    40201 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/team/team-1.jpg
--rw-rw-rw-   0        0        0    49059 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/team/team-2.jpg
--rw-rw-rw-   0        0        0    36680 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/team/team-3.jpg
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.291010 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/
--rw-rw-rw-   0        0        0    39727 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-1.jpg
--rw-rw-rw-   0        0        0    57584 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-2.jpg
--rw-rw-rw-   0        0        0    17247 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-3.jpg
--rw-rw-rw-   0        0        0    20220 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-4.jpg
--rw-rw-rw-   0        0        0    22595 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-5.jpg
--rw-rw-rw-   0        0        0   358976 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials-bg.bak.jpg
--rw-rw-rw-   0        0        0   447095 2023-02-10 00:26:03.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials-bg.jpg
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.292750 django-herobiz_ds-1.2.2/herobiz/static/herobiz/js/
--rw-rw-rw-   0        0        0     8445 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/js/main.js
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.364002 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/
--rw-rw-rw-   0        0        0      281 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_blog.scss
--rw-rw-rw-   0        0        0     3649 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_footer.scss
--rw-rw-rw-   0        0        0     3770 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_general.scss
--rw-rw-rw-   0        0        0     1118 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_header.scss
--rw-rw-rw-   0        0        0      643 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_index.scss
--rw-rw-rw-   0        0        0     5712 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_nav.scss
--rw-rw-rw-   0        0        0     1320 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_portfolio-details.scss
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.371867 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/
--rw-rw-rw-   0        0        0     2172 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_comments.scss
--rw-rw-rw-   0        0        0     3738 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_details.scss
--rw-rw-rw-   0        0        0      758 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_pagination.scss
--rw-rw-rw-   0        0        0     1813 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_posts-list.scss
--rw-rw-rw-   0        0        0     3480 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_sidebar.scss
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.395086 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/
--rw-rw-rw-   0        0        0     1676 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_about.scss
--rw-rw-rw-   0        0        0      377 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_clients.scss
--rw-rw-rw-   0        0        0     3086 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_contact.scss
--rw-rw-rw-   0        0        0     1882 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_cta.scss
--rw-rw-rw-   0        0        0     1674 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_faq.scss
--rw-rw-rw-   0        0        0      981 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_featured-services.scss
--rw-rw-rw-   0        0        0     1762 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_features.scss
--rw-rw-rw-   0        0        0     2205 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero-animated.scss
--rw-rw-rw-   0        0        0     1990 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero-fullscreen.scss
--rw-rw-rw-   0        0        0     1764 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero-static.scss
--rw-rw-rw-   0        0        0     3426 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero.scss
--rw-rw-rw-   0        0        0     3798 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_onfocus.scss
--rw-rw-rw-   0        0        0     2264 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_portfolio.scss
--rw-rw-rw-   0        0        0     2551 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_pricing.scss
--rw-rw-rw-   0        0        0     1512 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_recent-blog-posts.scss
--rw-rw-rw-   0        0        0     1718 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_services.scss
--rw-rw-rw-   0        0        0     1922 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_team.scss
--rw-rw-rw-   0        0        0     2203 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_testimonials.scss
--rw-rw-rw-   0        0        0      253 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/main.scss
--rw-rw-rw-   0        0        0     7960 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-blue.css
--rw-rw-rw-   0        0        0     7957 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-green.css
--rw-rw-rw-   0        0        0     7960 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-orange.css
--rw-rw-rw-   0        0        0     7962 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-pink.css
--rw-rw-rw-   0        0        0     7960 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-purple.css
--rw-rw-rw-   0        0        0     7954 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-red.css
--rw-rw-rw-   0        0        0     7997 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables.css
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.759122 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.397971 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/aos/
--rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/aos/aos.css
--rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/aos/aos.js
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.756797 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.584669 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210357 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131395 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210361 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131472 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110875 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40331 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110888 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48693 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   196435 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   115588 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   196378 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   115423 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237994 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   608416 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194901 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   522733 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237526 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   608236 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   195007 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   767573 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.724529 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   208123 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   452089 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    80496 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   333304 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   136335 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   308526 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    74054 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   221402 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   145677 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0   309667 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60480 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   217134 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.419439 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/
--rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.css
--rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.scss
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.428942 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/
--rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/index.html
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.758114 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.748538 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/
--rw-rw-rw-   0        0        0    17372 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/glightbox.css
--rw-rw-rw-   0        0        0    13749 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/glightbox.min.css
--rw-rw-rw-   0        0        0    52561 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/plyr.css
--rw-rw-rw-   0        0        0    45081 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/plyr.min.css
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.773444 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/js/
--rw-rw-rw-   0        0        0   109391 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/js/glightbox.js
--rw-rw-rw-   0        0        0    55880 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/js/glightbox.min.js
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.793879 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/isotope-layout/
--rw-rw-rw-   0        0        0    91398 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.js
--rw-rw-rw-   0        0        0    35445 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.min.js
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.809578 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/php-email-form/
--rw-rw-rw-   0        0        0   232688 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/php-email-form/php-email-form.php
--rw-rw-rw-   0        0        0     2590 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/php-email-form/validate.js
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.814669 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/swiper/
--rw-rw-rw-   0        0        0    16468 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.css
--rw-rw-rw-   0        0        0   143629 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js
--rw-rw-rw-   0        0        0   540438 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js.map
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:13.760303 django-herobiz_ds-1.2.2/herobiz/templates/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.908940 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/
--rw-rw-rw-   0        0        0     2851 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/__blog.html
--rw-rw-rw-   0        0        0     3811 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/__pricing.html
--rw-rw-rw-   0        0        0     2190 2023-02-04 02:48:15.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_about.html
--rw-rw-rw-   0        0        0      451 2023-02-08 03:01:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_clients.html
--rw-rw-rw-   0        0        0     3160 2023-02-06 05:24:42.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_contact.html
--rw-rw-rw-   0        0        0     1236 2023-02-10 01:19:49.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_cta.html
--rw-rw-rw-   0        0        0     1794 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_faq.html
--rw-rw-rw-   0        0        0     1867 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_features.html
--rw-rw-rw-   0        0        0     1009 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero1.html
--rw-rw-rw-   0        0        0     1741 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero2.html
--rw-rw-rw-   0        0        0      896 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero3.html
--rw-rw-rw-   0        0        0      896 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero4.html
--rw-rw-rw-   0        0        0     1852 2023-02-13 23:42:42.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_onfocus.html
--rw-rw-rw-   0        0        0     5579 2023-02-13 00:00:32.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_portfolio-details.html
--rw-rw-rw-   0        0        0     1518 2023-02-12 23:29:37.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_portfolio.html
--rw-rw-rw-   0        0        0     1043 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_services.html
--rw-rw-rw-   0        0        0     1531 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_team.html
--rw-rw-rw-   0        0        0     1273 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_testimonials.html
--rw-rw-rw-   0        0        0     1088 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_why_us.html
--rw-rw-rw-   0        0        0     1183 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/analytics.html
--rw-rw-rw-   0        0        0     2023 2023-05-09 01:20:12.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/footer.html
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.910171 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/forms/
--rw-rw-rw-   0        0        0     1341 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/forms/contact.php
--rw-rw-rw-   0        0        0     1261 2023-02-04 02:27:43.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/header.html
--rw-rw-rw-   0        0        0     4674 2023-02-05 23:22:03.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/index.html
--rw-rw-rw-   0        0        0     1488 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.2/herobiz/templates/herobiz/seo.html
-drwxrwxrwx   0        0        0        0 2023-05-09 01:21:14.921280 django-herobiz_ds-1.2.2/herobiz/templatetags/
--rw-rw-rw-   0        0        0        0 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/templatetags/__init__.py
--rw-rw-rw-   0        0        0     5227 2023-02-12 23:29:37.000000 django-herobiz_ds-1.2.2/herobiz/templatetags/herobiz_tags.py
--rw-rw-rw-   0        0        0      276 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.2/herobiz/urls.py
--rw-rw-rw-   0        0        0     3867 2023-02-04 01:14:57.000000 django-herobiz_ds-1.2.2/herobiz/views.py
--rw-rw-rw-   0        0        0      112 2022-11-26 09:41:37.000000 django-herobiz_ds-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      750 2023-05-09 01:21:14.932021 django-herobiz_ds-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-11-26 09:41:37.000000 django-herobiz_ds-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.588538 django-herobiz_ds-1.2.3/
+-rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      270 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3123 2023-07-24 06:44:39.588538 django-herobiz_ds-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.633653 django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/
+-rw-rw-rw-   0        0        0     3123 2023-07-24 06:44:38.000000 django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11723 2023-07-24 06:44:38.000000 django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:44:38.000000 django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-07-24 06:44:38.000000 django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 06:44:38.000000 django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.648451 django-herobiz_ds-1.2.3/herobiz/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/__init__.py
+-rw-rw-rw-   0        0        0      515 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/admin.py
+-rw-rw-rw-   0        0        0      152 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/apps.py
+-rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/forms.py
+-rw-rw-rw-   0        0        0     1234 2023-02-13 00:17:54.000000 django-herobiz_ds-1.2.3/herobiz/models.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.567922 django-herobiz_ds-1.2.3/herobiz/static/
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.575308 django-herobiz_ds-1.2.3/herobiz/static/herobiz/
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.664544 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/
+-rw-rw-rw-   0        0        0    64471 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/main.css
+-rw-rw-rw-   0        0        0     7622 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-blue.css
+-rw-rw-rw-   0        0        0     7619 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-green.css
+-rw-rw-rw-   0        0        0     7622 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-orange.css
+-rw-rw-rw-   0        0        0     7624 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-pink.css
+-rw-rw-rw-   0        0        0     7624 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-purple.css
+-rw-rw-rw-   0        0        0     7616 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-red.css
+-rw-rw-rw-   0        0        0     7615 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables.css
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.828745 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/
+-rw-rw-rw-   0        0        0      766 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/about-bg.png
+-rw-rw-rw-   0        0        0    71291 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/about.jpg
+-rw-rw-rw-   0        0        0     1738 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/apple-touch-icon.png
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.989941 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/
+-rw-rw-rw-   0        0        0    70413 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-1.jpg
+-rw-rw-rw-   0        0        0   124803 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-2.jpg
+-rw-rw-rw-   0        0        0    90577 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-3.jpg
+-rw-rw-rw-   0        0        0    90549 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-4.jpg
+-rw-rw-rw-   0        0        0   121809 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-5.jpg
+-rw-rw-rw-   0        0        0    72443 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-6.jpg
+-rw-rw-rw-   0        0        0    64790 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-author.jpg
+-rw-rw-rw-   0        0        0    85335 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-inside-post.jpg
+-rw-rw-rw-   0        0        0    83411 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-1.jpg
+-rw-rw-rw-   0        0        0    78239 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-2.jpg
+-rw-rw-rw-   0        0        0    71055 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-3.jpg
+-rw-rw-rw-   0        0        0   115012 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-4.jpg
+-rw-rw-rw-   0        0        0    93369 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-5.jpg
+-rw-rw-rw-   0        0        0    17444 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-1.jpg
+-rw-rw-rw-   0        0        0    15407 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-2.jpg
+-rw-rw-rw-   0        0        0    17041 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-3.jpg
+-rw-rw-rw-   0        0        0    17774 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-4.jpg
+-rw-rw-rw-   0        0        0    10855 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-5.jpg
+-rw-rw-rw-   0        0        0    14253 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-6.jpg
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.093765 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/
+-rw-rw-rw-   0        0        0    10383 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/aaid.png
+-rw-rw-rw-   0        0        0    78067 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/amc.png
+-rw-rw-rw-   0        0        0    68489 2023-02-08 02:57:18.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/ao.png
+-rw-rw-rw-   0        0        0    58360 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/cmc.png
+-rw-rw-rw-   0        0        0     8251 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/eao.png
+-rw-rw-rw-   0        0        0    10453 2023-02-08 02:53:49.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kamprs.png
+-rw-rw-rw-   0        0        0    18244 2023-02-08 02:43:47.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kaomi.png
+-rw-rw-rw-   0        0        0    72990 2023-02-08 02:47:31.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kaoms.png
+-rw-rw-rw-   0        0        0    88587 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/khmc.png
+-rw-rw-rw-   0        0        0    25920 2023-02-08 02:58:04.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kugh.png
+-rw-rw-rw-   0        0        0    27504 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/pnuh.png
+-rw-rw-rw-   0        0        0   302776 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/sev.png
+-rw-rw-rw-   0        0        0     5709 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/smc.png
+-rw-rw-rw-   0        0        0   150139 2022-11-26 09:41:34.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/snuh.png
+-rw-rw-rw-   0        0        0        0 2023-02-08 02:32:05.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/가로세로3대1정도png로.txt
+-rw-rw-rw-   0        0        0    63230 2023-02-05 23:21:12.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/cta.jpg
+-rw-rw-rw-   0        0        0    95604 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/faq.jpg
+-rw-rw-rw-   0        0        0      491 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/favicon.png
+-rw-rw-rw-   0        0        0     9582 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-1.svg
+-rw-rw-rw-   0        0        0    20971 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-2.svg
+-rw-rw-rw-   0        0        0    16706 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-3.svg
+-rw-rw-rw-   0        0        0    18350 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-4.svg
+-rw-rw-rw-   0        0        0    21346 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-5.svg
+-rw-rw-rw-   0        0        0    25920 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-6.svg
+-rw-rw-rw-   0        0        0    13287 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-bg.png
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.099585 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-carousel/
+-rw-rw-rw-   0        0        0    16021 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-carousel/hero-carousel-1.svg
+-rw-rw-rw-   0        0        0    44883 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-carousel/hero-carousel-2.svg
+-rw-rw-rw-   0        0        0    17290 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-carousel/hero-carousel-3.svg
+-rw-rw-rw-   0        0        0   208099 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-fullscreen-bg.jpg
+-rw-rw-rw-   0        0        0    13081 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/onfocus-content-bg.jpg
+-rw-rw-rw-   0        0        0    87953 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/onfocus-video-bg.jpg
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.209441 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/
+-rw-rw-rw-   0        0        0    67064 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/app-1.jpg
+-rw-rw-rw-   0        0        0    73871 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/app-2.jpg
+-rw-rw-rw-   0        0        0    42308 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/app-3.jpg
+-rw-rw-rw-   0        0        0    80146 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/books-1.jpg
+-rw-rw-rw-   0        0        0    60824 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/books-2.jpg
+-rw-rw-rw-   0        0        0    91462 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/books-3.jpg
+-rw-rw-rw-   0        0        0    25514 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/branding-1.jpg
+-rw-rw-rw-   0        0        0    52305 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/branding-2.jpg
+-rw-rw-rw-   0        0        0    77892 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/branding-3.jpg
+-rw-rw-rw-   0        0        0    62035 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/product-1.jpg
+-rw-rw-rw-   0        0        0    89298 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/product-2.jpg
+-rw-rw-rw-   0        0        0    20090 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/product-3.jpg
+-rw-rw-rw-   0        0        0    61855 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/pricing-bg.jpg
+-rw-rw-rw-   0        0        0    79550 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-1.jpg
+-rw-rw-rw-   0        0        0    50649 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-2.jpg
+-rw-rw-rw-   0        0        0    55307 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-3.jpg
+-rw-rw-rw-   0        0        0    65283 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-4.jpg
+-rw-rw-rw-   0        0        0    81737 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-5.jpg
+-rw-rw-rw-   0        0        0   111917 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-6.jpg
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.238909 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/team/
+-rw-rw-rw-   0        0        0    40201 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/team/team-1.jpg
+-rw-rw-rw-   0        0        0    49059 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/team/team-2.jpg
+-rw-rw-rw-   0        0        0    36680 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/team/team-3.jpg
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.279144 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/
+-rw-rw-rw-   0        0        0    39727 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-1.jpg
+-rw-rw-rw-   0        0        0    57584 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-2.jpg
+-rw-rw-rw-   0        0        0    17247 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-3.jpg
+-rw-rw-rw-   0        0        0    20220 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-4.jpg
+-rw-rw-rw-   0        0        0    22595 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-5.jpg
+-rw-rw-rw-   0        0        0   358976 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials-bg.bak.jpg
+-rw-rw-rw-   0        0        0   447095 2023-02-10 00:26:03.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials-bg.jpg
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.280370 django-herobiz_ds-1.2.3/herobiz/static/herobiz/js/
+-rw-rw-rw-   0        0        0     8445 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/js/main.js
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.308908 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/
+-rw-rw-rw-   0        0        0      281 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_blog.scss
+-rw-rw-rw-   0        0        0     3649 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_footer.scss
+-rw-rw-rw-   0        0        0     3770 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_general.scss
+-rw-rw-rw-   0        0        0     1118 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_header.scss
+-rw-rw-rw-   0        0        0      643 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_index.scss
+-rw-rw-rw-   0        0        0     5712 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_nav.scss
+-rw-rw-rw-   0        0        0     1320 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_portfolio-details.scss
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.318681 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/
+-rw-rw-rw-   0        0        0     2172 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_comments.scss
+-rw-rw-rw-   0        0        0     3738 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_details.scss
+-rw-rw-rw-   0        0        0      758 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_pagination.scss
+-rw-rw-rw-   0        0        0     1813 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_posts-list.scss
+-rw-rw-rw-   0        0        0     3480 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_sidebar.scss
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.353273 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/
+-rw-rw-rw-   0        0        0     1676 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_about.scss
+-rw-rw-rw-   0        0        0      377 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_clients.scss
+-rw-rw-rw-   0        0        0     3086 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_contact.scss
+-rw-rw-rw-   0        0        0     1882 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_cta.scss
+-rw-rw-rw-   0        0        0     1674 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_faq.scss
+-rw-rw-rw-   0        0        0      981 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_featured-services.scss
+-rw-rw-rw-   0        0        0     1762 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_features.scss
+-rw-rw-rw-   0        0        0     2205 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero-animated.scss
+-rw-rw-rw-   0        0        0     1990 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero-fullscreen.scss
+-rw-rw-rw-   0        0        0     1764 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero-static.scss
+-rw-rw-rw-   0        0        0     3426 2022-11-26 09:41:35.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero.scss
+-rw-rw-rw-   0        0        0     3798 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_onfocus.scss
+-rw-rw-rw-   0        0        0     2264 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_portfolio.scss
+-rw-rw-rw-   0        0        0     2551 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_pricing.scss
+-rw-rw-rw-   0        0        0     1512 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_recent-blog-posts.scss
+-rw-rw-rw-   0        0        0     1718 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_services.scss
+-rw-rw-rw-   0        0        0     1922 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_team.scss
+-rw-rw-rw-   0        0        0     2203 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_testimonials.scss
+-rw-rw-rw-   0        0        0      253 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/main.scss
+-rw-rw-rw-   0        0        0     7960 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-blue.css
+-rw-rw-rw-   0        0        0     7957 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-green.css
+-rw-rw-rw-   0        0        0     7960 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-orange.css
+-rw-rw-rw-   0        0        0     7962 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-pink.css
+-rw-rw-rw-   0        0        0     7960 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-purple.css
+-rw-rw-rw-   0        0        0     7954 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-red.css
+-rw-rw-rw-   0        0        0     7997 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables.css
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.584226 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.357878 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/aos/
+-rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/aos/aos.css
+-rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/aos/aos.js
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.579302 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.454960 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210357 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131395 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210361 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131472 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110875 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40331 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110888 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48693 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   196435 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   115588 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   196378 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   115423 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237994 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   608416 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194901 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   522733 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237526 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   608236 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   195007 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   767573 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.494478 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   208123 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   452089 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    80496 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   333304 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   136335 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   308526 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    74054 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   221402 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   145677 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0   309667 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60480 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   217134 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.366377 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/
+-rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.scss
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.370953 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/
+-rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/index.html
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.581557 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.504345 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/
+-rw-rw-rw-   0        0        0    17372 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/glightbox.css
+-rw-rw-rw-   0        0        0    13749 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/glightbox.min.css
+-rw-rw-rw-   0        0        0    52561 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/plyr.css
+-rw-rw-rw-   0        0        0    45081 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/plyr.min.css
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.509858 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/js/
+-rw-rw-rw-   0        0        0   109391 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/js/glightbox.js
+-rw-rw-rw-   0        0        0    55880 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/js/glightbox.min.js
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.514422 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/isotope-layout/
+-rw-rw-rw-   0        0        0    91398 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.js
+-rw-rw-rw-   0        0        0    35445 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.min.js
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.519524 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/php-email-form/
+-rw-rw-rw-   0        0        0   232688 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/php-email-form/php-email-form.php
+-rw-rw-rw-   0        0        0     2590 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/php-email-form/validate.js
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.526002 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/swiper/
+-rw-rw-rw-   0        0        0    16468 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.css
+-rw-rw-rw-   0        0        0   143629 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js
+-rw-rw-rw-   0        0        0   540438 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js.map
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:38.585253 django-herobiz_ds-1.2.3/herobiz/templates/
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.579981 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/
+-rw-rw-rw-   0        0        0     2851 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/__blog.html
+-rw-rw-rw-   0        0        0     3811 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/__pricing.html
+-rw-rw-rw-   0        0        0     2190 2023-02-04 02:48:15.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_about.html
+-rw-rw-rw-   0        0        0      451 2023-02-08 03:01:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_clients.html
+-rw-rw-rw-   0        0        0     3160 2023-02-06 05:24:42.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_contact.html
+-rw-rw-rw-   0        0        0     1236 2023-02-10 01:19:49.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_cta.html
+-rw-rw-rw-   0        0        0     1794 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_faq.html
+-rw-rw-rw-   0        0        0     1867 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_features.html
+-rw-rw-rw-   0        0        0     1009 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero1.html
+-rw-rw-rw-   0        0        0     1741 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero2.html
+-rw-rw-rw-   0        0        0      896 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero3.html
+-rw-rw-rw-   0        0        0      896 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero4.html
+-rw-rw-rw-   0        0        0     1852 2023-02-13 23:42:42.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_onfocus.html
+-rw-rw-rw-   0        0        0     5579 2023-02-13 00:00:32.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_portfolio-details.html
+-rw-rw-rw-   0        0        0     1518 2023-02-12 23:29:37.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_portfolio.html
+-rw-rw-rw-   0        0        0     1043 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_services.html
+-rw-rw-rw-   0        0        0     1531 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_team.html
+-rw-rw-rw-   0        0        0     1273 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_testimonials.html
+-rw-rw-rw-   0        0        0     1088 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_why_us.html
+-rw-rw-rw-   0        0        0     1183 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/analytics.html
+-rw-rw-rw-   0        0        0     2023 2023-05-09 01:20:12.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/footer.html
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.582494 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/forms/
+-rw-rw-rw-   0        0        0     1341 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/forms/contact.php
+-rw-rw-rw-   0        0        0     1467 2023-07-24 06:41:01.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/header.html
+-rw-rw-rw-   0        0        0     4674 2023-02-05 23:22:03.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/index.html
+-rw-rw-rw-   0        0        0     1488 2023-02-04 01:39:30.000000 django-herobiz_ds-1.2.3/herobiz/templates/herobiz/seo.html
+drwxrwxrwx   0        0        0        0 2023-07-24 06:44:39.586313 django-herobiz_ds-1.2.3/herobiz/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     5227 2023-02-12 23:29:37.000000 django-herobiz_ds-1.2.3/herobiz/templatetags/herobiz_tags.py
+-rw-rw-rw-   0        0        0      276 2022-11-26 09:41:36.000000 django-herobiz_ds-1.2.3/herobiz/urls.py
+-rw-rw-rw-   0        0        0     3867 2023-02-04 01:14:57.000000 django-herobiz_ds-1.2.3/herobiz/views.py
+-rw-rw-rw-   0        0        0      112 2022-11-26 09:41:37.000000 django-herobiz_ds-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      750 2023-07-24 06:44:39.590683 django-herobiz_ds-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-11-26 09:41:37.000000 django-herobiz_ds-1.2.3/setup.py
```

### Comparing `django-herobiz_ds-1.2.2/LICENSE` & `django-herobiz_ds-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/PKG-INFO` & `django-herobiz_ds-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-herobiz_ds
-Version: 1.2.2
+Version: 1.2.3
 Summary: herobiz_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-herobiz_ds-1.2.2/README.md` & `django-herobiz_ds-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/PKG-INFO` & `django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-herobiz-ds
-Version: 1.2.2
+Version: 1.2.3
 Summary: herobiz_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-herobiz_ds-1.2.2/django_herobiz_ds.egg-info/SOURCES.txt` & `django-herobiz_ds-1.2.3/django_herobiz_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/admin.py` & `django-herobiz_ds-1.2.3/herobiz/admin.py`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/forms.py` & `django-herobiz_ds-1.2.3/herobiz/forms.py`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/models.py` & `django-herobiz_ds-1.2.3/herobiz/models.py`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/main.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/main.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-blue.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-green.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-green.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-orange.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-pink.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-purple.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables-red.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables-red.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/css/variables.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/css/variables.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/about-bg.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/about-bg.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/about.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/about.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/apple-touch-icon.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-4.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-4.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-5.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-5.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-6.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-6.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-author.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-author.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-inside-post.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-inside-post.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-4.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-4.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/blog-recent-5.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/blog-recent-5.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-4.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-4.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-5.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-5.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/blog/comments-6.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/blog/comments-6.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/aaid.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/aaid.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/amc.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/amc.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/ao.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/ao.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/cmc.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/cmc.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/eao.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/eao.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kamprs.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kamprs.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kaomi.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kaomi.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kaoms.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kaoms.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/khmc.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/khmc.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/kugh.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/kugh.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/pnuh.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/pnuh.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/sev.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/sev.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/smc.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/smc.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/clients/snuh.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/clients/snuh.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/cta.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/cta.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/faq.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/faq.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-1.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-1.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-2.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-2.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-3.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-3.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-4.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-4.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-5.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-5.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/features-6.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/features-6.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-bg.png` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-bg.png`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-carousel/hero-carousel-1.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-carousel/hero-carousel-1.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-carousel/hero-carousel-2.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-carousel/hero-carousel-2.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-carousel/hero-carousel-3.svg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-carousel/hero-carousel-3.svg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/hero-fullscreen-bg.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/hero-fullscreen-bg.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/onfocus-content-bg.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/onfocus-content-bg.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/onfocus-video-bg.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/onfocus-video-bg.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/app-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/app-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/app-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/app-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/app-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/app-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/books-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/books-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/books-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/books-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/books-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/books-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/branding-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/branding-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/branding-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/branding-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/branding-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/branding-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/product-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/product-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/product-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/product-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/portfolio/product-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/portfolio/product-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/pricing-bg.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/pricing-bg.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-4.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-4.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-5.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-5.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/services-6.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/services-6.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/team/team-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/team/team-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/team/team-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/team/team-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/team/team-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/team/team-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-1.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-1.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-2.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-2.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-3.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-3.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-4.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-4.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials/testimonials-5.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials/testimonials-5.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials-bg.bak.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials-bg.bak.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/img/testimonials-bg.jpg` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/img/testimonials-bg.jpg`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/js/main.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/js/main.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_footer.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_general.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_header.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_index.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_index.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_nav.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/_portfolio-details.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/_portfolio-details.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_comments.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_comments.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_details.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_details.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_pagination.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_posts-list.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_posts-list.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/blog/_sidebar.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/blog/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_about.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_about.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_contact.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_contact.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_cta.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_cta.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_faq.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_faq.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_featured-services.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_featured-services.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_features.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_features.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero-animated.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero-animated.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero-fullscreen.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero-fullscreen.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero-static.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero-static.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_hero.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_hero.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_onfocus.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_onfocus.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_portfolio.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_portfolio.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_pricing.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_pricing.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_recent-blog-posts.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_recent-blog-posts.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_services.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_services.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_team.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_team.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/index/_testimonials.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/index/_testimonials.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-blue.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-green.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-green.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-orange.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-pink.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-purple.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables-red.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables-red.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/scss/variables.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/scss/variables.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/aos/aos.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/aos/aos.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.json` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.scss` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/bootstrap-icons/index.html` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/bootstrap-icons/index.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/glightbox.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/glightbox.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/plyr.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/css/plyr.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/js/glightbox.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/glightbox/js/glightbox.min.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.min.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/php-email-form/php-email-form.php` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/php-email-form/validate.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.css` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js.map` & `django-herobiz_ds-1.2.3/herobiz/static/herobiz/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/__blog.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/__blog.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/__pricing.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/__pricing.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_about.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_about.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_contact.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_contact.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_cta.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_cta.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_faq.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_faq.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_features.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_features.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero1.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero1.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero2.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero2.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero3.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero3.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_hero4.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_hero4.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_onfocus.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_onfocus.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_portfolio-details.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_portfolio-details.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_portfolio.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_portfolio.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_services.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_services.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_team.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_team.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_testimonials.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/_why_us.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/_why_us.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/analytics.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/analytics.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/footer.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/footer.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/forms/contact.php` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/header.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/header.html`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,21 @@
     {% endif %}
     </a>
 
     <nav id="navbar" class="navbar">
       <ul>
         <li><a class="nav-link scrollto" href="#">Home</a></li>
         <!-- 메뉴 -->
-        {% for component, _, title, is_show in components %}
+        {% for component, etc, title, is_show in components %}
           {% if is_show %}
-          <li><a class="nav-link scrollto" href="{% url 'herobiz:home' %}#{{ component }}">{{ title }}</a></li>
+            {% if component == 'direct_link' %}
+              <li><a class="nav-link scrollto" href="{{ etc }}" target="_blank">{{ title }}</a></li>
+            {% else %}
+              <li><a class="nav-link scrollto" href="{% url 'herobiz:home' %}#{{ component }}">{{ title }}</a></li>
+            {% endif %}
           {% endif %}
         {% endfor %}
       </ul>
       <i class="bi bi-list mobile-nav-toggle d-none"></i>
     </nav><!-- .navbar -->
 
     {% for component, is_use, _, _ in components %}
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
 {% load static %}
 
 {%_if_use_logo_%}__{%_else_%}
 ******_{{_basic_info.company_name_}}._******
 {%_endif_%}
 
     * Home
-    *  {% for component, _, title, is_show in components %} {% if is_show %}
+    *  {% for component, etc, title, is_show in components %} {% if is_show %}
+      {% if component == 'direct_link' %}
     * {{_title_}}
-    * {% endif %} {% endfor %}
+    * {% else %}
+    * {{_title_}}
+    * {% endif %} {% endif %} {% endfor %}
   {% for component, is_use, _, _ in components %} {% if component ==
 top_menu_btn.component and is_use %} {{_top_menu_btn.title_}} {% endif %} {%
 endfor %}
```

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/index.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/index.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templates/herobiz/seo.html` & `django-herobiz_ds-1.2.3/herobiz/templates/herobiz/seo.html`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/templatetags/herobiz_tags.py` & `django-herobiz_ds-1.2.3/herobiz/templatetags/herobiz_tags.py`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/herobiz/views.py` & `django-herobiz_ds-1.2.3/herobiz/views.py`

 * *Files identical despite different names*

### Comparing `django-herobiz_ds-1.2.2/setup.cfg` & `django-herobiz_ds-1.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6865 726f 6269   = django-herobi
 00000020: 7a5f 6473 0d0a 7665 7273 696f 6e20 3d20  z_ds..version = 
-00000030: 312e 322e 320d 0a61 7574 686f 7220 3d20  1.2.2..author = 
+00000030: 312e 322e 330d 0a61 7574 686f 7220 3d20  1.2.3..author = 
 00000040: 6879 756e 676a 696e 206b 696d 0d0a 6175  hyungjin kim..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2068 6a33  thor_email = hj3
 00000060: 3431 3540 676d 6169 6c2e 636f 6d0d 0a64  415@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2068 6572  escription = her
 00000080: 6f62 697a 5f70 726f 2070 6f72 7469 6e67  obiz_pro porting
 00000090: 2066 6f72 2064 6a61 6e67 6f0d 0a6c 6f6e   for django..lon
 000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

