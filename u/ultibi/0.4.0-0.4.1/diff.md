# Comparing `tmp/ultibi-0.4.0.tar.gz` & `tmp/ultibi-0.4.1.tar.gz`

## Comparing `ultibi-0.4.0.tar` & `ultibi-0.4.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/ultibi/Cargo.toml
--rw-r--r--   0     1001      123        0 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi/README.md
--rw-r--r--   0     1001      123       98 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi/src/lib.rs
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/frtb_engine/Cargo.toml
--rw-r--r--   0     1001      123      481 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/README.md
--rw-r--r--   0     1001      123    14931 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/Delta.csv
--rw-r--r--   0     1001      123      541 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
--rw-r--r--   0     1001      123     2160 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
--rw-r--r--   0     1001      123      159 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/hms.csv
--rw-r--r--   0     1001      123      177 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
--rw-r--r--   0     1001      123    20066 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/calc_params.rs
--rw-r--r--   0     1001      123       25 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/docs/mod.rs
--rw-r--r--   0     1001      123     1226 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/docs/optional_params.rs
--rw-r--r--   0     1001      123     1424 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/common.rs
--rw-r--r--   0     1001      123    11847 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
--rw-r--r--   0     1001      123     9484 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
--rw-r--r--   0     1001      123     7614 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs
--rw-r--r--   0     1001      123       96 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/mod.rs
--rw-r--r--   0     1001      123      787 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/totals.rs
--rw-r--r--   0     1001      123     4811 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/helpers.rs
--rw-r--r--   0     1001      123    10170 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/lib.rs
--rw-r--r--   0     1001      123     4151 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/measures.rs
--rw-r--r--   0     1001      123      188 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/prelude.rs
--rw-r--r--   0     1001      123       40 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/reports/mod.rs
--rw-r--r--   0     1001      123      349 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/reports/sbm/equity.rs
--rw-r--r--   0     1001      123       12 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/reports/sbm/mod.rs
--rw-r--r--   0     1001      123    26569 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights.rs
--rw-r--r--   0     1001      123     5421 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
--rw-r--r--   0     1001      123     5268 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/rrao/mod.rs
--rw-r--r--   0     1001      123     1374 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/buckets.rs
--rw-r--r--   0     1001      123    14537 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
--rw-r--r--   0     1001      123    13888 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
--rw-r--r--   0     1001      123     3704 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
--rw-r--r--   0     1001      123     7443 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
--rw-r--r--   0     1001      123    30238 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common.rs
--rw-r--r--   0     1001      123     9869 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs
--rw-r--r--   0     1001      123    19328 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
--rw-r--r--   0     1001      123    17723 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
--rw-r--r--   0     1001      123     3846 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
--rw-r--r--   0     1001      123    11817 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
--rw-r--r--   0     1001      123    15622 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
--rw-r--r--   0     1001      123    12479 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
--rw-r--r--   0     1001      123     2904 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
--rw-r--r--   0     1001      123     8796 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
--rw-r--r--   0     1001      123    15266 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
--rw-r--r--   0     1001      123    13490 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
--rw-r--r--   0     1001      123     2988 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
--rw-r--r--   0     1001      123     8074 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
--rw-r--r--   0     1001      123    17062 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
--rw-r--r--   0     1001      123    10966 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
--rw-r--r--   0     1001      123     2162 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
--rw-r--r--   0     1001      123    10440 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
--rw-r--r--   0     1001      123    14299 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
--rw-r--r--   0     1001      123    12036 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
--rw-r--r--   0     1001      123     2162 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
--rw-r--r--   0     1001      123    10230 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
--rw-r--r--   0     1001      123    14040 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
--rw-r--r--   0     1001      123    21914 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
--rw-r--r--   0     1001      123     2295 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
--rw-r--r--   0     1001      123    15734 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
--rw-r--r--   0     1001      123      221 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/mod.rs
--rw-r--r--   0     1001      123     5180 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/totals.rs
--rw-r--r--   0     1001      123    28643 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/statics.rs
--rw-r--r--   0     1001      123      753 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/totals.rs
--rw-r--r--   0     1001      123     1846 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/validate.rs
--rw-r--r--   0     1001      123     1832 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/common/mod.rs
--rw-r--r--   0     1001      123     1520 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/dependant.rs
--rw-r--r--   0     1001      123     4453 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/drc.rs
--rw-r--r--   0     1001      123      420 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/rrao.rs
--rw-r--r--   0     1001      123    18951 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm.rs
--rw-r--r--   0     1001      123      710 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm_totals.rs
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/ultibi_server/Cargo.toml
--rw-r--r--   0     1001      123      219 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/build.rs
--rw-r--r--   0     1001      123       35 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/api/mod.rs
--rw-r--r--   0     1001      123      754 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/api/open_api.rs
--rw-r--r--   0     1001      123     6456 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/api/routers.rs
--rw-r--r--   0     1001      123     1243 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/app.rs
--rw-r--r--   0     1001      123     2593 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/helpers.rs
--rw-r--r--   0     1001      123     1418 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/lib.rs
--rw-r--r--   0     1001      123      358 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/visual.rs
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/ultibi_core/Cargo.toml
--rw-r--r--   0     1001      123     2031 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/add_row.rs
--rw-r--r--   0     1001      123     3486 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/aggregations.rs
--rw-r--r--   0     1001      123      654 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/cache.rs
--rw-r--r--   0     1001      123     4782 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/datarequest.rs
--rw-r--r--   0     1001      123     2903 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/datasource.rs
--rw-r--r--   0     1001      123    10820 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/mod.rs
--rw-r--r--   0     1001      123     2156 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/new.rs
--rw-r--r--   0     1001      123      700 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/errors.rs
--rw-r--r--   0     1001      123    10937 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs
--rw-r--r--   0     1001      123     4628 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
--rw-r--r--   0     1001      123      478 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/mod.rs
--rw-r--r--   0     1001      123     2663 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/filters.rs
--rw-r--r--   0     1001      123       18 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/helpers/mod.rs
--rw-r--r--   0     1001      123      588 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/helpers/searches.rs
--rw-r--r--   0     1001      123     1413 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/acquire.rs
--rw-r--r--   0     1001      123     2059 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/awss3.rs
--rw-r--r--   0     1001      123     6085 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/helpers.rs
--rw-r--r--   0     1001      123     6863 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/mod.rs
--rw-r--r--   0     1001      123      371 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/lib.rs
--rw-r--r--   0     1001      123    11951 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/measure.rs
--rw-r--r--   0     1001      123     3362 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/overrides.rs
--rw-r--r--   0     1001      123      222 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/prelude.rs
--rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/reports/mod.rs
--rw-r--r--   0     1001      123     3332 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/reports/report.rs
--rw-r--r--   0     1001      123     1870 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/add_row.rs
--rw-r--r--   0     1001      123      734 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/agg_request.rs
--rw-r--r--   0     1001      123     1441 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/aggregations.rs
--rw-r--r--   0     1001      123        1 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/cache.rs
--rw-r--r--   0     1001      123     2210 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/common/mod.rs
--rw-r--r--   0     1001      123       95 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/bad_config.toml
--rw-r--r--   0     1001      123      553 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml
--rw-r--r--   0     1001      123      116 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/test_config.toml
--rw-r--r--   0     1001      123      354 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/testset.csv
--rw-r--r--   0     1001      123     1269 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/datasource.rs
--rw-r--r--   0     1001      123     3094 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/dependants.rs
--rw-r--r--   0     1001      123     1417 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/filters.rs
--rw-r--r--   0     1001      123     1056 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/overrides.rs
--rw-r--r--   0     1001      123     1144 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/source.rs
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.4.0/Cargo.toml
--rw-r--r--   0     1001      123      728 2023-07-22 15:33:29.000000 ultibi-0.4.0/.gitignore
--rw-r--r--   0     1001      123     5129 2023-07-22 15:33:29.000000 ultibi-0.4.0/LICENSE
--rw-r--r--   0     1001      123     2405 2023-07-22 15:33:29.000000 ultibi-0.4.0/Makefile
--rw-r--r--   0     1001      123     7071 2023-07-22 15:33:29.000000 ultibi-0.4.0/README.md
--rw-r--r--   0     1001      123     1559 2023-07-22 15:33:29.000000 ultibi-0.4.0/example.py
--rw-r--r--   0     1001      123     2098 2023-07-22 15:33:29.000000 ultibi-0.4.0/pyproject.toml
--rw-r--r--   0     1001      123       36 2023-07-22 15:33:29.000000 ultibi-0.4.0/requirements-lint.txt
--rw-r--r--   0     1001      123      307 2023-07-22 15:33:29.000000 ultibi-0.4.0/requirements.txt
--rw-r--r--   0     1001      123     3922 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/calculator.rs
--rw-r--r--   0     1001      123       48 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/conversions/mod.rs
--rw-r--r--   0     1001      123     3570 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/conversions/series.rs
--rw-r--r--   0     1001      123     3049 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/conversions/wrappers.rs
--rw-r--r--   0     1001      123     9008 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/dataset.rs
--rw-r--r--   0     1001      123     1786 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/datasource.rs
--rw-r--r--   0     1001      123     3833 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/errors.rs
--rw-r--r--   0     1001      123      693 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/filter.rs
--rw-r--r--   0     1001      123     2170 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/lib.rs
--rw-r--r--   0     1001      123     2521 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/measure.rs
--rw-r--r--   0     1001      123     1353 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/requests.rs
--rw-r--r--   0     1001      123     1762 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/data/datasource_config.toml
--rw-r--r--   0     1001      123     4042 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/docs/run_doc_examples.py
--rw-r--r--   0     1001      123     1613 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_compute.py
--rw-r--r--   0     1001      123     1692 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_ds.py
--rw-r--r--   0     1001      123      826 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_filters.py
--rw-r--r--   0     1001      123     2658 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_measure.py
--rw-r--r--   0     1001      123      878 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_source.py
--rw-r--r--   0     1001      123      918 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/__init__.py
--rw-r--r--   0     1001      123     1145 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/__init__.py
--rw-r--r--   0     1001      123     7999 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/dataset.py
--rw-r--r--   0     1001      123     2749 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/datasource.py
--rw-r--r--   0     1001      123     3257 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/filters.py
--rw-r--r--   0     1001      123     8407 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/measure.py
--rw-r--r--   0     1001      123     2950 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/requests.py
--rw-r--r--   0     1001      123        0 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/rust_module/__init__.py
--rw-r--r--   0        0        0   121894 2023-07-22 15:35:01.000000 ultibi-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     7979 1970-01-01 00:00:00.000000 ultibi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/ultibi_server/Cargo.toml
+-rw-r--r--   0     1001      123      219 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/build.rs
+-rw-r--r--   0     1001      123       35 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/api/mod.rs
+-rw-r--r--   0     1001      123      754 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/api/open_api.rs
+-rw-r--r--   0     1001      123     6456 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/api/routers.rs
+-rw-r--r--   0     1001      123     1243 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/app.rs
+-rw-r--r--   0     1001      123     2593 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/helpers.rs
+-rw-r--r--   0     1001      123     1418 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/lib.rs
+-rw-r--r--   0     1001      123      358 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_server/src/visual.rs
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/frtb_engine/Cargo.toml
+-rw-r--r--   0     1001      123      481 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/README.md
+-rw-r--r--   0     1001      123    14931 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/Delta.csv
+-rw-r--r--   0     1001      123      541 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
+-rw-r--r--   0     1001      123     2292 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
+-rw-r--r--   0     1001      123      159 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/hms.csv
+-rw-r--r--   0     1001      123      177 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
+-rw-r--r--   0     1001      123    20066 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/calc_params.rs
+-rw-r--r--   0     1001      123       25 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/docs/mod.rs
+-rw-r--r--   0     1001      123     1226 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/docs/optional_params.rs
+-rw-r--r--   0     1001      123     1424 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/common.rs
+-rw-r--r--   0     1001      123    11847 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
+-rw-r--r--   0     1001      123     9484 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
+-rw-r--r--   0     1001      123     7614 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_weights.rs
+-rw-r--r--   0     1001      123       96 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/mod.rs
+-rw-r--r--   0     1001      123      787 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/totals.rs
+-rw-r--r--   0     1001      123     4811 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/helpers.rs
+-rw-r--r--   0     1001      123    10170 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/lib.rs
+-rw-r--r--   0     1001      123     4151 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/measures.rs
+-rw-r--r--   0     1001      123      188 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/prelude.rs
+-rw-r--r--   0     1001      123       40 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/reports/mod.rs
+-rw-r--r--   0     1001      123      349 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/reports/sbm/equity.rs
+-rw-r--r--   0     1001      123       12 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/reports/sbm/mod.rs
+-rw-r--r--   0     1001      123    26569 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights.rs
+-rw-r--r--   0     1001      123     5421 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
+-rw-r--r--   0     1001      123     5268 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/rrao/mod.rs
+-rw-r--r--   0     1001      123     1374 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/buckets.rs
+-rw-r--r--   0     1001      123    14537 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
+-rw-r--r--   0     1001      123    13888 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
+-rw-r--r--   0     1001      123     3704 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
+-rw-r--r--   0     1001      123     7443 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
+-rw-r--r--   0     1001      123    30238 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common.rs
+-rw-r--r--   0     1001      123     9869 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common_curv.rs
+-rw-r--r--   0     1001      123    19328 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
+-rw-r--r--   0     1001      123    17723 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
+-rw-r--r--   0     1001      123     3846 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
+-rw-r--r--   0     1001      123    11817 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
+-rw-r--r--   0     1001      123    15622 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
+-rw-r--r--   0     1001      123    12479 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
+-rw-r--r--   0     1001      123     2904 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
+-rw-r--r--   0     1001      123     8796 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
+-rw-r--r--   0     1001      123    15266 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
+-rw-r--r--   0     1001      123    13490 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
+-rw-r--r--   0     1001      123     2988 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
+-rw-r--r--   0     1001      123     8074 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
+-rw-r--r--   0     1001      123    17062 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
+-rw-r--r--   0     1001      123    10966 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
+-rw-r--r--   0     1001      123    10440 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
+-rw-r--r--   0     1001      123    14299 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
+-rw-r--r--   0     1001      123    12009 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
+-rw-r--r--   0     1001      123    10230 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
+-rw-r--r--   0     1001      123    14040 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
+-rw-r--r--   0     1001      123    21914 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
+-rw-r--r--   0     1001      123     2295 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
+-rw-r--r--   0     1001      123    15734 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
+-rw-r--r--   0     1001      123      221 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/mod.rs
+-rw-r--r--   0     1001      123     5180 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/totals.rs
+-rw-r--r--   0     1001      123    28643 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/statics.rs
+-rw-r--r--   0     1001      123      753 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/totals.rs
+-rw-r--r--   0     1001      123     1846 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/src/validate.rs
+-rw-r--r--   0     1001      123     1832 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/common/mod.rs
+-rw-r--r--   0     1001      123     1520 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/dependant.rs
+-rw-r--r--   0     1001      123     4453 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/drc.rs
+-rw-r--r--   0     1001      123      420 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/rrao.rs
+-rw-r--r--   0     1001      123    18951 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm.rs
+-rw-r--r--   0     1001      123      710 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm_totals.rs
+-rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/ultibi_core/Cargo.toml
+-rw-r--r--   0     1001      123     2031 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/add_row.rs
+-rw-r--r--   0     1001      123     3486 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/aggregations.rs
+-rw-r--r--   0     1001      123      654 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/cache.rs
+-rw-r--r--   0     1001      123     4782 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/datarequest.rs
+-rw-r--r--   0     1001      123     2903 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/datasource.rs
+-rw-r--r--   0     1001      123    10820 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/mod.rs
+-rw-r--r--   0     1001      123     2156 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/new.rs
+-rw-r--r--   0     1001      123      700 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/errors.rs
+-rw-r--r--   0     1001      123    10937 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg.rs
+-rw-r--r--   0     1001      123     4628 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
+-rw-r--r--   0     1001      123      478 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/mod.rs
+-rw-r--r--   0     1001      123     2663 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/filters.rs
+-rw-r--r--   0     1001      123       18 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/helpers/mod.rs
+-rw-r--r--   0     1001      123      588 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/helpers/searches.rs
+-rw-r--r--   0     1001      123     1413 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/acquire.rs
+-rw-r--r--   0     1001      123     2059 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/awss3.rs
+-rw-r--r--   0     1001      123     6085 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/helpers.rs
+-rw-r--r--   0     1001      123     6863 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/io/mod.rs
+-rw-r--r--   0     1001      123      371 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/lib.rs
+-rw-r--r--   0     1001      123    11951 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/measure.rs
+-rw-r--r--   0     1001      123     3362 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/overrides.rs
+-rw-r--r--   0     1001      123      222 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/prelude.rs
+-rw-r--r--   0     1001      123       64 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/reports/mod.rs
+-rw-r--r--   0     1001      123     3332 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/src/reports/report.rs
+-rw-r--r--   0     1001      123     1870 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/add_row.rs
+-rw-r--r--   0     1001      123      734 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/agg_request.rs
+-rw-r--r--   0     1001      123     1441 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/aggregations.rs
+-rw-r--r--   0     1001      123        1 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/cache.rs
+-rw-r--r--   0     1001      123     2210 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/common/mod.rs
+-rw-r--r--   0     1001      123       95 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/bad_config.toml
+-rw-r--r--   0     1001      123      553 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/bad_config2.toml
+-rw-r--r--   0     1001      123      116 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/test_config.toml
+-rw-r--r--   0     1001      123      354 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/testset.csv
+-rw-r--r--   0     1001      123     1269 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/datasource.rs
+-rw-r--r--   0     1001      123     3094 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/dependants.rs
+-rw-r--r--   0     1001      123     1417 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/filters.rs
+-rw-r--r--   0     1001      123     1056 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/overrides.rs
+-rw-r--r--   0     1001      123     1144 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi_core/tests/source.rs
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 ultibi-0.4.1/local_dependencies/ultibi/Cargo.toml
+-rw-r--r--   0     1001      123        0 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi/README.md
+-rw-r--r--   0     1001      123       98 2023-07-24 19:30:20.000000 ultibi-0.4.1/local_dependencies/ultibi/src/lib.rs
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.4.1/Cargo.toml
+-rw-r--r--   0     1001      123      728 2023-07-24 19:30:20.000000 ultibi-0.4.1/.gitignore
+-rw-r--r--   0     1001      123     5129 2023-07-24 19:30:20.000000 ultibi-0.4.1/LICENSE
+-rw-r--r--   0     1001      123     2405 2023-07-24 19:30:20.000000 ultibi-0.4.1/Makefile
+-rw-r--r--   0     1001      123     7071 2023-07-24 19:30:20.000000 ultibi-0.4.1/README.md
+-rw-r--r--   0     1001      123     1559 2023-07-24 19:30:20.000000 ultibi-0.4.1/example.py
+-rw-r--r--   0     1001      123     2098 2023-07-24 19:30:20.000000 ultibi-0.4.1/pyproject.toml
+-rw-r--r--   0     1001      123       36 2023-07-24 19:30:20.000000 ultibi-0.4.1/requirements-lint.txt
+-rw-r--r--   0     1001      123      307 2023-07-24 19:30:20.000000 ultibi-0.4.1/requirements.txt
+-rw-r--r--   0     1001      123     3922 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/calculator.rs
+-rw-r--r--   0     1001      123       48 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/conversions/mod.rs
+-rw-r--r--   0     1001      123     3570 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/conversions/series.rs
+-rw-r--r--   0     1001      123     3049 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/conversions/wrappers.rs
+-rw-r--r--   0     1001      123     9008 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/dataset.rs
+-rw-r--r--   0     1001      123     1786 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/datasource.rs
+-rw-r--r--   0     1001      123     3833 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/errors.rs
+-rw-r--r--   0     1001      123      693 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/filter.rs
+-rw-r--r--   0     1001      123     2170 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/lib.rs
+-rw-r--r--   0     1001      123     2521 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/measure.rs
+-rw-r--r--   0     1001      123     1353 2023-07-24 19:30:20.000000 ultibi-0.4.1/src/requests.rs
+-rw-r--r--   0     1001      123     1762 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/data/datasource_config.toml
+-rw-r--r--   0     1001      123     4042 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/docs/run_doc_examples.py
+-rw-r--r--   0     1001      123     1613 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_compute.py
+-rw-r--r--   0     1001      123     1692 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_ds.py
+-rw-r--r--   0     1001      123      826 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_filters.py
+-rw-r--r--   0     1001      123     2658 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_measure.py
+-rw-r--r--   0     1001      123      878 2023-07-24 19:30:20.000000 ultibi-0.4.1/tests/unit/test_source.py
+-rw-r--r--   0     1001      123      918 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/__init__.py
+-rw-r--r--   0     1001      123     1145 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/__init__.py
+-rw-r--r--   0     1001      123     7999 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/dataset.py
+-rw-r--r--   0     1001      123     2730 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/datasource.py
+-rw-r--r--   0     1001      123     3257 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/filters.py
+-rw-r--r--   0     1001      123     8407 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/measure.py
+-rw-r--r--   0     1001      123     2950 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/internals/requests.py
+-rw-r--r--   0     1001      123        0 2023-07-24 19:30:20.000000 ultibi-0.4.1/ultibi/rust_module/__init__.py
+-rw-r--r--   0        0        0   121869 2023-07-24 19:31:51.000000 ultibi-0.4.1/Cargo.lock
+-rw-r--r--   0        0        0     7979 1970-01-01 00:00:00.000000 ultibi-0.4.1/PKG-INFO
```

### Comparing `ultibi-0.4.0/local_dependencies/ultibi/Cargo.toml` & `ultibi-0.4.1/local_dependencies/ultibi/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi"
-version= "0.4.0"
+version= "0.4.1"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/Cargo.toml` & `ultibi-0.4.1/local_dependencies/frtb_engine/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "frtb_engine"
-version= "0.4.0"
+version= "0.4.1"
 edition = "2021"
 publish = false
 license-file= "LICENSE"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/Delta.csv` & `ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/Delta.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv` & `ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml` & `ultibi-0.4.1/local_dependencies/frtb_engine/data/frtb/datasource_config.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 title = "setup.toml Example"
 
