# Comparing `tmp/pyrsm-0.9.0.tar.gz` & `tmp/pyrsm-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.9.0.tar", last modified: Thu Jul 20 09:01:14 2023, max compression
+gzip compressed data, was "pyrsm-0.9.1.tar", last modified: Mon Jul 24 01:43:55 2023, max compression
```

## Comparing `pyrsm-0.9.0.tar` & `pyrsm-0.9.1.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.150578 pyrsm-0.9.0/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.9.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-20 09:01:14.150650 pyrsm-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.9.0/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.9.0/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.119885 pyrsm-0.9.0/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      311 2023-07-20 08:59:54.000000 pyrsm-0.9.0/pyrsm/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.124818 pyrsm-0.9.0/pyrsm/basics/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.9.0/pyrsm/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.9.0/pyrsm/basics/central_limit_theorem.py
--rw-r--r--   0 root         (0) staff       (20)     8835 2023-07-20 06:02:23.000000 pyrsm-0.9.0/pyrsm/basics/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.9.0/pyrsm/basics/compare_props.py
--rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.9.0/pyrsm/basics/correlation.py
--rw-r--r--   0 root         (0) staff       (20)     9602 2023-07-20 08:21:43.000000 pyrsm-0.9.0/pyrsm/basics/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     6674 2023-07-20 08:58:12.000000 pyrsm-0.9.0/pyrsm/basics/goodness.py
--rw-r--r--   0 root         (0) staff       (20)    10022 2023-07-20 07:13:44.000000 pyrsm-0.9.0/pyrsm/basics/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)    46422 2023-07-20 05:21:13.000000 pyrsm-0.9.0/pyrsm/basics/probability_calculator_functions.py
--rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.9.0/pyrsm/basics/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.9.0/pyrsm/basics/single_prop.py
--rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.9.0/pyrsm/basics/utils.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.9.0/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.125175 pyrsm-0.9.0/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.9.0/pyrsm/data/__radiant-data-convert.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.127656 pyrsm-0.9.0/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/consider.parquet
--rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/consider_description.md
--rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/demand_uk.parquet
--rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/demand_uk_description.md
--rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/newspaper.parquet
--rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/newspaper_description.md
--rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/salary.parquet
--rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/salary_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.131104 pyrsm-0.9.0/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/avengers.parquet
--rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/avengers_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/publishers.parquet
--rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/publishers_description.md
--rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/superheroes.parquet
--rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/superheroes_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.131745 pyrsm-0.9.0/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/design/rndnames.parquet
--rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/design/rndnames_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.137967 pyrsm-0.9.0/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/catalog.parquet
--rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/catalog_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.9.0/pyrsm/data/model/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.9.0/pyrsm/data/model/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/direct_marketing.parquet
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/direct_marketing_description.md
--rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/dvd.parquet
--rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/dvd_description.md
--rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/fraud_data_description.md
--rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/houseprices.parquet
--rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/houseprices_description.md
--rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ideal.parquet
--rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ideal_description.md
--rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ketchup.parquet
--rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ketchup_description.md
--rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ratings.parquet
--rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ratings_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.9.0/pyrsm/data/model/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.9.0/pyrsm/data/model/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.142105 pyrsm-0.9.0/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/carpet.parquet
--rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/carpet_description.md
--rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city.parquet
--rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city2.parquet
--rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city2_description.md
--rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city_description.md
--rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/computer.parquet
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/computer_description.md
--rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/movie.parquet
--rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/movie_description.md
--rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/mp3.parquet
--rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/mp3_description.md
--rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/retailers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/retailers_description.md
--rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/shopping.parquet
--rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/shopping_description.md
--rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste.parquet
--rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste_description.md
--rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands.parquet
--rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands_description.md
--rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.9.0/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     9453 2023-07-20 05:17:59.000000 pyrsm-0.9.0/pyrsm/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    25723 2023-07-20 05:15:29.000000 pyrsm-0.9.0/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.9.0/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.9.0/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.145338 pyrsm-0.9.0/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)      191 2023-07-20 02:17:33.000000 pyrsm-0.9.0/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9915 2023-07-20 06:02:58.000000 pyrsm-0.9.0/pyrsm/radiant/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5502 2023-07-20 07:39:34.000000 pyrsm-0.9.0/pyrsm/radiant/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     5275 2023-07-20 08:58:55.000000 pyrsm-0.9.0/pyrsm/radiant/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     5358 2023-07-20 05:05:48.000000 pyrsm-0.9.0/pyrsm/radiant/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    10973 2023-07-20 01:36:07.000000 pyrsm-0.9.0/pyrsm/radiant/model_utils.py
--rw-r--r--   0 root         (0) staff       (20)    11336 2023-07-20 06:51:33.000000 pyrsm-0.9.0/pyrsm/radiant/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)     4885 2023-07-20 04:10:20.000000 pyrsm-0.9.0/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5545 2023-07-20 05:05:48.000000 pyrsm-0.9.0/pyrsm/radiant/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)    20121 2023-07-20 07:28:01.000000 pyrsm-0.9.0/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.145983 pyrsm-0.9.0/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.9.0/pyrsm/radiant/www/.DS_Store
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.147144 pyrsm-0.9.0/pyrsm/radiant/www/imgs/
--rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-nc-sa.png
--rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-sa.png
--rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.9.0/pyrsm/radiant/www/imgs/icon.png
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.148277 pyrsm-0.9.0/pyrsm/radiant/www/js/
--rw-r--r--   0 root         (0) staff       (20)      343 2023-07-20 00:49:53.000000 pyrsm-0.9.0/pyrsm/radiant/www/js/radiantUI.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.9.0/pyrsm/radiant/www/js/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.9.0/pyrsm/radiant/www/js/screenshot.js
--rw-r--r--   0 root         (0) staff       (20)      609 2023-07-20 01:32:43.000000 pyrsm-0.9.0/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9469 2023-07-20 05:16:59.000000 pyrsm-0.9.0/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.9.0/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.9.0/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.9.0/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.120794 pyrsm-0.9.0/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4022 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      242 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1055 2023-07-20 09:01:14.151005 pyrsm-0.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.150159 pyrsm-0.9.0/tests/
--rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.9.0/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.9.0/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.9.0/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.9.0/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.9.0/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.9.0/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.753359 pyrsm-0.9.1/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-24 01:43:55.753454 pyrsm-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.9.1/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.9.1/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.712963 pyrsm-0.9.1/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-24 01:42:19.000000 pyrsm-0.9.1/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.714995 pyrsm-0.9.1/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.9.1/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.9.1/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     8847 2023-07-22 13:22:08.000000 pyrsm-0.9.1/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.9.1/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.9.1/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9645 2023-07-22 13:13:41.000000 pyrsm-0.9.1/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     6717 2023-07-22 14:39:10.000000 pyrsm-0.9.1/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)    10022 2023-07-20 07:13:44.000000 pyrsm-0.9.1/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)    46422 2023-07-20 05:21:13.000000 pyrsm-0.9.1/pyrsm/basics/probability_calculator_functions.py
+-rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.9.1/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.9.1/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.9.1/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2847 2023-07-23 22:04:07.000000 pyrsm-0.9.1/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.717374 pyrsm-0.9.1/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.9.1/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.718780 pyrsm-0.9.1/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.723110 pyrsm-0.9.1/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.723446 pyrsm-0.9.1/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.728828 pyrsm-0.9.1/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.9.1/pyrsm/data/model/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.9.1/pyrsm/data/model/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ratings_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.9.1/pyrsm/data/model/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.9.1/pyrsm/data/model/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.733369 pyrsm-0.9.1/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3793 2023-07-20 19:08:24.000000 pyrsm-0.9.1/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9490 2023-07-23 22:05:12.000000 pyrsm-0.9.1/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25723 2023-07-20 05:15:29.000000 pyrsm-0.9.1/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.9.1/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.9.1/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.741488 pyrsm-0.9.1/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      216 2023-07-22 06:25:56.000000 pyrsm-0.9.1/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10003 2023-07-23 21:54:37.000000 pyrsm-0.9.1/pyrsm/radiant/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5585 2023-07-22 14:07:40.000000 pyrsm-0.9.1/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     4452 2023-07-22 20:03:41.000000 pyrsm-0.9.1/pyrsm/radiant/data_view.py
+-rw-r--r--   0 root         (0) staff       (20)     5358 2023-07-22 14:09:25.000000 pyrsm-0.9.1/pyrsm/radiant/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     5960 2023-07-22 14:08:11.000000 pyrsm-0.9.1/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    11256 2023-07-20 19:19:46.000000 pyrsm-0.9.1/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)    11364 2023-07-22 23:15:06.000000 pyrsm-0.9.1/pyrsm/radiant/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)     5483 2023-07-22 14:08:47.000000 pyrsm-0.9.1/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     6155 2023-07-23 22:33:41.000000 pyrsm-0.9.1/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    22324 2023-07-23 01:56:31.000000 pyrsm-0.9.1/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.742138 pyrsm-0.9.1/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.9.1/pyrsm/radiant/www/.DS_Store
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.746723 pyrsm-0.9.1/pyrsm/radiant/www/imgs/
+-rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-nc-sa.png
+-rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-sa.png
+-rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.9.1/pyrsm/radiant/www/imgs/icon.png
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.747165 pyrsm-0.9.1/pyrsm/radiant/www/js/
+-rw-r--r--   0 root         (0) staff       (20)      513 2023-07-23 21:45:57.000000 pyrsm-0.9.1/pyrsm/radiant/www/js/radiantUI.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.9.1/pyrsm/radiant/www/js/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.9.1/pyrsm/radiant/www/js/screenshot.js
+-rw-r--r--   0 root         (0) staff       (20)      829 2023-07-20 17:40:43.000000 pyrsm-0.9.1/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9554 2023-07-22 17:06:30.000000 pyrsm-0.9.1/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.9.1/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.9.1/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.9.1/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.713525 pyrsm-0.9.1/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4049 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      273 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1088 2023-07-24 01:43:55.753807 pyrsm-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.753233 pyrsm-0.9.1/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.9.1/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.9.1/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.9.1/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.9.1/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.9.1/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.9.1/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.9.1/tests/test_utils.py
```

### Comparing `pyrsm-0.9.0/LICENSE` & `pyrsm-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/MANIFEST.in` & `pyrsm-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/PKG-INFO` & `pyrsm-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.9.0/README.md` & `pyrsm-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/basics/central_limit_theorem.py` & `pyrsm-0.9.1/pyrsm/basics/central_limit_theorem.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/basics/compare_means.py` & `pyrsm-0.9.1/pyrsm/basics/compare_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         print(self.descriptive_stats.round(dec).to_string(index=False))
 
         comp_stats = self.comp_stats.copy()
         if not extra:
             comp_stats = comp_stats.iloc[:, [0, 1, 2, 3, -1]]
 
         comp_stats["p.value"] = ifelse(
-            comp_stats["p.value"] < 0.001, "< .001", comp_stats["p.value"]
+            comp_stats["p.value"] < 0.001, "< .001", round(comp_stats["p.value"], dec)
         )
         print(comp_stats.round(dec).to_string(index=False))
 
     def plot(self, plots: str = "scatter", nobs: int = -1) -> None:
         if plots == "scatter":
 
             if nobs < self.data.shape[0] and nobs != np.Inf and nobs != -1:
