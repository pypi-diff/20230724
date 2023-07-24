# Comparing `tmp/idessem-0.0.8.tar.gz` & `tmp/idessem-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idessem-0.0.8.tar", last modified: Tue Jul 18 21:09:10 2023, max compression
+gzip compressed data, was "idessem-0.0.9.tar", last modified: Mon Jul 24 14:36:29 2023, max compression
```

## Comparing `idessem-0.0.8.tar` & `idessem-0.0.9.tar`

### file list

```diff
@@ -1,113 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.458173 idessem-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 21:06:13.000000 idessem-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-18 21:09:10.458173 idessem-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-18 21:06:13.000000 idessem-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.438173 idessem-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.438173 idessem-0.0.8/idessem/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.442173 idessem-0.0.8/idessem/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_estatfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)    71544 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/log_matriz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/arquivos/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/avl_fpha1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/dataestudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/versaomodelo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/componentes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/componentes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/componentes/stagedatefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)   159757 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.438173 idessem-0.0.8/idessem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:09:10.458173 idessem-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-18 21:06:13.000000 idessem-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.454173 idessem-0.0.8/tests/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.454173 idessem-0.0.8/tests/dessem/componentes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/componentes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/componentes/test_stagedatefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)    29439 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_renovaveis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.454173 idessem-0.0.8/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.458173 idessem-0.0.8/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)   348001 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.769365 idessem-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 14:34:24.000000 idessem-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-24 14:36:29.769365 idessem-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-24 14:34:24.000000 idessem-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.753365 idessem-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.753365 idessem-0.0.9/idessem/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.757365 idessem-0.0.9/idessem/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71544 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/log_matriz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.761365 idessem-0.0.9/idessem/dessem/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.761365 idessem-0.0.9/idessem/dessem/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/arquivos/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/avl_fpha1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.761365 idessem-0.0.9/idessem/dessem/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/blocos/dataestudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/blocos/versaomodelo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.761365 idessem-0.0.9/idessem/dessem/modelos/componentes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/componentes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/componentes/stagedatefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159757 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/modelos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/dessem/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/idessem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.757365 idessem-0.0.9/idessem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-24 14:36:29.000000 idessem-0.0.9/idessem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-24 14:36:29.000000 idessem-0.0.9/idessem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:36:29.000000 idessem-0.0.9/idessem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 14:36:29.000000 idessem-0.0.9/idessem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 14:36:29.000000 idessem-0.0.9/idessem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:36:29.769365 idessem-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-24 14:34:24.000000 idessem-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.761365 idessem-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.765365 idessem-0.0.9/tests/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.765365 idessem-0.0.9/tests/dessem/componentes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/componentes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/componentes/test_stagedatefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29439 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/dessem/test_renovaveis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.765365 idessem-0.0.9/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:36:29.769365 idessem-0.0.9/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)   348001 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/arquivos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-24 14:34:24.000000 idessem-0.0.9/tests/mocks/mock_open.py
```

### Comparing `idessem-0.0.8/LICENSE.md` & `idessem-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/PKG-INFO` & `idessem-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.8/README.md` & `idessem-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/avl_altqueda.py` & `idessem-0.0.9/idessem/dessem/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/avl_desvfpha.py` & `idessem-0.0.9/idessem/dessem/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/avl_fpha1.py` & `idessem-0.0.9/idessem/dessem/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/des_log_relato.py` & `idessem-0.0.9/idessem/dessem/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/dessemarq.py` & `idessem-0.0.9/idessem/dessem/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/entdados.py` & `idessem-0.0.9/idessem/dessem/entdados.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/hidr.py` & `idessem-0.0.9/idessem/dessem/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/log_matriz.py` & `idessem-0.0.9/idessem/dessem/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/arquivos/arquivocsv.py` & `idessem-0.0.9/idessem/dessem/modelos/arquivos/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/avl_altqueda.py` & `idessem-0.0.9/idessem/dessem/modelos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/avl_desvfpha.py` & `idessem-0.0.9/idessem/dessem/modelos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/avl_fpha1.py` & `idessem-0.0.9/idessem/dessem/modelos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/blocos/dataestudo.py` & `idessem-0.0.9/idessem/dessem/modelos/blocos/dataestudo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/blocos/tabelacsv.py` & `idessem-0.0.9/idessem/dessem/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/blocos/versaomodelo.py` & `idessem-0.0.9/idessem/dessem/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/componentes/stagedatefield.py` & `idessem-0.0.9/idessem/dessem/modelos/componentes/stagedatefield.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/des_log_relato.py` & `idessem-0.0.9/idessem/dessem/modelos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/dessemarq.py` & `idessem-0.0.9/idessem/dessem/modelos/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/entdados.py` & `idessem-0.0.9/idessem/dessem/modelos/entdados.py`

 * *Files 0% similar despite different names*

```diff
@@ -1067,15 +1067,15 @@
 
     """
 
     IDENTIFIER = "DP  "
     IDENTIFIER_DIGITS = 4
     LINE = Line(
         [
-            IntegerField(2, 4),
+            IntegerField(3, 4),
             StageDateField(starting_position=8, special_day_character="I"),
             StageDateField(starting_position=16, special_day_character="F"),
             FloatField(10, 24, 1),
         ]
     )
 
     @property
@@ -1345,15 +1345,15 @@
 
     """
 
     IDENTIFIER = "CD "
     IDENTIFIER_DIGITS = 3
     LINE = Line(
         [
-            IntegerField(2, 4),
+            IntegerField(2, 3),
             IntegerField(2, 6),
             StageDateField(starting_position=9, special_day_character="I"),
             StageDateField(starting_position=17, special_day_character="F"),
             FloatField(10, 25, 2),
             FloatField(10, 35, 2),
         ]
     )