-#type can be either CSV or AwsCSV
+#type can be either CSV or AwsCSV 
 type = "CSV"
 
 #If using AwsCSV then provide the bucket name
 #bucket = "ultima-bi"
 
+# source_type defaults to "InMemory"
+# can be one of "InMemory", "Scan", "Db" (work in progress).
+#source_type = "InMemory"
+
 # Risk file paths, can be many, expecting at least one
-files = ["data/frtb/Delta.csv"]
+files = ["./data/frtb/Delta.csv"]
 
 # Optional: trade attributes
-attributes_path = "data/frtb/TradeAttributes.csv"
+attributes_path = "./data/frtb/TradeAttributes.csv"
 
 # Optional: Hierarchy
-hierarchy_path = "data/frtb/hms.csv"
+hierarchy_path = "./data/frtb/hms.csv"
 
 # file_1/file_2/file_3 <-> attributes
 # must be provided if attributes file is provided
 files_join_attributes = ["TradeId"]
 
 # attributes <-> hierarchy
 # must be provided if hierarchy file is provided
```

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/calc_params.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/calc_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/docs/optional_params.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/docs/optional_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/common.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/drc_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/drc/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/helpers.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/lib.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/measures.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/measures.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/risk_weights_crr2.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/rrao/mod.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/rrao/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/buckets.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/buckets.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/common_curv.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/equity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/delta.rs`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
                 return Ok(Some(Series::new("res", [0.])));
             };
 
             //21.4.4 |dw_sum| == kb for FX
             //21.4.5.a sb == dw_sum
             let dw_sum = df["dw_sum"].f64()?.to_ndarray()?; //Ok since we have filtered out NULLs above
                                                             // Early return Kb or Sb, ie the required metric