```

### Comparing `pyrsm-0.9.0/pyrsm/basics/compare_props.py` & `pyrsm-0.9.1/pyrsm/basics/compare_props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/basics/correlation.py` & `pyrsm-0.9.1/pyrsm/basics/correlation.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/basics/cross_tabs.py` & `pyrsm-0.9.1/pyrsm/basics/cross_tabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,15 @@
             tab = self.dev_std.transpose()
             args["title"] = "Deviation standardized"
             args.update(**kwargs)
             fig, ax = plt.subplots()
             tab.plot.bar(**args, ax=ax)
             ax.axhline(y=1.96, color="black", linestyle="--")
             ax.axhline(y=1.64, color="black", linestyle="--")
+            ax.axhline(y=0, color="black")
             ax.axhline(y=-1.96, color="black", linestyle="--")
             ax.axhline(y=-1.64, color="black", linestyle="--")
             ax.annotate("95%", xy=(0, 2.1), va="bottom", ha="center")
             ax.annotate("90%", xy=(0, 1.4), va="top", ha="center")
         if "perc_col" in plots:
             tab = self.perc_col.transpose().drop(columns="Total").drop("Total", axis=0)
             args["title"] = "Column percentages"
```

### Comparing `pyrsm-0.9.0/pyrsm/basics/goodness.py` & `pyrsm-0.9.1/pyrsm/basics/goodness.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
             tab = self.stdev.transpose()
             args["title"] = "Deviation standardized"
             args.update(**kwargs, legend=False)
             fig, ax = plt.subplots()
             tab.plot.bar(**args, ax=ax)
             ax.axhline(y=1.96, color="black", linestyle="--")
             ax.axhline(y=1.64, color="black", linestyle="--")
+            ax.axhline(y=0, color="black")
             ax.axhline(y=-1.96, color="black", linestyle="--")
             ax.axhline(y=-1.64, color="black", linestyle="--")
             ax.annotate("95%", xy=(0, 2.1), va="bottom", ha="center")
             ax.annotate("90%", xy=(0, 1.4), va="top", ha="center")
 
 
 if __name__ == "__main__":