```

### Comparing `idessem-0.0.8/idessem/dessem/modelos/hidr.py` & `idessem-0.0.9/idessem/dessem/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/log_matriz.py` & `idessem-0.0.9/idessem/dessem/modelos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/operut.py` & `idessem-0.0.9/idessem/dessem/modelos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/pdo_eco_fcfcortes.py` & `idessem-0.0.9/idessem/dessem/modelos/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih.py` & `idessem-0.0.9/idessem/dessem/modelos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih_polin.py` & `idessem-0.0.9/idessem/dessem/modelos/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/pdo_hidr.py` & `idessem-0.0.9/idessem/dessem/modelos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/pdo_oper_uct.py` & `idessem-0.0.9/idessem/dessem/modelos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/pdo_sist.py` & `idessem-0.0.9/idessem/dessem/modelos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/polinjus.py` & `idessem-0.0.9/idessem/dessem/modelos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/modelos/renovaveis.py` & `idessem-0.0.9/idessem/dessem/modelos/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/operut.py` & `idessem-0.0.9/idessem/dessem/operut.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,31 @@
     Armazena os dados de entrada do DESSEM referentes às
     configurações da operação das usinas térmelétricas.
 
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [BlocoUctPar, BlocoUcTerm, BlocoPint, BlocoInitUT, BlocoOper]
+    BLOCKS = [
+        BlocoUctPar,
+        BlocoUcTerm,
+        BlocoPint,
+        BlocoRegraNPTV,
+        BlocoAvlCmo,
+        BlocoCplexLog,
+        BlocoUctBusLoc,
+        BlocoUctHeurFp,
+        BlocoConstDados,
+        BlocoAjusteFcf,
+        BlocoTolerIlh,
+        BlocoCrossover,
+        BlocoEngolimento,
+        BlocoInitUT,
+        BlocoOper,
+    ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="operut.dat") -> "Operut":
         msg = (
```

### Comparing `idessem-0.0.8/idessem/dessem/pdo_eco_fcfcortes.py` & `idessem-0.0.9/idessem/dessem/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/pdo_eco_usih.py` & `idessem-0.0.9/idessem/dessem/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/pdo_eco_usih_polin.py` & `idessem-0.0.9/idessem/dessem/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/pdo_hidr.py` & `idessem-0.0.9/idessem/dessem/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/pdo_oper_uct.py` & `idessem-0.0.9/idessem/dessem/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/pdo_sist.py` & `idessem-0.0.9/idessem/dessem/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/polinjus.py` & `idessem-0.0.9/idessem/dessem/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem/dessem/renovaveis.py` & `idessem-0.0.9/idessem/dessem/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/idessem.egg-info/PKG-INFO` & `idessem-0.0.9/idessem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.8/idessem.egg-info/SOURCES.txt` & `idessem-0.0.9/idessem.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 idessem/dessem/pdo_oper_uct.py
 idessem/dessem/pdo_sist.py
 idessem/dessem/polinjus.py
 idessem/dessem/renovaveis.py
 idessem/dessem/modelos/__init__.py
 idessem/dessem/modelos/avl_altqueda.py
 idessem/dessem/modelos/avl_desvfpha.py
+idessem/dessem/modelos/avl_estatfpha.py
 idessem/dessem/modelos/avl_fpha1.py
 idessem/dessem/modelos/des_log_relato.py
 idessem/dessem/modelos/dessemarq.py
 idessem/dessem/modelos/entdados.py
 idessem/dessem/modelos/hidr.py
 idessem/dessem/modelos/log_matriz.py
 idessem/dessem/modelos/operut.py
@@ -55,14 +56,15 @@
 idessem/dessem/modelos/blocos/versaomodelo.py
 idessem/dessem/modelos/componentes/__init__.py
 idessem/dessem/modelos/componentes/stagedatefield.py
 tests/__init__.py
 tests/dessem/__init__.py
 tests/dessem/test_avl_altqueda.py
 tests/dessem/test_avl_desvfpha.py
+tests/dessem/test_avl_estatfpha.py
 tests/dessem/test_avl_fpha1.py
 tests/dessem/test_des_log_relato.py
 tests/dessem/test_dessemarq.py
 tests/dessem/test_entdados.py
 tests/dessem/test_hidr.py
 tests/dessem/test_log_matriz.py
 tests/dessem/test_operut.py
@@ -77,14 +79,15 @@
 tests/dessem/componentes/__init__.py
 tests/dessem/componentes/test_stagedatefield.py
 tests/mocks/__init__.py
 tests/mocks/mock_open.py
 tests/mocks/arquivos/__init__.py
 tests/mocks/arquivos/avl_altqueda.py
 tests/mocks/arquivos/avl_desvfpha.py
+tests/mocks/arquivos/avl_estatfpha.py
 tests/mocks/arquivos/avl_fpha1.py
 tests/mocks/arquivos/des_log_relato.py
 tests/mocks/arquivos/dessemarq.py
 tests/mocks/arquivos/entdados.py
 tests/mocks/arquivos/log_matriz.py
 tests/mocks/arquivos/operut.py
 tests/mocks/arquivos/pdo_eco_fcfcortes.py
```

### Comparing `idessem-0.0.8/setup.py` & `idessem-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/componentes/test_stagedatefield.py` & `idessem-0.0.9/tests/dessem/componentes/test_stagedatefield.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_avl_altqueda.py` & `idessem-0.0.9/tests/dessem/test_avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_avl_desvfpha.py` & `idessem-0.0.9/tests/dessem/test_avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_avl_fpha1.py` & `idessem-0.0.9/tests/dessem/test_avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_des_log_relato.py` & `idessem-0.0.9/tests/dessem/test_des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_dessemarq.py` & `idessem-0.0.9/tests/dessem/test_dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_entdados.py` & `idessem-0.0.9/tests/dessem/test_entdados.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_hidr.py` & `idessem-0.0.9/tests/dessem/test_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_log_matriz.py` & `idessem-0.0.9/tests/dessem/test_log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_operut.py` & `idessem-0.0.9/tests/dessem/test_operut.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,50 @@
 
 def test_atributos_encontrados_operut():
     m: MagicMock = mock_open(read_data="".join(MockOperut))
     with patch("builtins.open", m):
         op = Operut.read(ARQ_TESTE)
         assert op.condicoes_iniciais is not None
         assert op.limites_e_condicoes_operativas is not None
+        assert op.uctpar is not None
+        assert op.ucterm is not None
+        assert op.pint is not None
+        assert op.regranptv is not None
+        assert op.avlcmo is not None
+        assert op.cplexlog is not None
+        assert op.uctbusloc is None
+        assert op.uctheurfp is None
+        assert op.constdados is None
+        assert op.ajustefcf is None
+        assert op.tolerilh is None
+        assert op.crossover is None
+        assert op.engolimento is None
+        assert op.tratainviabilha is None
 
 
 def test_atributos_nao_encontrados_operut():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         op = Operut.read(ARQ_TESTE)
         assert op.condicoes_iniciais is None
         assert op.limites_e_condicoes_operativas is None
+        assert op.uctpar is None
+        assert op.ucterm is None
+        assert op.pint is None
+        assert op.regranptv is None
+        assert op.avlcmo is None
+        assert op.cplexlog is None
+        assert op.uctbusloc is None
+        assert op.uctheurfp is None
+        assert op.constdados is None
+        assert op.ajustefcf is None
+        assert op.tolerilh is None
+        assert op.crossover is None
+        assert op.engolimento is None
+        assert op.tratainviabilha is None
 
 
 # Bloco INIT
 def test_eq_blocoinit():
     m: MagicMock = mock_open(read_data="".join(MockBlocoInit))
     b1 = BlocoInitUT()
     with patch("builtins.open", m):
```

### Comparing `idessem-0.0.8/tests/dessem/test_pdo_eco_fcfcortes.py` & `idessem-0.0.9/tests/dessem/test_pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_pdo_eco_usih.py` & `idessem-0.0.9/tests/dessem/test_pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_pdo_eco_usih_polin.py` & `idessem-0.0.9/tests/dessem/test_pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_pdo_hidr.py` & `idessem-0.0.9/tests/dessem/test_pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_pdo_oper_uct.py` & `idessem-0.0.9/tests/dessem/test_pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_pdo_sist.py` & `idessem-0.0.9/tests/dessem/test_pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_polinjus.py` & `idessem-0.0.9/tests/dessem/test_polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/dessem/test_renovaveis.py` & `idessem-0.0.9/tests/dessem/test_renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/avl_altqueda.py` & `idessem-0.0.9/tests/mocks/arquivos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/avl_desvfpha.py` & `idessem-0.0.9/tests/mocks/arquivos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/avl_fpha1.py` & `idessem-0.0.9/tests/mocks/arquivos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/des_log_relato.py` & `idessem-0.0.9/tests/mocks/arquivos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/dessemarq.py` & `idessem-0.0.9/tests/mocks/arquivos/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/entdados.py` & `idessem-0.0.9/tests/mocks/arquivos/entdados.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/log_matriz.py` & `idessem-0.0.9/tests/mocks/arquivos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/operut.py` & `idessem-0.0.9/tests/mocks/arquivos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/pdo_eco_fcfcortes.py` & `idessem-0.0.9/tests/mocks/arquivos/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih.py` & `idessem-0.0.9/tests/mocks/arquivos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih_polin.py` & `idessem-0.0.9/tests/mocks/arquivos/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/pdo_hidr.py` & `idessem-0.0.9/tests/mocks/arquivos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/pdo_oper_uct.py` & `idessem-0.0.9/tests/mocks/arquivos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/pdo_sist.py` & `idessem-0.0.9/tests/mocks/arquivos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/polinjus.py` & `idessem-0.0.9/tests/mocks/arquivos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/arquivos/renovaveis.py` & `idessem-0.0.9/tests/mocks/arquivos/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.8/tests/mocks/mock_open.py` & `idessem-0.0.9/tests/mocks/mock_open.py`

 * *Files identical despite different names*