-            dbg!(&dw_sum);
             let res_len = columns[0].len();
             if let ReturnMetric::Sb = rtrn {
                 return Ok(Some(Series::new("res", [dw_sum.sum()])));
             }
 
             let kbs: Array1<f64> = dw_sum.iter().map(|x| x.abs()).collect();
             if let ReturnMetric::Kb = rtrn {
```

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/vega.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/fx/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/girr/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/sbm/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/statics.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/statics.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/src/validate.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/src/validate.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/tests/common/mod.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/tests/dependant.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/tests/dependant.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/tests/drc.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/tests/drc.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm_totals.rs` & `ultibi-0.4.1/local_dependencies/frtb_engine/tests/sbm_totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_server/Cargo.toml` & `ultibi-0.4.1/local_dependencies/ultibi_server/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_server"
-version= "0.4.0"
+version= "0.4.1"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_server/src/api/open_api.rs` & `ultibi-0.4.1/local_dependencies/ultibi_server/src/api/open_api.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_server/src/api/routers.rs` & `ultibi-0.4.1/local_dependencies/ultibi_server/src/api/routers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_server/src/app.rs` & `ultibi-0.4.1/local_dependencies/ultibi_server/src/app.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_server/src/helpers.rs` & `ultibi-0.4.1/local_dependencies/ultibi_server/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_server/src/lib.rs` & `ultibi-0.4.1/local_dependencies/ultibi_server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/Cargo.toml` & `ultibi-0.4.1/local_dependencies/ultibi_core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_core"
-version= "0.4.0"
+version= "0.4.1"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/add_row.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/aggregations.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/cache.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/datarequest.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/datarequest.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/datasource.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/mod.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/new.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/dataset/new.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/errors.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/filters.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/helpers/searches.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/helpers/searches.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/io/acquire.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/acquire.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/io/awss3.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/awss3.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/io/helpers.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/io/mod.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/io/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/measure.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/overrides.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/src/reports/report.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/src/reports/report.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/add_row.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/agg_request.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/agg_request.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/aggregations.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/common/mod.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/data/bad_config2.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/datasource.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/dependants.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/dependants.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/filters.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/overrides.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/overrides.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/local_dependencies/ultibi_core/tests/source.rs` & `ultibi-0.4.1/local_dependencies/ultibi_core/tests/source.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/Cargo.toml` & `ultibi-0.4.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyultima"
-version= "0.4.0"
+version= "0.4.1"
 edition = "2021"
 publish = false
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ultibi"
```

### Comparing `ultibi-0.4.0/.gitignore` & `ultibi-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/LICENSE` & `ultibi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/Makefile` & `ultibi-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/README.md` & `ultibi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/example.py` & `ultibi-0.4.1/example.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/pyproject.toml` & `ultibi-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/calculator.rs` & `ultibi-0.4.1/src/calculator.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/conversions/series.rs` & `ultibi-0.4.1/src/conversions/series.rs`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![allow(dead_code)]
 
-use std::collections::HashMap;
-use polars::export::arrow;
 use arrow::ffi;
+use polars::export::arrow;
 use polars::prelude::*;
+use std::collections::HashMap;
 //use polars_arrow::export::arrow;
 use pyo3::exceptions::PyValueError;
 use pyo3::ffi::Py_uintptr_t;
 use pyo3::prelude::*;
 use pyo3::types::IntoPyDict;
 use pyo3::{PyAny, PyObject, PyResult};
```

### Comparing `ultibi-0.4.0/src/conversions/wrappers.rs` & `ultibi-0.4.1/src/conversions/wrappers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/dataset.rs` & `ultibi-0.4.1/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/datasource.rs` & `ultibi-0.4.1/src/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/errors.rs` & `ultibi-0.4.1/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/filter.rs` & `ultibi-0.4.1/src/filter.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/lib.rs` & `ultibi-0.4.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/measure.rs` & `ultibi-0.4.1/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/src/requests.rs` & `ultibi-0.4.1/src/requests.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/tests/data/datasource_config.toml` & `ultibi-0.4.1/tests/data/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/tests/docs/run_doc_examples.py` & `ultibi-0.4.1/tests/docs/run_doc_examples.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/tests/unit/test_compute.py` & `ultibi-0.4.1/tests/unit/test_compute.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/tests/unit/test_ds.py` & `ultibi-0.4.1/tests/unit/test_ds.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/tests/unit/test_filters.py` & `ultibi-0.4.1/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/tests/unit/test_measure.py` & `ultibi-0.4.1/tests/unit/test_measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/tests/unit/test_source.py` & `ultibi-0.4.1/tests/unit/test_source.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/ultibi/__init__.py` & `ultibi-0.4.1/ultibi/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/ultibi/internals/__init__.py` & `ultibi-0.4.1/ultibi/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/ultibi/internals/dataset.py` & `ultibi-0.4.1/ultibi/internals/dataset.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/ultibi/internals/datasource.py` & `ultibi-0.4.1/ultibi/internals/datasource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from polars import DataFrame, LazyFrame
-from typing_extensions import Self
 
 from ..rust_module.ultibi_engine import DataSourceWrapper
 
 
 class DataSource:
     """Represents a Source of your Data. The source can be:
     1) An In Memory Dataframe. This is the fastest way to perform computations.
@@ -51,19 +50,19 @@
     >>> ds.prepare()
 
     """
 
     inner: DataSourceWrapper
 
     @classmethod
-    def inmemory(cls, data: DataFrame) -> Self:
+    def inmemory(cls, data: DataFrame) -> "DataSource":
         return cls(data)
 
     @classmethod
-    def scan(cls, data: LazyFrame) -> Self:
+    def scan(cls, data: LazyFrame) -> "DataSource":
         return cls(data)
 
     def __init__(self, data: "DataFrame | LazyFrame | str"):
         if isinstance(data, DataFrame):
             self.inner = DataSourceWrapper.from_frame(data)
 
         elif isinstance(data, LazyFrame):
```

### Comparing `ultibi-0.4.0/ultibi/internals/filters.py` & `ultibi-0.4.1/ultibi/internals/filters.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/ultibi/internals/measure.py` & `ultibi-0.4.1/ultibi/internals/measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/ultibi/internals/requests.py` & `ultibi-0.4.1/ultibi/internals/requests.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.4.0/Cargo.lock` & `ultibi-0.4.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1261,17 +1261,17 @@
 checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32c"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3dfea2db42e9927a3845fb268a10a72faed6d416065f77873f05e411457c363e"
+checksum = "d8f48d60e5b4d2c53d5c2b1d8a58c849a70ae5e5509b08a48d047e3b65714a74"
 dependencies = [
  "rustc_version",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -1648,15 +1648,15 @@
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frtb_engine"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "log",
  "ndarray",
  "once_cell",
  "polars",
  "rayon",
  "serde",
@@ -2094,15 +2094,14 @@
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
- "serde",
 ]
 
 [[package]]
 name = "indexmap"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
@@ -2328,17 +2327,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.9"
+version = "1.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
+checksum = "24e6ab01971eb092ffe6a7d42f49f9ff42662f17604681e2843ad65077ba47dc"
 dependencies = [
  "cc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
@@ -3367,15 +3366,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyultima"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "ciborium",
  "frtb_engine",
  "once_cell",
  "polars",
  "pyo3",
  "serde_json",
@@ -3387,17 +3386,17 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.31"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "r2d2"
 version = "0.8.10"
@@ -3853,26 +3852,26 @@
 name = "semver"
 version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.174"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b88756493a5bd5e5395d53baa70b194b05764ab85b59e43e4b8f4e1192fa9b1"
+checksum = "5d25439cd7397d044e2748a6fe2432b5e85db703d6d097bd014b3c0ad1ebff0b"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.174"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e5c3a298c7f978e53536f95a63bdc4c4a64550582f31a0359a9afda6aede62e"
+checksum = "b23f7ade6f110613c0d63858ddb8b94c1041f550eab58a16b371bdf2c9c80ab4"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.27",
 ]
 
 [[package]]
@@ -4218,15 +4217,15 @@
  "redox_syscall 0.3.5",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "template_drivers"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "actix-files",
  "actix-web",
  "actix-web-httpauth",
  "actix-web-static-files",
  "anyhow",
  "clap",
@@ -4565,23 +4564,23 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ultibi"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "ultibi_core",
  "ultibi_server",
 ]
 
 [[package]]
 name = "ultibi_core"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "aws-config",
  "aws-sdk-s3",
  "connectorx",
  "dashmap",
  "derivative",
  "futures",