```

### Comparing `pyrsm-0.9.0/pyrsm/basics/probability_calculator.py` & `pyrsm-0.9.1/pyrsm/basics/probability_calculator.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/basics/probability_calculator_functions.py` & `pyrsm-0.9.1/pyrsm/basics/probability_calculator_functions.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/basics/single_mean.py` & `pyrsm-0.9.1/pyrsm/basics/single_mean.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/basics/single_prop.py` & `pyrsm-0.9.1/pyrsm/basics/single_prop.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/bins.py` & `pyrsm-0.9.1/pyrsm/bins.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,18 @@
     Numpy array with bin numbers for each numeric value in x
 
     Examples
     --------
     xtile(np.arange(10), 5)
     xtile(np.arange(10), 5, rev=True)
     """
+
     x = np.array(x)
-    breaks = np.quantile(x[np.isnan(x) == False], np.arange(0, n + 1) / n)
+    breaks = np.quantile(x[~np.isnan(x)], np.arange(0, n + 1) / n)
+    breaks
     if len(np.unique(breaks)) == len(breaks):
         bins = pd.cut(x, breaks, include_lowest=True, labels=False) + 1
     else:
         bins = bincode(x, breaks)
 
     if rev is True:
         bins = (n + 1) - bins
```

### Comparing `pyrsm-0.9.0/pyrsm/data/__radiant-data-convert.py` & `pyrsm-0.9.1/pyrsm/data/__radiant-data-convert.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/basics/consider.parquet` & `pyrsm-0.9.1/pyrsm/data/basics/consider.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/basics/consider_description.md` & `pyrsm-0.9.1/pyrsm/data/basics/consider_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/basics/demand_uk.parquet` & `pyrsm-0.9.1/pyrsm/data/basics/demand_uk.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/basics/newspaper.parquet` & `pyrsm-0.9.1/pyrsm/data/basics/newspaper.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/basics/newspaper_description.md` & `pyrsm-0.9.1/pyrsm/data/basics/newspaper_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/basics/salary.parquet` & `pyrsm-0.9.1/pyrsm/data/basics/salary.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/basics/salary_description.md` & `pyrsm-0.9.1/pyrsm/data/basics/salary_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/data/avengers.parquet` & `pyrsm-0.9.1/pyrsm/data/data/avengers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/data/diamonds.parquet` & `pyrsm-0.9.1/pyrsm/data/data/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/data/diamonds_description.md` & `pyrsm-0.9.1/pyrsm/data/data/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/data/publishers.parquet` & `pyrsm-0.9.1/pyrsm/data/data/publishers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/data/superheroes.parquet` & `pyrsm-0.9.1/pyrsm/data/data/superheroes.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/data/titanic.parquet` & `pyrsm-0.9.1/pyrsm/data/data/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/data/titanic_description.md` & `pyrsm-0.9.1/pyrsm/data/data/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/design/rndnames.parquet` & `pyrsm-0.9.1/pyrsm/data/design/rndnames.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/catalog.parquet` & `pyrsm-0.9.1/pyrsm/data/model/catalog.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/catalog_description.md` & `pyrsm-0.9.1/pyrsm/data/model/catalog_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/diamonds.parquet` & `pyrsm-0.9.1/pyrsm/data/model/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/diamonds_description.md` & `pyrsm-0.9.1/pyrsm/data/model/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/direct_marketing.parquet` & `pyrsm-0.9.1/pyrsm/data/model/direct_marketing.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/direct_marketing_description.md` & `pyrsm-0.9.1/pyrsm/data/model/direct_marketing_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/dvd.parquet` & `pyrsm-0.9.1/pyrsm/data/model/dvd.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/dvd_description.md` & `pyrsm-0.9.1/pyrsm/data/model/dvd_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/fraud_data_description.md` & `pyrsm-0.9.1/pyrsm/data/model/fraud_data_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/houseprices.parquet` & `pyrsm-0.9.1/pyrsm/data/model/houseprices.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/houseprices_description.md` & `pyrsm-0.9.1/pyrsm/data/model/houseprices_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/ideal.parquet` & `pyrsm-0.9.1/pyrsm/data/model/ideal.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/ketchup.parquet` & `pyrsm-0.9.1/pyrsm/data/model/ketchup.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/ketchup_description.md` & `pyrsm-0.9.1/pyrsm/data/model/ketchup_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/ratings.parquet` & `pyrsm-0.9.1/pyrsm/data/model/ratings.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/titanic.parquet` & `pyrsm-0.9.1/pyrsm/data/model/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/model/titanic_description.md` & `pyrsm-0.9.1/pyrsm/data/model/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/carpet.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/carpet.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/carpet_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/carpet_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/city.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/city.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/city2.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/city2.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/computer.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/computer.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/computer_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/computer_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/movie.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/movie.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/movie_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/movie_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/mp3.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/mp3.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/mp3_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/mp3_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/retailers.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/retailers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/retailers_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/retailers_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/shopping.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/shopping.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/shopping_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/shopping_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands.parquet` & `pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands_description.md` & `pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/example_data.py` & `pyrsm-0.9.1/pyrsm/example_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,21 +56,29 @@
                     description[key] = load_description(
                         file_path.replace(".parquet", "")
                     )
         return data, description
 
     if pkg is None and name is None:
         data, description = mkdct(
-            [d for d in os.listdir(base_path) if not d.startswith("__")]
+            [
+                d
+                for d in os.listdir(base_path)
+                if not d.startswith("__") and not d.startswith(".")
+            ]
         )
     elif pkg is not None and name is None:
         data, description = mkdct([pkg])
     elif pkg is None and name is not None:
         data, description = mkdct(
-            [d for d in os.listdir(base_path) if not d.startswith("__")]
+            [
+                d
+                for d in os.listdir(base_path)
+                if not d.startswith("__") and not d.startswith(".")
+            ]
         )
         if dct is None:
             data = data[name]
             description = description[name]
     elif pkg is not None and name is not None:
         data = load_data(os.path.join(base_path, pkg, f"{name}.parquet"))
         description = load_description(os.path.join(base_path, pkg, name))
```

### Comparing `pyrsm-0.9.0/pyrsm/logistic.py` & `pyrsm-0.9.1/pyrsm/logistic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from typing import Union, Optional
-import re
 import pandas as pd
 import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib.ticker as ticker
 from statsmodels.genmod.families import Binomial
 from statsmodels.genmod.families.links import Logit
 import statsmodels.formula.api as smf
 from scipy import stats
 from .utils import ifelse, setdiff
 from .model import sig_stars, model_fit, or_ci, or_plot, sim_prediction, predict_ci
 from .model import vif as calc_vif
@@ -97,15 +94,15 @@
         df["coefficient"] = df["coefficient"].round(2)
         df["std.error"] = df["std.error"].round(dec)
         df["z.value"] = df["z.value"].round(dec)
         df["p.value"] = ifelse(
             df["p.value"] < 0.001, "< .001", df["p.value"].round(dec)
         )
         df["OR%"] = [f"{round(o, max(dec-2, 0))}%" for o in df["OR%"]]
-
+        df["index"] = df["index"].str.replace("[T.", "[", regex=False)
         df = df.set_index("index")
         df.index.name = None
         print(f"\n{df.to_string()}")
         print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
         print(f"\n{model_fit(self.fitted)}")
 
         if ci:
@@ -121,31 +118,30 @@
                 print("\nVariance inflation factors:")
                 print(f"\n{calc_vif(self.fitted).to_string()}")
 
         if test is not None and len(test) > 0:
             self.chisq_test(test=test, dec=dec)
 
     def predict(
-        self, data=None, cmd=None, dc=False, ci=False, conf=0.95
+        self, data=None, cmd=None, data_cmd=None, ci=False, conf=0.95
     ) -> pd.DataFrame:
         """
         Predict values for a linear regression model
         """
         if data is None:
             data = self.data
         data = data.loc[:, self.evar].copy()
-        if cmd is not None:
-            if dc:
-                for k, v in cmd.items():
-                    data[k] = v
-            else:
-                data = sim_prediction(data=data, vary=cmd)
+        if data_cmd is not None:
+            for k, v in data_cmd.items():
+                data[k] = v
+        elif cmd is not None:
+            data = sim_prediction(data=data, vary=cmd)
 
         if ci:
-            if dc:
+            if data_cmd is not None:
                 raise ValueError(
                     "Confidence intervals not available when using the Data & Command option"
                 )
             else:
                 return pd.concat(
                     [data, predict_ci(self.fitted, data, conf=conf)], axis=1
                 )
@@ -213,29 +209,29 @@
         form = f"{self.rvar} ~ "
         if len(evar) == 0 and len(sint) == 0:
             form += "1"
         else:
             form += f"{' + '.join(evar + sint)}"
 
         # ensure constraints are unique
-        pattern = r"(\[T\.[^\]]*\])\:"
-        hypotheses = list(
-            set(
-                [
-                    f"({c} = 0)"
-                    for c in self.fitted.model.exog_names
-                    for v in test
-                    if f"{v}:" in c
-                    or f":{v}" in c
-                    or f"{v}[T." in c
-                    or v == c
-                    or v == re.sub(pattern, ":", c)
-                ]
-            )
-        )
+        # pattern = r"(\[T\.[^\]]*\])\:"
+        # hypotheses = list(
+        #     set(
+        #         [
+        #             f"({c} = 0)"
+        #             for c in self.fitted.model.exog_names
+        #             for v in test
+        #             if f"{v}:" in c
+        #             or f":{v}" in c
+        #             or f"{v}[T." in c
+        #             or v == c
+        #             or v == re.sub(pattern, ":", c)
+        #         ]
+        #     )
+        # )
 
         print(f"\nModel 1: {form}")
         print(f"Model 2: {self.form}")
 
         # Wald test (faster but not as accurate)
         # out = self.fitted.wald_test(hypotheses, scalar=True)
         # pvalue = ifelse(out.pvalue < 0.001, "< .001", round(out.pvalue, dec))
```

### Comparing `pyrsm-0.9.0/pyrsm/model.py` & `pyrsm-0.9.1/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/notebook.py` & `pyrsm-0.9.1/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/perf.py` & `pyrsm-0.9.1/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/props.py` & `pyrsm-0.9.1/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/radiant/compare_means.py` & `pyrsm-0.9.1/pyrsm/radiant/compare_means.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session, req
-import webbrowser, nest_asyncio, uvicorn
-import signal, os, sys, tempfile
+import webbrowser
+import nest_asyncio
+import uvicorn
+import signal
+import os
+import sys
+import tempfile
 import pyrsm as rsm
 from pyrsm.utils import ifelse
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 
 def ui_summary():
@@ -108,42 +113,43 @@
 )
 
 
 class basics_compare_means:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
 
-    def shiny_ui(self):
+    def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Compare means",
+                "<< Basics > Compare means >>",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
                         ru.ui_plot(choices, plots_extra),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
+            *args,
             ru.ui_help(
                 "https://github.com/vnijs/pyrsm/blob/main/examples/basics-compare-means.ipynb",
                 "Compare means example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data = ru.make_data_elements(self, input, output)
+        get_data = ru.make_data_elements(self, input, output, session)
 
         # --- section unique to each app ---
         @output(id="ui_cvar1")
         @render.ui
         def ui_cvar1():
             isCat = get_data()["var_types"]["isCat"]
             return ui.input_select(
@@ -250,14 +256,15 @@
             args_string = ru.drop_default_args(args, rsm.basics.compare_means.summary)
             return f"""cm.summary({args_string})"""
 
         mu.make_summary(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="cm",
             sum_fun=rsm.basics.compare_means.summary,
             sc=summary_code,
         )
 
@@ -268,14 +275,15 @@
             )
             return f"""cm.plot({args_string})"""
 
         mu.make_plot(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="cm",
             pc=plot_code,
         )
 
         # --- section standard for all apps ---
@@ -317,10 +325,8 @@
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    import pyrsm as rsm
-
     compare_means()
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/cross_tabs.py` & `pyrsm-0.9.1/pyrsm/radiant/cross_tabs.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,42 +36,43 @@
 plots.update(choices)
 
 
 class basics_cross_tabs:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
 
-    def shiny_ui(self):
+    def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Cross-tabs",
+                "<< Basics > Cross-tabs >>",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
                         ru.ui_plot(plots),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
+            *args,
             ru.ui_help(
                 "https://github.com/vnijs/pyrsm/blob/main/examples/basics-cross-tabs.ipynb",
                 "Cross-tabs example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data = ru.make_data_elements(self, input, output)
+        get_data = ru.make_data_elements(self, input, output, session)
 
         # --- section unique to each app ---
         @output(id="ui_var1")
         @render.ui
         def ui_var1():
             isCat = get_data()["var_types"]["isCat"]
             return ui.input_select(
@@ -123,28 +124,30 @@
             args = [c for c in input.output()]
             return f"""ct.summary(output={args})"""
 
         mu.make_summary(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="ct",
             sum_fun=rsm.basics.cross_tabs.summary,
             sc=summary_code,
         )
 
         def plot_code():
             return f"""ct.plot(plots="{input.plots()}")"""
 
         mu.make_plot(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="ct",
             pc=plot_code,
         )
 
         # --- section standard for all apps ---
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/goodness.py` & `pyrsm-0.9.1/pyrsm/radiant/goodness.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,42 +38,43 @@
 plots.update(choices)
 
 
 class basics_goodness:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
 
-    def shiny_ui(self):
+    def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Goodness-of-fit",
+                "<< Basics > Goodness-of-fit >>",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
                         ru.ui_plot(plots),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
+            *args,
             ru.ui_help(
                 "https://github.com/vnijs/pyrsm/blob/main/examples/basics-goodness.ipynb",
                 "Goodness-of-fit example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data = ru.make_data_elements(self, input, output)
+        get_data = ru.make_data_elements(self, input, output, session)
 
         # --- section unique to each app ---
         @output(id="ui_var")
         @render.ui
         def ui_var1():
             isCat = get_data()["var_types"]["isCat"]
             return ui.input_select(
@@ -118,28 +119,30 @@
             args = [c for c in input.output()]
             return f"""gf.summary(output={args})"""
 
         mu.make_summary(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="gf",
             sum_fun=rsm.basics.goodness.summary,
             sc=summary_code,
         )
 
         def plot_code():
             return f"""gf.plot(plots="{input.plots()}")"""
 
         mu.make_plot(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="gf",
             pc=plot_code,
         )
 
         # --- section standard for all apps ---
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/logistic.py` & `pyrsm-0.9.1/pyrsm/radiant/logistic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+from starlette.applications import Starlette
+from starlette.routing import Mount
+from starlette.staticfiles import StaticFiles
 from shiny import App, ui, render, reactive, Inputs, Outputs, Session
+from pathlib import Path
 import webbrowser, nest_asyncio, uvicorn
 import signal, os, sys, tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
@@ -55,43 +59,44 @@
 )
 
 
 class model_logistic:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
 
-    def shiny_ui(self):
+    def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Model > Logistic regression (GLM)",
+                "<< Model > Logistic regression (GLM) >>",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ru.ui_summary(summary_extra),
                         mu.ui_predict(self),
                         ru.ui_plot(choices, plots_extra),
                     ),
                     ui.column(8, ru.ui_main_model()),
                 ),
             ),
+            *args,
             ru.ui_help(
                 "https://github.com/vnijs/pyrsm/blob/main/examples/model-logistic-regression.ipynb",
                 "Logistic regression (GLM) example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data = ru.make_data_elements(self, input, output)
+        get_data = ru.make_data_elements(self, input, output, session)
 
         # @reactive.Effect
         # def print_inputs():
         #     print(input.rvar())
         #     print(input.evar())
 
         # --- section standard for all model apps ---
@@ -115,32 +120,35 @@
         show_code, estimate = mu.make_estimate(
             self, input, output, get_data, fun="logistic", ret="lr", debug=False
         )
         mu.make_summary(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="lr",
             sum_fun=rsm.logistic.summary,
         )
         mu.make_predict(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="lr",
             pred_fun=rsm.logistic.predict,
         )
         mu.make_plot(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="lr",
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
@@ -155,36 +163,47 @@
 def logistic(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
+    debug: bool = False,
 ):
     """
     Launch a Radiant-for-Python app for logistic regression analysis
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="model")
     rc = model_logistic(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
-    temp = tempfile.NamedTemporaryFile()
-    sys.stdout = open(temp.name, "w")
-    sys.stderr = open(temp.name, "w")
+    if not debug:
+        temp = tempfile.NamedTemporaryFile()
+        sys.stdout = open(temp.name, "w")
+        sys.stderr = open(temp.name, "w")
+
+    app = App(rc.shiny_ui(ru.radiant_navbar()), rc.shiny_server)
+    www_dir = Path(__file__).parent.parent / "radiant" / "www"
+    app_static = StaticFiles(directory=www_dir, html=False)
+
+    routes = [
+        Mount("/www", app=app_static),
+        Mount("/", app=app),
+    ]
 
     uvicorn.run(
-        App(rc.shiny_ui(), rc.shiny_server),
+        Starlette(debug=debug, routes=routes),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     # titanic, titanic_description = rsm.load_data(pkg="data", name="titanic")
     # logistic({"titanic": titanic}, {"titanic": titanic_description}, code=True)
-    logistic()
+    logistic(debug=True)
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/model_utils.py` & `pyrsm-0.9.1/pyrsm/radiant/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,17 @@
             ]  # get data into local scope
 
             return eval(estimation_code()[0])
 
     return show_code, estimate
 
 
-def make_summary(self, input, output, show_code, estimate, ret, sum_fun, sc=None):
+def make_summary(
+    self, input, output, session, show_code, estimate, ret, sum_fun, sc=None
+):
     if sc is None:
 
         def summary_code():
             args = {c: True for c in input.controls()}
             if input.evar_test() is not None and len(input.evar_test()) > 0:
                 args["test"] = list(input.evar_test())
 
@@ -231,52 +233,58 @@
     else:
         summary_code = sc
 
     @output(id="show_summary_code")
     @render.text
     def show_summary_code():
         cmd = f"""{show_code()}\n{summary_code()}"""
-        return ru.code_formatter(cmd, self)
+        # return ru.code_formatter(cmd, self)
+        return ru.code_formatter(cmd, self, input, session, id="copy_summary")
 
     @output(id="summary")
     @render.text
     def summary():
         out = io.StringIO()
         with redirect_stdout(out), redirect_stderr(out):
             locals()[ret] = estimate()  # get model object into local scope
             eval(summary_code())
         return out.getvalue()
 
 
-def make_predict(self, input, output, show_code, estimate, ret, pred_fun):
+def make_predict(self, input, output, session, show_code, estimate, ret, pred_fun):
     def predict_code():
         args = {}
         cmd = input.pred_cmd().strip()
 
         if input.pred_type() == "Data":
-            args["df"] = input.pred_datasets()
+            args["data"] = input.pred_datasets()
         elif input.pred_type() == "Command" and not ru.is_empty(cmd):
-            args["df"] = None
+            args["data"] = None
             args["cmd"] = cmd
         elif input.pred_type() == "Data & Command" and not ru.is_empty(cmd):
-            args["df"] = input.pred_datasets()
-            args["cmd"] = cmd
-            args["dc"] = True
+            args["data"] = input.pred_datasets()
+            args["data_cmd"] = cmd
 
         ci = input.pred_ci()
         if ci:
             args.update({"ci": ci, "conf": input.conf()})
 
         args_string = ru.drop_default_args(args, pred_fun)
         return f"""{ret}.predict({args_string})"""
 
     @output(id="show_predict_code")
     @render.text
     def show_predict_code():
-        return ru.code_formatter(f"""{show_code()}\npred = {predict_code()}""", self)
+        return ru.code_formatter(
+            f"""{show_code()}\npred = {predict_code()}""",
+            self,
+            input,
+            session,
+            id="copy_predict",
+        )
 
     @output(id="predict")
     @render.data_frame
     def predict():
         if input.pred_type() != "None":
             locals()[ret] = estimate()  # get model object into local scope
             if input.pred_type() in ["Data", "Data & Command"]:
@@ -291,15 +299,15 @@
                 summary += " (100K rows shown)"
 
             return render.DataTable(pred.round(3), summary=summary)
         else:
             return None
 
 
-def make_plot(self, input, output, show_code, estimate, ret, pc=None):
+def make_plot(self, input, output, session, show_code, estimate, ret, pc=None):
 
     if pc is None:
 
         def plot_code():
             plots = input.plots()
             if plots == "pred":
                 incl = list(input.incl_evar())
@@ -319,15 +327,16 @@
 
     @output(id="show_plot_code")
     @render.text
     def show_plot_code():
         plots = input.plots()
         if plots != "None":
             cmd = f"""{show_code()}\n{plot_code()}"""
-            return ru.code_formatter(cmd, self)
+            # return ru.code_formatter(cmd, self)
+            return ru.code_formatter(cmd, self, input, session, id="copy_plot")
 
     @reactive.Calc
     def gen_plot():
         locals()[ret] = estimate()
         eval(f"""{plot_code()}""")
         fig = plt.gcf()
         width, height = fig.get_size_inches()  # Get the size in inches
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/probability_calculator.py` & `pyrsm-0.9.1/pyrsm/radiant/probability_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,28 +72,29 @@
     )
 
 
 class basics_probability_calculator:
     def __init__(self, code=True) -> None:
         self.code = code
 
-    def shiny_ui(self):
+    def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Probability calculator",
+                "<< Basics > Probability calculator >>",
                 ui.row(
                     ui.column(
                         3,
                         ui_summary(),
                         ui_type(),
                     ),
                     ui.column(8, ui_main_pc()),
                 ),
             ),
+            *args,
             ru.ui_help(
                 "https://github.com/vnijs/pyrsm/blob/main/examples/basics-probability-calculator.ipynb",
                 "Probability calculator example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
@@ -132,15 +133,15 @@
                     placeholder="Insert list [1/4, 1/8, 5/8]",
                     value="[1 / 4, 1 / 8, 5 / 8]",
                 ),
             )
 
         @output(id="ui_pc_expo")
         @render.ui
-        def ui_pc_chisq():
+        def ui_pc_expo():
             return ui.input_numeric("expo_rate", label="Rate:", value=1, min=1)
 
         @output(id="ui_pc_fdist")
         @render.ui
         def ui_pc_fdist():
             return ru.make_side_by_side(
                 ui.input_numeric(
@@ -149,15 +150,15 @@
                 ui.input_numeric(
                     "fdist_df2", label="Degrees of freedom 2:", value=10, min=0
                 ),
             )
 
         @output(id="ui_pc_lnorm")
         @render.ui
-        def ui_pc_norm():
+        def ui_pc_lnorm():
             return ru.make_side_by_side(
                 ui.input_numeric("lnorm_mean", label="Mean log:", value=0),
                 ui.input_numeric("lnorm_stdev", label="St. dev. log:", value=1, min=0),
             )
 
         @output(id="ui_pc_norm")
         @render.ui
@@ -258,29 +259,29 @@
             args_string = ru.drop_default_args(args, fun)
             return f"""pc.summary({args_string})"""
 
         @output(id="show_summary_code")
         @render.text
         def show_summary_code():
             cmd = f"""import pyrsm as rsm\npc = {estimation_code()}\n{summary_code()}\npc.plot()"""
-            return ru.code_formatter(cmd, self)  # , id="copy_pc")
+            return ru.code_formatter(cmd, self, input, session)
 
         @output(id="summary")
         @render.text
         def summary():
             out = io.StringIO()
             with redirect_stdout(out), redirect_stderr(out):
                 pc = estimate()  # get estimation object into local scope
                 eval(summary_code())
             return out.getvalue()
 
         @reactive.Calc
         def gen_plot():
             locals()["pc"] = estimate()
-            eval(f"""pc.plot()""")
+            eval("""pc.plot()""")
             fig = plt.gcf()
             width, height = fig.get_size_inches()  # Get the size in inches
             return fig, width * 96, height * 96
 
         @output(id="plot")
         @render.plot
         def plot():
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/regress.py` & `pyrsm-0.9.1/pyrsm/radiant/regress.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+from starlette.applications import Starlette
+from starlette.routing import Mount
+from starlette.staticfiles import StaticFiles
 from shiny import App, ui, reactive, Inputs, Outputs, Session
+from pathlib import Path
 import webbrowser, nest_asyncio, uvicorn, os, signal
-import signal, os, io, sys, tempfile
+import signal, os, sys, tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "None": "None",
     "dist": "Distribution",
@@ -59,75 +63,79 @@
 )
 
 
 class model_regress:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
 