@@ -4594,15 +4593,15 @@
  "tokio",
  "toml 0.7.6",
  "utoipa",
 ]
 
 [[package]]
 name = "ultibi_server"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "actix-web",
  "actix-web-static-files",
  "anyhow",
  "dotenv",
  "log",
  "mime",
@@ -4686,31 +4685,30 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "utoipa"
-version = "3.3.0"
+version = "3.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68ae74ef183fae36d650f063ae7bde1cacbe1cd7e72b617cbe1e985551878b98"
+checksum = "8c624186f22e625eb8faa777cb33d34cd595aa16d1742aa1d8b6cf35d3e4dda9"
 dependencies = [
- "indexmap 1.9.3",
+ "indexmap 2.0.0",
  "serde",
  "serde_json",
  "utoipa-gen",
 ]
 
 [[package]]
 name = "utoipa-gen"
-version = "3.3.0"
+version = "3.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ea8ac818da7e746a63285594cce8a96f5e00ee31994e655bd827569cb8b137b"
+checksum = "b9ce5f21ca77e010f5283fa791c6ab892c68b3668a1bdc6b7ac6cf978f5d5b30"
 dependencies = [
- "lazy_static",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
  "syn 2.0.27",
 ]
```

### Comparing `ultibi-0.4.0/PKG-INFO` & `ultibi-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultibi
-Version: 0.4.0
+Version: 0.4.1
 Classifier: Programming Language :: Rust
 Classifier: License :: Free To Use But Restricted
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultibi Version: 0.4.0 Classifier: Programming
+Metadata-Version: 2.1 Name: ultibi Version: 0.4.1 Classifier: Programming
 Language :: Rust Classifier: License :: Free To Use But Restricted Classifier:
 Topic :: Scientific/Engineering Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: polars >=0.18.7 License-File: LICENSE Summary: Flexible
 DataFrame Operations via UI Keywords:
 dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-
```