-    def shiny_ui(self):
+    def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Model > Linear regression (OLS)",
+                "<< Model > Linear regression (OLS) >>",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ru.ui_summary(summary_extra),
                         mu.ui_predict(self),
                         ru.ui_plot(choices, plots_extra),
                     ),
                     ui.column(8, ru.ui_main_model()),
                 ),
             ),
+            *args,
             ru.ui_help(
                 "https://github.com/vnijs/pyrsm/blob/main/examples/model-linear-regression.ipynb",
                 "Linear regression (OLS) example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data = ru.make_data_elements(self, input, output)
+        get_data = ru.make_data_elements(self, input, output, session)
 
         # --- section standard for all model apps ---
         ru.reestimate(input)
 
         # --- section unique to each app ---
         mu.make_model_inputs(input, output, get_data, "isNum")
         mu.make_int_inputs(input, output, get_data)
         show_code, estimate = mu.make_estimate(
             self, input, output, get_data, fun="regress", ret="reg", debug=False
         )
         mu.make_summary(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="reg",
             sum_fun=rsm.regress.summary,
         )
         mu.make_predict(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="reg",
             pred_fun=rsm.regress.predict,
         )
         mu.make_plot(
             self,
             input,
             output,
+            session,
             show_code,
             estimate,
             ret="reg",
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
@@ -142,34 +150,45 @@
 def regress(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
+    debug: bool = False,
 ):
     """
     Launch a Radiant-for-Python app for linear regression analysis
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="model")
     rc = model_regress(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
-    temp = tempfile.NamedTemporaryFile()
-    sys.stdout = open(temp.name, "w")
-    sys.stderr = open(temp.name, "w")
+    if not debug:
+        temp = tempfile.NamedTemporaryFile()
+        sys.stdout = open(temp.name, "w")
+        sys.stderr = open(temp.name, "w")
+
+    app = App(rc.shiny_ui(ru.radiant_navbar()), rc.shiny_server)
+    www_dir = Path(__file__).parent.parent / "radiant" / "www"
+    app_static = StaticFiles(directory=www_dir, html=False)
+
+    routes = [
+        Mount("/www", app=app_static),
+        Mount("/", app=app),
+    ]
 
     uvicorn.run(
-        App(rc.shiny_ui(), rc.shiny_server),
+        Starlette(debug=debug, routes=routes),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    regress()
+    regress(debug=True)
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/utils.py` & `pyrsm-0.9.1/pyrsm/radiant/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import black, os, signal, inspect, time
+import black
+import inspect
+from shiny import req
 from htmltools import tags, div, css
 from itertools import combinations
 from shiny import render, ui, reactive
 from faicons import icon_svg
-from pathlib import Path
 import pandas as pd
 import polars as pl
 from pyrsm.utils import ifelse
 from pyrsm.example_data import load_data
 
 
 def get_dfs(pkg=None, name=None, obj=pd.DataFrame):
@@ -35,40 +36,25 @@
     )
 
 
 def head_content():
     """
     Return the head content for the shiny app
     """
-
-    www_dir = Path(__file__).parent / "www"
-    ui.tags.link(rel="shortcut icon", href=f"{www_dir}/imgs/icon.png")
-
-    www_dir = Path(__file__).parent / "www"
     return ui.head_content(
         # from https://github.com/rstudio/py-shiny/issues/491#issuecomment-1579138681
         ui.tags.link(
             href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/agate.min.css",
             rel="stylesheet",
         ),
-        # ui.tags.link(rel="shortcut icon", href=f"{www_dir}/imgs/icon.png"),
-        ui.tags.link(rel="icon", type="image/png", href=f"{www_dir}/imgs/icon.png"),
-        ui.include_css((www_dir / "style.css")),
-        # ui.include_js(www_dir / "js/returnTextAreaBinding.js"),
-        # ui.include_js(www_dir / "js/radiantUI.js"), # too slow on startup? Throws an error
-        # ui.include_js(www_dir / "js/screenshot.js"),
-        ui.tags.script(
-            (www_dir / "js/returnTextAreaBinding.js").read_text(),
-        ),
-        ui.tags.script(
-            (www_dir / "js/radiantUI.js").read_text(),
-        ),
-        ui.tags.script(
-            (www_dir / "js/screenshot.js").read_text(),
-        ),
+        ui.tags.link(rel="shortcut icon", href=f"/www/imgs/icon.png"),
+        ui.tags.link(href="/www/style.css", rel="stylesheet"),
+        ui.tags.script(src="/www/js/returnTextAreaBinding.js"),
+        ui.tags.script(src="/www/js/radiantUI.js"),
+        ui.tags.script(src="/www/js/screenshot.js"),
         ui.tags.script(
             src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js",
         ),
         ui.tags.script(
             src="//html2canvas.hertzen.com/dist/html2canvas.min.js",
         ),
     )
@@ -88,51 +74,73 @@
             isinstance(descriptions, dict),
             descriptions,
             {"description": descriptions},
         )
     self.dataset_list = list(datasets.keys())
     self.code = code  # keep code windows open or closed by default
     self.stop_code = ""
+    self.state = {}
 
 
 def escape_quotes(cmd):
     return cmd.replace('"', '\\"').replace("'", "\\'")
 
 
 def quote(v, k, ignore=["data"]):
     if isinstance(v, str) and k not in ignore and not (v[0] + v[-1] == "{}"):
         v = escape_quotes(v)
         return f'"{v}"'
     else:
         return v
 
 
-def copy_icon(cmd):
+def copy_icon(cmd, id):
     cmd = escape_quotes(cmd).replace("\n", "\\n")
     return (
         ui.input_action_link(
-            "copy",
+            id,
             None,
             icon=icon_svg("copy", width="1.5em", height="1.5em"),
             title="Copy to clipboard",
             onclick=f'copyToClipboard("{cmd}");',
         ),
     )
 
 
-def code_formatter(code, self):
+def copy_reset(input, session, id="copy"):
+    @reactive.Effect
+    @reactive.event(input[id], ignore_none=True)
+    async def copy_success():
+        ui.update_action_link(
+            id,
+            icon=icon_svg("check", fill="green", width="1.5em", height="1.5em"),
+        )
+        # await session.send_custom_message("reset_copy", "")
+
+    @reactive.Effect
+    @reactive.event(input.copy_reset, ignore_none=True)
+    async def copy_reset():
+        req(input[id])
+        ui.update_action_link(
+            id,
+            icon=icon_svg("copy", width="1.5em", height="1.5em"),
+        )
+
+
+def code_formatter(code, self, input, session, id="copy"):
     """
     Format python code using black
     """
     cmd = self.stop_code = black.format_str(code, mode=black.Mode())
+    copy_reset(input, session, id=id)
     return ui.TagList(
         ui.HTML(
             f"<details {ifelse(self.code, 'open', '')}><summary>View generated python code</summary>"
         ),
-        copy_icon(cmd),
+        copy_icon(cmd, id=id),
         ui.markdown(f"""\n```python\n{cmd.rstrip()}\n```"""),
         ui.tags.script("hljs.highlightAll();"),
         ui.HTML("</details>"),
         ui.br(),
     )
 
 
@@ -203,19 +211,21 @@
         "data_name": data_name,
         "description": description,
         "var_types": var_types,
         "code": code,
     }
 
 
-def make_data_elements(self, input, output):
+def make_data_elements(self, input, output, session):
     @output(id="show_data_code")
     @render.ui
     def show_data_code():
-        return code_formatter(get_data(self, input)["code"], self)
+        return code_formatter(
+            get_data(self, input)["code"], self, input, session, id="copy_data"
+        )
 
     @output(id="show_data")
     @render.data_frame
     def show_data():
         data = get_data(self, input)["data"]
         summary = "Viewing rows {start} through {end} of {total}"
         if data.shape[0] > 100_000:
@@ -274,53 +284,58 @@
 def iterms(vars, nway=2, sep=":"):
     cvars = list(combinations(vars, 2))
     if nway > 2:
         cvars += list(combinations(vars, nway))
     return [f"{sep}".join(c) for c in cvars]
 
 
-def ui_data(self):
-    return (
+def ui_view(self):
+    return ui.panel_well(
+        ui.input_select(
+            "datasets",
+            "Datasets:",
+            self.dataset_list,
+            selected=self.state.get("datasets", None),
+        ),
+        ui.input_checkbox("show_filter", "Show data filter", value=True),
         ui.panel_conditional(
-            "input.tabs == 'Data'",
-            ui.panel_well(
-                ui.input_select("datasets", "Datasets:", self.dataset_list),
-                ui.input_checkbox("show_filter", "Show data filter", value=True),
-                ui.panel_conditional(
-                    "input.show_filter == true",
-                    # ui.input_radio_buttons(
-                    #     "data_language",
-                    #     "Data language",
-                    #     ["Pandas", "Polars", "SQL"],
-                    #     inline=True,
-                    # ),
-                    input_return_text_area(
-                        "data_filter",
-                        "Data Filter:",
-                        rows=2,
-                        placeholder="Provide a filter (e.g., price >  5000) and press return",
-                    ),
-                    input_return_text_area(
-                        "data_sort",
-                        "Data sort:",
-                        rows=2,
-                        placeholder="Sort (e.g., ['color', 'price'], ascending=[True, False])) and press return",
-                    ),
-                    input_return_text_area(
-                        "data_slice",
-                        "Data slice (rows):",
-                        rows=1,
-                        placeholder="e.g., 0:50 and press return",
-                    ),
-                ),
+            "input.show_filter == true",
+            # ui.input_radio_buttons(
+            #     "data_language",
+            #     "Data language",
+            #     ["Pandas", "Polars", "SQL"],
+            #     inline=True,
+            # ),
+            input_return_text_area(
+                "data_filter",
+                "Data Filter:",
+                rows=2,
+                value=self.state.get("data_filter", ""),
+                placeholder="Provide a filter (e.g., price >  5000) and press return",
+            ),
+            input_return_text_area(
+                "data_sort",
+                "Data sort:",
+                rows=2,
+                placeholder="Sort (e.g., ['color', 'price'], ascending=[True, False])) and press return",
+            ),
+            input_return_text_area(
+                "data_slice",
+                "Data slice (rows):",
+                rows=1,
+                placeholder="e.g., 0:50 and press return",
             ),
         ),
     )
 
 
+def ui_data(self):
+    return ui.panel_conditional("input.tabs == 'Data'", ui_view(self))
+
+
 def ui_summary(*args):
     return ui.panel_conditional(
         "input.tabs == 'Summary'",
         ui.panel_well(
             ui.input_action_button(
                 "run",
                 "Estimate model",
@@ -348,26 +363,27 @@
             ),
             *args,
         ),
     )
 
 
 def ui_data_main():
-    data_main = ui.nav(
-        "Data",
+    return ui.div(
         ui.output_ui("show_data_code"),
         ui.output_data_frame("show_data"),
         ui.output_ui("show_description"),
     )
-    return data_main
 
 
 def ui_main_basics(height="500px", width="700px"):
     return ui.navset_tab_card(
-        ui_data_main(),
+        ui.nav(
+            "Data",
+            ui_data_main(),
+        ),
         ui.nav(
             "Summary",
             ui.output_ui("show_summary_code"),
             ui.output_text_verbatim("summary"),
         ),
         ui.nav(
             "Plot",
@@ -376,15 +392,18 @@
         ),
         id="tabs",
     )
 
 
 def ui_main_model():
     return ui.navset_tab_card(
-        ui_data_main(),
+        ui.nav(
+            "Data",
+            ui_data_main(),
+        ),
         ui.nav(
             "Summary",
             ui.output_ui("show_estimation_code"),
             ui.output_ui("show_summary_code"),
             ui.output_text_verbatim("summary"),
         ),
         ui.nav(
@@ -398,14 +417,75 @@
             # ui.output_plot("plot", height="800px", width="700px"),
             ui.output_ui("plot_container"),
         ),
         id="tabs",
     )
 
 
+def radiant_navbar():
+    return (
+        ui.nav_control(
+            ui.input_action_link("data", "Data", onclick='window.location.href = "/";')
+        ),
+        ui.nav_menu(
+            "Basics",
+            ui.nav_control(
+                # "Probability",
+                ui.input_action_link(
+                    "pc",
+                    "Probability Calculator",
+                    # onclick='window.location.href = "/basics/prob-calc/?SSUID=local-e47b75";',
+                    onclick='window.location.href = "/basics/prob-calc/";',
+                ),
+                # "----",
+                # "Means",
+                ui.input_action_link(
+                    "sm",
+                    "Single mean",
+                    onclick='window.location.href = "/basics/single-mean/";',
+                ),
+                ui.input_action_link(
+                    "cm",
+                    "Compare means",
+                    onclick='window.location.href = "/basics/compare-means/";',
+                ),
+                # "----",
+                # "Proportions",
+                # "----",
+                # "Tables",
+                ui.input_action_link(
+                    "gt",
+                    "Goodness of fit",
+                    onclick='window.location.href = "/basics/goodness/";',
+                ),
+                ui.input_action_link(
+                    "ct",
+                    "Cross-tabs",
+                    onclick='window.location.href = "/basics/cross-tabs/";',
+                ),
+            ),
+        ),
+        ui.nav_menu(
+            "Models",
+            ui.nav_control(
+                ui.input_action_link(
+                    "reg",
+                    "Linear Regression (OLS)",
+                    onclick='window.location.href = "/models/regress/";',
+                ),
+                ui.input_action_link(
+                    "lr",
+                    "Logistic Regression (GLM)",
+                    onclick='window.location.href = "/models/logistic/";',
+                ),
+            ),
+        ),
+    )
+
+
 def ui_stop():
     return (
         ui.nav_control(
             ui.input_action_link(
                 "screenshot",
                 "Screenshot",
                 icon=icon_svg("camera"),
```

### Comparing `pyrsm-0.9.0/pyrsm/radiant/www/.DS_Store` & `pyrsm-0.9.1/pyrsm/radiant/www/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-nc-sa.png` & `pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-sa.png` & `pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/radiant/www/imgs/icon.png` & `pyrsm-0.9.1/pyrsm/radiant/www/imgs/icon.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/radiant/www/js/returnTextAreaBinding.js` & `pyrsm-0.9.1/pyrsm/radiant/www/js/returnTextAreaBinding.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/radiant/www/js/screenshot.js` & `pyrsm-0.9.1/pyrsm/radiant/www/js/screenshot.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/regress.py` & `pyrsm-0.9.1/pyrsm/regress.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         df = self.coef.copy()
         df["coefficient"] = df["coefficient"].round(2)
         df["std.error"] = df["std.error"].round(dec)
         df["t.value"] = df["t.value"].round(dec)
         df["p.value"] = ifelse(
             df["p.value"] < 0.001, "< .001", df["p.value"].round(dec)
         )
+        df["index"] = df["index"].str.replace("[T.", "[", regex=False)
         df = df.set_index("index")
         df.index.name = None
         print(f"\n{df.to_string()}")
         print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
         print(f"\n{model_fit(self.fitted)}")
 
         if ci:
@@ -143,31 +144,30 @@
                 print("\nVariance inflation factors:")
                 print(f"\n{calc_vif(self.fitted).to_string()}")
 
         if test is not None and len(test) > 0:
             self.f_test(test=test, dec=dec)
 
     def predict(
-        self, data=None, cmd=None, dc=False, ci=False, conf=0.95
+        self, data=None, cmd=None, data_cmd=None, ci=False, conf=0.95
     ) -> pd.DataFrame:
         """
         Predict values for a linear regression model
         """
         if data is None:
             data = self.data
         data = data.loc[:, self.evar].copy()
-        if cmd is not None:
-            if dc:
-                for k, v in cmd.items():
-                    data[k] = v
-            else:
-                data = sim_prediction(data=data, vary=cmd)
+        if data_cmd is not None:
+            for k, v in data_cmd.items():
+                data[k] = v
+        elif cmd is not None:
+            data = sim_prediction(data=data, vary=cmd)
 
         if ci:
-            if dc:
+            if data_cmd is not None:
                 raise ValueError(
                     "Confidence intervals not available when using the Data & Command option"
                 )
             else:
                 return pd.concat(
                     [data, predict_ci(self.fitted, data, conf=conf)], axis=1
                 )
```

### Comparing `pyrsm-0.9.0/pyrsm/stats.py` & `pyrsm-0.9.1/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/utils.py` & `pyrsm-0.9.1/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm/visualize.py` & `pyrsm-0.9.1/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.9.1/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.9.0/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.9.1/pyrsm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 pyrsm/data/multivariate/toothpaste.parquet
 pyrsm/data/multivariate/toothpaste_description.md
 pyrsm/data/multivariate/tpbrands.parquet
 pyrsm/data/multivariate/tpbrands_description.md
 pyrsm/radiant/__init__.py
 pyrsm/radiant/compare_means.py
 pyrsm/radiant/cross_tabs.py
+pyrsm/radiant/data_view.py
 pyrsm/radiant/goodness.py
 pyrsm/radiant/logistic.py
 pyrsm/radiant/model_utils.py
 pyrsm/radiant/probability_calculator.py
 pyrsm/radiant/regress.py
 pyrsm/radiant/single_mean.py
 pyrsm/radiant/utils.py
```

### Comparing `pyrsm-0.9.0/setup.cfg` & `pyrsm-0.9.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 	Bug Reports=https://github.com/vnijs/pyrsm/issues
 	Source=https://github.com/vnijs/pyrsm
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
-	shiny>=0.3.3
+	shiny>=0.4.0
+	shinyswatch>=0.2.4
 	faicons>=0.2.1
 	numpy>=1.17.3
-	pandas>=0.25.2
-	polars>=0.17.14
+	pandas>=2.0.3
+	polars>=0.18.7
+	duckdb>=0.8.1
 	ipykernel>=6.23.1
 	seaborn>=0.9.0
 	matplotlib>=3.1.1
 	statsmodels>=0.10.1
 	scipy>=1.4.1
 	scikit-learn>=1.0.2
 	IPython>=8.0.1
```

### Comparing `pyrsm-0.9.0/tests/test_basics.py` & `pyrsm-0.9.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/tests/test_bins.py` & `pyrsm-0.9.1/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/tests/test_example_data.py` & `pyrsm-0.9.1/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/tests/test_perf.py` & `pyrsm-0.9.1/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/tests/test_regression.py` & `pyrsm-0.9.1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/tests/test_stats.py` & `pyrsm-0.9.1/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.0/tests/test_utils.py` & `pyrsm-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

