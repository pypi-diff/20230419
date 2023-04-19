# Comparing `tmp/ultibi-0.2.0.tar.gz` & `tmp/ultibi-0.3.0.tar.gz`

## Comparing `ultibi-0.2.0.tar` & `ultibi-0.3.0.tar`

### file list

```diff
@@ -1,141 +1,150 @@
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.2.0/local_dependencies/ultibi_server/Cargo.toml
--rw-r--r--   0     1001      123      219 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/build.rs
--rw-r--r--   0     1001      123       35 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/src/api/mod.rs
--rw-r--r--   0     1001      123      638 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/src/api/open_api.rs
--rw-r--r--   0     1001      123     6651 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/src/api/routers.rs
--rw-r--r--   0     1001      123     1264 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/src/app.rs
--rw-r--r--   0     1001      123     2593 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/src/helpers.rs
--rw-r--r--   0     1001      123     1432 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/src/lib.rs
--rw-r--r--   0     1001      123      433 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_server/src/visual.rs
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 ultibi-0.2.0/local_dependencies/frtb_engine/Cargo.toml
--rw-r--r--   0     1001      123      481 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/README.md
--rw-r--r--   0     1001      123    14931 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/Delta.csv
--rw-r--r--   0     1001      123      541 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
--rw-r--r--   0     1001      123     2160 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
--rw-r--r--   0     1001      123      159 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/hms.csv
--rw-r--r--   0     1001      123      177 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
--rw-r--r--   0     1001      123    13945 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/calc_params.rs
--rw-r--r--   0     1001      123       25 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/docs/mod.rs
--rw-r--r--   0     1001      123     1226 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/docs/optional_params.rs
--rw-r--r--   0     1001      123     1404 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/common.rs
--rw-r--r--   0     1001      123    11392 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
--rw-r--r--   0     1001      123     9035 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
--rw-r--r--   0     1001      123     7597 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs
--rw-r--r--   0     1001      123       96 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/mod.rs
--rw-r--r--   0     1001      123      747 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/totals.rs
--rw-r--r--   0     1001      123     4811 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/helpers.rs
--rw-r--r--   0     1001      123     8664 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/lib.rs
--rw-r--r--   0     1001      123     3733 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/measures.rs
--rw-r--r--   0     1001      123      188 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/prelude.rs
--rw-r--r--   0     1001      123    26424 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/risk_weights.rs
--rw-r--r--   0     1001      123     5402 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
--rw-r--r--   0     1001      123     5023 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/rrao/mod.rs
--rw-r--r--   0     1001      123     1374 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/buckets.rs
--rw-r--r--   0     1001      123    13097 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
--rw-r--r--   0     1001      123    13419 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
--rw-r--r--   0     1001      123       64 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
--rw-r--r--   0     1001      123     3523 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
--rw-r--r--   0     1001      123     6936 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
--rw-r--r--   0     1001      123    29762 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/common.rs
--rw-r--r--   0     1001      123     9776 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs
--rw-r--r--   0     1001      123    18137 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
--rw-r--r--   0     1001      123    17086 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
--rw-r--r--   0     1001      123       64 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
--rw-r--r--   0     1001      123     3665 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
--rw-r--r--   0     1001      123    11289 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
--rw-r--r--   0     1001      123    14537 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
--rw-r--r--   0     1001      123    11963 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
--rw-r--r--   0     1001      123     2772 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
--rw-r--r--   0     1001      123     8286 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
--rw-r--r--   0     1001      123    14181 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
--rw-r--r--   0     1001      123    12980 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
--rw-r--r--   0     1001      123     2856 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
--rw-r--r--   0     1001      123     7567 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
--rw-r--r--   0     1001      123    15942 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
--rw-r--r--   0     1001      123    10386 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
--rw-r--r--   0     1001      123       64 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
--rw-r--r--   0     1001      123     2030 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
--rw-r--r--   0     1001      123     9914 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
--rw-r--r--   0     1001      123    13455 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
--rw-r--r--   0     1001      123    11491 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
--rw-r--r--   0     1001      123       64 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
--rw-r--r--   0     1001      123     2030 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
--rw-r--r--   0     1001      123     9651 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
--rw-r--r--   0     1001      123    13328 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
--rw-r--r--   0     1001      123    21367 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
--rw-r--r--   0     1001      123       64 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
--rw-r--r--   0     1001      123     2163 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
--rw-r--r--   0     1001      123    15143 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
--rw-r--r--   0     1001      123      221 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/mod.rs
--rw-r--r--   0     1001      123     4994 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/totals.rs
--rw-r--r--   0     1001      123    28643 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/statics.rs
--rw-r--r--   0     1001      123      713 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/totals.rs
--rw-r--r--   0     1001      123     1881 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/src/validate.rs
--rw-r--r--   0     1001      123     1745 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/tests/common/mod.rs
--rw-r--r--   0     1001      123     1486 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/tests/dependant.rs
--rw-r--r--   0     1001      123     4487 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/tests/drc.rs
--rw-r--r--   0     1001      123      420 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/tests/rrao.rs
--rw-r--r--   0     1001      123    18903 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/tests/sbm.rs
--rw-r--r--   0     1001      123      744 2023-03-28 20:53:25.000000 ultibi-0.2.0/local_dependencies/frtb_engine/tests/sbm_totals.rs
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 ultibi-0.2.0/local_dependencies/ultibi/Cargo.toml
--rw-r--r--   0     1001      123        0 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi/README.md
--rw-r--r--   0     1001      123       73 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi/src/lib.rs
--rw-r--r--   0        0        0     1361 1970-01-01 00:00:00.000000 ultibi-0.2.0/local_dependencies/ultibi_core/Cargo.toml
--rw-r--r--   0     1001      123     2012 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/add_row.rs
--rw-r--r--   0     1001      123     3452 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/aggregations.rs
--rw-r--r--   0     1001      123      654 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/cache.rs
--rw-r--r--   0     1001      123     4204 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/datarequest.rs
--rw-r--r--   0     1001      123    10145 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/dataset.rs
--rw-r--r--   0     1001      123     1589 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/acquire.rs
--rw-r--r--   0     1001      123     2020 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/awss3.rs
--rw-r--r--   0     1001      123     5293 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/helpers.rs
--rw-r--r--   0     1001      123     7509 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/mod.rs
--rw-r--r--   0     1001      123        9 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/errors.rs
--rw-r--r--   0     1001      123    10956 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs
--rw-r--r--   0     1001      123     4594 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
--rw-r--r--   0     1001      123      464 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/execution/mod.rs
--rw-r--r--   0     1001      123     2592 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/filters.rs
--rw-r--r--   0     1001      123       18 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/helpers/mod.rs
--rw-r--r--   0     1001      123      538 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/helpers/searches.rs
--rw-r--r--   0     1001      123      358 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/lib.rs
--rw-r--r--   0     1001      123    11434 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/measure.rs
--rw-r--r--   0     1001      123     5459 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/overrides.rs
--rw-r--r--   0     1001      123      230 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/src/prelude.rs
--rw-r--r--   0     1001      123     1884 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/add_row.rs
--rw-r--r--   0     1001      123      741 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/agg_request.rs
--rw-r--r--   0     1001      123     1543 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/aggregations.rs
--rw-r--r--   0     1001      123        1 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/cache.rs
--rw-r--r--   0     1001      123     2001 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/common/mod.rs
--rw-r--r--   0     1001      123       95 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/data/bad_config.toml
--rw-r--r--   0     1001      123      553 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml
--rw-r--r--   0     1001      123      116 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/data/test_config.toml
--rw-r--r--   0     1001      123      354 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/data/testset.csv
--rw-r--r--   0     1001      123     1250 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/datasource.rs
--rw-r--r--   0     1001      123     3115 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/dependants.rs
--rw-r--r--   0     1001      123     1485 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/filters.rs
--rw-r--r--   0     1001      123        1 2023-03-28 20:53:26.000000 ultibi-0.2.0/local_dependencies/ultibi_core/tests/overrides.rs
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 ultibi-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      728 2023-03-28 20:53:26.000000 ultibi-0.2.0/.gitignore
--rw-r--r--   0     1001      123     2436 2023-03-28 20:53:26.000000 ultibi-0.2.0/Makefile
--rw-r--r--   0     1001      123      781 2023-03-28 20:53:26.000000 ultibi-0.2.0/README.md
--rw-r--r--   0     1001      123     1559 2023-03-28 20:53:26.000000 ultibi-0.2.0/example.py
--rw-r--r--   0     1001      123     1429 2023-03-28 20:53:26.000000 ultibi-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123       36 2023-03-28 20:53:26.000000 ultibi-0.2.0/requirements-lint.txt
--rw-r--r--   0     1001      123      307 2023-03-28 20:53:26.000000 ultibi-0.2.0/requirements.txt
--rw-r--r--   0     1001      123     3398 2023-03-28 20:53:26.000000 ultibi-0.2.0/src/conversion.rs
--rw-r--r--   0     1001      123     2881 2023-03-28 20:53:26.000000 ultibi-0.2.0/src/errors.rs
--rw-r--r--   0     1001      123     9108 2023-03-28 20:53:26.000000 ultibi-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     1353 2023-03-28 20:53:26.000000 ultibi-0.2.0/src/requests.rs
--rw-r--r--   0     1001      123     1762 2023-03-28 20:53:26.000000 ultibi-0.2.0/tests/data/datasource_config.toml
--rw-r--r--   0     1001      123     4042 2023-03-28 20:53:26.000000 ultibi-0.2.0/tests/docs/run_doc_examples.py
--rw-r--r--   0     1001      123      542 2023-03-28 20:53:26.000000 ultibi-0.2.0/tests/unit/test_compute.py
--rw-r--r--   0     1001      123     1512 2023-03-28 20:53:26.000000 ultibi-0.2.0/tests/unit/test_ds.py
--rw-r--r--   0     1001      123      374 2023-03-28 20:53:26.000000 ultibi-0.2.0/ultibi/__init__.py
--rw-r--r--   0     1001      123      611 2023-03-28 20:53:26.000000 ultibi-0.2.0/ultibi/internals/__init__.py
--rw-r--r--   0     1001      123     6142 2023-03-28 20:53:26.000000 ultibi-0.2.0/ultibi/internals/dataset.py
--rw-r--r--   0     1001      123     2952 2023-03-28 20:53:26.000000 ultibi-0.2.0/ultibi/internals/requests.py
--rw-r--r--   0     1001      123        0 2023-03-28 20:53:26.000000 ultibi-0.2.0/ultibi/rust_module/__init__.py
--rw-r--r--   0        0        0    95489 2023-03-28 20:56:20.000000 ultibi-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 ultibi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 ultibi-0.3.0/local_dependencies/frtb_engine/Cargo.toml
+-rw-r--r--   0     1001      123      481 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/README.md
+-rw-r--r--   0     1001      123    14931 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/Delta.csv
+-rw-r--r--   0     1001      123      541 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
+-rw-r--r--   0     1001      123     2160 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
+-rw-r--r--   0     1001      123      159 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/hms.csv
+-rw-r--r--   0     1001      123      177 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
+-rw-r--r--   0     1001      123    20066 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/calc_params.rs
+-rw-r--r--   0     1001      123       25 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/docs/mod.rs
+-rw-r--r--   0     1001      123     1226 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/docs/optional_params.rs
+-rw-r--r--   0     1001      123     1424 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/common.rs
+-rw-r--r--   0     1001      123    11840 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
+-rw-r--r--   0     1001      123     9483 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
+-rw-r--r--   0     1001      123     7606 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs
+-rw-r--r--   0     1001      123       96 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/mod.rs
+-rw-r--r--   0     1001      123      787 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/totals.rs
+-rw-r--r--   0     1001      123     4811 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/helpers.rs
+-rw-r--r--   0     1001      123     8968 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/lib.rs
+-rw-r--r--   0     1001      123     3780 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/measures.rs
+-rw-r--r--   0     1001      123      188 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/prelude.rs
+-rw-r--r--   0     1001      123    26516 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/risk_weights.rs
+-rw-r--r--   0     1001      123     5408 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
+-rw-r--r--   0     1001      123     5268 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/rrao/mod.rs
+-rw-r--r--   0     1001      123     1374 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/buckets.rs
+-rw-r--r--   0     1001      123    14177 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
+-rw-r--r--   0     1001      123    13866 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
+-rw-r--r--   0     1001      123     3699 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
+-rw-r--r--   0     1001      123     7432 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
+-rw-r--r--   0     1001      123    29827 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/common.rs
+-rw-r--r--   0     1001      123     9793 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs
+-rw-r--r--   0     1001      123    19318 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
+-rw-r--r--   0     1001      123    17703 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
+-rw-r--r--   0     1001      123     3841 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
+-rw-r--r--   0     1001      123    11803 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
+-rw-r--r--   0     1001      123    15617 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
+-rw-r--r--   0     1001      123    12459 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
+-rw-r--r--   0     1001      123     2904 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
+-rw-r--r--   0     1001      123     8782 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
+-rw-r--r--   0     1001      123    15261 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
+-rw-r--r--   0     1001      123    13479 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
+-rw-r--r--   0     1001      123     2988 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
+-rw-r--r--   0     1001      123     8063 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
+-rw-r--r--   0     1001      123    17052 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
+-rw-r--r--   0     1001      123    10900 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
+-rw-r--r--   0     1001      123    10428 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
+-rw-r--r--   0     1001      123    14289 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
+-rw-r--r--   0     1001      123    11992 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
+-rw-r--r--   0     1001      123    10166 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
+-rw-r--r--   0     1001      123    14030 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
+-rw-r--r--   0     1001      123    21887 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
+-rw-r--r--   0     1001      123     2295 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
+-rw-r--r--   0     1001      123    15657 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
+-rw-r--r--   0     1001      123      221 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/mod.rs
+-rw-r--r--   0     1001      123     5170 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/totals.rs
+-rw-r--r--   0     1001      123    28643 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/statics.rs
+-rw-r--r--   0     1001      123      753 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/totals.rs
+-rw-r--r--   0     1001      123     1881 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/src/validate.rs
+-rw-r--r--   0     1001      123     1756 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/tests/common/mod.rs
+-rw-r--r--   0     1001      123     1486 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/tests/dependant.rs
+-rw-r--r--   0     1001      123     4487 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/tests/drc.rs
+-rw-r--r--   0     1001      123      420 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/tests/rrao.rs
+-rw-r--r--   0     1001      123    18903 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/tests/sbm.rs
+-rw-r--r--   0     1001      123      744 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/frtb_engine/tests/sbm_totals.rs
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.0/local_dependencies/ultibi/Cargo.toml
+-rw-r--r--   0     1001      123        0 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi/README.md
+-rw-r--r--   0     1001      123       73 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi/src/lib.rs
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.0/local_dependencies/ultibi_server/Cargo.toml
+-rw-r--r--   0     1001      123      219 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/build.rs
+-rw-r--r--   0     1001      123       35 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/src/api/mod.rs
+-rw-r--r--   0     1001      123      638 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/src/api/open_api.rs
+-rw-r--r--   0     1001      123     6651 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/src/api/routers.rs
+-rw-r--r--   0     1001      123     1264 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/src/app.rs
+-rw-r--r--   0     1001      123     2593 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/src/helpers.rs
+-rw-r--r--   0     1001      123     1432 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/src/lib.rs
+-rw-r--r--   0     1001      123      433 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_server/src/visual.rs
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 ultibi-0.3.0/local_dependencies/ultibi_core/Cargo.toml
+-rw-r--r--   0     1001      123     2031 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/add_row.rs
+-rw-r--r--   0     1001      123     3486 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/aggregations.rs
+-rw-r--r--   0     1001      123      654 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/cache.rs
+-rw-r--r--   0     1001      123     4244 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/datarequest.rs
+-rw-r--r--   0     1001      123     9751 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/dataset.rs
+-rw-r--r--   0     1001      123     1782 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/acquire.rs
+-rw-r--r--   0     1001      123     2059 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/awss3.rs
+-rw-r--r--   0     1001      123     5329 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/helpers.rs
+-rw-r--r--   0     1001      123     7509 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/mod.rs
+-rw-r--r--   0     1001      123        9 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/errors.rs
+-rw-r--r--   0     1001      123    10956 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs
+-rw-r--r--   0     1001      123     4594 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
+-rw-r--r--   0     1001      123      464 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/execution/mod.rs
+-rw-r--r--   0     1001      123     2585 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/filters.rs
+-rw-r--r--   0     1001      123       18 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/helpers/mod.rs
+-rw-r--r--   0     1001      123      545 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/helpers/searches.rs
+-rw-r--r--   0     1001      123      358 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/lib.rs
+-rw-r--r--   0     1001      123    11996 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/measure.rs
+-rw-r--r--   0     1001      123     5459 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/overrides.rs
+-rw-r--r--   0     1001      123      230 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/src/prelude.rs
+-rw-r--r--   0     1001      123     1884 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/add_row.rs
+-rw-r--r--   0     1001      123      741 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/agg_request.rs
+-rw-r--r--   0     1001      123     1543 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/aggregations.rs
+-rw-r--r--   0     1001      123        1 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/cache.rs
+-rw-r--r--   0     1001      123     2067 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/common/mod.rs
+-rw-r--r--   0     1001      123       95 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/data/bad_config.toml
+-rw-r--r--   0     1001      123      553 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml
+-rw-r--r--   0     1001      123      116 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/data/test_config.toml
+-rw-r--r--   0     1001      123      354 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/data/testset.csv
+-rw-r--r--   0     1001      123     1250 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/datasource.rs
+-rw-r--r--   0     1001      123     3115 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/dependants.rs
+-rw-r--r--   0     1001      123     1485 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/filters.rs
+-rw-r--r--   0     1001      123        1 2023-04-19 15:41:11.000000 ultibi-0.3.0/local_dependencies/ultibi_core/tests/overrides.rs
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 ultibi-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      728 2023-04-19 15:41:11.000000 ultibi-0.3.0/.gitignore
+-rw-r--r--   0     1001      123     2403 2023-04-19 15:41:11.000000 ultibi-0.3.0/Makefile
+-rw-r--r--   0     1001      123     4516 2023-04-19 15:41:11.000000 ultibi-0.3.0/README.md
+-rw-r--r--   0     1001      123     1559 2023-04-19 15:41:11.000000 ultibi-0.3.0/example.py
+-rw-r--r--   0     1001      123     1429 2023-04-19 15:41:11.000000 ultibi-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123       36 2023-04-19 15:41:11.000000 ultibi-0.3.0/requirements-lint.txt
+-rw-r--r--   0     1001      123      307 2023-04-19 15:41:11.000000 ultibi-0.3.0/requirements.txt
+-rw-r--r--   0     1001      123     3682 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/calculator.rs
+-rw-r--r--   0     1001      123       48 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/conversions/mod.rs
+-rw-r--r--   0     1001      123     3542 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/conversions/series.rs
+-rw-r--r--   0     1001      123     3049 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/conversions/wrappers.rs
+-rw-r--r--   0     1001      123     7737 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/dataset.rs
+-rw-r--r--   0     1001      123     3303 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/errors.rs
+-rw-r--r--   0     1001      123      693 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/filter.rs
+-rw-r--r--   0     1001      123     1986 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123     2521 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/measure.rs
+-rw-r--r--   0     1001      123     1353 2023-04-19 15:41:11.000000 ultibi-0.3.0/src/requests.rs
+-rw-r--r--   0     1001      123     1762 2023-04-19 15:41:11.000000 ultibi-0.3.0/tests/data/datasource_config.toml
+-rw-r--r--   0     1001      123     4042 2023-04-19 15:41:11.000000 ultibi-0.3.0/tests/docs/run_doc_examples.py
+-rw-r--r--   0     1001      123      591 2023-04-19 15:41:11.000000 ultibi-0.3.0/tests/unit/test_compute.py
+-rw-r--r--   0     1001      123     1507 2023-04-19 15:41:11.000000 ultibi-0.3.0/tests/unit/test_ds.py
+-rw-r--r--   0     1001      123     2658 2023-04-19 15:41:11.000000 ultibi-0.3.0/tests/unit/test_measure.py
+-rw-r--r--   0     1001      123      848 2023-04-19 15:41:11.000000 ultibi-0.3.0/ultibi/__init__.py
+-rw-r--r--   0     1001      123     1062 2023-04-19 15:41:11.000000 ultibi-0.3.0/ultibi/internals/__init__.py
+-rw-r--r--   0     1001      123     6735 2023-04-19 15:41:11.000000 ultibi-0.3.0/ultibi/internals/dataset.py
+-rw-r--r--   0     1001      123     3133 2023-04-19 15:41:11.000000 ultibi-0.3.0/ultibi/internals/filters.py
+-rw-r--r--   0     1001      123     5202 2023-04-19 15:41:11.000000 ultibi-0.3.0/ultibi/internals/measure.py
+-rw-r--r--   0     1001      123     2952 2023-04-19 15:41:11.000000 ultibi-0.3.0/ultibi/internals/requests.py
+-rw-r--r--   0     1001      123        0 2023-04-19 15:41:11.000000 ultibi-0.3.0/ultibi/rust_module/__init__.py
+-rw-r--r--   0        0        0   101983 2023-04-19 15:43:08.000000 ultibi-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 ultibi-0.3.0/PKG-INFO
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_server/Cargo.toml` & `ultibi-0.3.0/local_dependencies/ultibi_server/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_server"
-version= "0.2.0"
+version= "0.3.0"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_server/src/api/open_api.rs` & `ultibi-0.3.0/local_dependencies/ultibi_server/src/api/open_api.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_server/src/api/routers.rs` & `ultibi-0.3.0/local_dependencies/ultibi_server/src/api/routers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_server/src/app.rs` & `ultibi-0.3.0/local_dependencies/ultibi_server/src/app.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_server/src/helpers.rs` & `ultibi-0.3.0/local_dependencies/ultibi_server/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_server/src/lib.rs` & `ultibi-0.3.0/local_dependencies/ultibi_server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/Cargo.toml` & `ultibi-0.3.0/local_dependencies/frtb_engine/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [package]
 name = "frtb_engine"
-version= "0.2.0"
+version= "0.3.0"
 edition = "2021"
 publish = false
 license-file= "LICENSE"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 ultibi = {path = "../ultibi" }
-polars = { version = "0.25.1", features = [
+polars = { version = "0.28.0", features = [
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
     "csv-file",
-    "diagonal_concat","strings", "ndarray", "lazy", "is_in", "dtype-categorical", "performant", "partition_by", "concat_str",
-] }
+    "diagonal_concat",
+    "serde-lazy"
+,"strings", "ndarray", "lazy", "is_in", "dtype-categorical", "performant", "partition_by", "concat_str"] }
 serde = { version = "1.0", features = ["derive","derive"] }
 serde_json = "1.0"
 once_cell = "1.12"
 ndarray = {version = "0.15.6", features = ["matrixmultiply-threading", "rayon", "serde"] }
 rayon = "1.5.3"
 strum = {version="0.24", features = ["derive"] }
 log = "0.4"
 yearfrac = "0.1.4"
+smartstring = "*"
 
 [dev-dependencies]
 
 [features]
 CRR2 = []
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/Delta.csv` & `ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/Delta.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv` & `ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml` & `ultibi-0.3.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/docs/optional_params.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/docs/optional_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/common.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/common.rs`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,30 @@
     //Not sure why compiler doesn't like this
     //let format = format.map(|x| &**x);
     let format = format.map(|x| x.to_owned());
     apply_multiple(
         move |columns| {
             let z = columns[0]
                 .utf8()?
-                .as_date(format.as_deref())?
+                .as_date(format.as_deref(), false)?
                 .as_date_iter()
                 .zip(
                     columns[1]
                         .utf8()?
-                        .as_date(format.as_deref())?
+                        .as_date(format.as_deref(), false)?
                         .as_date_iter(),
                 )
                 .map(|(x, y)| {
                     if let (Some(x), Some(y)) = (x, y) {
                         Some(dc.yearfrac(x, y))
                     } else {
                         None
                     }
                 })
                 .collect();
-            Ok(z)
+            Ok(Some(z))
         },
         &[col("COB"), col("MaturityDate")],
         GetOutput::from_type(DataType::Float64),
         false,
     )
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs`

 * *Files 19% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 "jtd"  => &columns[4],
                 "w"    => &columns[5],
                 "s"    => &columns[6],
             ]?;
 
             // Safety Step
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             // First, sum over bucket, obligor and seniority
             let mut lf = df
                 .lazy()
                 .filter(col("rc").eq(lit("DRC_nonSec")))
                 .groupby([col("b"), col("rf"), col("rft")])
@@ -79,15 +79,15 @@
                 ]);
 
             let schema = lf.schema()?;
 
             // Safety step
             df = lf.collect()?;
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
             lf = df.lazy();
 
             // Do you want to aggregate as per  22.19?
             // Note, the algorithm is O(N), but we loose Negative GrossJTD position changes,
             // (and might end up with a different Credit Quality, but same obligor)
             // This shouldn't be a problem since we sum positions (netShort netLong) anyway,
@@ -141,34 +141,34 @@
                         .then(col("scaled_jtd"))
                         .otherwise(NULL.lit())
                         .alias("NetShortJTD"),
                 ])
                 .with_column(
                     col("NetShortJTD")
                         .map(
-                            |x| Ok(x.f64()?.apply(|y| y.abs()).into_series()),
+                            |x| Ok(Some(x.f64()?.apply(|y| y.abs()).into_series())),
                             GetOutput::from_type(DataType::Float64),
                         )
                         .alias("NetAbsShortJTD"),
                 );
             // Apply Weights
             df = lf.collect()?;
 
             match rtrn {
                 ReturnMetric::NetLongJTD => {
-                    return Ok(Series::new(
+                    return Ok(Some(Series::new(
                         "Res",
                         [df["NetLongJTD"].sum::<f64>().unwrap_or_default()],
-                    ))
+                    )))
                 }
                 ReturnMetric::NetShortJTD => {
-                    return Ok(Series::new(
+                    return Ok(Some(Series::new(
                         "Res",
                         [df["NetShortJTD"].sum::<f64>().unwrap_or_default()],
-                    ))
+                    )))
                 }
                 _ => (),
             };
             lf = df
                 .lazy()
                 .groupby([col("b")])
                 .agg([
@@ -192,32 +192,32 @@
                 .with_column(
                     (col("WeightedNetLongJTD") - col("WeightedNetAbsShortJTD") * col("HBR"))
                         .alias("DRCBucket"),
                 );
             df = lf.collect()?;
 
             match rtrn {
-                ReturnMetric::Hbr => Ok(Series::new(
+                ReturnMetric::Hbr => Ok(Some(Series::new(
                     "Res",
                     [df["HBR"].sum::<f64>().unwrap_or_default()],
-                )),
-                ReturnMetric::WeightedNetLongJTD => Ok(Series::new(
+                ))),
+                ReturnMetric::WeightedNetLongJTD => Ok(Some(Series::new(
                     "Res",
                     [df["WeightedNetLongJTD"].sum::<f64>().unwrap_or_default()],
-                )),
-                ReturnMetric::WeightedNetAbsShortJTD => Ok(Series::new(
+                ))),
+                ReturnMetric::WeightedNetAbsShortJTD => Ok(Some(Series::new(
                     "Res",
                     [df["WeightedNetAbsShortJTD"]
                         .sum::<f64>()
                         .unwrap_or_default()],
-                )),
-                _ => Ok(Series::new(
+                ))),
+                _ => Ok(Some(Series::new(
                     "Res",
                     [df["DRCBucket"].sum::<f64>().unwrap_or_default()],
-                )),
+                ))),
             }
         },
         &[
             col("RiskClass"),
             col("BucketBCBS"),
             col("RiskFactor"),
             col("SeniorityRank"),
@@ -230,56 +230,64 @@
     )
 }
 
 pub(crate) fn drc_nonsec_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "DRC nonSec GrossJTD".to_string(),
-            calculator: Box::new(drc_nonsec_grossjtd),
+            calculator: std::sync::Arc::new(drc_nonsec_grossjtd),
             aggregation: None,
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC nonSec GrossJTD Scaled".to_string(),
-            calculator: Box::new(drc_nonsec_grossjtd_scaled),
+            calculator: std::sync::Arc::new(drc_nonsec_grossjtd_scaled),
             aggregation: None,
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC nonSec CapitalCharge".to_string(),
-            calculator: Box::new(drc_nonsec_charge),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_nonsec_charge),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC nonSec NetLongJTD".to_string(),
-            calculator: Box::new(drc_nonsec_netlongjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_nonsec_netlongjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC nonSec NetShortJTD".to_string(),
-            calculator: Box::new(drc_nonsec_netshortjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_nonsec_netshortjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC nonSec NetLongJTD Weighted".to_string(),
-            calculator: Box::new(drc_nonsec_weightednetlongjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_nonsec_weightednetlongjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC nonSec NetAbsShortJTD Weighted".to_string(),
-            calculator: Box::new(drc_nonsec_weightednetabsshortjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_nonsec_weightednetabsshortjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
         // HBR Only makes sence at Bucket level
         Measure::Base(BaseMeasure {
             name: "DRC nonSec HBR".to_string(),
-            calculator: Box::new(drc_nonsec_hbr),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_nonsec_hbr),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_nonSec"))),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs`

 * *Files 12% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 "jtd"  => &columns[5],
                 "w"    => &columns[6],
                 "s"    => &columns[7],
             ]?;
 
             // Safety Step
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             // First, sum over bucket, obligor and seniority
             let mut lf = df
                 .lazy()
                 .filter(col("rc").eq(lit("DRC_Sec_nonCTP")))
                 .groupby([col("b"), col("rf"), col("rft"), col("tr")])
@@ -69,15 +69,15 @@
                     (col("jtd") * col("s")).sum().alias("scaled_jtd"),
                     col("w").first(),
                 ]);
 
             // Safety step
             df = lf.collect()?;
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
             lf = df.lazy();
 
             // TODO  22.30
 
             // Split Scaled GrossJTD into NetLong and NetShort
             df = lf.collect()?;
@@ -92,34 +92,34 @@
                         .then(col("scaled_jtd"))
                         .otherwise(NULL.lit())
                         .alias("NetShortJTD"),
                 ])
                 .with_column(
                     col("NetShortJTD")
                         .map(
-                            |x| Ok(x.f64()?.apply(|y| y.abs()).into_series()),
+                            |x| Ok(Some(x.f64()?.apply(|y| y.abs()).into_series())),
                             GetOutput::from_type(DataType::Float64),
                         )
                         .alias("NetAbsShortJTD"),
                 );
             // Apply Weights
             df = lf.collect()?;
 
             match rtrn {
                 ReturnMetric::NetLongJTD => {
-                    return Ok(Series::new(
+                    return Ok(Some(Series::new(
                         "Res",
                         [df["NetLongJTD"].sum::<f64>().unwrap_or_default()],
-                    ))
+                    )))
                 }
                 ReturnMetric::NetShortJTD => {
-                    return Ok(Series::new(
+                    return Ok(Some(Series::new(
                         "Res",
                         [df["NetShortJTD"].sum::<f64>().unwrap_or_default()],
-                    ))
+                    )))
                 }
                 _ => (),
             };
             lf = df
                 .lazy()
                 .groupby([col("b")])
                 .agg([
@@ -143,32 +143,32 @@
                 .with_column(
                     (col("WeightedNetLongJTD") - col("WeightedNetAbsShortJTD") * col("HBR"))
                         .alias("DRCBucket"),
                 );
             df = lf.collect()?;
 
             match rtrn {
-                ReturnMetric::Hbr => Ok(Series::new(
+                ReturnMetric::Hbr => Ok(Some(Series::new(
                     "Res",
                     [df["HBR"].sum::<f64>().unwrap_or_default()],
-                )),
-                ReturnMetric::WeightedNetLongJTD => Ok(Series::new(
+                ))),
+                ReturnMetric::WeightedNetLongJTD => Ok(Some(Series::new(
                     "Res",
                     [df["WeightedNetLongJTD"].sum::<f64>().unwrap_or_default()],
-                )),
-                ReturnMetric::WeightedNetAbsShortJTD => Ok(Series::new(
+                ))),
+                ReturnMetric::WeightedNetAbsShortJTD => Ok(Some(Series::new(
                     "Res",
                     [df["WeightedNetAbsShortJTD"]
                         .sum::<f64>()
                         .unwrap_or_default()],
-                )),
-                _ => Ok(Series::new(
+                ))),
+                _ => Ok(Some(Series::new(
                     "Res",
                     [df["DRCBucket"].sum::<f64>().unwrap_or_default()],
-                )),
+                ))),
             }
         },
         &[
             col("RiskClass"),
             col("BucketBCBS"),
             col("RiskFactor"),
             col("RiskFactorType"), //Seniority
@@ -182,55 +182,63 @@
     )
 }
 
 pub(crate) fn drc_secnonctp_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP GrossJTD".to_string(),
-            calculator: Box::new(drc_secnonctp_grossjtd),
+            calculator: std::sync::Arc::new(drc_secnonctp_grossjtd),
             aggregation: None,
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_Sec_nonCTP"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP GrossJTD Scaled".to_string(),
-            calculator: Box::new(drc_secnonctp_grossjtd_scaled),
+            calculator: std::sync::Arc::new(drc_secnonctp_grossjtd_scaled),
             aggregation: None,
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_Sec_nonCTP"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP CapitalCharge".to_string(),
-            calculator: Box::new(drc_secnonctp_charge),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_secnonctp_charge),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_Sec_nonCTP"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP NetLongJTD".to_string(),
-            calculator: Box::new(drc_secnonctp_netlongjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_secnonctp_netlongjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_Sec_nonCTP"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP NetShortJTD".to_string(),
-            calculator: Box::new(drc_secnonctp_netshortjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_secnonctp_netshortjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_Sec_nonCTP"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP NetLongJTD Weighted".to_string(),
-            calculator: Box::new(drc_secnonctp_weightednetlongjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_secnonctp_weightednetlongjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_Sec_nonCTP"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP NetShortJTD Weighted".to_string(),
-            calculator: Box::new(drc_secnonctp_weightednetabsshortjtd),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_secnonctp_weightednetabsshortjtd),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_Sec_nonCTP"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "DRC Sec nonCTP HBR".to_string(),
-            calculator: Box::new(drc_secnonctp_hbr),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(drc_secnonctp_hbr),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("RiskClass").eq(lit("DRC_SecNonCTP"))),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         "Key" => key,
         "RiskWeightDRC" => weight,
         "RiskClass" => vec!["DRC_Sec_nonCTP"; len],
         "RiskCategory" => vec!["DRC"; len],
     ]
     .unwrap() // We must not fail on default frame
     .lazy()
-    .with_column(concat_lst([col("RiskWeightDRC")]))
+    .with_column(concat_lst([col("RiskWeightDRC")]).unwrap())
     .collect()
     .unwrap() // we should never fail on default frame
 }
 
 ///CreditQuality_Seniority - Weight
 pub(crate) fn drc_secnonctp_weights_frame() -> DataFrame {
     let (key, weight): (Vec<String>, Vec<f64>) = drc_secnonctp_weights_raw()
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/drc/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/drc/totals.rs`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 pub(crate) fn drc_charge(_: &CPM) -> PolarsResult<Expr> {
     Ok(col("DRC nonSec CapitalCharge") + col("DRC Sec nonCTP CapitalCharge"))
 }
 
 pub(crate) fn drc_total_measures() -> Vec<Measure> {
     vec![DependantMeasure {
         name: "DRC Charge".to_string(),
-        calculator: Box::new(drc_charge),
+        calculator: std::sync::Arc::new(drc_charge),
         depends_upon: vec![
             ("DRC nonSec CapitalCharge".to_string(), "scalar".to_string()),
             (
                 "DRC Sec nonCTP CapitalCharge".to_string(),
                 "scalar".to_string(),
             ),
         ],
+        calc_params: vec![],
     }
     .into()]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/helpers.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/lib.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Series, NULL,
 };
 //use polars:: series::Series, lazy::dsl::when};
 use prelude::{drc::common::drc_scalinng, frtb_measure_vec};
 use risk_weights::*;
 use sbm::buckets;
 
-use std::collections::BTreeMap;
+use std::collections::{BTreeMap, HashSet};
 
 pub struct FRTBDataSet {
     pub frame: LazyFrame,
     pub measures: MeasuresMap,
     pub build_params: BTreeMap<String, String>,
     pub cache: Cache,
 }
@@ -62,15 +62,25 @@
     fn set_lazyframe_inplace(&mut self, lf: LazyFrame) {
         self.frame = lf;
     }
     fn get_measures(&self) -> &MeasuresMap {
         &self.measures
     }
     fn calc_params(&self) -> Vec<CalcParameter> {
-        FRTB_CALC_PARAMS.clone()
+        let mut res = vec![];
+
+        for measure in self.get_measures().values() {
+            res.extend_from_slice(measure.calc_params())
+        }
+
+        res.extend_from_slice(FRTB_CALC_PARAMS.as_ref());
+
+        let hash_res: HashSet<CalcParameter> = res.into_iter().collect();
+
+        hash_res.into_iter().collect()
     }
 
     fn new(frame: LazyFrame, mm: MeasuresMap, build_params: CPM) -> Self {
         let mut res = Self {
             frame,
             measures: mm,
             build_params,
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/measures.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/measures.rs`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,18 @@
 
 use crate::totals::sa_total_measures;
 
 /// Exporting Measures
 pub(crate) fn frtb_measure_vec() -> Vec<Measure> {
     let non_rc_specific = vec![Measure::Base(BaseMeasure {
         name: "RiskWeights".to_string(),
-        calculator: Box::new(sens_weights),
-        aggregation: Some("first"),
+        calculator: std::sync::Arc::new(sens_weights),
+        aggregation: Some("first".into()),
         precomputefilter: None,
+        calc_params: vec![],
     })];
 
     let mut res = vec![];
     res.extend(fx_delta_measures());
     res.extend(fx_vega_measures());
     res.extend(fx_curv_measures());
     res.extend(fx_total_measures());
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/risk_weights.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/risk_weights.rs`

 * *Files 1% similar despite different names*

```diff
@@ -562,15 +562,15 @@
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights"])]);
 
     // FX SECOND HERE
     lf1 = lf1.with_column(
         col("BucketBCBS")
             .map(
-                |s| Ok(s.utf8()?.str_slice(0, Some(3))?.into_series()),
+                |s| Ok(Some(s.utf8()?.str_slice(0, Some(3))?.into_series())),
                 GetOutput::from_type(DataType::Utf8),
             )
             .alias("Bucket"),
     );
     let right_on = [col("RiskClass"), col("RiskCategory"), col("Bucket")];
     lf1 = lf1.join(
         weights.rc_rcat_b_weights_second,
@@ -604,47 +604,47 @@
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights"])]);
 
     let join_on = [
         col("RiskClass"),
         col("RiskCategory"),
         col("CreditQuality").map(
-            |s| Ok(s.utf8()?.to_uppercase().into_series()),
+            |s| Ok(Some(s.utf8()?.to_uppercase().into_series())),
             GetOutput::from_type(DataType::Utf8),
         ),
     ];
     let mut lf1 = lf1.join(
         weights.drc_nonsec_weights_frame,
         join_on.clone(),
         join_on,
         JoinType::Left,
     );
     lf1 = lf1
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights"])]);
 
     //drc_secnonctp_weights
-    let left_on = [
-        col("RiskClass"),
-        col("RiskCategory"),
+    lf1 = lf1.with_column(
         concat_str(
             [
                 col("CreditQuality").map(
-                    |s| Ok(s.utf8()?.to_uppercase().into_series()),
+                    |s| Ok(Some(s.utf8()?.to_uppercase().into_series())),
                     GetOutput::from_type(DataType::Utf8),
                 ),
                 col("RiskFactorType").map(
-                    |s| Ok(s.utf8()?.to_uppercase().into_series()),
+                    |s| Ok(Some(s.utf8()?.to_uppercase().into_series())),
                     GetOutput::from_type(DataType::Utf8),
                 ),
             ],
             "_",
         )
         .alias("Key"),
-    ];
+    );
+
+    let left_on = [col("RiskClass"), col("RiskCategory"), col("Key")];
     let right_on = [col("RiskClass"), col("RiskCategory"), col("Key")];
     let mut lf1 = lf1.join(
         weights.drc_secnonctp_weights,
         left_on,
         right_on,
         JoinType::Left,
     );
@@ -746,15 +746,15 @@
         "Weights" => vec![xccy_weights, infl_weights, yield_weights],
         "RiskFactorType" => ["XCCY", "Inflation", "Yield"],
         "RiskClass" => vec!["GIRR"; 3],
         "RiskCategory" => vec!["Delta"; 3],
     ]
     .unwrap() // We must not fail on default frame
     .lazy()
-    .with_column(concat_lst([col("Weights")]))
+    .with_column(concat_lst([col("Weights")]).unwrap()) // don't expect to fail on default
     .collect()
     .expect("failed on IR Delta weights") // We must not fail on default frame
 }
 
 /// Checks if `some_str` is a path
 /// If not tries to serialise it
 /// Checks for expected columns
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     );
     lf1 = lf1.rename(["WeightsCRR2"], ["SensWeightsCRR2"]);
 
     let join_on = [
         col("RiskClass"),
         col("RiskCategory"),
         col("CreditQuality").map(
-            |s| Ok(s.utf8()?.to_uppercase().into_series()),
+            |s| Ok(Some(s.utf8()?.to_uppercase().into_series())),
             GetOutput::from_type(DataType::Utf8),
         ),
     ];
     let mut lf1 = lf1.join(
         weights.drc_nonsec_weights_frame_crr2,
         join_on.clone(),
         join_on,
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/rrao/mod.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/rrao/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
             let res = if let Some(weight) = weight {
                 notional * weight
             } else {
                 notional
             };
 
-            Ok(res.into_series())
+            Ok(Some(res.into_series()))
         },
         &[col("TradeId"), col(rrao_type), col("Notional")],
         GetOutput::from_type(DataType::Float64),
         false,
     )
 }
 
@@ -78,15 +78,15 @@
             let mut df = df![
                 "id"   => &columns[0],
                 "e"    => &columns[1],
                 "o"    => &columns[2],
                 "n"    => &columns[3],
             ]?;
 
-            df = df.unique(Some(&["id".to_string()]), UniqueKeepStrategy::First)?;
+            df = df.unique(Some(&["id".to_string()]), UniqueKeepStrategy::First, None)?;
 
             df = df
                 .lazy()
                 .with_column(
                     when(col("e"))
                         .then(col("n") * lit(exotic_weight))
                         .when(col("o"))
@@ -94,15 +94,15 @@
                         .otherwise(NULL.lit())
                         .alias("rrao"),
                 )
                 .collect()?;
 
             let res = df["rrao"].sum::<f64>().unwrap_or_else(|| 0.);
             //Ok(Series::from_vec("rrao", vec![res; columns[0].len()]))
-            Ok(Series::new("res", [res]))
+            Ok(Some(Series::new("res", [res])))
         },
         &[
             col("TradeId"),
             col("EXOTIC_RRAO"),
             col("OTHER_RRAO"),
             col("Notional"),
         ],
@@ -112,37 +112,42 @@
 }
 
 /// Exporting Measures
 pub(crate) fn rrao_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "Exotic RRAO Notional".to_string(),
-            calculator: Box::new(exotic_notional),
+            calculator: std::sync::Arc::new(exotic_notional),
             aggregation: None,
             precomputefilter: Some(col("EXOTIC_RRAO").or(col("OTHER_RRAO"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Other RRAO Notional".to_string(),
-            calculator: Box::new(other_notional),
+            calculator: std::sync::Arc::new(other_notional),
             aggregation: None,
             precomputefilter: Some(col("EXOTIC_RRAO").or(col("OTHER_RRAO"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Exotic RRAO Charge".to_string(),
-            calculator: Box::new(exotic_charge),
+            calculator: std::sync::Arc::new(exotic_charge),
             aggregation: None,
             precomputefilter: Some(col("EXOTIC_RRAO").or(col("OTHER_RRAO"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Other RRAO Charge".to_string(),
-            calculator: Box::new(other_charge),
+            calculator: std::sync::Arc::new(other_charge),
             aggregation: None,
             precomputefilter: Some(col("EXOTIC_RRAO").or(col("OTHER_RRAO"))),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "RRAO Charge".to_string(),
-            calculator: Box::new(rrao_charge),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(rrao_charge),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(col("EXOTIC_RRAO").or(col("OTHER_RRAO"))),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/buckets.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/buckets.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs`

 * *Files 19% similar despite different names*

```diff
@@ -112,227 +112,249 @@
 }
 
 /// Exporting Measures
 pub(crate) fn com_curv_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "Commodity CurvatureDelta".to_string(),
-            calculator: Box::new(com_curv_delta),
+            calculator: std::sync::Arc::new(com_curv_delta),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity CurvatureDelta Weighted".to_string(),
-            calculator: Box::new(com_curv_delta_weighted),
+            calculator: std::sync::Arc::new(com_curv_delta_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity PnLup".to_string(),
-            calculator: Box::new(com_pnl_up),
+            calculator: std::sync::Arc::new(com_pnl_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity PnLdown".to_string(),
-            calculator: Box::new(com_pnl_down),
+            calculator: std::sync::Arc::new(com_pnl_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity CVRup".to_string(),
-            calculator: Box::new(com_cvr_up),
+            calculator: std::sync::Arc::new(com_cvr_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity CVRdown".to_string(),
-            calculator: Box::new(com_cvr_down),
+            calculator: std::sync::Arc::new(com_cvr_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature KbPlus Medium".to_string(),
-            calculator: Box::new(com_curvature_kb_plus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_plus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature KbMinus Medium".to_string(),
-            calculator: Box::new(com_curvature_kb_minus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_minus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature Kb Medium".to_string(),
-            calculator: Box::new(com_curvature_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature Sb Medium".to_string(),
-            calculator: Box::new(com_curvature_sb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_sb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity CurvatureCharge Medium".to_string(),
-            calculator: Box::new(com_curvature_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature KbPlus Low".to_string(),
-            calculator: Box::new(com_curvature_kb_plus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_plus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature KbMinus Low".to_string(),
-            calculator: Box::new(com_curvature_kb_minus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_minus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature Kb Low".to_string(),
-            calculator: Box::new(com_curvature_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature Sb Low".to_string(),
-            calculator: Box::new(com_curvature_sb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_sb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity CurvatureCharge Low".to_string(),
-            calculator: Box::new(com_curvature_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature KbPlus High".to_string(),
-            calculator: Box::new(com_curvature_kb_plus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_plus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature KbMinus High".to_string(),
-            calculator: Box::new(com_curvature_kb_minus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_minus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature Kb High".to_string(),
-            calculator: Box::new(com_curvature_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity Curvature Sb High".to_string(),
-            calculator: Box::new(com_curvature_sb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_sb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity CurvatureCharge High".to_string(),
-            calculator: Box::new(com_curvature_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curvature_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity CurvatureCharge MAX".to_string(),
-            calculator: Box::new(com_curv_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_curv_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs`

 * *Files 9% similar despite different names*

```diff
@@ -191,36 +191,36 @@
                     (col("y15") * col("w").arr().get(lit(8))).sum(),
                     (col("y20") * col("w").arr().get(lit(9))).sum(),
                     (col("y30") * col("w").arr().get(lit(10))).sum(),
                 ])
                 // No need to fill null here
                 .collect()?;
 
-            let mut id_vars = vec!["b".to_string(), "rf".to_string(), "loc".to_string()];
-            if let Some(rho_ovrd) = &rho_overwrite {
-                id_vars.push(rho_ovrd.column.clone())
-            };
-
-            let ma = MeltArgs {
-                id_vars,
+            let mut ma = MeltArgs {
+                streamable: false,
+                id_vars: vec!["b".into(), "rf".into(), "loc".into()],
                 value_vars: vec![
-                    "y0".to_string(),
-                    "y025".to_string(),
-                    "y05".to_string(),
-                    "y1".to_string(),
-                    "y2".to_string(),
-                    "y3".to_string(),
-                    "y5".to_string(),
-                    "y10".to_string(),
-                    "y15".to_string(),
-                    "y20".to_string(),
-                    "y30".to_string(),
+                    "y0".into(),
+                    "y025".into(),
+                    "y05".into(),
+                    "y1".into(),
+                    "y2".into(),
+                    "y3".into(),
+                    "y5".into(),
+                    "y10".into(),
+                    "y15".into(),
+                    "y20".into(),
+                    "y30".into(),
                 ],
-                variable_name: Some("tenor".to_string()),
-                value_name: Some("weighted_sens".to_string()),
+                variable_name: Some("tenor".into()),
+                value_name: Some("weighted_sens".into()),
+            };
+
+            if let Some(rho_ovrd) = &rho_overwrite {
+                ma.id_vars.push(rho_ovrd.column.clone().into())
             };
 
             df = df.melt2(ma)?;
 
             // If Rho Override was provided, we need to check if such column is present
             let kbs_sbs = all_kbs_sbs_onsq(
                 df,
@@ -236,16 +236,16 @@
                 &rho_overwrite,
             )?;
 
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs.into_iter().unzip();
             let res_len = columns[0].len();
 
             match rtrn {
-                ReturnMetric::Kb => return Ok(Series::new("Res", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("Res", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("Res", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("Res", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
             across_bucket_agg(kbs, sbs, &com_gamma, res_len, SBMChargeType::DeltaVega)
         },
         columns,
         GetOutput::from_type(DataType::Float64),
         true,
@@ -266,107 +266,117 @@
 }
 
 /// Exporting Measures
 pub(crate) fn com_delta_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaSens".to_string(),
-            calculator: Box::new(total_commodity_delta_sens),
+            calculator: std::sync::Arc::new(total_commodity_delta_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaSens Weighted".to_string(),
-            calculator: Box::new(commodity_delta_sens_weighted),
+            calculator: std::sync::Arc::new(commodity_delta_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaSb".to_string(),
-            calculator: Box::new(commodity_delta_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(commodity_delta_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaKb Low".to_string(),
-            calculator: Box::new(commodity_delta_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(commodity_delta_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaKb Medium".to_string(),
-            calculator: Box::new(commodity_delta_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(commodity_delta_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaKb High".to_string(),
-            calculator: Box::new(commodity_delta_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(commodity_delta_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaCharge Low".to_string(),
-            calculator: Box::new(commodity_delta_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(commodity_delta_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaCharge Medium".to_string(),
-            calculator: Box::new(commodity_delta_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(commodity_delta_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaCharge High".to_string(),
-            calculator: Box::new(commodity_delta_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(commodity_delta_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity DeltaCharge MAX".to_string(),
-            calculator: Box::new(com_delta_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_delta_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs`

 * *Files 15% similar despite different names*

```diff
@@ -27,76 +27,80 @@
     ]))
 }
 
 pub(crate) fn com_total_measures() -> Vec<Measure> {
     vec![
         Measure::Dependant(DependantMeasure {
             name: "Commodity TotalCharge Low".to_string(),
-            calculator: Box::new(com_total_low),
+            calculator: std::sync::Arc::new(com_total_low),
             depends_upon: vec![
                 (
                     "Commodity DeltaCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 ("Commodity VegaCharge Low".to_string(), "scalar".to_string()),
                 (
                     "Commodity CurvatureCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "Commodity TotalCharge Medium".to_string(),
-            calculator: Box::new(com_total_medium),
+            calculator: std::sync::Arc::new(com_total_medium),
             depends_upon: vec![
                 (
                     "Commodity DeltaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity VegaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity CurvatureCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "Commodity TotalCharge High".to_string(),
-            calculator: Box::new(com_total_high),
+            calculator: std::sync::Arc::new(com_total_high),
             depends_upon: vec![
                 (
                     "Commodity DeltaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity VegaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity CurvatureCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "Commodity TotalCharge MAX".to_string(),
-            calculator: Box::new(com_total_max),
+            calculator: std::sync::Arc::new(com_total_max),
             depends_upon: vec![
                 (
                     "Commodity TotalCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity TotalCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity TotalCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs`

 * *Files 21% similar despite different names*

```diff
@@ -89,107 +89,117 @@
 }
 
 /// Exporting Measures
 pub(crate) fn com_vega_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "Commodity VegaSens".to_string(),
-            calculator: Box::new(total_com_vega_sens),
+            calculator: std::sync::Arc::new(total_com_vega_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaSens Weighted".to_string(),
-            calculator: Box::new(total_com_vega_sens_weighted),
+            calculator: std::sync::Arc::new(total_com_vega_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaSb".to_string(),
-            calculator: Box::new(com_vega_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaKb Low".to_string(),
-            calculator: Box::new(com_vega_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaCharge Low".to_string(),
-            calculator: Box::new(com_vega_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaKb Medium".to_string(),
-            calculator: Box::new(com_vega_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaCharge Medium".to_string(),
-            calculator: Box::new(com_vega_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaKb High".to_string(),
-            calculator: Box::new(com_vega_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaCharge High".to_string(),
-            calculator: Box::new(com_vega_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "Commodity VegaCharge MAX".to_string(),
-            calculator: Box::new(com_vega_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(com_vega_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Commodity"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/common.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/common.rs`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             //RiskClass
             let mask = columns[0].utf8()?.equal(rc);
             //RiskCategory
             let mask1 = columns[1].utf8()?.equal(rcat);
 
             let risk_filtered = columns[2].f64()?.set(&!(mask & mask1), None)?;
 
-            Ok(risk_filtered.into_series())
+            Ok(Some(risk_filtered.into_series()))
         },
         &[col("RiskClass"), col("RiskCategory"), risk],
         GetOutput::from_type(DataType::Float64),
         false,
     )
 }
 
@@ -71,15 +71,15 @@
     apply_multiple(
         move |columns| {
             //RiskClass
             let mask = columns[0].utf8()?.equal(rc);
 
             let risk_filtered = columns[1].f64()?.set(&!mask, None)?;
 
-            Ok(risk_filtered.into_series())
+            Ok(Some(risk_filtered.into_series()))
         },
         &[col("RiskClass"), risk],
         GetOutput::from_type(DataType::Float64),
         false,
     )
 }
 
@@ -98,15 +98,15 @@
             let mask = columns[0].utf8()?.equal(rc);
             //RiskCategory
             let mask1 = columns[3].utf8()?.equal(rcat);
 
             let delta = columns[1].f64()?.set(&!(mask & mask1), None)?;
 
             let x = delta.multiply(&columns[2])?;
-            Ok(x)
+            Ok(Some(x))
         },
         &[
             col("RiskClass"),
             col(delta_tenor),
             col(weights_col).arr().get(lit(weight_idx)),
             col("RiskCategory"),
         ],
@@ -122,15 +122,15 @@
 
 pub(crate) fn across_bucket_agg<I: IntoIterator<Item = f64>>(
     kbs: I,
     sbs: I,
     gamma: &Array2<f64>,
     _: usize,
     sbm_type: SBMChargeType,
-) -> PolarsResult<Series> {
+) -> PolarsResult<Option<Series>> {
     let kbs_arr = Array1::from_iter(kbs);
     let sbs_arr = Array1::from_iter(sbs);
 
     //21.4.5 sum{ sum {gamma*s_b*s_c} }
     let a = sbs_arr.dot(gamma);
     let b = a.dot(&sbs_arr);
 
@@ -159,15 +159,15 @@
 
         SBMChargeType::Curvature => f64::max(sum, 0.).sqrt(),
     };
 
     // The function is supposed to return a series of same len as the input, hence we broadcast the result
     //let res_arr = Array::from_elem(res_len, res);
     // if option panics on .unwrap() implement match and use .iter() and then Series from iter
-    Ok(Series::new("Res", [res]))
+    Ok(Some(Series::new("Res", [res])))
     // Ok( Series::new("res", res_arr.as_slice().unwrap() ) )
 }
 
 pub(crate) enum SBMChargeType {
     DeltaVega,
     Curvature,
 }
@@ -210,15 +210,15 @@
 {
     let n_buckets = bucket_rho_diff_rf.len();
     let mut reskbs_sbs: Vec<PolarsResult<(f64, f64)>> = Vec::with_capacity(n_buckets);
     for _ in 0..n_buckets {
         reskbs_sbs.push(Ok((0., 0.)))
     }
 
-    let arc_mtx = Arc::new(Mutex::new(reskbs_sbs));
+    let arc_mtx = std::sync::Arc::new(Mutex::new(reskbs_sbs));
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
     df.partition_by(["b"])?.par_iter().for_each(|bucket_df| {
         // Safety: since partition, we must have at least one member
         let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
         // validating also bucket is not greater than max index of bucket_rho_diff_rf
         let b_as_idx_plus_1 = match b_as_idx_plus_1 {
             AnyValue::Utf8(st) => st.parse::<usize>().ok().and_then(|b_id| {
@@ -412,15 +412,15 @@
     F: Fn(f64) -> f64 + Sync + Send + Copy,
 {
     let mut reskbs_sbs: Vec<PolarsResult<(f64, f64)>> = Vec::with_capacity(n_buckets);
     for _ in 0..n_buckets {
         reskbs_sbs.push(Ok((0., 0.)))
     }
 
-    let arc_mtx = Arc::new(Mutex::new(reskbs_sbs));
+    let arc_mtx = std::sync::Arc::new(Mutex::new(reskbs_sbs));
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
     df.fill_null(FillNullStrategy::Zero)?
         .partition_by(["b"])?
         .par_iter()
         .for_each(|bucket_df| {
             // Ok to go unsafe here becaause we validate length in [equity_delta_charge_distributor]
             let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
@@ -650,15 +650,15 @@
     let n_buckets = rho_diff_curve.len();
 
     let mut reskbs_sbs: Vec<PolarsResult<(String, (f64, f64))>> = Vec::with_capacity(n_buckets);
     for _ in 0..n_buckets {
         reskbs_sbs.push(Ok(("".to_string(), (0., 0.))))
     }
 
-    let arc_mtx = Arc::new(Mutex::new(reskbs_sbs));
+    let arc_mtx = std::sync::Arc::new(Mutex::new(reskbs_sbs));
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
     df.partition_by(["b"])?.par_iter().for_each(|bucket_df| {
         // Safety: since we are in partition, bucket_df["b"] has at least one element
         let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
         let b_as_idx_plus_1 =
             match b_as_idx_plus_1 {
                 AnyValue::Utf8(st) => st.parse::<usize>().ok().and_then(|b_id| {
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
             let pnl_up_or_down_is_not_null = mask1 | mask2;
 
             let risk_filtered = columns[3]
                 .f64()?
                 .set(&!(mask & pnl_up_or_down_is_not_null), None)?;
 
-            Ok(risk_filtered.into_series())
+            Ok(Some(risk_filtered.into_series()))
         },
         &[col("RiskClass"), col("PnL_Up"), col("PnL_Down"), risk],
         GetOutput::from_type(DataType::Float64),
         false,
     )
 }
 
@@ -162,15 +162,15 @@
     let mut res_kb_cvr: Vec<(PolarsResult<(f64, f64)>, PolarsResult<(f64, f64)>)> =
         Vec::with_capacity(n_buckets);
     //let mut res_kbminus_cvrdown: Vec<Result<(f64, f64)>> = Vec::with_capacity(n_buckets);
     for _ in 0..n_buckets {
         res_kb_cvr.push((Ok((0., 0.)), Ok((0., 0.))))
     }
 
-    let arc_mtx_kbpm_cvr = Arc::new(Mutex::new(res_kb_cvr));
+    let arc_mtx_kbpm_cvr = std::sync::Arc::new(Mutex::new(res_kb_cvr));
 
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
     df.partition_by(["b"])?.par_iter().for_each(|bucket_df| {
         // Ok to go unsafe here becaause we validate length in [equity_delta_charge_distributor]
         let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
         let b_as_idx_plus_1 =
             match b_as_idx_plus_1 {
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs`

 * *Files 8% similar despite different names*

```diff
@@ -172,43 +172,46 @@
                     cvr_up_5().sum().alias("cvr_up"),
                     cvr_down_5().sum().alias("cvr_down"),
                 ])
                 //.fill_null(lit::<f64>(0.))
                 .collect()?;
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             let res_len = columns[0].len();
             let (kb_plus_cvr_up, kb_minus_cvr_down): (Vec<(f64, f64)>, Vec<(f64, f64)>) =
                 curvature_kb_plus_minus(df, &csr_curv_rho, special_bucket)?;
             let (kb_plus, cvr_up): (Vec<f64>, Vec<f64>) = kb_plus_cvr_up.into_iter().unzip();
             let (kb_minus, cvr_down): (Vec<f64>, Vec<f64>) = kb_minus_cvr_down.into_iter().unzip();
 
             match return_metric {
                 ReturnMetric::KbPlus => {
-                    return Ok(Series::new("kb_plus", [kb_plus.iter().sum::<f64>()]))
+                    return Ok(Some(Series::new("kb_plus", [kb_plus.iter().sum::<f64>()])))
                 }
                 ReturnMetric::KbMinus => {
-                    return Ok(Series::new("kb_minus", [kb_minus.iter().sum::<f64>()]))
+                    return Ok(Some(Series::new(
+                        "kb_minus",
+                        [kb_minus.iter().sum::<f64>()],
+                    )))
                 }
                 _ => (),
             }
 
             let a = Some;
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs_curvature(
                 kb_plus,
                 kb_minus,
                 cvr_up.into_iter().map(a),
                 cvr_down.into_iter().map(a),
             )?;
             match return_metric {
-                ReturnMetric::Kb => return Ok(Series::new("kbs", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("sbs", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("kbs", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("sbs", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             let phi = phi(&sbs);
             let gamma = phi * csr_curv_gamma.view();
 
             across_bucket_agg(kbs, sbs, &gamma, res_len, SBMChargeType::Curvature)
@@ -243,227 +246,249 @@
 }
 
 /// Exporting Measures
 pub(crate) fn csrnonsec_curv_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CurvatureDelta".to_string(),
-            calculator: Box::new(csrnonsec_curv_delta),
+            calculator: std::sync::Arc::new(csrnonsec_curv_delta),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CurvatureDeltaWeighted".to_string(),
-            calculator: Box::new(csrnonsec_curv_delta_weighted),
+            calculator: std::sync::Arc::new(csrnonsec_curv_delta_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec PnLup".to_string(),
-            calculator: Box::new(csrnonsec_pnl_up),
+            calculator: std::sync::Arc::new(csrnonsec_pnl_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec PnLdown".to_string(),
-            calculator: Box::new(csrnonsec_pnl_down),
+            calculator: std::sync::Arc::new(csrnonsec_pnl_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CVRup".to_string(),
-            calculator: Box::new(csrnonsec_cvr_up),
+            calculator: std::sync::Arc::new(csrnonsec_cvr_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CVRdown".to_string(),
-            calculator: Box::new(csrnonsec_cvr_down),
+            calculator: std::sync::Arc::new(csrnonsec_cvr_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature KbPlus Medium".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_plus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_plus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature KbMinus Medium".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_minus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_minus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature Kb Medium".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature Sb Medium".to_string(),
-            calculator: Box::new(csrnonsec_curvature_sb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_sb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CurvatureCharge Medium".to_string(),
-            calculator: Box::new(csrnonsec_curvature_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature KbPlus Low".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_plus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_plus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature KbMinus Low".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_minus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_minus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature Kb Low".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature Sb Low".to_string(),
-            calculator: Box::new(csrnonsec_curvature_sb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_sb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CurvatureCharge Low".to_string(),
-            calculator: Box::new(csrnonsec_curvature_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature KbPlus High".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_plus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_plus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature KbMinus High".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_minus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_minus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature Kb High".to_string(),
-            calculator: Box::new(csrnonsec_curvature_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec Curvature Sb High".to_string(),
-            calculator: Box::new(csrnonsec_curvature_sb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_sb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CurvatureCharge High".to_string(),
-            calculator: Box::new(csrnonsec_curvature_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curvature_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec CurvatureCharge MAX".to_string(),
-            calculator: Box::new(csrnonsec_curv_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_curv_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs`

 * *Files 5% similar despite different names*

```diff
@@ -254,14 +254,18 @@
                 "w1" =>   &columns[10],
                 "w2" =>   &columns[11],
                 "w3" =>   &columns[12],
                 "w4" =>   &columns[13],
                 "w5" =>   &columns[14]
             ]?;
 
+            if df.height() == 0 {
+                return Ok(Some(Series::new("res", [0.])));
+            };
+
             // concat_lst is actually slower than
             let df = df
                 .lazy()
                 .filter(
                     col("rc")
                         .eq(lit(risk_class))
                         .and(col("rcat").eq(lit(risk_cat))),
@@ -336,16 +340,16 @@
                 ],
                 Some(base_tenor_rho),
             )?;
 
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs.into_iter().unzip();
 
             match rtrn {
-                ReturnMetric::Kb => return Ok(Series::new("kbs", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("sbs", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("kbs", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("sbs", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             across_bucket_agg(kbs, sbs, &gamma, columns[0].len(), SBMChargeType::DeltaVega)
         },
         &[
             col("RiskClass"),
@@ -382,107 +386,117 @@
 }
 
 /// Exporting Measures
 pub(crate) fn csrnonsec_delta_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaSens".to_string(),
-            calculator: Box::new(total_csr_nonsec_delta_sens),
+            calculator: std::sync::Arc::new(total_csr_nonsec_delta_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaSens Weighted".to_string(),
-            calculator: Box::new(csr_nonsec_delta_sens_weighted),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaSb".to_string(),
-            calculator: Box::new(csr_nonsec_delta_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaKb Low".to_string(),
-            calculator: Box::new(csr_nonsec_delta_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaKb Medium".to_string(),
-            calculator: Box::new(csr_nonsec_delta_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaKb High".to_string(),
-            calculator: Box::new(csr_nonsec_delta_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaCharge Low".to_string(),
-            calculator: Box::new(csr_nonsec_delta_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaCharge Medium".to_string(),
-            calculator: Box::new(csr_nonsec_delta_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaCharge High".to_string(),
-            calculator: Box::new(csr_nonsec_delta_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_delta_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec DeltaCharge MAX".to_string(),
-            calculator: Box::new(csrnonsec_delta_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_delta_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs`

 * *Files 4% similar despite different names*

```diff
@@ -28,79 +28,83 @@
     ]))
 }
 
 pub(crate) fn csrnonsec_total_measures() -> Vec<Measure> {
     vec![
         Measure::Dependant(DependantMeasure {
             name: "CSR nonSec TotalCharge Low".to_string(),
-            calculator: Box::new(csrnonsec_total_low),
+            calculator: std::sync::Arc::new(csrnonsec_total_low),
             depends_upon: vec![
                 (
                     "CSR nonSec DeltaCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec VegaCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec CurvatureCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "CSR nonSec TotalCharge Medium".to_string(),
-            calculator: Box::new(csrnonsec_total_medium),
+            calculator: std::sync::Arc::new(csrnonsec_total_medium),
             depends_upon: vec![
                 (
                     "CSR nonSec DeltaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec VegaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec CurvatureCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "CSR nonSec TotalCharge High".to_string(),
-            calculator: Box::new(csrnonsec_total_high),
+            calculator: std::sync::Arc::new(csrnonsec_total_high),
             depends_upon: vec![
                 (
                     "CSR nonSec DeltaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec VegaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec CurvatureCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "CSR nonSec TotalCharge MAX".to_string(),
-            calculator: Box::new(csrnonsec_total_max),
+            calculator: std::sync::Arc::new(csrnonsec_total_max),
             depends_upon: vec![
                 (
                     "CSR nonSec TotalCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec TotalCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR nonSec TotalCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs`

 * *Files 11% similar despite different names*

```diff
@@ -164,31 +164,31 @@
                     (col("y5") * col("w")).sum(),
                     (col("y10") * col("w")).sum(),
                 ])
                 //.fill_null(lit::<f64>(0.))
                 .collect()?;
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             let kbs_sbs = all_kbs_sbs_single_type(
                 df,
                 &opt_mat_rho,
                 &rho_diff_curve,
                 scenario_fn,
                 &["y05", "y1", "y3", "y5", "y10"],
                 special_bucket,
             )?;
 
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs.into_iter().unzip();
 
             match rtrn {
-                ReturnMetric::Kb => return Ok(Series::new("kbs", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("sbs", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("kbs", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("sbs", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             across_bucket_agg(kbs, sbs, &gamma, columns[0].len(), SBMChargeType::DeltaVega)
         },
         &[
             col("RiskClass"),
@@ -220,107 +220,117 @@
 }
 
 /// Exporting Measures
 pub(crate) fn csrnonsec_vega_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaSens".to_string(),
-            calculator: Box::new(total_csrnonsec_vega_sens),
+            calculator: std::sync::Arc::new(total_csrnonsec_vega_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaSens Weighted".to_string(),
-            calculator: Box::new(total_csrnonsec_vega_sens_weighted_bcbs),
+            calculator: std::sync::Arc::new(total_csrnonsec_vega_sens_weighted_bcbs),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaSb".to_string(),
-            calculator: Box::new(csr_nonsec_vega_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_vega_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaCharge Low".to_string(),
-            calculator: Box::new(csr_nonsec_vega_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_vega_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaKb Low".to_string(),
-            calculator: Box::new(csr_nonsec_vega_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_vega_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaCharge Medium".to_string(),
-            calculator: Box::new(csr_nonsec_vega_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_vega_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaKb Medium".to_string(),
-            calculator: Box::new(csr_nonsec_vega_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_vega_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaCharge High".to_string(),
-            calculator: Box::new(csr_nonsec_vega_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_vega_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaKb High".to_string(),
-            calculator: Box::new(csr_nonsec_vega_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_nonsec_vega_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR nonSec VegaCharge MAX".to_string(),
-            calculator: Box::new(csrnonsec_vega_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrnonsec_vega_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_nonSec"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs`

 * *Files 12% similar despite different names*

```diff
@@ -139,227 +139,249 @@
 }
 
 /// Exporting Measures
 pub(crate) fn csrsecctp_curv_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CurvatureDelta".to_string(),
-            calculator: Box::new(csrsecctp_curv_delta),
+            calculator: std::sync::Arc::new(csrsecctp_curv_delta),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CurvatureDelta_Weighted".to_string(),
-            calculator: Box::new(csrsecctp_curv_delta_weighted),
+            calculator: std::sync::Arc::new(csrsecctp_curv_delta_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP PnLup".to_string(),
-            calculator: Box::new(csrsecctp_pnl_up),
+            calculator: std::sync::Arc::new(csrsecctp_pnl_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP PnLdown".to_string(),
-            calculator: Box::new(csrsecctp_pnl_down),
+            calculator: std::sync::Arc::new(csrsecctp_pnl_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CVRup".to_string(),
-            calculator: Box::new(csrsecctp_cvr_up),
+            calculator: std::sync::Arc::new(csrsecctp_cvr_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CVRdown".to_string(),
-            calculator: Box::new(csrsecctp_cvr_down),
+            calculator: std::sync::Arc::new(csrsecctp_cvr_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature KbPlus Medium".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_plus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_plus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature KbMinus Medium".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_minus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_minus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature Kb Medium".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature Sb Medium".to_string(),
-            calculator: Box::new(csrsecctp_curvature_sb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_sb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CurvatureCharge Medium".to_string(),
-            calculator: Box::new(csrsecctp_curvature_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature KbPlus Low".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_plus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_plus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature KbMinus Low".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_minus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_minus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature Kb Low".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature Sb Low".to_string(),
-            calculator: Box::new(csrsecctp_curvature_sb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_sb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CurvatureCharge Low".to_string(),
-            calculator: Box::new(csrsecctp_curvature_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature KbPlus High".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_plus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_plus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature KbMinus High".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_minus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_minus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature Kb High".to_string(),
-            calculator: Box::new(csrsecctp_curvature_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP Curvature Sb High".to_string(),
-            calculator: Box::new(csrsecctp_curvature_sb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_sb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CurvatureCharge High".to_string(),
-            calculator: Box::new(csrsecctp_curvature_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curvature_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP CurvatureCharge MAX".to_string(),
-            calculator: Box::new(csrsecctp_curv_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_curv_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,335 +1,308 @@
-//! CSR Sec CTP Delta Calculations
-
-use crate::helpers::*;
-use sbm::csr_nonsec::delta::csr_nonsec_delta_charge;
-use ultibi::{polars::prelude::max_exprs, BaseMeasure, CPM};
+//! Main Equity Delta Calculator
+//! For construction of Rho Note:
+//! We never have same type AND same issuer since these were netted
+//! ie never APPspot APPspot
+//! APPLspot APPLrepo is 0.999*1 because spot != repo(0.999), and APP APP (1)
+//! APPLspot GOOGspot/APPLrepo GOOGrepo
+//! is 1*0.25 because spot == spot (1) and Goog != App (0.25)
+//! Apprepo Googspot is 0.999*0.25 because repo != spot and App != Goog (0.25)
+//! Hence, it's sufficient to build two matrixes:
+//! 1 based on rft and 2 based on rf
 
 use crate::prelude::*;
+use ultibi::{
+    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
+    BaseMeasure, IntoLazy, CPM,
+};
 
-pub fn total_csr_sec_ctp_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("Delta", "CSR_Sec_CTP", total_delta_sens()))
-}
-/// Helper functions
+use ndarray::Array2;
 
-fn csr_sec_ctp_delta_sens_weighted_05y_bcbs() -> Expr {
-    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_05Y", "SensWeights", 0)
+/// Total Equity Delta Sens
+pub(crate) fn equity_delta_sens(_: &CPM) -> PolarsResult<Expr> {
+    Ok(rc_rcat_sens("Delta", "Equity", col("SensitivitySpot")))
 }
-fn csr_sec_ctp_delta_sens_weighted_1y_bcbs() -> Expr {
-    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_1Y", "SensWeights", 1)
+// wrapper of equity_delta_sens_weighted_spot which takes a param o
+pub(crate) fn equity_delta_sens_weighted(_: &CPM) -> PolarsResult<Expr> {
+    Ok(equity_delta_sens_weighted_spot())
 }
-fn csr_sec_ctp_delta_sens_weighted_3y_bcbs() -> Expr {
-    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_3Y", "SensWeights", 2)
+///
+pub(crate) fn equity_delta_sens_weighted_spot() -> Expr {
+    rc_tenor_weighted_sens("Delta", "Equity", "SensitivitySpot", "SensWeights", 0)
 }
-fn csr_sec_ctp_delta_sens_weighted_5y_bcbs() -> Expr {
-    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_5Y", "SensWeights", 3)
+/// Interm Result: Equity Delta Sb <--> Sb Low == Sb Medium == Sb High
+pub(crate) fn eq_delta_sb(op: &CPM) -> PolarsResult<Expr> {
+    equity_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
 }
-fn csr_sec_ctp_delta_sens_weighted_10y_bcbs() -> Expr {
-    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_10Y", "SensWeights", 4)
+/// Interm Result: Equity Kb Low
+pub(crate) fn eq_delta_kb_low(op: &CPM) -> PolarsResult<Expr> {
+    equity_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
 }
-
-//CRR2
-#[cfg(feature = "CRR2")]
-fn csr_sec_ctp_delta_sens_weighted_05y_crr2() -> Expr {
-    rc_tenor_weighted_sens(
-        "Delta",
-        "CSR_Sec_CTP",
-        "Sensitivity_05Y",
-        "SensWeightsCRR2",
-        0,
-    )
+/// Interm Result: Equity Kb Medium
+pub(crate) fn eq_delta_kb_medium(op: &CPM) -> PolarsResult<Expr> {
+    equity_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
 }
-#[cfg(feature = "CRR2")]
-fn csr_sec_ctp_delta_sens_weighted_1y_crr2() -> Expr {
-    rc_tenor_weighted_sens(
-        "Delta",
-        "CSR_Sec_CTP",
-        "Sensitivity_1Y",
-        "SensWeightsCRR2",
-        1,
-    )
-}
-#[cfg(feature = "CRR2")]
-fn csr_sec_ctp_delta_sens_weighted_3y_crr2() -> Expr {
-    rc_tenor_weighted_sens(
-        "Delta",
-        "CSR_Sec_CTP",
-        "Sensitivity_3Y",
-        "SensWeightsCRR2",
-        2,
-    )
-}
-#[cfg(feature = "CRR2")]
-fn csr_sec_ctp_delta_sens_weighted_5y_crr2() -> Expr {
-    rc_tenor_weighted_sens(
-        "Delta",
-        "CSR_Sec_CTP",
-        "Sensitivity_5Y",
-        "SensWeightsCRR2",
-        3,
-    )
-}
-#[cfg(feature = "CRR2")]
-fn csr_sec_ctp_delta_sens_weighted_10y_crr2() -> Expr {
-    rc_tenor_weighted_sens(
-        "Delta",
-        "CSR_Sec_CTP",
-        "Sensitivity_10Y",
-        "SensWeightsCRR2",
-        4,
-    )
-}
-
-/// Total weighted CSR non-Sec Delta
-/// Not used in calculation
-pub(crate) fn csr_sec_ctp_delta_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    let juri: Jurisdiction = get_jurisdiction(op)?;
-
-    match juri {
-        #[cfg(feature = "CRR2")]
-        Jurisdiction::CRR2 => Ok(csr_sec_ctp_delta_sens_weighted_05y_crr2().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_1y_crr2().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_3y_crr2().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_5y_crr2().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_10y_crr2().fill_null(0.)),
-        Jurisdiction::BCBS => Ok(csr_sec_ctp_delta_sens_weighted_05y_bcbs().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_1y_bcbs().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_3y_bcbs().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_5y_bcbs().fill_null(0.)
-            + csr_sec_ctp_delta_sens_weighted_10y_bcbs().fill_null(0.)),
-    }
-}
-
-//Interm Results
-///Sb is same for each scenario
-pub(crate) fn csr_sec_ctp_delta_sb(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_ctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
+/// Interm Result: Equity Kb High
+pub(crate) fn eq_delta_kb_high(op: &CPM) -> PolarsResult<Expr> {
+    equity_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-pub(crate) fn csr_sec_ctp_delta_kb_low(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_ctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
+///calculate Equity Delta High Capital charge
+pub(crate) fn equity_delta_charge_high(op: &CPM) -> PolarsResult<Expr> {
+    equity_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
-pub(crate) fn csr_sec_ctp_delta_kb_medium(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_ctp_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
+///calculate Equity Delta Medium Capital charge
+pub(crate) fn equity_delta_charge_medium(op: &CPM) -> PolarsResult<Expr> {
+    equity_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
-pub(crate) fn csr_sec_ctp_delta_kb_high(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_ctp_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
+///calculate Equity Delta Low Capital charge
+pub(crate) fn equity_delta_charge_low(op: &CPM) -> PolarsResult<Expr> {
+    equity_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
-///calculate CSR non-Sec Delta Low Capital charge
-pub(crate) fn csr_sec_ctp_delta_charge_low(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_ctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
-}
-
-///calculate CSR non-Sec Delta Medium Capital charge
-pub(crate) fn csr_sec_ctp_delta_charge_medium(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_ctp_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
-}
-
-///calculate CSR non-Sec Delta High Capital charge
-pub(crate) fn csr_sec_ctp_delta_charge_high(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_ctp_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
-}
-
-/// Helper funciton
-/// Extracts relevant fields from OptionalParams
-/// And pass them to the main Delta Charge calculator accordingly
-/// calls csr_nonsec_delta_charge because the calculation is identical
-fn csr_sec_ctp_delta_charge_distributor(
+fn equity_delta_charge_distributor(
     op: &CPM,
     scenario: &'static ScenarioConfig,
     rtrn: ReturnMetric,
 ) -> PolarsResult<Expr> {
     let _suffix = scenario.as_str();
-    let juri: Jurisdiction = get_jurisdiction(op)?;
-
-    // First, obtaining parameters specific to jurisdiciton
-    let (weight, bucket_col, name_rho_vec, gamma, n_buckets, special_bucket) = match juri {
-        #[cfg(feature = "CRR2")]
-        Jurisdiction::CRR2 => (
-            [
-                col("SensWeightsCRR2").arr().get(lit(0)),
-                col("SensWeightsCRR2").arr().get(lit(1)),
-                col("SensWeightsCRR2").arr().get(lit(2)),
-                col("SensWeightsCRR2").arr().get(lit(3)),
-                col("SensWeightsCRR2").arr().get(lit(4)),
-            ],
-            col("BucketCRR2"),
-            Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_crr2),
-            &scenario.csr_ctp_delta_vega_gamma_crr2,
-            18usize,
-            Option::<usize>::None,
-        ),
-        Jurisdiction::BCBS => (
-            [
-                col("SensWeights").arr().get(lit(0)),
-                col("SensWeights").arr().get(lit(1)),
-                col("SensWeights").arr().get(lit(2)),
-                col("SensWeights").arr().get(lit(3)),
-                col("SensWeights").arr().get(lit(4)),
-            ],
-            col("BucketBCBS"),
-            Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_bcbs),
-            &scenario.csr_ctp_delta_vega_gamma_bcbs,
-            16usize,
-            Option::<usize>::None,
-        ),
-    };
-
-    // Checking if request contains overrides
-    let base_csr_ctp_rho_tenor = get_optional_parameter(
+    let eq_gamma = get_optional_parameter_array(
         op,
-        "csr_ctp_delta_diff_tenor_rho_base",
-        &scenario.csr_ctp_delta_diff_tenor_rho_base,
+        format!("eq_delta_gamma{_suffix}").as_str(),
+        &scenario.eq_delta_vega_gamma,
     )?;
-
-    let name_rho_vec = get_optional_parameter_vec(
+    let base_eq_rho_bucket = get_optional_parameter(
         op,
-        "csr_ctp_delta_diff_name_rho_per_bucket_base",
-        &name_rho_vec,
+        "eq_delta_diff_name_rho_per_bucket_base",
+        &scenario.eq_delta_vega_diff_name_rho_per_bucket_base,
     )?;
-
-    let base_csr_ctp_rho_basis = get_optional_parameter(
+    let eq_rho_diff_type = get_optional_parameter(
         op,
-        "csr_ctp_diff_basis_rho_base",
-        &scenario.csr_nonsec_delta_diff_basis_rho_base,
+        "eq_delta_diff_type_rho_base",
+        &scenario.eq_delta_diff_type_rho_base,
     )?;
 
-    let gamma =
-        get_optional_parameter_array(op, format!("csr_ctp_delta_gamma{_suffix}").as_str(), gamma)?;
-
-    // CTP calc is identical to nonSec, with the only exception on rho, gamma and number of buckets
-    Ok(csr_nonsec_delta_charge(
-        weight,
-        base_csr_ctp_rho_tenor,
-        name_rho_vec,
-        base_csr_ctp_rho_basis,
-        bucket_col,
+    Ok(equity_delta_charge(
+        eq_gamma,
+        base_eq_rho_bucket,
+        eq_rho_diff_type,
         scenario.scenario_fn,
-        gamma,
-        n_buckets,
-        special_bucket,
-        "CSR_Sec_CTP",
-        "Delta",
         rtrn,
     ))
 }
 
+/// calculate FX Delta Capital charge
+fn equity_delta_charge<F>(
+    gamma: Array2<f64>,
+    eq_rho_bucket: [f64; 13],
+    eq_rho_diff_type: f64,
+    scenario_fn: F,
+    rtrn: ReturnMetric,
+) -> Expr
+where
+    F: Fn(f64) -> f64 + Sync + Send + Copy + 'static,
+{
+    // inner function
+    apply_multiple(
+        move |columns| {
+            let mut df = df![
+                "rcat" => &columns[0],
+                "rc"   => &columns[1],
+                "b"    => &columns[2],
+                "rf"   => &columns[3],
+                "rft"  => &columns[4],
+                "d"    => &columns[5],
+                "w"    => &columns[6],
+            ]?;
+
+            // 21.4.3 - Netting
+            df = df
+                .lazy()
+                .filter(
+                    col("rc")
+                        .eq(lit("Equity"))
+                        .and(col("rcat").eq(lit("Delta"))),
+                )
+                .with_columns([
+                    when(col("rft").eq(lit("EqSpot")))
+                        .then((col("d") * col("w")).alias("Spot"))
+                        .otherwise(NULL.lit()),
+                    when(col("rft").eq(lit("EqRepo")))
+                        .then((col("d") * col("w")).alias("Repo"))
+                        .otherwise(NULL.lit()),
+                ])
+                .groupby([col("b"), col("rf")])
+                .agg([col("Spot").sum(), col("Repo").sum()])
+                .collect()?;
+
+            if df.height() == 0 {
+                return Ok(Some(Series::new("res", [0.])));
+            };
+
+            // 21.78
+            let kbs_sbs = all_kbs_sbs_two_types(
+                df,
+                13,
+                &eq_rho_bucket,
+                eq_rho_diff_type,
+                scenario_fn,
+                Some(11),
+                &[("Spot", "Repo")],
+                None,
+            )?;
+
+            let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs.into_iter().unzip();
+
+            // Early return Kb or Sb is that is the required metric
+
+            match rtrn {
+                ReturnMetric::Kb => return Ok(Some(Series::new("kbs", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("sbs", [sbs.iter().sum::<f64>()]))),
+                _ => (),
+            }
+
+            across_bucket_agg(kbs, sbs, &gamma, columns[0].len(), SBMChargeType::DeltaVega)
+        },
+        &[
+            col("RiskCategory"),
+            col("RiskClass"),
+            col("BucketBCBS"),
+            col("RiskFactor"),
+            col("RiskFactorType"),
+            col("SensitivitySpot"),
+            col("SensWeights").arr().get(lit(0)),
+        ],
+        GetOutput::from_type(DataType::Float64),
+        true,
+    )
+}
+
 /// Returns max of three scenarios
+///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
-fn csrsecctp_delta_max(op: &CPM) -> PolarsResult<Expr> {
+fn eq_delta_max(op: &CPM) -> PolarsResult<Expr> {
     Ok(max_exprs(&[
-        csr_sec_ctp_delta_charge_low(op)?,
-        csr_sec_ctp_delta_charge_medium(op)?,
-        csr_sec_ctp_delta_charge_high(op)?,
+        equity_delta_charge_low(op)?,
+        equity_delta_charge_medium(op)?,
+        equity_delta_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
-pub(crate) fn csrsecctp_delta_measures() -> Vec<Measure> {
+pub(crate) fn eq_delta_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaSens".to_string(),
-            calculator: Box::new(total_csr_sec_ctp_delta_sens),
+            name: "EQ DeltaSens".to_string(),
+            calculator: std::sync::Arc::new(equity_delta_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaSens Weighted".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_sens_weighted),
+            name: "EQ DeltaSens Weighted".to_string(),
+            calculator: std::sync::Arc::new(equity_delta_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaSb".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_sb),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaSb".to_string(),
+            calculator: std::sync::Arc::new(eq_delta_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaKb Low".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_kb_low),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaKb Low".to_string(),
+            calculator: std::sync::Arc::new(eq_delta_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaKb Medium".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_kb_medium),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaKb Medium".to_string(),
+            calculator: std::sync::Arc::new(eq_delta_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaKb High".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_kb_high),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaKb High".to_string(),
+            calculator: std::sync::Arc::new(eq_delta_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaCharge Low".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_charge_low),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaCharge Low".to_string(),
+            calculator: std::sync::Arc::new(equity_delta_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaCharge Medium".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_charge_medium),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaCharge Medium".to_string(),
+            calculator: std::sync::Arc::new(equity_delta_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaCharge High".to_string(),
-            calculator: Box::new(csr_sec_ctp_delta_charge_high),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaCharge High".to_string(),
+            calculator: std::sync::Arc::new(equity_delta_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec CTP DeltaCharge MAX".to_string(),
-            calculator: Box::new(csrsecctp_delta_max),
-            aggregation: Some("scalar"),
+            name: "EQ DeltaCharge MAX".to_string(),
+            calculator: std::sync::Arc::new(eq_delta_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
+                    .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs`

 * *Files 12% similar despite different names*

```diff
@@ -19,61 +19,64 @@
         + col("CSR Sec CTP CurvatureCharge High"))
 }
 
 pub(crate) fn csrsecctp_total_measures() -> Vec<Measure> {
     vec![
         Measure::Dependant(DependantMeasure {
             name: "CSR Sec CTP TotalCharge Low".to_string(),
-            calculator: Box::new(csrsecctp_total_low),
+            calculator: std::sync::Arc::new(csrsecctp_total_low),
             depends_upon: vec![
                 (
                     "CSR Sec CTP DeltaCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec CTP VegaCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec CTP CurvatureCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "CSR Sec CTP TotalCharge Medium".to_string(),
-            calculator: Box::new(csrsecctp_total_medium),
+            calculator: std::sync::Arc::new(csrsecctp_total_medium),
             depends_upon: vec![
                 (
                     "CSR Sec CTP DeltaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec CTP VegaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec CTP CurvatureCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "CSR Sec CTP TotalCharge High".to_string(),
-            calculator: Box::new(csrsecctp_total_high),
+            calculator: std::sync::Arc::new(csrsecctp_total_high),
             depends_upon: vec![
                 (
                     "CSR Sec CTP DeltaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec CTP VegaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec CTP CurvatureCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs`

 * *Files 17% similar despite different names*

```diff
@@ -120,107 +120,117 @@
 }
 
 /// Exporting Measures
 pub(crate) fn csrsecctp_vega_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaSens".to_string(),
-            calculator: Box::new(total_csrsecctp_vega_sens),
+            calculator: std::sync::Arc::new(total_csrsecctp_vega_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaSens Weighted".to_string(),
-            calculator: Box::new(total_csrsecctp_vega_sens_weighted),
+            calculator: std::sync::Arc::new(total_csrsecctp_vega_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaSb".to_string(),
-            calculator: Box::new(csrsecctp_vega_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaCharge Low".to_string(),
-            calculator: Box::new(csrsecctp_vega_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaKb Low".to_string(),
-            calculator: Box::new(csrsecctp_vega_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaCharge Medium".to_string(),
-            calculator: Box::new(csrsecctp_vega_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaKb Medium".to_string(),
-            calculator: Box::new(csrsecctp_vega_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaCharge High".to_string(),
-            calculator: Box::new(csrsecctp_vega_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaKb High".to_string(),
-            calculator: Box::new(csrsecctp_vega_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec CTP VegaCharge MAX".to_string(),
-            calculator: Box::new(csrsecctp_vega_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecctp_vega_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs`

 * *Files 7% similar despite different names*

```diff
@@ -120,227 +120,249 @@
 }
 
 /// Exporting Measures
 pub(crate) fn csrsecnonctp_curv_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CurvatureDelta".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curv_delta),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curv_delta),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CurvatureDelta Weighted".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curv_delta_weighted),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curv_delta_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP PnLup".to_string(),
-            calculator: Box::new(csr_sec_nonctp_pnl_up),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_pnl_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP PnLdown".to_string(),
-            calculator: Box::new(csr_sec_nonctp_pnl_down),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_pnl_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CVRup".to_string(),
-            calculator: Box::new(csr_sec_nonctp_cvr_up),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_cvr_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CVRdown".to_string(),
-            calculator: Box::new(csr_sec_nonctp_cvr_down),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_cvr_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature KbPlus Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_plus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_plus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature KbMinus Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_minus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_minus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature Kb Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature Sb Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_sb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_sb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CurvatureCharge Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature KbPlus Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_plus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_plus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature KbMinus Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_minus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_minus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature Kb Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature Sb Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_sb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_sb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CurvatureCharge Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature KbPlus High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_plus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_plus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature KbMinus High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_minus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_minus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature Kb High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP Curvature Sb High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_sb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_sb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CurvatureCharge High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_curvature_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_curvature_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP CurvatureCharge MAX".to_string(),
-            calculator: Box::new(csrsecnonctp_curv_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecnonctp_curv_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,381 +1,345 @@
-//! CSR Sec non-CTP Delta Calculations
+//! CSR Sec CTP Delta Calculations
 
-use crate::prelude::*;
-use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput, MeltArgs},
-    BaseMeasure, IntoLazy, CPM,
-};
+use crate::helpers::*;
+use sbm::csr_nonsec::delta::csr_nonsec_delta_charge;
+use ultibi::{polars::prelude::max_exprs, BaseMeasure, CPM};
 
-use ndarray::Array2;
+use crate::prelude::*;
 
-pub fn total_csr_sec_nonctp_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("CSR_Sec_nonCTP", "Delta", total_delta_sens()))
+pub fn total_csr_sec_ctp_delta_sens(_: &CPM) -> PolarsResult<Expr> {
+    Ok(rc_rcat_sens("Delta", "CSR_Sec_CTP", total_delta_sens()))
 }
 /// Helper functions
 
-fn csr_sec_nonctp_delta_sens_weighted_05y_bcbs() -> Expr {
+fn csr_sec_ctp_delta_sens_weighted_05y_bcbs() -> Expr {
+    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_05Y", "SensWeights", 0)
+}
+fn csr_sec_ctp_delta_sens_weighted_1y_bcbs() -> Expr {
+    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_1Y", "SensWeights", 1)
+}
+fn csr_sec_ctp_delta_sens_weighted_3y_bcbs() -> Expr {
+    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_3Y", "SensWeights", 2)
+}
+fn csr_sec_ctp_delta_sens_weighted_5y_bcbs() -> Expr {
+    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_5Y", "SensWeights", 3)
+}
+fn csr_sec_ctp_delta_sens_weighted_10y_bcbs() -> Expr {
+    rc_tenor_weighted_sens("Delta", "CSR_Sec_CTP", "Sensitivity_10Y", "SensWeights", 4)
+}
+
+//CRR2
+#[cfg(feature = "CRR2")]
+fn csr_sec_ctp_delta_sens_weighted_05y_crr2() -> Expr {
     rc_tenor_weighted_sens(
         "Delta",
-        "CSR_Sec_nonCTP",
+        "CSR_Sec_CTP",
         "Sensitivity_05Y",
-        "SensWeights",
+        "SensWeightsCRR2",
         0,
     )
 }
-fn csr_sec_nonctp_delta_sens_weighted_1y_bcbs() -> Expr {
+#[cfg(feature = "CRR2")]
+fn csr_sec_ctp_delta_sens_weighted_1y_crr2() -> Expr {
     rc_tenor_weighted_sens(
         "Delta",
-        "CSR_Sec_nonCTP",
+        "CSR_Sec_CTP",
         "Sensitivity_1Y",
-        "SensWeights",
-        0,
+        "SensWeightsCRR2",
+        1,
     )
 }
-fn csr_sec_nonctp_delta_sens_weighted_3y_bcbs() -> Expr {
+#[cfg(feature = "CRR2")]
+fn csr_sec_ctp_delta_sens_weighted_3y_crr2() -> Expr {
     rc_tenor_weighted_sens(
         "Delta",
-        "CSR_Sec_nonCTP",
+        "CSR_Sec_CTP",
         "Sensitivity_3Y",
-        "SensWeights",
-        0,
+        "SensWeightsCRR2",
+        2,
     )
 }
-fn csr_sec_nonctp_delta_sens_weighted_5y_bcbs() -> Expr {
+#[cfg(feature = "CRR2")]
+fn csr_sec_ctp_delta_sens_weighted_5y_crr2() -> Expr {
     rc_tenor_weighted_sens(
         "Delta",
-        "CSR_Sec_nonCTP",
+        "CSR_Sec_CTP",
         "Sensitivity_5Y",
-        "SensWeights",
-        0,
+        "SensWeightsCRR2",
+        3,
     )
 }
-fn csr_sec_nonctp_delta_sens_weighted_10y_bcbs() -> Expr {
+#[cfg(feature = "CRR2")]
+fn csr_sec_ctp_delta_sens_weighted_10y_crr2() -> Expr {
     rc_tenor_weighted_sens(
         "Delta",
-        "CSR_Sec_nonCTP",
+        "CSR_Sec_CTP",
         "Sensitivity_10Y",
-        "SensWeights",
-        0,
+        "SensWeightsCRR2",
+        4,
     )
 }
 
-/// Total weighted CSR Sec nonCTP Delta
+/// Total weighted CSR non-Sec Delta
 /// Not used in calculation
-pub(crate) fn csr_sec_nonctp_delta_sens_weighted(_: &CPM) -> PolarsResult<Expr> {
-    Ok(csr_sec_nonctp_delta_sens_weighted_05y_bcbs().fill_null(0.)
-        + csr_sec_nonctp_delta_sens_weighted_1y_bcbs().fill_null(0.)
-        + csr_sec_nonctp_delta_sens_weighted_3y_bcbs().fill_null(0.)
-        + csr_sec_nonctp_delta_sens_weighted_5y_bcbs().fill_null(0.)
-        + csr_sec_nonctp_delta_sens_weighted_10y_bcbs().fill_null(0.))
+pub(crate) fn csr_sec_ctp_delta_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
+    let juri: Jurisdiction = get_jurisdiction(op)?;
+
+    match juri {
+        #[cfg(feature = "CRR2")]
+        Jurisdiction::CRR2 => Ok(csr_sec_ctp_delta_sens_weighted_05y_crr2().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_1y_crr2().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_3y_crr2().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_5y_crr2().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_10y_crr2().fill_null(0.)),
+        Jurisdiction::BCBS => Ok(csr_sec_ctp_delta_sens_weighted_05y_bcbs().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_1y_bcbs().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_3y_bcbs().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_5y_bcbs().fill_null(0.)
+            + csr_sec_ctp_delta_sens_weighted_10y_bcbs().fill_null(0.)),
+    }
 }
-//Interm results
-pub(crate) fn csr_sec_nonctp_delta_sb(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_nonctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
+
+//Interm Results
+///Sb is same for each scenario
+pub(crate) fn csr_sec_ctp_delta_sb(op: &CPM) -> PolarsResult<Expr> {
+    csr_sec_ctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
 }
 
-pub(crate) fn csr_sec_nonctp_delta_kb_low(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_nonctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
+pub(crate) fn csr_sec_ctp_delta_kb_low(op: &CPM) -> PolarsResult<Expr> {
+    csr_sec_ctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-pub(crate) fn csr_sec_nonctp_delta_kb_medium(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_nonctp_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
+pub(crate) fn csr_sec_ctp_delta_kb_medium(op: &CPM) -> PolarsResult<Expr> {
+    csr_sec_ctp_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-pub(crate) fn csr_sec_nonctp_delta_kb_high(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_nonctp_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
+pub(crate) fn csr_sec_ctp_delta_kb_high(op: &CPM) -> PolarsResult<Expr> {
+    csr_sec_ctp_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
 ///calculate CSR non-Sec Delta Low Capital charge
-pub(crate) fn csr_sec_nonctp_delta_charge_low(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_nonctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+pub(crate) fn csr_sec_ctp_delta_charge_low(op: &CPM) -> PolarsResult<Expr> {
+    csr_sec_ctp_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
 ///calculate CSR non-Sec Delta Medium Capital charge
-pub(crate) fn csr_sec_nonctp_delta_charge_medium(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_nonctp_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+pub(crate) fn csr_sec_ctp_delta_charge_medium(op: &CPM) -> PolarsResult<Expr> {
+    csr_sec_ctp_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
 ///calculate CSR non-Sec Delta High Capital charge
-pub(crate) fn csr_sec_nonctp_delta_charge_high(op: &CPM) -> PolarsResult<Expr> {
-    csr_sec_nonctp_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+pub(crate) fn csr_sec_ctp_delta_charge_high(op: &CPM) -> PolarsResult<Expr> {
+    csr_sec_ctp_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
 /// Helper funciton
 /// Extracts relevant fields from OptionalParams
 /// And pass them to the main Delta Charge calculator accordingly
 /// calls csr_nonsec_delta_charge because the calculation is identical
-fn csr_sec_nonctp_delta_charge_distributor(
+fn csr_sec_ctp_delta_charge_distributor(
     op: &CPM,
     scenario: &'static ScenarioConfig,
     rtrn: ReturnMetric,
 ) -> PolarsResult<Expr> {
     let _suffix = scenario.as_str();
+    let juri: Jurisdiction = get_jurisdiction(op)?;
 
-    let rho_tenor = get_optional_parameter(
-        op,
-        "csr_sec_nonctp_delta_diff_tenor_rho_base",
-        &scenario.csr_sec_nonctp_delta_diff_tenor_rho_base,
-    )?;
+    // First, obtaining parameters specific to jurisdiciton
+    let (weight, bucket_col, name_rho_vec, gamma, n_buckets, special_bucket) = match juri {
+        #[cfg(feature = "CRR2")]
+        Jurisdiction::CRR2 => (
+            [
+                col("SensWeightsCRR2").arr().get(lit(0)),
+                col("SensWeightsCRR2").arr().get(lit(1)),
+                col("SensWeightsCRR2").arr().get(lit(2)),
+                col("SensWeightsCRR2").arr().get(lit(3)),
+                col("SensWeightsCRR2").arr().get(lit(4)),
+            ],
+            col("BucketCRR2"),
+            Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_crr2),
+            &scenario.csr_ctp_delta_vega_gamma_crr2,
+            18usize,
+            Option::<usize>::None,
+        ),
+        Jurisdiction::BCBS => (
+            [
+                col("SensWeights").arr().get(lit(0)),
+                col("SensWeights").arr().get(lit(1)),
+                col("SensWeights").arr().get(lit(2)),
+                col("SensWeights").arr().get(lit(3)),
+                col("SensWeights").arr().get(lit(4)),
+            ],
+            col("BucketBCBS"),
+            Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_bcbs),
+            &scenario.csr_ctp_delta_vega_gamma_bcbs,
+            16usize,
+            Option::<usize>::None,
+        ),
+    };
 
-    let rho_name = get_optional_parameter_vec(
+    // Checking if request contains overrides
+    let base_csr_ctp_rho_tenor = get_optional_parameter(
         op,
-        "csr_sec_nonctp_delta_diff_name_rho_per_bucket_base",
-        &scenario
-            .csr_sec_nonctp_curv_diff_name_rho_per_bucket
-            .to_vec(),
+        "csr_ctp_delta_diff_tenor_rho_base",
+        &scenario.csr_ctp_delta_diff_tenor_rho_base,
     )?;
 
-    let rho_tranche = get_optional_parameter(
+    let name_rho_vec = get_optional_parameter_vec(
         op,
-        "csr_sec_nonctp_delta_diff_tranche_rho_base",
-        &scenario.csr_sec_nonctp_delta_diff_tranche_rho_base,
+        "csr_ctp_delta_diff_name_rho_per_bucket_base",
+        &name_rho_vec,
     )?;
 
-    let gamma = get_optional_parameter_array(
+    let base_csr_ctp_rho_basis = get_optional_parameter(
         op,
-        format!("csr_sec_nonctp_delta_gamma{_suffix}").as_str(),
-        &scenario.csr_sec_nonctp_delta_vega_gamma,
+        "csr_ctp_diff_basis_rho_base",
+        &scenario.csr_nonsec_delta_diff_basis_rho_base,
     )?;
 
+    let gamma =
+        get_optional_parameter_array(op, format!("csr_ctp_delta_gamma{_suffix}").as_str(), gamma)?;
+
     // CTP calc is identical to nonSec, with the only exception on rho, gamma and number of buckets
-    Ok(csr_sec_nonctp_delta_charge(
-        rho_tenor,
-        rho_name,
-        rho_tranche,
+    Ok(csr_nonsec_delta_charge(
+        weight,
+        base_csr_ctp_rho_tenor,
+        name_rho_vec,
+        base_csr_ctp_rho_basis,
+        bucket_col,
         scenario.scenario_fn,
         gamma,
-        Some(25),
-        "CSR_Sec_nonCTP",
+        n_buckets,
+        special_bucket,
+        "CSR_Sec_CTP",
         "Delta",
         rtrn,
     ))
 }
 
-#[allow(clippy::too_many_arguments)]
-pub(crate) fn csr_sec_nonctp_delta_charge<F>(
-    rho_tenor: f64,
-    rho_name: Vec<f64>,
-    rho_rft: f64,
-    scenario_fn: F,
-    gamma: Array2<f64>,
-    special_bucket: Option<usize>,
-    risk_class: &'static str,
-    risk_cat: &'static str,
-    rtrn: ReturnMetric,
-) -> Expr
-where
-    F: Fn(f64) -> f64 + Sync + Send + Copy + 'static,
-{
-    apply_multiple(
-        move |columns| {
-            let df = df![
-                "rcat" =>   &columns[10],
-                "rc" =>   &columns[0],
-                "rf" =>   &columns[1],
-                "tran"=>  &columns[2],
-                "b" =>    &columns[3],
-                "y05" =>  &columns[4],
-                "y1" =>   &columns[5],
-                "y3" =>   &columns[6],
-                "y5" =>   &columns[7],
-                "y10" =>  &columns[8],
-                "w"   =>  &columns[9]
-            ]?;
-
-            let df = df
-                .lazy()
-                .filter(
-                    col("rc")
-                        .eq(lit(risk_class))
-                        .and(col("rcat").eq(lit(risk_cat))),
-                )
-                .groupby([col("b"), col("rf"), col("tran")])
-                .agg([
-                    (col("y05") * col("w")).sum(),
-                    (col("y1") * col("w")).sum(),
-                    (col("y3") * col("w")).sum(),
-                    (col("y5") * col("w")).sum(),
-                    (col("y10") * col("w")).sum(),
-                ])
-                // No need to fill null here
-                .collect()?;
-
-            if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
-            };
-
-            let ma = MeltArgs {
-                id_vars: vec!["b".to_string(), "rf".to_string(), "tran".to_string()],
-                value_vars: vec![
-                    "y05".to_string(),
-                    "y1".to_string(),
-                    "y3".to_string(),
-                    "y5".to_string(),
-                    "y10".to_string(),
-                ],
-                variable_name: Some("tenor".to_string()),
-                value_name: Some("weighted_sens".to_string()),
-            };
-            let df = df.melt2(ma)?;
-            // 21.4.4 - 21.5.a
-            let kbs_sbs = all_kbs_sbs_onsq(
-                df,
-                "tenor",
-                rho_tenor,
-                "rf",
-                &rho_name,
-                "tran",
-                rho_rft,
-                "weighted_sens",
-                scenario_fn,
-                special_bucket,
-                &None,
-            )?;
-
-            let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs.into_iter().unzip();
-            let res_len = columns[0].len();
-            match rtrn {
-                ReturnMetric::Kb => return Ok(Series::new("kbs", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("sbs", [sbs.iter().sum::<f64>()])),
-                _ => (),
-            }
-
-            // 21.57 OR 325aj
-            // Shape of gamma depends on regulation
-            across_bucket_agg(kbs, sbs, &gamma, res_len, SBMChargeType::DeltaVega)
-        },
-        &[
-            col("RiskClass"),
-            col("RiskFactor"),
-            col("Tranche"),
-            col("BucketBCBS"),
-            col("Sensitivity_05Y"),
-            col("Sensitivity_1Y"),
-            col("Sensitivity_3Y"),
-            col("Sensitivity_5Y"),
-            col("Sensitivity_10Y"),
-            col("SensWeights").arr().get(lit(0)),
-            col("RiskCategory"),
-        ],
-        GetOutput::from_type(DataType::Float64),
-        true,
-    )
-}
-
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
-fn csrsecnonctp_delta_max(op: &CPM) -> PolarsResult<Expr> {
+fn csrsecctp_delta_max(op: &CPM) -> PolarsResult<Expr> {
     Ok(max_exprs(&[
-        csr_sec_nonctp_delta_charge_low(op)?,
-        csr_sec_nonctp_delta_charge_medium(op)?,
-        csr_sec_nonctp_delta_charge_high(op)?,
+        csr_sec_ctp_delta_charge_low(op)?,
+        csr_sec_ctp_delta_charge_medium(op)?,
+        csr_sec_ctp_delta_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
-pub(crate) fn csrsecnonctp_delta_measures() -> Vec<Measure> {
+pub(crate) fn csrsecctp_delta_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaSens".to_string(),
-            calculator: Box::new(total_csr_sec_nonctp_delta_sens),
+            name: "CSR Sec CTP DeltaSens".to_string(),
+            calculator: std::sync::Arc::new(total_csr_sec_ctp_delta_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaSens Weighted".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_sens_weighted),
+            name: "CSR Sec CTP DeltaSens Weighted".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaKb Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_kb_low),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaSb".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaKb Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_kb_medium),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaKb Low".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaKb High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_kb_high),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaKb Medium".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaSb".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_sb),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaKb High".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaCharge Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_charge_low),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaCharge Low".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaCharge Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_charge_medium),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaCharge Medium".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaCharge High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_delta_charge_high),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaCharge High".to_string(),
+            calculator: std::sync::Arc::new(csr_sec_ctp_delta_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "CSR Sec nonCTP DeltaCharge MAX".to_string(),
-            calculator: Box::new(csrsecnonctp_delta_max),
-            aggregation: Some("scalar"),
+            name: "CSR Sec CTP DeltaCharge MAX".to_string(),
+            calculator: std::sync::Arc::new(csrsecctp_delta_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
-                    .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
+                    .and(col("RiskClass").eq(lit("CSR_Sec_CTP"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs`

 * *Files 15% similar despite different names*

```diff
@@ -19,61 +19,64 @@
         + col("CSR Sec nonCTP CurvatureCharge High"))
 }
 
 pub(crate) fn csrsecnonctp_total_measures() -> Vec<Measure> {
     vec![
         Measure::Dependant(DependantMeasure {
             name: "CSR Sec nonCTP TotalCharge Low".to_string(),
-            calculator: Box::new(csrsecnonctp_total_low),
+            calculator: std::sync::Arc::new(csrsecnonctp_total_low),
             depends_upon: vec![
                 (
                     "CSR Sec nonCTP DeltaCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec nonCTP VegaCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec nonCTP CurvatureCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "CSR Sec nonCTP TotalCharge Medium".to_string(),
-            calculator: Box::new(csrsecnonctp_total_medium),
+            calculator: std::sync::Arc::new(csrsecnonctp_total_medium),
             depends_upon: vec![
                 (
                     "CSR Sec nonCTP DeltaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec nonCTP VegaCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec nonCTP CurvatureCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "CSR Sec nonCTP TotalCharge High".to_string(),
-            calculator: Box::new(csrsecnonctp_total_high),
+            calculator: std::sync::Arc::new(csrsecnonctp_total_high),
             depends_upon: vec![
                 (
                     "CSR Sec nonCTP DeltaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec nonCTP VegaCharge High".to_string(),
                     "scalar".to_string(),
                 ),
                 (
                     "CSR Sec nonCTP CurvatureCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs`

 * *Files 6% similar despite different names*

```diff
@@ -94,107 +94,117 @@
 }
 
 /// Exporting Measures
 pub(crate) fn csrsecnonctp_vega_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaSens".to_string(),
-            calculator: Box::new(total_csr_sec_nonctp_vega_sens),
+            calculator: std::sync::Arc::new(total_csr_sec_nonctp_vega_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaSens Weighted".to_string(),
-            calculator: Box::new(total_csr_sec_nonctp_vega_sens_weighted),
+            calculator: std::sync::Arc::new(total_csr_sec_nonctp_vega_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaSb".to_string(),
-            calculator: Box::new(csr_sec_nonctp_vega_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_vega_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaCharge Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_vega_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_vega_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaKb Low".to_string(),
-            calculator: Box::new(csr_sec_nonctp_vega_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_vega_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaCharge Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_vega_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_vega_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaKb Medium".to_string(),
-            calculator: Box::new(csr_sec_nonctp_vega_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_vega_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaCharge High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_vega_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_vega_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaKb High".to_string(),
-            calculator: Box::new(csr_sec_nonctp_vega_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csr_sec_nonctp_vega_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "CSR Sec nonCTP VegaCharge MAX".to_string(),
-            calculator: Box::new(csrsecnonctp_vega_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(csrsecnonctp_vega_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("CSR_Sec_nonCTP"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs`

 * *Files 8% similar despite different names*

```diff
@@ -132,42 +132,42 @@
                 .agg([
                     cvr_up_spot().sum().alias("cvr_up"),
                     cvr_down_spot().sum().alias("cvr_down"),
                 ])
                 .collect()?;
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
             let (kb_plus_cvr_up, kb_minus_cvr_down): (Vec<(f64, f64)>, Vec<(f64, f64)>) =
                 curvature_kb_plus_minus(df, &eq_curv_rho, special_bucket)?;
             let (kb_plus, cvr_up): (Vec<f64>, Vec<f64>) = kb_plus_cvr_up.into_iter().unzip();
             let (kb_minus, cvr_down): (Vec<f64>, Vec<f64>) = kb_minus_cvr_down.into_iter().unzip();
 
             match return_metric {
                 ReturnMetric::KbPlus => {
-                    return Ok(Series::new("res", [kb_plus.iter().sum::<f64>()]))
+                    return Ok(Some(Series::new("res", [kb_plus.iter().sum::<f64>()])))
                 }
                 ReturnMetric::KbMinus => {
-                    return Ok(Series::new("res", [kb_minus.iter().sum::<f64>()]))
+                    return Ok(Some(Series::new("res", [kb_minus.iter().sum::<f64>()])))
                 }
                 _ => (),
             }
 
             // If we want to reuse [kbs_sbs_curvature] the iterator has to be over Option<f64>
             let a = Some;
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs_curvature(
                 kb_plus,
                 kb_minus,
                 cvr_up.into_iter().map(a),
                 cvr_down.into_iter().map(a),
             )?;
             match return_metric {
-                ReturnMetric::Kb => return Ok(Series::new("kbs", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("sbs", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("kbs", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("sbs", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             let phi = phi(&sbs);
             let gamma = phi * eq_curv_gamma.view();
 
             across_bucket_agg(kbs, sbs, &gamma, columns[0].len(), SBMChargeType::Curvature)
@@ -200,227 +200,249 @@
 }
 
 /// Exporting Measures
 pub(crate) fn eq_curv_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "EQ CurvatureDelta".to_string(),
-            calculator: Box::new(eq_curv_delta),
+            calculator: std::sync::Arc::new(eq_curv_delta),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ CurvatureDelta_Weighted".to_string(),
-            calculator: Box::new(eq_curv_delta_weighted),
+            calculator: std::sync::Arc::new(eq_curv_delta_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ PnLup".to_string(),
-            calculator: Box::new(eq_pnl_up),
+            calculator: std::sync::Arc::new(eq_pnl_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ PnLdown".to_string(),
-            calculator: Box::new(eq_pnl_down),
+            calculator: std::sync::Arc::new(eq_pnl_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ CVRup".to_string(),
-            calculator: Box::new(eq_cvr_up),
+            calculator: std::sync::Arc::new(eq_cvr_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ CVRdown".to_string(),
-            calculator: Box::new(eq_cvr_down),
+            calculator: std::sync::Arc::new(eq_cvr_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature KbPlus Medium".to_string(),
-            calculator: Box::new(eq_curvature_kb_plus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_plus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature KbMinus Medium".to_string(),
-            calculator: Box::new(eq_curvature_kb_minus_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_minus_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature Kb Medium".to_string(),
-            calculator: Box::new(eq_curvature_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature Sb Medium".to_string(),
-            calculator: Box::new(eq_curvature_sb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_sb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ CurvatureCharge Medium".to_string(),
-            calculator: Box::new(eq_curvature_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature KbPlus Low".to_string(),
-            calculator: Box::new(eq_curvature_kb_plus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_plus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature KbMinus Low".to_string(),
-            calculator: Box::new(eq_curvature_kb_minus_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_minus_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature Kb Low".to_string(),
-            calculator: Box::new(eq_curvature_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature Sb Low".to_string(),
-            calculator: Box::new(eq_curvature_sb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_sb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ CurvatureCharge Low".to_string(),
-            calculator: Box::new(eq_curvature_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature KbPlus High".to_string(),
-            calculator: Box::new(eq_curvature_kb_plus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_plus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature KbMinus High".to_string(),
-            calculator: Box::new(eq_curvature_kb_minus_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_minus_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature Kb High".to_string(),
-            calculator: Box::new(eq_curvature_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ Curvature Sb High".to_string(),
-            calculator: Box::new(eq_curvature_sb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_sb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ CurvatureCharge High".to_string(),
-            calculator: Box::new(eq_curvature_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curvature_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "EQ CurvatureCharge MAX".to_string(),
-            calculator: Box::new(eq_curv_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(eq_curv_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,298 +1,296 @@
-//! Main Equity Delta Calculator
-//! For construction of Rho Note:
-//! We never have same type AND same issuer since these were netted
-//! ie never APPspot APPspot
-//! APPLspot APPLrepo is 0.999*1 because spot != repo(0.999), and APP APP (1)
-//! APPLspot GOOGspot/APPLrepo GOOGrepo
-//! is 1*0.25 because spot == spot (1) and Goog != App (0.25)
-//! Apprepo Googspot is 0.999*0.25 because repo != spot and App != Goog (0.25)
-//! Hence, it's sufficient to build two matrixes:
-//! 1 based on rft and 2 based on rf
-
 use crate::prelude::*;
 use ultibi::{
     polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
     BaseMeasure, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
-/// Total Equity Delta Sens
-pub(crate) fn equity_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("Delta", "Equity", col("SensitivitySpot")))
-}
-// wrapper of equity_delta_sens_weighted_spot which takes a param o
-pub(crate) fn equity_delta_sens_weighted(_: &CPM) -> PolarsResult<Expr> {
-    Ok(equity_delta_sens_weighted_spot())
+pub fn total_eq_vega_sens(_: &CPM) -> PolarsResult<Expr> {
+    Ok(rc_rcat_sens("Vega", "Equity", total_vega_curv_sens()))
 }
-///
-pub(crate) fn equity_delta_sens_weighted_spot() -> Expr {
-    rc_tenor_weighted_sens("Delta", "Equity", "SensitivitySpot", "SensWeights", 0)
+
+pub fn total_eq_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
+    total_eq_vega_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
 }
-/// Interm Result: Equity Delta Sb <--> Sb Low == Sb Medium == Sb High
-pub(crate) fn eq_delta_sb(op: &CPM) -> PolarsResult<Expr> {
-    equity_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
+///Interm Result
+pub(crate) fn equity_vega_sb(op: &CPM) -> PolarsResult<Expr> {
+    equity_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Sb)
 }
-/// Interm Result: Equity Kb Low
-pub(crate) fn eq_delta_kb_low(op: &CPM) -> PolarsResult<Expr> {
-    equity_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
+pub(crate) fn equity_vega_kb_low(op: &CPM) -> PolarsResult<Expr> {
+    equity_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
 }
-/// Interm Result: Equity Kb Medium
-pub(crate) fn eq_delta_kb_medium(op: &CPM) -> PolarsResult<Expr> {
-    equity_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
+
+///calculate Equity Vega Low Capital charge
+pub(crate) fn equity_vega_charge_low(op: &CPM) -> PolarsResult<Expr> {
+    equity_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
-/// Interm Result: Equity Kb High
-pub(crate) fn eq_delta_kb_high(op: &CPM) -> PolarsResult<Expr> {
-    equity_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
+
+///Interm Result
+pub(crate) fn equity_vega_kb_medium(op: &CPM) -> PolarsResult<Expr> {
+    equity_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-///calculate Equity Delta High Capital charge
-pub(crate) fn equity_delta_charge_high(op: &CPM) -> PolarsResult<Expr> {
-    equity_delta_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+///calculate Equity Vega Low Capital charge
+pub(crate) fn equity_vega_charge_medium(op: &CPM) -> PolarsResult<Expr> {
+    equity_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
-///calculate Equity Delta Medium Capital charge
-pub(crate) fn equity_delta_charge_medium(op: &CPM) -> PolarsResult<Expr> {
-    equity_delta_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+///Interm Result
+pub(crate) fn equity_vega_kb_high(op: &CPM) -> PolarsResult<Expr> {
+    equity_vega_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-///calculate Equity Delta Low Capital charge
-pub(crate) fn equity_delta_charge_low(op: &CPM) -> PolarsResult<Expr> {
-    equity_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+///calculate Equity Vega Low Capital charge
+pub(crate) fn equity_vega_charge_high(op: &CPM) -> PolarsResult<Expr> {
+    equity_vega_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
-fn equity_delta_charge_distributor(
+/// Helper funciton
+/// Extracts relevant fields from OptionalParams
+fn equity_vega_charge_distributor(
     op: &CPM,
     scenario: &'static ScenarioConfig,
     rtrn: ReturnMetric,
 ) -> PolarsResult<Expr> {
     let _suffix = scenario.as_str();
+    //TODO check
     let eq_gamma = get_optional_parameter_array(
         op,
-        format!("eq_delta_gamma{_suffix}").as_str(),
+        format!("eq_vega_gamma{_suffix}").as_str(),
         &scenario.eq_delta_vega_gamma,
     )?;
     let base_eq_rho_bucket = get_optional_parameter(
         op,
-        "eq_delta_diff_name_rho_per_bucket_base",
+        "eq_vega_rho_diff_name_per_bucket_base",
         &scenario.eq_delta_vega_diff_name_rho_per_bucket_base,
     )?;
-    let eq_rho_diff_type = get_optional_parameter(
-        op,
-        "eq_delta_diff_type_rho_base",
-        &scenario.eq_delta_diff_type_rho_base,
-    )?;
+    let eq_vega_rho =
+        get_optional_parameter_array(op, "eq_opt_mat_vega_rho_base", &scenario.base_vega_rho)?;
 
-    Ok(equity_delta_charge(
+    Ok(equity_vega_charge(
+        eq_vega_rho,
         eq_gamma,
-        base_eq_rho_bucket,
-        eq_rho_diff_type,
+        base_eq_rho_bucket.to_vec(),
         scenario.scenario_fn,
         rtrn,
+        Some("11"),
+        "Equity",
     ))
 }
 
-/// calculate FX Delta Capital charge
-fn equity_delta_charge<F>(
+/// calculate Equity Vega Capital charge. Used for Commodity also
+pub(crate) fn equity_vega_charge<F>(
+    opt_mat_rho: Array2<f64>,
     gamma: Array2<f64>,
-    eq_rho_bucket: [f64; 13],
-    eq_rho_diff_type: f64,
+    eq_rho_bucket: Vec<f64>,
     scenario_fn: F,
     rtrn: ReturnMetric,
+    special_bucket: Option<&'static str>,
+    rc: &'static str,
 ) -> Expr
 where
     F: Fn(f64) -> f64 + Sync + Send + Copy + 'static,
 {
     // inner function
     apply_multiple(
         move |columns| {
-            let mut df = df![
+            let df = df![
                 "rcat" => &columns[0],
-                "rc"   => &columns[1],
-                "b"    => &columns[2],
-                "rf"   => &columns[3],
-                "rft"  => &columns[4],
-                "d"    => &columns[5],
-                "w"    => &columns[6],
+                "rc" =>   &columns[1],
+                "b" =>    &columns[2],
+                "rf" =>   &columns[3],
+                "y05" =>  &columns[4],
+                "y1" =>   &columns[5],
+                "y3" =>   &columns[6],
+                "y5" =>   &columns[7],
+                "y10" =>  &columns[8],
+                "wght" => &columns[9],
             ]?;
 
             // 21.4.3 - Netting
-            df = df
+            let df = df
                 .lazy()
-                .filter(
-                    col("rc")
-                        .eq(lit("Equity"))
-                        .and(col("rcat").eq(lit("Delta"))),
-                )
-                .with_columns([
-                    when(col("rft").eq(lit("EqSpot")))
-                        .then((col("d") * col("w")).alias("Spot"))
-                        .otherwise(NULL.lit()),
-                    when(col("rft").eq(lit("EqRepo")))
-                        .then((col("d") * col("w")).alias("Repo"))
-                        .otherwise(NULL.lit()),
-                ])
+                .filter(col("rc").eq(lit(rc)).and(col("rcat").eq(lit("Vega"))))
                 .groupby([col("b"), col("rf")])
-                .agg([col("Spot").sum(), col("Repo").sum()])
+                .agg([
+                    (col("y05") * col("wght")).sum().alias("y05"),
+                    (col("y1") * col("wght")).sum().alias("y1"),
+                    (col("y3") * col("wght")).sum().alias("y3"),
+                    (col("y5") * col("wght")).sum().alias("y5"),
+                    (col("y10") * col("wght")).sum().alias("y10"),
+                ])
+                //.fill_null(0.)
                 .collect()?;
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
+            // Compute present buckets
 
-            // 21.78
-            let kbs_sbs = all_kbs_sbs_two_types(
+            // USE all_kbs_sbs here, this helps skipping unnecessary
+            // iterations over buckets which are not present
+            let kbs_sbs = all_kbs_sbs_single_type(
                 df,
-                13,
+                &opt_mat_rho,
                 &eq_rho_bucket,
-                eq_rho_diff_type,
                 scenario_fn,
-                Some(11),
-                &[("Spot", "Repo")],
-                None,
+                &["y05", "y1", "y3", "y5", "y10"],
+                special_bucket,
             )?;
 
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs.into_iter().unzip();
 
             // Early return Kb or Sb is that is the required metric
-
             match rtrn {
-                ReturnMetric::Kb => return Ok(Series::new("kbs", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("sbs", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("kbs", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("sbs", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             across_bucket_agg(kbs, sbs, &gamma, columns[0].len(), SBMChargeType::DeltaVega)
         },
         &[
             col("RiskCategory"),
             col("RiskClass"),
             col("BucketBCBS"),
             col("RiskFactor"),
-            col("RiskFactorType"),
-            col("SensitivitySpot"),
+            col("Sensitivity_05Y"),
+            col("Sensitivity_1Y"),
+            col("Sensitivity_3Y"),
+            col("Sensitivity_5Y"),
+            col("Sensitivity_10Y"),
             col("SensWeights").arr().get(lit(0)),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
-
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
-fn eq_delta_max(op: &CPM) -> PolarsResult<Expr> {
+fn eq_vega_max(op: &CPM) -> PolarsResult<Expr> {
     Ok(max_exprs(&[
-        equity_delta_charge_low(op)?,
-        equity_delta_charge_medium(op)?,
-        equity_delta_charge_high(op)?,
+        equity_vega_charge_low(op)?,
+        equity_vega_charge_medium(op)?,
+        equity_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
-pub(crate) fn eq_delta_measures() -> Vec<Measure> {
+pub(crate) fn eq_vega_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaSens".to_string(),
-            calculator: Box::new(equity_delta_sens),
+            name: "EQ VegaSens".to_string(),
+            calculator: std::sync::Arc::new(total_eq_vega_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaSens Weighted".to_string(),
-            calculator: Box::new(equity_delta_sens_weighted),
+            name: "EQ VegaSens Weighted".to_string(),
+            calculator: std::sync::Arc::new(total_eq_vega_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaSb".to_string(),
-            calculator: Box::new(eq_delta_sb),
-            aggregation: Some("scalar"),
+            name: "EQ VegaSb".to_string(),
+            calculator: std::sync::Arc::new(equity_vega_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaKb Low".to_string(),
-            calculator: Box::new(eq_delta_kb_low),
-            aggregation: Some("scalar"),
+            name: "EQ VegaKb Low".to_string(),
+            calculator: std::sync::Arc::new(equity_vega_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaKb Medium".to_string(),
-            calculator: Box::new(eq_delta_kb_medium),
-            aggregation: Some("scalar"),
+            name: "EQ VegaCharge Low".to_string(),
+            calculator: std::sync::Arc::new(equity_vega_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaKb High".to_string(),
-            calculator: Box::new(eq_delta_kb_high),
-            aggregation: Some("scalar"),
+            name: "EQ VegaKb Medium".to_string(),
+            calculator: std::sync::Arc::new(equity_vega_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaCharge Low".to_string(),
-            calculator: Box::new(equity_delta_charge_low),
-            aggregation: Some("scalar"),
+            name: "EQ VegaCharge Medium".to_string(),
+            calculator: std::sync::Arc::new(equity_vega_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaCharge Medium".to_string(),
-            calculator: Box::new(equity_delta_charge_medium),
-            aggregation: Some("scalar"),
+            name: "EQ VegaKb High".to_string(),
+            calculator: std::sync::Arc::new(equity_vega_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaCharge High".to_string(),
-            calculator: Box::new(equity_delta_charge_high),
-            aggregation: Some("scalar"),
+            name: "EQ VegaCharge High".to_string(),
+            calculator: std::sync::Arc::new(equity_vega_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ DeltaCharge MAX".to_string(),
-            calculator: Box::new(eq_delta_max),
-            aggregation: Some("scalar"),
+            name: "EQ VegaCharge MAX".to_string(),
+            calculator: std::sync::Arc::new(eq_vega_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
-                    .eq(lit("Delta"))
+                    .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("Equity"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs`

 * *Files 8% similar despite different names*

```diff
@@ -15,37 +15,40 @@
     Ok(col("EQ DeltaCharge High") + col("EQ VegaCharge High") + col("EQ CurvatureCharge High"))
 }
 
 pub(crate) fn eq_total_measures() -> Vec<Measure> {
     vec![
         Measure::Dependant(DependantMeasure {
             name: "EQ TotalCharge Low".to_string(),
-            calculator: Box::new(eq_total_low),
+            calculator: std::sync::Arc::new(eq_total_low),
             depends_upon: vec![
                 ("EQ DeltaCharge Low".to_string(), "scalar".to_string()),
                 ("EQ VegaCharge Low".to_string(), "scalar".to_string()),
                 ("EQ CurvatureCharge Low".to_string(), "scalar".to_string()),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "EQ TotalCharge Medium".to_string(),
-            calculator: Box::new(eq_total_medium),
+            calculator: std::sync::Arc::new(eq_total_medium),
             depends_upon: vec![
                 ("EQ DeltaCharge Medium".to_string(), "scalar".to_string()),
                 ("EQ VegaCharge Medium".to_string(), "scalar".to_string()),
                 (
                     "EQ CurvatureCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "EQ TotalCharge High".to_string(),
-            calculator: Box::new(eq_total_high),
+            calculator: std::sync::Arc::new(eq_total_high),
             depends_upon: vec![
                 ("EQ DeltaCharge High".to_string(), "scalar".to_string()),
                 ("EQ VegaCharge High".to_string(), "scalar".to_string()),
                 ("EQ CurvatureCharge High".to_string(), "scalar".to_string()),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/vega.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,286 +1,289 @@
+use crate::helpers::{get_optional_parameter, get_optional_parameter_array, ReturnMetric};
 use crate::prelude::*;
+use crate::sbm::common::{across_bucket_agg, rc_rcat_sens, total_vega_curv_sens, SBMChargeType};
+use ndarray::{Array1, Array2, Axis};
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
-    BaseMeasure, IntoLazy, CPM,
+    polars::prelude::{apply_multiple, df, max_exprs, DataType, Float64Type, GetOutput},
+    CPM,
 };
+use ultibi::{BaseMeasure, IntoLazy};
 
-use ndarray::Array2;
-
-pub fn total_eq_vega_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("Vega", "Equity", total_vega_curv_sens()))
+pub fn total_fx_vega_sens(_: &CPM) -> PolarsResult<Expr> {
+    Ok(rc_rcat_sens("Vega", "FX", total_vega_curv_sens()))
 }
 
-pub fn total_eq_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    total_eq_vega_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
-}
-///Interm Result
-pub(crate) fn equity_vega_sb(op: &CPM) -> PolarsResult<Expr> {
-    equity_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Sb)
-}
-pub(crate) fn equity_vega_kb_low(op: &CPM) -> PolarsResult<Expr> {
-    equity_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
+pub fn total_fx_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
+    Ok(total_fx_vega_sens(op)? * col("SensWeights").arr().get(lit(0)))
 }
 
-///calculate Equity Vega Low Capital charge
-pub(crate) fn equity_vega_charge_low(op: &CPM) -> PolarsResult<Expr> {
-    equity_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+/// Sb Low == Sb Medium == Sb High
+/// FX Vega Sb is identical to total_fx_vega_sens_weighted
+pub(crate) fn fx_vega_sb(op: &CPM) -> PolarsResult<Expr> {
+    fx_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
 }
 
-///Interm Result
-pub(crate) fn equity_vega_kb_medium(op: &CPM) -> PolarsResult<Expr> {
-    equity_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
+/// Interm Result: FX Vega Low Kb
+pub(crate) fn fx_vega_kb_low(op: &CPM) -> PolarsResult<Expr> {
+    fx_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-///calculate Equity Vega Low Capital charge
-pub(crate) fn equity_vega_charge_medium(op: &CPM) -> PolarsResult<Expr> {
-    equity_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+/// Interm Result: FX Vega Medium Kb
+pub(crate) fn fx_vega_kb_medium(op: &CPM) -> PolarsResult<Expr> {
+    fx_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-///Interm Result
-pub(crate) fn equity_vega_kb_high(op: &CPM) -> PolarsResult<Expr> {
-    equity_vega_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
+/// Interm Result: FX Vega High Kb
+pub(crate) fn fx_vega_kb_high(op: &CPM) -> PolarsResult<Expr> {
+    fx_vega_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::Kb)
 }
 
-///calculate Equity Vega Low Capital charge
-pub(crate) fn equity_vega_charge_high(op: &CPM) -> PolarsResult<Expr> {
-    equity_vega_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+///calculate FX Vega Low Capital charge
+pub(crate) fn fx_vega_charge_low(op: &CPM) -> PolarsResult<Expr> {
+    fx_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+}
+///calculate FX Vega Medium Capital charge
+pub(crate) fn fx_vega_charge_medium(op: &CPM) -> PolarsResult<Expr> {
+    fx_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::CapitalCharge)
+}
+///calculate FX Vega High Capital charge
+pub(crate) fn fx_vega_charge_high(op: &CPM) -> PolarsResult<Expr> {
+    fx_vega_charge_distributor(op, &HIGH_CORR_SCENARIO, ReturnMetric::CapitalCharge)
 }
 
 /// Helper funciton
 /// Extracts relevant fields from OptionalParams
-fn equity_vega_charge_distributor(
+fn fx_vega_charge_distributor(
     op: &CPM,
     scenario: &'static ScenarioConfig,
     rtrn: ReturnMetric,
 ) -> PolarsResult<Expr> {
     let _suffix = scenario.as_str();
-    //TODO check
-    let eq_gamma = get_optional_parameter_array(
+
+    let fx_vega_rho = get_optional_parameter_array(
         op,
-        format!("eq_vega_gamma{_suffix}").as_str(),
-        &scenario.eq_delta_vega_gamma,
+        format!("fx_opt_mat_vega_rho{_suffix}").as_str(),
+        &scenario.fx_opt_mat_vega_rho,
     )?;
-    let base_eq_rho_bucket = get_optional_parameter(
+    let fx_vega_gamma = get_optional_parameter(
         op,
-        "eq_vega_rho_diff_name_per_bucket_base",
-        &scenario.eq_delta_vega_diff_name_rho_per_bucket_base,
+        format!("fx_vega_gamma{_suffix}").as_str(),
+        &scenario.fx_delta_vega_gamma,
     )?;
-    let eq_vega_rho =
-        get_optional_parameter_array(op, "eq_opt_mat_vega_rho_base", &scenario.base_vega_rho)?;
 
-    Ok(equity_vega_charge(
-        eq_vega_rho,
-        eq_gamma,
-        base_eq_rho_bucket.to_vec(),
-        scenario.scenario_fn,
-        rtrn,
-        Some("11"),
-        "Equity",
-    ))
+    fx_vega_charge(fx_vega_rho, fx_vega_gamma, rtrn)
 }
 
-/// calculate Equity Vega Capital charge. Used for Commodity also
-pub(crate) fn equity_vega_charge<F>(
-    opt_mat_rho: Array2<f64>,
-    gamma: Array2<f64>,
-    eq_rho_bucket: Vec<f64>,
-    scenario_fn: F,
+fn fx_vega_charge(
+    fx_vega_rho: Array2<f64>,
+    fx_vega_gamma: f64,
     rtrn: ReturnMetric,
-    special_bucket: Option<&'static str>,
-    rc: &'static str,
-) -> Expr
-where
-    F: Fn(f64) -> f64 + Sync + Send + Copy + 'static,
-{
-    // inner function
-    apply_multiple(
+) -> PolarsResult<Expr> {
+    Ok(apply_multiple(
         move |columns| {
             let df = df![
                 "rcat" => &columns[0],
                 "rc" =>   &columns[1],
                 "b" =>    &columns[2],
-                "rf" =>   &columns[3],
-                "y05" =>  &columns[4],
-                "y1" =>   &columns[5],
-                "y3" =>   &columns[6],
-                "y5" =>   &columns[7],
-                "y10" =>  &columns[8],
-                "wght" => &columns[9],
+                "y05" =>  &columns[3],
+                "y1" =>   &columns[4],
+                "y3" =>   &columns[5],
+                "y5" =>   &columns[6],
+                "y10" =>  &columns[7],
+                "wght" => &columns[8]
             ]?;
 
-            // 21.4.3 - Netting
             let df = df
                 .lazy()
-                .filter(col("rc").eq(lit(rc)).and(col("rcat").eq(lit("Vega"))))
-                .groupby([col("b"), col("rf")])
+                .filter(col("rc").eq(lit("FX")).and(col("rcat").eq(lit("Vega"))))
+                .groupby([col("b")])
                 .agg([
-                    (col("y05") * col("wght")).sum().alias("y05"),
-                    (col("y1") * col("wght")).sum().alias("y1"),
-                    (col("y3") * col("wght")).sum().alias("y3"),
-                    (col("y5") * col("wght")).sum().alias("y5"),
-                    (col("y10") * col("wght")).sum().alias("y10"),
+                    (col("y05") * col("wght")).sum(),
+                    (col("y1") * col("wght")).sum(),
+                    (col("y3") * col("wght")).sum(),
+                    (col("y5") * col("wght")).sum(),
+                    (col("y10") * col("wght")).sum(),
                 ])
-                //.fill_null(0.)
+                .select(&[col("*").exclude(["b"])])
+                .fill_null(lit::<f64>(0.))
                 .collect()?;
 
+            let res_len = columns[0].len();
+
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
-            // Compute present buckets
 
-            // USE all_kbs_sbs here, this helps skipping unnecessary
-            // iterations over buckets which are not present
-            let kbs_sbs = all_kbs_sbs_single_type(
-                df,
-                &opt_mat_rho,
-                &eq_rho_bucket,
-                scenario_fn,
-                &["y05", "y1", "y3", "y5", "y10"],
-                special_bucket,
-            )?;
-
-            let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs.into_iter().unzip();
-
-            // Early return Kb or Sb is that is the required metric
-            match rtrn {
-                ReturnMetric::Kb => return Ok(Series::new("kbs", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("sbs", [sbs.iter().sum::<f64>()])),
-                _ => (),
+            let sens = df.to_ndarray::<Float64Type>()?;
+
+            let sbs = sens.sum_axis(Axis(1));
+
+            // Early return Kb or Sb, ie the required metric
+            if let ReturnMetric::Sb = rtrn {
+                return Ok(Some(Series::new("res", [sbs.sum()])));
+            }
+
+            // Interm step
+            let _kbs = sens.dot(&fx_vega_rho);
+            // Actual kbs
+            // TODO use uninit here
+            let mut kbs = Array1::<f64>::zeros(sbs.len());
+
+            _kbs.axis_iter(Axis(0)).enumerate().for_each(|(i, arr)| {
+                let a = unsafe { kbs.uget_mut(i) };
+                *a = f64::max(arr.dot(&sens.row(i)), 0.).sqrt();
+            });
+
+            if let ReturnMetric::Kb = rtrn {
+                return Ok(Some(Series::new("res", [kbs.sum()])));
             }
 
-            across_bucket_agg(kbs, sbs, &gamma, columns[0].len(), SBMChargeType::DeltaVega)
+            let mut gamma = Array2::from_elem((kbs.len(), kbs.len()), fx_vega_gamma);
+            let zeros = Array1::zeros(kbs.len());
+            gamma.diag_mut().assign(&zeros);
+
+            across_bucket_agg(kbs, sbs, &gamma, res_len, SBMChargeType::DeltaVega)
         },
         &[
             col("RiskCategory"),
             col("RiskClass"),
             col("BucketBCBS"),
-            col("RiskFactor"),
             col("Sensitivity_05Y"),
             col("Sensitivity_1Y"),
             col("Sensitivity_3Y"),
             col("Sensitivity_5Y"),
             col("Sensitivity_10Y"),
             col("SensWeights").arr().get(lit(0)),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
-    )
+    ))
 }
+
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
-fn eq_vega_max(op: &CPM) -> PolarsResult<Expr> {
+fn fx_vega_max(op: &CPM) -> PolarsResult<Expr> {
     Ok(max_exprs(&[
-        equity_vega_charge_low(op)?,
-        equity_vega_charge_medium(op)?,
-        equity_vega_charge_high(op)?,
+        fx_vega_charge_low(op)?,
+        fx_vega_charge_medium(op)?,
+        fx_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
-pub(crate) fn eq_vega_measures() -> Vec<Measure> {
+pub(crate) fn fx_vega_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
-            name: "EQ VegaSens".to_string(),
-            calculator: Box::new(total_eq_vega_sens),
+            name: "FX VegaSens".to_string(),
+            calculator: std::sync::Arc::new(total_fx_vega_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaSens Weighted".to_string(),
-            calculator: Box::new(total_eq_vega_sens_weighted),
+            name: "FX VegaSens Weighted".to_string(),
+            calculator: std::sync::Arc::new(total_fx_vega_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaSb".to_string(),
-            calculator: Box::new(equity_vega_sb),
-            aggregation: Some("scalar"),
+            name: "FX VegaSb".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaKb Low".to_string(),
-            calculator: Box::new(equity_vega_kb_low),
-            aggregation: Some("scalar"),
+            name: "FX VegaKb Low".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaCharge Low".to_string(),
-            calculator: Box::new(equity_vega_charge_low),
-            aggregation: Some("scalar"),
+            name: "FX VegaKb Medium".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaKb Medium".to_string(),
-            calculator: Box::new(equity_vega_kb_medium),
-            aggregation: Some("scalar"),
+            name: "FX VegaKb High".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaCharge Medium".to_string(),
-            calculator: Box::new(equity_vega_charge_medium),
-            aggregation: Some("scalar"),
+            name: "FX VegaCharge Low".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaKb High".to_string(),
-            calculator: Box::new(equity_vega_kb_high),
-            aggregation: Some("scalar"),
+            name: "FX VegaCharge Medium".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaCharge High".to_string(),
-            calculator: Box::new(equity_vega_charge_high),
-            aggregation: Some("scalar"),
+            name: "FX VegaCharge High".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
-            name: "EQ VegaCharge MAX".to_string(),
-            calculator: Box::new(eq_vega_max),
-            aggregation: Some("scalar"),
+            name: "FX VegaCharge MAX".to_string(),
+            calculator: std::sync::Arc::new(fx_vega_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
-                    .and(col("RiskClass").eq(lit("Equity"))),
+                    .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 /// Wrapper used for FX only. Filteres where BucketBCBS is of
 /// th form ...CCY where CCY is the reporting CCY
 fn risk_filtered_by_ccy(op: &CPM, risk: Expr) -> PolarsResult<Expr> {
     let ccy_regex = ccy_regex(op)?;
     Ok(risk.apply_many(
         move |columns| {
-            let mask = columns[1].utf8()?.contains(ccy_regex.as_str())?;
+            let mask = columns[1].utf8()?.contains(ccy_regex.as_str(), false)?;
 
             let res = columns[0].f64()?.set(&!mask, None)?;
 
-            Ok(res.into_series())
+            Ok(Some(res.into_series()))
         },
         &[col("BucketBCBS")],
         GetOutput::from_type(DataType::Float64),
     ))
 }
 /// FX Curvature Delta, filtered by reporting ccy
 pub fn fx_curv_delta(op: &CPM) -> PolarsResult<Expr> {
@@ -52,15 +52,16 @@
     } else {
         apply_multiple(
             |columns| {
                 let mult: Vec<f64> = vec![1.; columns[0].len()];
                 let mult = Float64Chunked::from_vec("multiplicator", mult);
                 let mask = columns[1].bool()?.fill_null_with_values(false)?;
                 let mult = mult.set(&mask, Some(1.5))?.into_series();
-                columns[0].f64()?.divide(&mult)
+                let div = columns[0].f64()?.divide(&mult)?;
+                Ok(Some(div))
             },
             &[risk, col("FxCurvDivEligibility")],
             GetOutput::from_type(DataType::Float64),
             false,
         )
     }
 }
@@ -146,54 +147,56 @@
             let df = df
                 .lazy()
                 .filter(
                     col("rc")
                         .eq(lit("FX"))
                         .and(col("CurvatureRiskWeight").is_not_null())
                         .and(col("b").apply(
-                            move |col| Ok(col.utf8()?.contains(&ccy_regex)?.into_series()),
+                            move |col| {
+                                Ok(Some(col.utf8()?.contains(&ccy_regex, false)?.into_series()))
+                            },
                             GetOutput::from_type(DataType::Boolean),
                         )),
                 )
                 .collect()?;
 
             let res_len = columns[0].len();
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             let df = df
                 .lazy()
                 .groupby([col("b")])
                 .agg([
                     fx_cvr_up_down(div, cvr_up_spot()).sum().alias("cvr_up"),
                     fx_cvr_up_down(div, cvr_down_spot()).sum().alias("cvr_down"),
                 ])
                 .collect()?;
 
             let kb_plus: Vec<f64> = kb_plus_minus_simple(&df["cvr_up"])?;
             if let ReturnMetric::KbPlus = return_metric {
-                return Ok(Series::new("res", [kb_plus.iter().sum::<f64>()]));
+                return Ok(Some(Series::new("res", [kb_plus.iter().sum::<f64>()])));
             }
 
             let kb_minus: Vec<f64> = kb_plus_minus_simple(&df["cvr_down"])?;
             if let ReturnMetric::KbMinus = return_metric {
-                return Ok(Series::new("res", [kb_minus.iter().sum::<f64>()]));
+                return Ok(Some(Series::new("res", [kb_minus.iter().sum::<f64>()])));
             }
 
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs_curvature(
                 kb_plus,
                 kb_minus,
                 df["cvr_up"].f64()?.into_iter(),
                 df["cvr_down"].f64()?.into_iter(),
             )?;
             match return_metric {
-                ReturnMetric::Kb => return Ok(Series::new("res", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("res", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("res", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("res", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             // 325ag
             let mut gamma = Array2::from_elem((kbs.len(), kbs.len()), gamma);
             let phi = phi(&sbs);
             gamma = gamma * phi;
@@ -231,147 +234,161 @@
 }
 
 /// Exporting Measures
 pub(crate) fn fx_curv_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "FX CurvatureDelta".to_string(),
-            calculator: Box::new(fx_curv_delta),
+            calculator: std::sync::Arc::new(fx_curv_delta),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX CurvatureDelta Weighted".to_string(),
-            calculator: Box::new(fx_curv_delta_weighted),
+            calculator: std::sync::Arc::new(fx_curv_delta_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX PnLup".to_string(),
-            calculator: Box::new(fx_pnl_up),
+            calculator: std::sync::Arc::new(fx_pnl_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX PnLdown".to_string(),
-            calculator: Box::new(fx_pnl_down),
+            calculator: std::sync::Arc::new(fx_pnl_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX CVRup".to_string(),
-            calculator: Box::new(fx_cvr_up),
+            calculator: std::sync::Arc::new(fx_cvr_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX CVRdown".to_string(),
-            calculator: Box::new(fx_cvr_down),
+            calculator: std::sync::Arc::new(fx_cvr_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX Curvature KbPlus".to_string(),
-            calculator: Box::new(fx_curvature_kb_plus),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curvature_kb_plus),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX Curvature KbMinus".to_string(),
-            calculator: Box::new(fx_curvature_kb_minus),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curvature_kb_minus),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX Curvature Kb".to_string(),
-            calculator: Box::new(fx_curvature_kb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curvature_kb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX Curvature Sb".to_string(),
-            calculator: Box::new(fx_curvature_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curvature_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX CurvatureCharge Low".to_string(),
-            calculator: Box::new(fx_curvature_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curvature_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX CurvatureCharge Medium".to_string(),
-            calculator: Box::new(fx_curvature_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curvature_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX CurvatureCharge High".to_string(),
-            calculator: Box::new(fx_curvature_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curvature_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX CurvatureCharge MAX".to_string(),
-            calculator: Box::new(fx_curv_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_curv_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs`

 * *Files 17% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 pub(crate) fn fx_delta_sens_repccy(op: &CPM) -> PolarsResult<Expr> {
     let ccy_regex = ccy_regex(op)?;
     Ok(apply_multiple(
         move |columns| {
             let mask1 = columns[0].utf8()?.equal("FX");
 
             // function to take rep_ccy as an argument
-            let mask2 = columns[1].utf8()?.contains(ccy_regex.as_str())?;
+            let mask2 = columns[1].utf8()?.contains(ccy_regex.as_str(), false)?;
 
             // function to take rep_ccy as an argument
             let mask3 = columns[3].utf8()?.equal("Delta");
 
             // Set delta's which don't match mask1 or mask2 to None (ie NaN)
             let delta = columns[2].f64()?.set(&!(mask1 & mask2 & mask3), None)?;
 
-            Ok(delta.into_series())
+            Ok(Some(delta.into_series()))
         },
         &[
             col("RiskClass"),
             col("BucketBCBS"),
             col("SensitivitySpot"),
             col("RiskCategory"),
         ],
@@ -127,47 +127,52 @@
                 "rc"   => &columns[1],
                 "b"    => &columns[2],
                 "d"    => &columns[3],
                 "w"    => &columns[4],
             ]?;
 
             let ccy_regex = ccy_regex.clone();
-            let df = df
+            let mut df = df
                 .lazy()
                 .filter(
                     col("rc")
                         .eq(lit("FX"))
                         .and(col("rcat").eq(lit("Delta")))
                         .and(col("b").apply(
-                            move |col| Ok(col.utf8()?.contains(&ccy_regex)?.into_series()),
+                            move |col| {
+                                Ok(Some(col.utf8()?.contains(&ccy_regex, false)?.into_series()))
+                            },
                             GetOutput::from_type(DataType::Boolean),
                         )),
                 )
                 .groupby([col("b")])
                 .agg([(col("d") * col("w")).sum().alias("dw_sum")])
                 // Drop nulls (ie other reporting ccys)
                 .drop_nulls(Some(vec![col("dw_sum")]))
                 .collect()?;
 
+            df.rechunk();
+
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             //21.4.4 |dw_sum| == kb for FX
             //21.4.5.a sb == dw_sum
             let dw_sum = df["dw_sum"].f64()?.to_ndarray()?; //Ok since we have filtered out NULLs above
                                                             // Early return Kb or Sb, ie the required metric
+            dbg!(&dw_sum);
             let res_len = columns[0].len();
             if let ReturnMetric::Sb = rtrn {
-                return Ok(Series::new("res", [dw_sum.sum()]));
+                return Ok(Some(Series::new("res", [dw_sum.sum()])));
             }
 
             let kbs: Array1<f64> = dw_sum.iter().map(|x| x.abs()).collect();
             if let ReturnMetric::Kb = rtrn {
-                return Ok(Series::new("res", [kbs.sum()]));
+                return Ok(Some(Series::new("res", [kbs.sum()])));
             }
 
             let mut gamma = Array::from_elem((dw_sum.len(), dw_sum.len()), gamma);
             let zeros = Array::zeros(dw_sum.len());
             gamma.diag_mut().assign(&zeros);
 
             across_bucket_agg(
@@ -208,95 +213,103 @@
     //let fx_delta_gamma_low  = FRTB_CALC_PARAMS_MAP.get("fx_delta_gamma_low").unwrap(); // it must be present
     //let fx_delta_gamma_medium  = FRTB_CALC_PARAMS_MAP.get("fx_delta_gamma_medium").unwrap(); // it must be present
     //let fx_delta_gamma_high  = FRTB_CALC_PARAMS_MAP.get("fx_delta_gamma_high").unwrap(); // it must be present
 
     vec![
         Measure::Base(BaseMeasure {
             name: "FX DeltaSens".to_string(),
-            calculator: Box::new(fx_delta_sens_repccy),
+            calculator: std::sync::Arc::new(fx_delta_sens_repccy),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
-            //calc_params: &[*reporting_ccy, *jurisdiction]
+
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX DeltaSens Weighted".to_string(),
-            calculator: Box::new(fx_delta_sens_weighted),
+            calculator: std::sync::Arc::new(fx_delta_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
             //calc_params: &[*reporting_ccy, *jurisdiction]
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX DeltaSb".to_string(),
-            calculator: Box::new(fx_delta_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_delta_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
             //calc_params: &[*reporting_ccy, *jurisdiction, *fx_delta_gamma_low, *fx_delta_gamma_medium, *fx_delta_gamma_high]
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX DeltaKb".to_string(),
-            calculator: Box::new(fx_delta_kb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_delta_kb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
             //calc_params: &[*reporting_ccy, *jurisdiction, *fx_delta_gamma_low, *fx_delta_gamma_medium, *fx_delta_gamma_high]
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX DeltaCharge Low".to_string(),
-            calculator: Box::new(fx_delta_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_delta_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
             //calc_params: &[*reporting_ccy, *jurisdiction, *fx_delta_gamma_low, *fx_delta_gamma_medium, *fx_delta_gamma_high]
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX DeltaCharge Medium".to_string(),
-            calculator: Box::new(fx_delta_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_delta_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
             //calc_params: &[*reporting_ccy, *jurisdiction, *fx_delta_gamma_low, *fx_delta_gamma_medium, *fx_delta_gamma_high]
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX DeltaCharge High".to_string(),
-            calculator: Box::new(fx_delta_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_delta_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
             //calc_params: &[*reporting_ccy, *jurisdiction, *fx_delta_gamma_low, *fx_delta_gamma_medium, *fx_delta_gamma_high]
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "FX DeltaCharge MAX".to_string(),
-            calculator: Box::new(fx_delta_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(fx_delta_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("FX"))),
             ),
             //calc_params: &[*reporting_ccy, *jurisdiction, *fx_delta_gamma_low, *fx_delta_gamma_medium, *fx_delta_gamma_high]
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs`

 * *Files 4% similar despite different names*

```diff
@@ -15,37 +15,40 @@
     Ok(col("FX DeltaCharge High") + col("FX VegaCharge High") + col("FX CurvatureCharge High"))
 }
 
 pub(crate) fn fx_total_measures() -> Vec<Measure> {
     vec![
         Measure::Dependant(DependantMeasure {
             name: "FX TotalCharge Low".to_string(),
-            calculator: Box::new(fx_total_low),
+            calculator: std::sync::Arc::new(fx_total_low),
             depends_upon: vec![
                 ("FX DeltaCharge Low".to_string(), "scalar".to_string()),
                 ("FX VegaCharge Low".to_string(), "scalar".to_string()),
                 ("FX CurvatureCharge Low".to_string(), "scalar".to_string()),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "FX TotalCharge Medium".to_string(),
-            calculator: Box::new(fx_total_medium),
+            calculator: std::sync::Arc::new(fx_total_medium),
             depends_upon: vec![
                 ("FX DeltaCharge Medium".to_string(), "scalar".to_string()),
                 ("FX VegaCharge Medium".to_string(), "scalar".to_string()),
                 (
                     "FX CurvatureCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "FX TotalCharge High".to_string(),
-            calculator: Box::new(fx_total_high),
+            calculator: std::sync::Arc::new(fx_total_high),
             depends_upon: vec![
                 ("FX DeltaCharge High".to_string(), "scalar".to_string()),
                 ("FX VegaCharge High".to_string(), "scalar".to_string()),
                 ("FX CurvatureCharge High".to_string(), "scalar".to_string()),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs`

 * *Files 6% similar despite different names*

```diff
@@ -138,36 +138,36 @@
                     cvr_up().sum().alias("cvr_up"),
                     cvr_down().sum().alias("cvr_down"),
                 ])
                 //.fill_null(lit::<f64>(0.))
                 .collect()?;
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             let kb_plus: Vec<f64> = kb_plus_minus_simple(&df["cvr_up"])?;
             if let ReturnMetric::KbPlus = return_metric {
-                return Ok(Series::new("res", [kb_plus.iter().sum::<f64>()]));
+                return Ok(Some(Series::new("res", [kb_plus.iter().sum::<f64>()])));
             }
 
             let kb_minus: Vec<f64> = kb_plus_minus_simple(&df["cvr_down"])?;
             if let ReturnMetric::KbMinus = return_metric {
-                return Ok(Series::new("res", [kb_minus.iter().sum::<f64>()]));
+                return Ok(Some(Series::new("res", [kb_minus.iter().sum::<f64>()])));
             }
 
             let (kbs, sbs): (Vec<f64>, Vec<f64>) = kbs_sbs_curvature(
                 kb_plus,
                 kb_minus,
                 df["cvr_up"].f64()?.into_iter(),
                 df["cvr_down"].f64()?.into_iter(),
             )?;
             match return_metric {
-                ReturnMetric::Kb => return Ok(Series::new("res", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("res", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("res", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("res", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             let _buckets: Vec<&str> = df["b"]
                 .utf8()?
                 .into_iter()
                 .map(|s| s.unwrap_or("Default"))
@@ -230,147 +230,161 @@
 }
 
 /// Exporting Measures
 pub(crate) fn girr_curv_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "GIRR CurvatureDelta".to_string(),
-            calculator: Box::new(ir_curv_delta),
+            calculator: std::sync::Arc::new(ir_curv_delta),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR PnLup".to_string(),
-            calculator: Box::new(girr_pnl_up),
+            calculator: std::sync::Arc::new(girr_pnl_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR PnLdown".to_string(),
-            calculator: Box::new(girr_pnl_down),
+            calculator: std::sync::Arc::new(girr_pnl_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR CurvatureDelta Weighted".to_string(),
-            calculator: Box::new(girr_curv_delta_weighted),
+            calculator: std::sync::Arc::new(girr_curv_delta_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR CVRup".to_string(),
-            calculator: Box::new(girr_cvr_up),
+            calculator: std::sync::Arc::new(girr_cvr_up),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR CVRdown".to_string(),
-            calculator: Box::new(girr_cvr_down),
+            calculator: std::sync::Arc::new(girr_cvr_down),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR Curvature KbPlus".to_string(),
-            calculator: Box::new(girr_curvature_kb_plus),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curvature_kb_plus),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR Curvature KbMinus".to_string(),
-            calculator: Box::new(girr_curvature_kb_minus),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curvature_kb_minus),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR Curvature Kb".to_string(),
-            calculator: Box::new(girr_curvature_kb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curvature_kb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR Curvature Sb".to_string(),
-            calculator: Box::new(girr_curvature_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curvature_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR CurvatureCharge Low".to_string(),
-            calculator: Box::new(girr_curvature_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curvature_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR CurvatureCharge Medium".to_string(),
-            calculator: Box::new(girr_curvature_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curvature_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR CurvatureCharge High".to_string(),
-            calculator: Box::new(girr_curvature_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curvature_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR CurvatureCharge MAX".to_string(),
-            calculator: Box::new(girr_curv_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_curv_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,15 @@
                         .otherwise(NULL.lit())
                         .alias("Inflation"),
                 ])
                 .select([col("*").exclude(["rft"])])
                 .collect()?;
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             let part = df.partition_by(["b"])?;
 
             let res_buckets_kbs_sbs: PolarsResult<Vec<(String, (f64, f64))>> = part
                 .into_par_iter()
                 .map(|bdf| {
@@ -316,24 +316,24 @@
                         Some((girr_delta_rho_infl, girr_delta_rho_xccy)),
                         None,
                     )
                 })
                 .collect();
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             let (_buckets, (kbs, sbs)): (Vec<String>, (Vec<f64>, Vec<f64>)) =
                 res_buckets_kbs_sbs?.into_iter().unzip();
 
             // Early return Kb or Sb is that is the required metric
             match return_metric {
-                ReturnMetric::Kb => return Ok(Series::new("res", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("res", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("res", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("res", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
             // Need to differentiate between CRR2 and BCBS
             // 325ag
             let mut gamma = match juri {
                 #[cfg(feature = "CRR2")]
                 Jurisdiction::CRR2 => {
@@ -452,107 +452,117 @@
     ]))
 }
 /// Exporting Measures
 pub(crate) fn girr_delta_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaSens".to_string(),
-            calculator: Box::new(total_ir_delta_sens),
+            calculator: std::sync::Arc::new(total_ir_delta_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaSens Weighted".to_string(),
-            calculator: Box::new(girr_delta_sens_weighted),
+            calculator: std::sync::Arc::new(girr_delta_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaSb".to_string(),
-            calculator: Box::new(girr_delta_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaCharge Low".to_string(),
-            calculator: Box::new(girr_delta_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaKb Low".to_string(),
-            calculator: Box::new(girr_delta_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaCharge Medium".to_string(),
-            calculator: Box::new(girr_delta_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaKb Medium".to_string(),
-            calculator: Box::new(girr_delta_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaCharge High".to_string(),
-            calculator: Box::new(girr_delta_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaKb High".to_string(),
-            calculator: Box::new(girr_delta_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR DeltaCharge MAX".to_string(),
-            calculator: Box::new(girr_delta_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_delta_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Delta"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs`

 * *Files 8% similar despite different names*

```diff
@@ -19,40 +19,43 @@
         + col("GIRR CurvatureCharge High"))
 }
 
 pub(crate) fn girr_total_measures() -> Vec<Measure> {
     vec![
         Measure::Dependant(DependantMeasure {
             name: "GIRR TotalCharge Low".to_string(),
-            calculator: Box::new(girr_total_low),
+            calculator: std::sync::Arc::new(girr_total_low),
             depends_upon: vec![
                 ("GIRR DeltaCharge Low".to_string(), "scalar".to_string()),
                 ("GIRR VegaCharge Low".to_string(), "scalar".to_string()),
                 ("GIRR CurvatureCharge Low".to_string(), "scalar".to_string()),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "GIRR TotalCharge Medium".to_string(),
-            calculator: Box::new(girr_total_medium),
+            calculator: std::sync::Arc::new(girr_total_medium),
             depends_upon: vec![
                 ("GIRR DeltaCharge Medium".to_string(), "scalar".to_string()),
                 ("GIRR VegaCharge Medium".to_string(), "scalar".to_string()),
                 (
                     "GIRR CurvatureCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "GIRR TotalCharge High".to_string(),
-            calculator: Box::new(girr_total_high),
+            calculator: std::sync::Arc::new(girr_total_high),
             depends_upon: vec![
                 ("GIRR DeltaCharge High".to_string(), "scalar".to_string()),
                 ("GIRR VegaCharge High".to_string(), "scalar".to_string()),
                 (
                     "GIRR CurvatureCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs`

 * *Files 7% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                     (col("y5") * col("weight")).sum(),
                     (col("y10") * col("weight")).sum(),
                 ])
                 .fill_null(lit::<f64>(0.))
                 .collect()?;
 
             if df.height() == 0 {
-                return Ok(Series::new("res", [0.]));
+                return Ok(Some(Series::new("res", [0.])));
             };
 
             let part = df.partition_by(["b"])?;
             let res_buckets_kbs_sbs: PolarsResult<Vec<((&str, f64), f64)>> = part
                 .par_iter()
                 .map(|bdf| girr_vega_bucket_kb_sb(bdf, &girr_vega_opt_rho))
                 .collect();
@@ -175,16 +175,16 @@
             let buckets_kbs_sbs = res_buckets_kbs_sbs?;
             let (buckets_kbs, sbs): (Vec<(&str, f64)>, Vec<f64>) =
                 buckets_kbs_sbs.into_iter().unzip();
             let (_buckets, kbs): (Vec<&str>, Vec<f64>) = buckets_kbs.into_iter().unzip();
 
             // Early return Kb or Sb, ie the required metric
             match return_metric {
-                ReturnMetric::Kb => return Ok(Series::new("res", [kbs.iter().sum::<f64>()])),
-                ReturnMetric::Sb => return Ok(Series::new("res", [sbs.iter().sum::<f64>()])),
+                ReturnMetric::Kb => return Ok(Some(Series::new("res", [kbs.iter().sum::<f64>()]))),
+                ReturnMetric::Sb => return Ok(Some(Series::new("res", [sbs.iter().sum::<f64>()]))),
                 _ => (),
             }
 
             // 325ag
             let mut gamma = match juri {
                 #[cfg(feature = "CRR2")]
                 Jurisdiction::CRR2 => build_girr_crr2_gamma(
@@ -327,107 +327,117 @@
 }
 
 /// Exporting Measures
 pub(crate) fn girr_vega_measures() -> Vec<Measure> {
     vec![
         Measure::Base(BaseMeasure {
             name: "GIRR VegaSens".to_string(),
-            calculator: Box::new(total_ir_vega_sens),
+            calculator: std::sync::Arc::new(total_ir_vega_sens),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaSens Weighted".to_string(),
-            calculator: Box::new(girr_vega_sens_weighted),
+            calculator: std::sync::Arc::new(girr_vega_sens_weighted),
             aggregation: None,
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaSb".to_string(),
-            calculator: Box::new(girr_vega_sb),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_sb),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaCharge Low".to_string(),
-            calculator: Box::new(girr_vega_charge_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_charge_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaKb Low".to_string(),
-            calculator: Box::new(girr_vega_kb_low),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_kb_low),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaCharge Medium".to_string(),
-            calculator: Box::new(girr_vega_charge_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_charge_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaKb Medium".to_string(),
-            calculator: Box::new(girr_vega_kb_medium),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_kb_medium),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaCharge High".to_string(),
-            calculator: Box::new(girr_vega_charge_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_charge_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaKb High".to_string(),
-            calculator: Box::new(girr_vega_kb_high),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_kb_high),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
         Measure::Base(BaseMeasure {
             name: "GIRR VegaCharge MAX".to_string(),
-            calculator: Box::new(girr_vega_max),
-            aggregation: Some("scalar"),
+            calculator: std::sync::Arc::new(girr_vega_max),
+            aggregation: Some("scalar".into()),
             precomputefilter: Some(
                 col("RiskCategory")
                     .eq(lit("Vega"))
                     .and(col("RiskClass").eq(lit("GIRR"))),
             ),
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/sbm/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/sbm/totals.rs`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 }
 
 pub(crate) fn sbm_total_measures() -> Vec<Measure> {
     vec![
         // Testing dependency
         Measure::Dependant(DependantMeasure {
             name: "SBM Charge Medium".to_string(),
-            calculator: Box::new(sbm_charge_medium_dep),
+            calculator: std::sync::Arc::new(sbm_charge_medium_dep),
             depends_upon: vec![
                 ("FX TotalCharge Medium".to_string(), "scalar".to_string()),
                 ("GIRR TotalCharge Medium".to_string(), "scalar".to_string()),
                 ("EQ TotalCharge Medium".to_string(), "scalar".to_string()),
                 (
                     "CSR Sec nonCTP TotalCharge Medium".to_string(),
                     "scalar".to_string(),
@@ -64,18 +64,19 @@
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity TotalCharge Medium".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "SBM Charge Low".to_string(),
-            calculator: Box::new(sbm_charge_low_dep),
+            calculator: std::sync::Arc::new(sbm_charge_low_dep),
             depends_upon: vec![
                 ("FX TotalCharge Low".to_string(), "scalar".to_string()),
                 ("GIRR TotalCharge Low".to_string(), "scalar".to_string()),
                 ("EQ TotalCharge Low".to_string(), "scalar".to_string()),
                 (
                     "CSR Sec nonCTP TotalCharge Low".to_string(),
                     "scalar".to_string(),
@@ -89,18 +90,19 @@
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity TotalCharge Low".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "SBM Charge High".to_string(),
-            calculator: Box::new(sbm_charge_high_dep),
+            calculator: std::sync::Arc::new(sbm_charge_high_dep),
             depends_upon: vec![
                 ("FX TotalCharge High".to_string(), "scalar".to_string()),
                 ("GIRR TotalCharge High".to_string(), "scalar".to_string()),
                 ("EQ TotalCharge High".to_string(), "scalar".to_string()),
                 (
                     "CSR Sec nonCTP TotalCharge High".to_string(),
                     "scalar".to_string(),
@@ -114,19 +116,21 @@
                     "scalar".to_string(),
                 ),
                 (
                     "Commodity TotalCharge High".to_string(),
                     "scalar".to_string(),
                 ),
             ],
+            calc_params: vec![],
         }),
         Measure::Dependant(DependantMeasure {
             name: "SBM Charge".to_string(),
-            calculator: Box::new(sbm_charge_dep),
+            calculator: std::sync::Arc::new(sbm_charge_dep),
             depends_upon: vec![
                 ("SBM Charge Low".to_string(), "scalar".to_string()),
                 ("SBM Charge Medium".to_string(), "scalar".to_string()),
                 ("SBM Charge High".to_string(), "scalar".to_string()),
             ],
+            calc_params: vec![],
         }),
     ]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/statics.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/statics.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/totals.rs`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 fn sa_charge(_: &CPM) -> PolarsResult<Expr> {
     Ok(col("SBM Charge") + col("DRC Charge") + col("RRAO Charge"))
 }
 
 pub(crate) fn sa_total_measures() -> Vec<Measure> {
     vec![Measure::Dependant(DependantMeasure {
         name: "SA Charge".to_string(),
-        calculator: Box::new(sa_charge),
+        calculator: std::sync::Arc::new(sa_charge),
         depends_upon: vec![
             ("SBM Charge".to_string(), "scalar".to_string()),
             ("DRC Charge".to_string(), "scalar".to_string()),
             ("RRAO Charge".to_string(), "scalar".to_string()),
         ],
+        calc_params: vec![],
     })]
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/src/validate.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/src/validate.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/tests/common/mod.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/tests/common/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     let conf_path = r"data/frtb/datasource_config.toml";
     let conf = read_toml2::<DataSourceConfig>(conf_path)
         .expect("Can not proceed without valid Data Set Up"); //Unrecovarable error
     let mut data: FRTBDataSet = DataSet::from_config(conf);
     data.validate_frame(None, ValidateSet::ALL)
         .expect("failed to validate");
     data.prepare().expect("Failed to prepare");
-    Arc::new(data)
+    std::sync::Arc::new(data)
 });
 
 #[ignore]
 #[allow(dead_code)]
 pub fn assert_results(req: &str, expected_sum: f64, epsilon: Option<f64>) {
     let ep = if let Some(e) = epsilon { e } else { 1e-5 };
     let data_req = serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
```

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/tests/dependant.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/tests/dependant.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/tests/drc.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/tests/drc.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/tests/sbm.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/tests/sbm.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/frtb_engine/tests/sbm_totals.rs` & `ultibi-0.3.0/local_dependencies/frtb_engine/tests/sbm_totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/Cargo.toml` & `ultibi-0.3.0/local_dependencies/ultibi_core/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [package]
 name = "ultibi_core"
-version= "0.2.0"
+version= "0.3.0"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 serde = { version = "1.0", features = ["derive","derive"] }
-polars = { version = "0.25.1", features = [
+polars = { version = "0.28.0", features = [
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
     "csv-file",
     "diagonal_concat",
+    "serde-lazy"
+,
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
     "csv-file",
     "diagonal_concat",
-    "describe",
-] }
+    "describe"] }
 serde_json = "1.0"
 toml = "0.7.2"
 once_cell = "1.12"
 derivative = "2.2"
 #AWS S3
 aws-config = { version = "0.49.0", optional = true }
 aws-sdk-s3 = { version = "0.19.0", optional = true }
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/add_row.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/add_row.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use std::collections::BTreeMap;
 use std::sync::Arc;
 
+use polars::frame::row::Row;
 use polars::functions::diag_concat_df;
-use polars::prelude::{row::Row, AnyValue, DataFrame, Field, PolarsResult, Schema};
+use polars::prelude::{AnyValue, DataFrame, Field, PolarsResult, Schema};
 use serde::{Deserialize, Serialize};
 
 use crate::overrides::string_to_any;
 
 /// wrapper for Additional Rows used in [AggregationRequest]
 #[derive(Serialize, Deserialize, Default, Debug, Clone, PartialEq, Eq, Hash)]
 #[cfg_attr(feature = "openapi", derive(utoipa::ToSchema))]
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/aggregations.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/aggregations.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 //! This module defines supported aggregations
 
 use std::collections::HashMap;
 
 use derivative::Derivative;
 use once_cell::sync::Lazy;
-use polars::prelude::{Expr, QuantileInterpolOptions};
+use polars::{
+    lazy::dsl::lit,
+    prelude::{Expr, QuantileInterpolOptions},
+};
 
 /// To represent availiable agg types living in [BASE_CALCS]
 pub type AggregationName = String;
 pub type FinalColumnName = String;
 pub type AggregationFunction = fn(Expr, &str) -> (Expr, String);
 
 /// The list of supported aggregations will be changing ofter, hence keep it as HashMap
@@ -51,15 +54,15 @@
             },
         ),
         (
             "quantile95low",
             Aggregation {
                 name_suffix: "quantile_95_lower".to_string(),
                 aggregated_expr_fn: Box::new(|e: Expr| {
-                    e.quantile(0.95, QuantileInterpolOptions::Lower)
+                    e.quantile(lit(0.95), QuantileInterpolOptions::Lower)
                 }),
             },
         ),
         (
             "first",
             Aggregation {
                 name_suffix: "first".to_string(),
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/cache.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/datarequest.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/datarequest.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use std::collections::BTreeMap;
 
 use crate::aggregations::AggregationName;
+use crate::filters::FilterE;
 use crate::overrides::Override;
 use crate::MeasureName;
 use crate::{add_row::AdditionalRows, filters::AndOrFltrChain};
 
 use serde::{Deserialize, Serialize};
 
 pub type CPM = BTreeMap<String, String>;
@@ -36,28 +37,28 @@
     // general fields
     /// Name of your request
     /// Usefull when used as a template
     #[serde(default)]
     pub name: Option<String>,
     /// Measure: (Name: String, Action: String) where Name will be looked up in
     /// MeasuresMap of the DataSet
-    pub measures: Vec<(MeasureName, AggregationName)>,
+    pub measures: Vec<(String, String)>,
     /// Which column do you want to Group By?
     pub groupby: Vec<String>,
     /// Filter your data (pre compute),
-    /// Vec<Vec<FilterE>>
+    /// See AndOrFltrChain
     #[serde(default)]
-    pub filters: AndOrFltrChain,
+    pub filters: Vec<Vec<FilterE>>,
     #[serde(default)]
     pub overrides: Vec<Override>,
     #[serde(default, alias = "additionalRows")]
     pub add_row: AdditionalRows,
     /// Map/Dict
     #[serde(default)]
-    pub calc_params: CPM,
+    pub calc_params: BTreeMap<String, String>,
     /// drop rows where all results are NULL or 0
     #[serde(default)]
     pub hide_zeros: bool,
     /// Show totals
     #[serde(default)]
     pub totals: bool,
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/dataset.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/dataset.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::collections::BTreeMap;
+use std::collections::{BTreeMap, HashSet};
 
 use polars::prelude::*;
 use serde::{ser::SerializeMap, Serialize, Serializer};
 
 use crate::cache::{Cache, CacheableDataSet};
 use crate::{derive_basic_measures_vec, execute, Measure, CPM};
 use crate::{CalcParameter, ComputeRequest, DataSourceConfig, MeasuresMap};
@@ -31,62 +31,39 @@
         ultibi_server::run_server(self)
     }
     /// Polars DataFrame clone is cheap:
     /// https://stackoverflow.com/questions/72320911/how-to-avoid-deep-copy-when-using-groupby-in-polars-rust
     /// This method gets the main LazyFrame of the Dataset
     fn get_lazyframe(&self) -> &LazyFrame;
 
-    //// Set LazyFrame of your DataSet
-    //// TODO try make prepare
-    //fn set_lazyframe(self, lf: LazyFrame) -> Self
-    //where
-    //    Self: Sized;
-
     /// Modify lf in place
     fn set_lazyframe_inplace(&mut self, lf: LazyFrame);
 
     /// Get all measures associated with the DataSet
     fn get_measures(&self) -> &MeasuresMap;
 
-    //fn from_config(conf: DataSourceConfig) -> Self
-    //where
-    //    Self: Sized,
-    //{
-    //    let (frame, measure_cols, build_params) = conf.build();
-    //    let mm: MeasuresMap = MeasuresMap::from_iter(measure_cols);
-    //    Self::new(frame, mm, build_params)
-    //}
+    /// See [DataSetBase] and [CalcParameter] for description of the parameters
+    fn new(frame: LazyFrame, mm: MeasuresMap, params: CPM) -> Self
+    where
+        Self: Sized;
 
     /// Cannot be defined since returns Self which is a Struct.
     /// Not possible to call [DataSet::new] either since it's not on self
     fn from_config(conf: DataSourceConfig) -> Self
     where
         Self: Sized,
     {
         let (frame, measure_cols, bp) = conf.build();
         let mm: MeasuresMap = MeasuresMap::from_iter(measure_cols);
         Self::new(frame, mm, bp)
     }
 
-    /// TODO remove this, this is not good for production
-    //fn from_config_for_tests(mut conf: DataSourceConfig, path_to_file_location: &str) -> Self
-    //where
-    //    Self: Sized,
-    //{
-    //    conf.change_path_on_abs_if_not_exist(path_to_file_location);
-    //    let (frame, measure_cols, build_params) = conf.build();
-    //    let mm: MeasuresMap = MeasuresMap::from_iter(measure_cols);
-    //    Self::new(frame, mm, build_params)
-    //}
-
-    /// See [DataSetBase] and [CalcParameter] for description of the parameters
-    fn new(frame: LazyFrame, mm: MeasuresMap, params: CPM) -> Self
-    where
-        Self: Sized;
-
+    /// Either place your desired numeric columns and bespokes in
+    /// *ms and set include_numeric_cols_as_measures = False
+    /// or set your bespokes in *ms and include_numeric_cols_as_measures = True
     /// See [DataSetBase] and [CalcParameter] for description of the parameters
     fn from_vec(
         frame: LazyFrame,
         mut ms: Vec<Measure>,
         include_numeric_cols_as_measures: bool,
         params: CPM,
     ) -> Self
@@ -144,15 +121,23 @@
         } else {
             Ok(self.get_lazyframe().clone())
         }
     }
 
     /// Calc params are used for the UI and hence are totally optional
     fn calc_params(&self) -> Vec<CalcParameter> {
-        vec![]
+        let mut res = vec![];
+
+        for measure in self.get_measures().values() {
+            res.extend_from_slice(measure.calc_params())
+        }
+
+        let hash_res: HashSet<CalcParameter> = res.into_iter().collect();
+
+        hash_res.into_iter().collect()
     }
 
     /// Limits overridable columns which you can override in
     /// See [AggregationRequest::overrides]
     fn overridable_columns(&self) -> Vec<String> {
         self.get_lazyframe()
             .schema()
@@ -233,15 +218,15 @@
 }
 
 // TODO return Result
 pub fn numeric_columns(schema: Arc<Schema>) -> Vec<String> {
     schema
         .iter_fields()
         .filter(|f| f.data_type().is_numeric())
-        .map(|f| f.name)
+        .map(|f| f.name.to_string())
         .collect::<Vec<String>>()
 }
 
 /// restrict columns which can be fields to Utf8 and Bool
 pub fn fields_columns(schema: Arc<Schema>) -> Vec<String> {
     schema
         .iter_fields()
@@ -255,43 +240,43 @@
                     | DataType::Int16
                     | DataType::UInt32
                     | DataType::Int32
                     | DataType::UInt64
                     | DataType::Int64
             )
         })
-        .map(|field| field.name)
+        .map(|field| field.name.to_string())
         .collect::<Vec<String>>()
 }
 
 /// DataTypes supported for overrides are defined in [overrides::string_to_lit]
 pub(crate) fn overrides_columns(schema: Arc<Schema>) -> Vec<String> {
     schema
         .iter_fields()
         .filter(|c| match c.data_type() {
             DataType::Utf8 | DataType::Boolean | DataType::Float64 => true,
             DataType::List(x) => {
                 matches!(x.as_ref(), DataType::Float64)
             }
             _ => false,
         })
-        .map(|c| c.name)
+        .map(|c| c.name.to_string())
         .collect::<Vec<String>>()
 }
 
 impl Serialize for dyn DataSet {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let measures = self
             .get_measures()
             .iter()
-            .map(|(x, m)| (x, *m.aggregation()))
-            .collect::<BTreeMap<&String, Option<&str>>>();
+            .map(|(x, m)| (x, m.aggregation()))
+            .collect::<BTreeMap<&String, &Option<String>>>();
 
         let ordered_measures: BTreeMap<_, _> = measures.iter().collect();
         let utf8_cols = self
             .get_lazyframe()
             .schema()
             .map(fields_columns)
             .unwrap_or_default();
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/acquire.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/acquire.rs`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,34 @@
 /// TODO: calls .validate()
 ///
 /// Then .prepare()
 ///
 /// If streaming is False - also collects
 ///
 /// *`collect` - indicates if DF should be collected
+/// *`prepare` - indicates if DF should be prepared
+/// *`bespoke_measures` - bespoke measures
+
 #[allow(clippy::uninlined_format_args)]
-pub fn build_validate_prepare<DS: DataSet>(
+pub fn config_build_validate_prepare<DS: DataSet>(
     config_path: &str,
     collect: bool,
     prepare: bool,
+    bespoke_measures: MeasuresMap,
 ) -> impl DataSet {
     // Read Config
     let conf = read_toml2::<DataSourceConfig>(config_path)
         .expect("Can not proceed without valid Data Set Up"); //Unrecovarable error
 
     let (lf, measure_vec, build_params) = conf.build();
 
-    let mut data = DS::new(lf, MeasuresMap::from_iter(measure_vec), build_params);
+    let mut mm = MeasuresMap::from_iter(measure_vec);
+    mm.extend(bespoke_measures);
+
+    let mut data = DS::new(lf, mm, build_params);
 
     // If cfg is streaming then we can't collect, otherwise collect to check errors
     if collect {
         let now = Instant::now();
         data.collect().expect("Failed to read frame");
         let elapsed = now.elapsed();
         println!("Time to Read/Aggregate DF: {:.6?}", elapsed);
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/awss3.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/awss3.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use std::sync::Arc;
+
 //use aws_sdk_s3::Region;
 //use aws_config::meta::region::RegionProviderChain;
 use aws_sdk_s3::Client;
 
 //use std::borrow::Cow;
 use futures::future::join_all;
 use tokio::runtime::Builder;
@@ -57,13 +59,13 @@
         .await
         .expect("Failed to collect aggregated bytes");
     let bytes = bytes.into_bytes();
 
     let cursor = std::io::Cursor::new(bytes);
 
     let df = CsvReader::new(cursor)
-        .with_dtypes(Some(schema))
+        .with_dtypes(Some(Arc::new(schema.clone())))
         .finish()
         .expect("Failed to read CSV");
 
     df
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/helpers.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/helpers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::collections::BTreeMap;
 
 use polars::{
     prelude::{
-        col, concat, DataFrame, DataType, Expr, Field, JoinType, LazyCsvReader, LazyFrame, Literal,
-        NamedFrom, PolarsResult, Schema, NULL,
+        col, concat, DataFrame, DataType, Expr, Field, JoinType, LazyCsvReader, LazyFileListReader,
+        LazyFrame, Literal, NamedFrom, PolarsResult, Schema, NULL,
     },
     series::Series,
 };
 
 use crate::{derive_basic_measures_vec, numeric_columns, Measure};
 
 /// creates an empty frame with columns
@@ -32,15 +32,15 @@
 
     let schema = Schema::from_iter(vc);
 
     // if path provided, then we expect it to be of the correct format
     // unrecoverable. Panic if failed to read file
     let lf = LazyCsvReader::new(path)
         .has_header(true)
-        .with_parse_dates(true)
+        .with_try_parse_dates(true)
         .with_dtype_overwrite(Some(&schema))
         //.with_ignore_parser_errors(ignore)
         .finish()
         .unwrap_or_else(|_| panic!("Error reading file: {path}"));
 
     lf
 }
@@ -73,15 +73,15 @@
     // if measures were provided
     let measures = if !measures.is_empty() {
         let schema = concatinated_frame
             .schema()
             .expect("Could not extract Schema");
         let fields = schema
             .iter_fields()
-            .map(|f| f.name)
+            .map(|f| f.name.to_string())
             .collect::<Vec<String>>();
 
         // Checking if each measure is present in DF
         measures.iter().for_each(|col| {
             if !fields.contains(col) {
                 panic!("Measure: {col}, is not part of the fields: {fields:?}",)
             }
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/datasource/mod.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/datasource/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/filters.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/filters.rs`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 pub(crate) fn fltr_neq(c: &str, v: &str) -> Expr {
     match v {
         "null" => col(c).is_not_null(),
         _ => col(c).cast(DataType::Utf8).neq(lit::<&str>(v)),
     }
 }
 
-pub(crate) fn fltr_chain(chain: &AndOrFltrChain) -> Option<Expr> {
+pub fn fltr_chain(chain: &AndOrFltrChain) -> Option<Expr> {
     let mut res: Option<Expr> = None;
 
     // Loop from outer vec to inner
     for inner in chain {
         if !inner.is_empty() {
             let mut it = inner.iter();
             let mut inner_res = it.next().unwrap().to_expr();
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/helpers/searches.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/helpers/searches.rs`

 * *Files 25% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 /// Filters Series by `pat`
 /// Returns unique values
 /// TODO cache function
 pub fn filter_contains_unique(srs: &Series, pat: &str) -> PolarsResult<Series> {
     let mask = srs
         .utf8()?
         .to_lowercase()
-        .contains(pat.to_lowercase().as_str())?;
+        .contains(pat.to_lowercase().as_str(), false)?;
     let filtered = srs.filter(&mask)?;
     // Stable in order to preserve the order for pagination
     filtered.unique_stable()
 }
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/measure.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/measure.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use derivative::Derivative;
 //use derivative::Derivative;
 use polars::prelude::{col, Expr, PolarsError, PolarsResult};
 use serde::Serialize;
 //use serde::Serialize;
-use std::collections::BTreeMap;
+use std::{collections::BTreeMap, sync::Arc};
 
 use crate::{
     aggregations::{Aggregation, AggregationName},
     CPM,
 };
 
 //pub type OCPM = BTreeMap<String, String>;
@@ -16,86 +16,92 @@
 /// This alias to represent a measure name, a unique string
 pub type MeasureName = String;
 
 /// (Measure Name, Measure)
 pub type MeasuresMap = BTreeMap<MeasureName, Measure>;
 
 //type Calculator = Box<dyn Fn(&OCP) -> Expr + Send + Sync>;
-type Calculator = Box<dyn Fn(&CPM) -> PolarsResult<Expr> + Send + Sync>;
+pub type Calculator = Arc<dyn Fn(&CPM) -> PolarsResult<Expr> + Send + Sync>;
 
 /// This struct is purely for DataSet descriptive purposes(for now).
 /// Recall measure may take parameters in form of HashMap<paramName, paramValue>
 /// This struct returns all possible paramNames for the given Dataset (for UI purposes only)
-#[derive(Debug, Default, Clone, Copy, Serialize)]
+#[derive(Debug, Default, Clone, Serialize, Hash, PartialEq, Eq)]
 pub struct CalcParameter {
-    pub name: &'static str,
-    pub default: Option<&'static str>,
-    pub type_hint: Option<&'static str>,
+    pub name: String,
+    pub default: Option<String>,
+    pub type_hint: Option<String>,
 }
 
 /// Measure is the essentially a Struct of a calculator and a name
-//#[derive(Clone)]
+#[derive(Clone)]
 pub struct BaseMeasure {
     pub name: MeasureName,
     /// Main function which performs the calculation
     /// Executed in .groupby().agg() context
     pub calculator: Calculator,
 
     // TODO find a nice way to attach calc_params to a measure
     // parameters which will go into calculator
-    //pub calc_params: &'static [CalcParameter],
+    // pub calc_params: &'static [CalcParameter],
     /// Optional: this field is to restrict aggregation option to certain type only
     /// for example where it makes sence to aggregate with "first" and not "sum"
-    pub aggregation: Option<&'static str>,
+    pub aggregation: Option<String>,
 
     /// Optional
     /// Say you want to compute CSR Delta by Bucket
     ///
     /// You are only interested in CSR Buckets, all other would be 0,
     /// So we want to avoid unnecessary calculations.
     ///
     /// This field is an optional filter on DataFrame, placed PRIOR to the computation
     pub precomputefilter: Option<Expr>,
+
+    /// Calc params
+    /// Will determine the list of Params in the UI
+    pub calc_params: Vec<CalcParameter>,
 }
 
-//
-//BaseMeasure (EXPR)
 /// Dependant Measure cannot be computed directly. Instead it is broken down into it's parents
 /// parents get executed, and then used to compute the DependantMeasure.
 ///
 /// Useful for caching.
 ///
 /// No precomputefilter - it is inherited from parents
 #[derive(Derivative)]
 #[derivative(Debug)]
+#[derive(Clone)]
 pub struct DependantMeasure {
     pub name: MeasureName,
 
     /// executed within .with_columns() context
     #[derivative(Debug = "ignore")]
     pub calculator: Calculator, // MAX, SUM...
 
-    /// parameters which will go into calculator
+    // parameters which will go into calculator
     // pub calc_params: Vec<String>,
 
     // this field is to restrict aggregation option to certain type only
     // for example where it makes sence to aggregate with "first" and not "sum"
     // must be one of BASE_CALCS
     // Currently every dep measure is "scalar", see [Measure::aggregation]
     // pub aggregation: Option<&'static str>,
-
     /// Vec<(Depends Upon Measure Name, Aggregation type)>
     /// eg vec![(FXDeltaCharge, scalar), (Sensitivity, mean)]
     pub depends_upon: Vec<(String, String)>,
+
+    /// Calc params
+    /// Will determine the list of Params in the UI
+    pub calc_params: Vec<CalcParameter>,
 }
 
 /// AggRequest --> execute -->  split DependantMeasure into BaseMeasure's (BaseMeasure leave as they are) --> execute_aggregation --> combine back into original request
 /// make cahce default (ie not a feature)
 /// do not change the OUTPUT of any existing .get_measures() - because user/client does not/should not care about what kind of measure they are calling
-//#[derive(Clone)]
+#[derive(Clone)]
 pub enum Measure {
     /// A typical measure
     /// execute_aggregation .groupby().agg(X)
     Base(BaseMeasure),
     /// DependantMeasure depends on BaseMeasure
     /// Executed within .with_columns() context
     Dependant(DependantMeasure),
@@ -119,57 +125,65 @@
         I: IntoIterator<Item = Measure>,
     {
         v.into_iter()
             .map(|measure| (measure.name().clone(), measure))
             .collect()
     }
 }
+use once_cell::sync::Lazy;
+pub(crate) static SCALAR: Lazy<Option<String>> = Lazy::new(|| Some("scalar".into()));
 
 impl Measure {
-    pub fn aggregation(&self) -> &Option<&'static str> {
+    pub fn aggregation(&self) -> &Option<String> {
         match self {
             Measure::Base(BaseMeasure { aggregation, .. }) => aggregation,
-            Measure::Dependant(_) => &Some("scalar"),
+            Measure::Dependant(_) => &SCALAR,
         }
     }
 
     pub fn name(&self) -> &MeasureName {
         match self {
             Measure::Base(BaseMeasure { name, .. })
             | Measure::Dependant(DependantMeasure { name, .. }) => name,
         }
     }
+    pub fn calc_params(&self) -> &Vec<CalcParameter> {
+        match self {
+            Measure::Base(BaseMeasure { calc_params, .. })
+            | Measure::Dependant(DependantMeasure { calc_params, .. }) => calc_params,
+        }
+    }
     pub fn calculator(&self) -> &Calculator {
         match self {
             Measure::Base(BaseMeasure { calculator, .. })
             | Measure::Dependant(DependantMeasure { calculator, .. }) => calculator,
         }
     }
 }
 
 impl Default for BaseMeasure {
     fn default() -> BaseMeasure {
         BaseMeasure {
             name: "Default".into(),
-            calculator: Box::new(|_: &CPM| Ok(col("*"))),
-            //calc_params: &[],
+            calculator: Arc::new(|_: &CPM| Ok(col("*"))),
+            calc_params: vec![],
             aggregation: None,
             precomputefilter: None,
         }
     }
 }
 
 pub fn derive_basic_measures_vec(dataset_numer_cols: Vec<String>) -> Vec<Measure> {
     dataset_numer_cols
         .iter()
         .map(|x| {
             let y = x.clone();
             Measure::Base(BaseMeasure {
                 name: x.clone(),
-                calculator: Box::new(move |_| Ok(col(y.as_str()))),
+                calculator: Arc::new(move |_| Ok(col(y.as_str()))),
                 ..Default::default()
             })
         })
         .collect::<Vec<Measure>>()
 }
 
 /// This is the main [Measure] processed, ie it holds the final name, final Expr(with aggregation)
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/src/overrides.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/src/overrides.rs`

 * *Files 4% similar despite different names*

```diff
@@ -113,30 +113,30 @@
         "Argument {value} could not be parsed into column {column_name} format. Argument should be a {dt}",
     );
 
     match dt {
         // RW column is a list for example
         DataType::List(x) => match **x {
             DataType::Float64 => serde_json::from_str::<Vec<f64>>(value)
-                .map_err(|_| PolarsError::SchemaMisMatch(emsg.into()))
+                .map_err(|_| PolarsError::SchemaMismatch(emsg.into()))
                 .map(|vc| AnyValue::List(Series::from_vec("NewVal", vc))),
-            _ => Err(PolarsError::SchemaMisMatch(
+            _ => Err(PolarsError::SchemaMismatch(
                 "Only List f64 columns can be overwritten".into(),
             )),
         },
         // All Numeric columns are f64
         DataType::Float64 => {
             let f = serde_json::from_str::<f64>(value)
-                .map_err(|_| PolarsError::SchemaMisMatch(emsg.into()))?;
+                .map_err(|_| PolarsError::SchemaMismatch(emsg.into()))?;
             Ok(AnyValue::Float64(f))
         }
         // Boolean column
         DataType::Boolean => Ok(AnyValue::Boolean(
             serde_json::from_str::<bool>(value)
-                .map_err(|_| PolarsError::SchemaMisMatch(emsg.into()))?,
+                .map_err(|_| PolarsError::SchemaMismatch(emsg.into()))?,
         )),
         // All Other columns are
         DataType::Utf8 => Ok(AnyValue::Utf8(value)),
 
         _ => Err(PolarsError::ComputeError(
             format!("Column {column_name} of this format cannot be overwritten",).into(),
         )),
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/add_row.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/agg_request.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/agg_request.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/aggregations.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/common/mod.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/common/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -33,27 +33,29 @@
         .collect();
 
     let df = LazyCsvReader::new(path).finish().unwrap();
 
     let measures = vec![
         Measure::Dependant(DependantMeasure {
             name: "DivAge".to_string(),
-            calculator: Box::new(|op: &CPM| {
+            calculator: Arc::new(|op: &CPM| {
                 let n = op.get("count").unwrap().parse::<f64>().unwrap();
                 Ok(col("Age_sum") / n.into())
             }),
             depends_upon: vec![("Age".to_string(), "sum".to_string())],
+            calc_params: vec![],
         }),
         DependantMeasure {
             name: "NoSuchMeasureTest".to_string(),
-            calculator: Box::new(|op: &CPM| {
+            calculator: Arc::new(|op: &CPM| {
                 let n = op.get("count").unwrap().parse::<f64>().unwrap();
                 Ok(col("NoSuchMeasure_sum") / n.into())
             }),
             depends_upon: vec![("NoSuchMeasure".to_string(), "sum".to_string())],
+            calc_params: vec![],
         }
         .into(),
     ];
 
     let mut data: DataSetBase = DataSet::from_vec(df, measures, true, Default::default());
 
     data.prepare().unwrap();
```

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/datasource.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/dependants.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/dependants.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/local_dependencies/ultibi_core/tests/filters.rs` & `ultibi-0.3.0/local_dependencies/ultibi_core/tests/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/Cargo.toml` & `ultibi-0.3.0/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [package]
 name = "pyultima"
-version= "0.2.0"
+version= "0.3.0"
 edition = "2021"
 publish = false
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ultibi"
 crate-type = ["cdylib"]
 
 [package.metadata.maturin]
 name = "ultibi.rust_module.ultima_pyengine"
 
 [dependencies]
 pyo3 = { version = "0.18.1", features = ["extension-module", "abi3-py37"] }
-polars = { version = "0.25.1", features = [
+polars = { version = "0.28.0", features = [
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
     "csv-file",
     "diagonal_concat",
+    "serde-lazy"
 ] }
-polars-arrow = "0.25.1"
+polars-arrow = "0.28.0"
 ultibi = { path = "local_dependencies/ultibi", features=["ui"] }
 frtb_engine = { path = "local_dependencies/frtb_engine", features=["CRR2"] }
 serde_json = "1.0"
 thiserror = "1.0.38"
+once_cell = "1.17.1"
 
 [features]
```

### Comparing `ultibi-0.2.0/.gitignore` & `ultibi-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/Makefile` & `ultibi-0.3.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	$(VENV_BIN)/pip install -r requirements-lint.txt
 
 .PHONY: develop
 build: venv  ## Compile and install Polars for development
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate && maturin develop
 
 .PHONY: build
-build: venv  ## Compile and install Polars for development
+build: venv  ## Build whl
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate && maturin build -i=$(PY311) --release
 
 .PHONY: develop-release
 build-release: venv  ## Compile and install a faster Polars binary
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate && maturin develop --release
 
 .PHONY: fmt
```

### Comparing `ultibi-0.2.0/example.py` & `ultibi-0.3.0/example.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/pyproject.toml` & `ultibi-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/src/conversion.rs` & `ultibi-0.3.0/src/conversions/series.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #![allow(dead_code)]
 
+use std::collections::HashMap;
+
 use arrow::ffi;
 use polars::prelude::*;
 use polars_arrow::export::arrow;
 use pyo3::exceptions::PyValueError;
 use pyo3::ffi::Py_uintptr_t;
 use pyo3::prelude::*;
+use pyo3::types::IntoPyDict;
 use pyo3::{PyAny, PyObject, PyResult};
 
 /// Take an arrow array from python and convert it to a rust arrow array.
 /// This operation does not copy data.
 fn array_to_rust(arrow_array: &PyAny) -> PyResult<ArrayRef> {
     // prepare a pointer to receive the Array struct
     let array = Box::new(ffi::ArrowArray::empty());
@@ -80,15 +83,16 @@
         // pyarrow array
         let pyarrow_array = to_py_array(py, pyarrow, array)?;
 
         // import polars
         let polars = py.import("polars").expect("Install polars first");
         let out = polars.call_method1("from_arrow", (pyarrow_array,))?;
         // Have to rename now since it doesn't work in to_py_array schema
-        out.call_method1("rename", (name, true))?;
+        let kwargs = HashMap::from([("in_place", true)]);
+        out.call_method("rename", (name,), Some(kwargs.into_py_dict(py)))?;
 
         Ok(out.to_object(py))
     })
 }
 
 pub fn rust_dataframe_to_py_series(dataframe: &DataFrame) -> PyResult<PyObject> {
     let columns = dataframe.get_columns();
```

### Comparing `ultibi-0.2.0/src/errors.rs` & `ultibi-0.3.0/src/errors.rs`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,25 @@
 impl std::convert::From<PyUltimaErr> for PyErr {
     fn from(err: PyUltimaErr) -> PyErr {
         //let default = || PyRuntimeError::new_err(format!("{:?}", &err));
 
         use PyUltimaErr::*;
         match &err {
             Polars(err) => match err {
-                PolarsError::NotFound(name) => NotFoundError::new_err(name.to_string()),
+                PolarsError::ColumnNotFound(name) => NotFoundError::new_err(name.to_string()),
                 PolarsError::ComputeError(err) => ComputeError::new_err(err.to_string()),
+                PolarsError::SchemaFieldNotFound(err) => {
+                    SchemaFieldNotFound::new_err(err.to_string())
+                }
+                PolarsError::StructFieldNotFound(err) => {
+                    StructFieldNotFound::new_err(err.to_string())
+                }
                 PolarsError::NoData(err) => NoDataError::new_err(err.to_string()),
-                PolarsError::ShapeMisMatch(err) => ShapeError::new_err(err.to_string()),
-                PolarsError::SchemaMisMatch(err) => SchemaError::new_err(err.to_string()),
+                PolarsError::ShapeMismatch(err) => ShapeError::new_err(err.to_string()),
+                PolarsError::SchemaMismatch(err) => SchemaError::new_err(err.to_string()),
                 PolarsError::Io(err) => PyIOError::new_err(err.to_string()),
                 PolarsError::ArrowError(err) => ArrowErrorException::new_err(format!("{err}")),
                 PolarsError::Duplicate(err) => DuplicateError::new_err(err.to_string()),
                 PolarsError::InvalidOperation(err) => {
                     InvalidOperationError::new_err(err.to_string())
                 }
             },
@@ -67,7 +73,9 @@
 create_exception!(exceptions, ArrowErrorException, PyException);
 create_exception!(exceptions, ShapeError, PyException);
 create_exception!(exceptions, SchemaError, PyException);
 create_exception!(exceptions, DuplicateError, PyException);
 create_exception!(exceptions, InvalidOperationError, PyException);
 create_exception!(exceptions, SerdeJsonError, PyException);
 create_exception!(exceptions, OtherError, PyException);
+create_exception!(exceptions, SchemaFieldNotFound, PyException);
+create_exception!(exceptions, StructFieldNotFound, PyException);
```

### Comparing `ultibi-0.2.0/src/requests.rs` & `ultibi-0.3.0/src/requests.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/tests/data/datasource_config.toml` & `ultibi-0.3.0/tests/data/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/tests/docs/run_doc_examples.py` & `ultibi-0.3.0/tests/docs/run_doc_examples.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/tests/unit/test_compute.py` & `ultibi-0.3.0/tests/unit/test_compute.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,7 +15,11 @@
         request = dict(measures=[["a", "sum"]], groupby=["c"])
 
         result = ds.compute(request)
 
         expected = pl.DataFrame({"c": ["a", "b"], "a_sum": [3, 3]})
 
         self.assertTrue(result.frame_equal(expected))
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `ultibi-0.2.0/tests/unit/test_ds.py` & `ultibi-0.3.0/tests/unit/test_ds.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
         frame = dataset.frame()
 
         dataset.validate()
 
         dataset.prepare()
 
-        assert "jurisdiction" in [cp["name"] for cp in dataset.calc_params]
+        assert "jurisdiction" in [cp[0] for cp in dataset.calc_params]
         assert "FX Curvature KbMinus" in dataset.measures
         assert isinstance(frame, pl.DataFrame)
         assert "TradeId" in frame
 
     def test_ds_from_frame(self) -> None:
         data = {"a": [1, 2, 3], "b": [4, 5, 6], "c": ["a", "a", "b"]}
         df = pl.DataFrame(data)
```

### Comparing `ultibi-0.2.0/ultibi/internals/dataset.py` & `ultibi-0.3.0/ultibi/internals/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 from __future__ import annotations
 
 from typing import Any, Type, TypeVar
 
 import polars as pl
 
 import ultibi.internals as uli
+from ultibi.internals.measure import Measure
 
 from ..rust_module.ultima_pyengine import DataSetWrapper
 
+TMeasure = TypeVar("TMeasure", bound=Measure)
+
+
 # Create a generic variable that can be 'Parent', or any subclass.
 DS = TypeVar("DS", bound="DataSet")
 
 
 class DataSet:
     """
     Main DataSet class
 
     Holds data, optionally validates and prepares Data,
      and finally executes request.
     """
 
-    ds: DataSetWrapper
+    inner: DataSetWrapper
     prepared: bool
 
     def __init__(self, ds: DataSetWrapper, prepared: bool = False) -> None:
-        self._ds = ds
+        """
+        Class constructor - not to br called directly.
+        call .from_frame() or .from_config()
+        """
+        self.inner = ds
         self.prepared = prepared
 
         """All column which you can group by. Currently those are string 
             and bool columns
         """
-        self.fields: list[str] = self._ds.fields()
+        self.fields: list[str] = self.inner.fields()
 
         """{measureName: "aggtype restriction(if any, otherwise
             None)"}. If none, then you can use any of the availiable agg operations.
             Check :func:`~ultima.internals.aggregation_ops` for supported aggregation
              operations
         """
-        self.measures: "dict[str, str | None]" = self._ds.measures()
+        self.measures: "dict[str, str | None]" = self.inner.measures()
 
         """parameters which you can pass to the Request for the given DataSet
 
         Returns:
             list[dict[str, str|None]]: List of {"name": parameter name to be
             passed to the request, "hint": type hint of the param}
         """
-        self.calc_params: "list[dict[str, str|None]]" = self._ds.calc_params()
+        self.calc_params: "list[tuple[str, str|None, str|None]]" = (
+            self.inner.calc_params()
+        )
 
     @classmethod
     def from_config_path(
         cls: Type[DS], path: str, collect: bool = True, prepare: bool = False
     ) -> DS:
         """
         Reads path to <config>.toml
@@ -69,60 +79,68 @@
     @classmethod
     def from_frame(
         cls: Type[DS],
         df: pl.DataFrame,
         measures: "list[str] | None" = None,
         build_params: "dict[str, str] | None" = None,
         prepared: bool = True,
+        bespoke_measures: "list[TMeasure] | None" = None,
     ) -> DS:
         """
         Build DataSet directly from df
 
         Args:
             cls (Type[T]): _description_
             df (polars.DataFrame): _description_
-            measures (list[str], optional): Used as a constrained on measures.
+            measures (list[str], optional): Used as a constrained on which columns are
+                measures.
                 Defaults to all numeric columns in the dataframe.
             build_params (dict | None, optional): Params to be used in prepare. Defaults
              to None.
             prepared (bool, optional): Was your DataFrame already prepared? Defaults
             to True.
 
         Returns:
             T: Self
         """
-        return cls(DataSetWrapper.from_frame(df, measures, build_params), prepared)
+        bespoke_measures = (
+            [m.inner for m in bespoke_measures] if bespoke_measures else None
+        )
+        return cls(
+            DataSetWrapper.from_frame(df, measures, build_params, bespoke_measures),
+            prepared,
+        )
 
     def prepare(self, collect: bool = True) -> None:
         """Does nothing unless overriden. To be used for one of computations.
             eg Weights Assignments
 
         Args:
             collect (cool): non-lazy mode. Evaluates.
 
         Raises:
             OtherError: Calling prepare on an already prepared dataset
         """
         if not self.prepared:
-            self._ds.prepare(collect)
+            self.inner.prepare(collect)
             self.prepared = True
         else:
             raise uli.OtherError("Calling prepare on an already prepared dataset")
 
     def validate(self) -> None:
         """Raises:
            uli.NoDataError: Calling prepare on an already prepared dataset
 
         Note: If you can guarantee your particular calculation would not require
         the missing columns you can proceed at your own risk!
         """
-        self._ds.validate()
+        self.inner.validate()
 
     def frame(self) -> pl.DataFrame:
-        vec_srs = self._ds.frame()
+        vec_srs = self.inner.frame()
         return pl.DataFrame(vec_srs)
 
     def compute(
         self, req: "dict[Any, Any]|uli.ComputeRequest", streaming: bool = False
     ) -> pl.DataFrame:
         """Make sure that requested groupby and filters exist in self.columns,
         Make sure that requested measures exist in self.measures
@@ -138,15 +156,15 @@
         Returns:
             pl.DataFrame: If your request and data were constructed properly.
         """
 
         if isinstance(req, dict):
             req = uli.ComputeRequest(req)
 
-        vec_srs = self._ds.compute(req._ar, streaming)
+        vec_srs = self.inner.compute(req._ar, streaming)
 
         return pl.DataFrame(vec_srs)
 
     def execute(
         self, req: "dict[Any, Any]|uli.ComputeRequest", streaming: bool = False
     ) -> pl.DataFrame:
         from warnings import warn
@@ -160,15 +178,15 @@
         >>> import os
         >>> os.environ["RUST_LOG"] = "info"
         >>> os.environ["ADDRESS"] = "0.0.0.0:8000"
         """
         # Streaming mode calls prepare on each request
         # If already prepared we don't want to call it again
         streaming = not self.prepared
-        self._ds.ui(streaming)
+        self.inner.ui(streaming)
 
 
 class FRTBDataSet(DataSet):
     """FRTB flavour of DataSet"""
 
     @classmethod
     def from_config_path(
@@ -181,9 +199,10 @@
     @classmethod
     def from_frame(
         cls: Type[DS],
         df: pl.DataFrame,
         measures: "list[str] | None" = None,
         build_params: "dict[str, str] | None" = None,
         prepared: bool = False,
+        bespoke_measures: "list[TMeasure] | None" = None,
     ) -> DS:
         return cls(DataSetWrapper.frtb_from_frame(df, measures, build_params), prepared)
```

### Comparing `ultibi-0.2.0/ultibi/internals/requests.py` & `ultibi-0.3.0/ultibi/internals/requests.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.2.0/Cargo.lock` & `ultibi-0.3.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -293,86 +293,137 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.2.6"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "342258dd14006105c2b75ab1bd7543a03bdf0cfc94383303ac212a04939dff6f"
+checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
 dependencies = [
  "anstyle",
  "anstyle-parse",
+ "anstyle-query",
  "anstyle-wincon",
- "concolor-override",
- "concolor-query",
+ "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "0.3.5"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23ea9e81bd02e310c216d080f6223c179012256e5151c41db88d12c88a1684d2"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7d1bb534e9efed14f3e5f44e7dd1a4f709384023a4165199a4241e18dff0116"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "anstyle-wincon"
-version = "0.2.0"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3127af6145b149f3287bb9a0d10ad9c5692dba8c53ad48285e5bec4063834fa"
+checksum = "4bcd8291a340dd8ac70e18878bc4501dd7b4ff970cfa21c207d36ece51ea88fd"
 dependencies = [
  "anstyle",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
 
 [[package]]
+name = "array-init-cursor"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
+
+[[package]]
+name = "arrow-format"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07884ea216994cdc32a2d5f8274a8bee979cfe90274b83f86f440866ee3132c7"
+dependencies = [
+ "planus",
+ "serde",
+]
+
+[[package]]
 name = "arrow2"
-version = "0.14.2"
+version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee6f62e41078c967a4c063fcbdfd3801a2a9632276402c045311c4d73d0845f3"
+checksum = "c3c63cf31f1416ed2fab8f91e8488e10129f47bd89c553ec354a06751d5697f3"
 dependencies = [
- "ahash 0.7.6",
+ "ahash 0.8.3",
+ "arrow-format",
  "bytemuck",
  "chrono",
  "dyn-clone",
  "either",
  "ethnum",
  "foreign_vec",
+ "futures",
+ "getrandom",
  "hash_hasher",
  "lexical-core",
+ "lz4",
  "multiversion",
  "num-traits",
+ "rustc_version",
  "simdutf8",
  "strength_reduce",
+ "zstd",
 ]
 
 [[package]]
 name = "askama_escape"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "619743e34b5ba4e9703bba34deac3427c72507c7159f5fd030aea8cac0cfe341"
 
 [[package]]
+name = "async-trait"
+version = "0.1.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "atoi"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi 0.1.19",
  "libc",
@@ -529,17 +580,17 @@
  "aws-types",
  "http",
  "tracing",
 ]
 
 [[package]]
 name = "aws-sigv4"
-version = "0.49.0"
+version = "0.49.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d33790cecae42b999d197074c8a19e9b96b9e346284a6f93989e7489c9fa0f5"
+checksum = "8222295f2b74e8f361f3ce6d247fe50fadd862951db6e15401b04a66ab4cb528"
 dependencies = [
  "aws-smithy-eventstream",
  "aws-smithy-http",
  "bytes",
  "form_urlencoded",
  "hex",
  "http",
@@ -778,15 +829,15 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
@@ -847,35 +898,36 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
  "iana-time-zone",
  "js-sys",
  "num-integer",
  "num-traits",
+ "serde",
  "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.0"
+version = "4.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6efb5f0a41b5ef5b50c5da28c07609c20091df0c1fc33d418fa2a7e693c2b624"
+checksum = "49f9152d70e42172fdb87de2efd7327160beee37886027cf86f30a233d5b30b4"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.0"
+version = "4.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "671fcaa5debda4b9a84aa7fde49c907c8986c0e6ab927e04217c9cb74e7c8bc9"
+checksum = "e067b220911598876eb55d52725ddcc201ffe3f0904018195973bc5b012ea2ca"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
@@ -885,15 +937,15 @@
 version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
@@ -905,41 +957,32 @@
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "comfy-table"
 version = "6.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e7b787b0dc42e8111badfdbe4c3059158ccb2db8780352fa1b01e8ccf45cc4d"
 dependencies = [
  "crossterm",
  "strum",
  "strum_macros",
  "unicode-width",
 ]
 
 [[package]]
-name = "concolor-override"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a855d4a1978dc52fb0536a04d384c2c0c1aa273597f08b77c8c4d3b2eec6037f"
-
-[[package]]
-name = "concolor-query"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d11d52c3d7ca2e6d0040212be9e4dbbcd78b6447f535b6b561f449427944cf"
-dependencies = [
- "windows-sys 0.45.0",
-]
-
-[[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
 name = "cookie"
@@ -960,17 +1003,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
 dependencies = [
@@ -993,17 +1036,17 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -1044,15 +1087,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64e6c0fbe2c17357405f7c758c1ef960fce08bdfb2c03d88d2a18d7e09c4b67"
 dependencies = [
  "bitflags",
  "crossterm_winapi",
  "libc",
  "mio",
- "parking_lot",
+ "parking_lot 0.12.1",
  "signal-hook",
  "signal-hook-mio",
  "winapi",
 ]
 
 [[package]]
 name = "crossterm_winapi"
@@ -1070,23 +1113,14 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "csv-core"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "ct-logs"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1a816186fa68d9e426e3cb4ae4dff1fcd8e4a2c34b781bf7a822574a0d0aac8"
 dependencies = [
  "sct",
 ]
@@ -1111,15 +1145,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
@@ -1128,28 +1162,28 @@
 name = "cxxbridge-macro"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
- "hashbrown",
+ "hashbrown 0.12.3",
  "lock_api",
  "once_cell",
- "parking_lot_core",
+ "parking_lot_core 0.9.7",
 ]
 
 [[package]]
 name = "derivative"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
@@ -1252,21 +1286,21 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -1278,14 +1312,20 @@
 [[package]]
 name = "ethnum"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0198b9d0078e0f30dedc7acbb21c974e838fc8fae3ee170128658a98cb2c1c04"
 
 [[package]]
+name = "fast-float"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
+
+[[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
@@ -1334,104 +1374,105 @@
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frtb_engine"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "log",
  "ndarray",
  "once_cell",
  "polars",
  "rayon",
  "serde",
  "serde_json",
+ "smartstring",
  "strum",
  "ultibi",
  "yearfrac",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "531ac96c6ff5fd7c62263c5e3c67a603af4fcaee2e1a0ae5565ba3a11e69e549"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "164713a5a0dcc3e7b4b1ed7d3b433cabc18025386f9339346e8daf15963cf7ac"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1997dd9df74cdac935c76252744c1ed5794fac083242ea4fe77ef3ed60ba0f83"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d422fa3cbe3b40dca574ab087abb5bc98258ea57eea3fd6f1fa7162c778b91"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb14ed937631bd8b8b8977f2c198443447a8355b6e3ca599f38c975e5a963b6"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec93083a4aecafb2a80a885c9de1f0ccae9dbd32c2bb54b0c3a65690e0b8d2f2"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -1449,34 +1490,36 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
+ "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.16"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5be7b54589b581f624f566bf5d8eb2bab1db736c51528720b6bd36b96b55924d"
+checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -1494,16 +1537,22 @@
 checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+
+[[package]]
+name = "hashbrown"
+version = "0.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
- "ahash 0.7.6",
+ "ahash 0.8.3",
  "rayon",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1586,17 +1635,17 @@
 checksum = "df004cfca50ef23c36850aaaa59ad52cc70d0e90243c3c7737a4dd32dc7a3c4f"
 dependencies = [
  "quick-error",
 ]
 
 [[package]]
 name = "hyper"
-version = "0.14.25"
+version = "0.14.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc5e554ff619822309ffd57d8734d77cd5ce6238bc956f037ea06c58238c9899"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -1640,17 +1689,17 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
@@ -1679,15 +1728,15 @@
 [[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
  "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1700,39 +1749,39 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09270fd4fa1111bc614ed2246c7ef56239a3063d5be0d1ec3b589c505d400aeb"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipnet"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.5"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8687c819457e979cc940d09cb16e42a1bf70aa6b60a549de6d3a62a0ee90c69e"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
@@ -1858,29 +1907,29 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.30"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8c7cbf8b89019683667e347572e6d55a7df7ea36b0c4ce69961b0cde67b174"
+checksum = "43a558e3d911bc3c7bfc8c78bc580b404d6e51c1cefbf656e176a94b49b0df40"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "link-cplusplus"
@@ -1889,17 +1938,17 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "3f508063cc7bb32987c71511216bd5a32be15bccb6a80b52df8b9d7f01fc3aa2"
 
 [[package]]
 name = "local-channel"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f303ec0e94c6c54447f84f3b0ef7af769858a9c4ef56ef2a986d3dcd4c3fc9c"
 dependencies = [
@@ -1931,14 +1980,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "lz4"
+version = "1.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
+dependencies = [
+ "libc",
+ "lz4-sys",
+]
+
+[[package]]
+name = "lz4-sys"
+version = "1.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57d27b317e207b10f69f5e75494119e391a96f48861ae870d1da6edac98ca900"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "matrixmultiply"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
 dependencies = [
  "num_cpus",
  "once_cell",
@@ -1977,17 +2046,17 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.34"
+version = "0.1.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dcb174b18635f7561a0c6c9fc2ce57218ac7523cf72c50af80e2d79ab8f3ba1"
+checksum = "3d88dad3f985ec267a3fcb7a1726f5cb1a7e8cad8b646e70a84f967210df23da"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -2023,30 +2092,32 @@
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "multiversion"
-version = "0.6.1"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "025c962a3dd3cc5e0e520aa9c612201d127dcdf28616974961a649dca64f5373"
+checksum = "e6a87eede2251ca235e5573086d01d2ab6b59dfaea54c2be10f9320980f7e8f7"
 dependencies = [
  "multiversion-macros",
+ "target-features",
 ]
 
 [[package]]
 name = "multiversion-macros"
-version = "0.6.1"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a3e2bde382ebf960c1f3e79689fa5941625fe9bf694a1cb64af3e85faff3af"
+checksum = "1af1abf82261d780d114014eff4b555e47d823f3b84f893c4388572b40e089fb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
+ "target-features",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -2075,36 +2146,29 @@
  "num-traits",
  "rawpointer",
  "rayon",
  "serde",
 ]
 
 [[package]]
-name = "num"
-version = "0.4.0"
+name = "now"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
+checksum = "6d89e9874397a1f0a52fc1f197a8effd9735223cb2390e9dcc83ac6cd02923d0"
 dependencies = [
- "num-bigint",
- "num-complex",
- "num-integer",
- "num-iter",
- "num-rational",
- "num-traits",
+ "chrono",
 ]
 
 [[package]]
-name = "num-bigint"
-version = "0.4.3"
+name = "ntapi"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+checksum = "bc51db7b362b205941f71232e56c625156eb9a929f8cf74a428fd5bc094a4afc"
 dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
+ "winapi",
 ]
 
 [[package]]
 name = "num-complex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
@@ -2119,37 +2183,14 @@
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
-name = "num-iter"
-version = "0.1.43"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
-dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
-name = "num-rational"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
-dependencies = [
- "autocfg",
- "num-bigint",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
  "libm",
@@ -2169,76 +2210,100 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "openssl"
-version = "0.10.48"
+version = "0.10.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518915b97df115dd36109bfa429a48b8f737bd05508cf9588977b599648926d2"
+checksum = "7e30d8bc91859781f0a943411186324d580f2bbeb71b452fe91ae344806af3f1"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.83"
+version = "0.9.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "666416d899cf077260dac8698d60a60b435a46d57e82acb1be3d0dad87284e5b"
+checksum = "0d3d193fb1488ad46ffe3aaabc912cc931d02ee8518fe2959aea8ef52718b0c0"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "parking_lot"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+dependencies = [
+ "instant",
+ "lock_api",
+ "parking_lot_core 0.8.6",
+]
+
+[[package]]
+name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core",
+ "parking_lot_core 0.9.7",
+]
+
+[[package]]
+name = "parking_lot_core"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
+dependencies = [
+ "cfg-if",
+ "instant",
+ "libc",
+ "redox_syscall 0.2.16",
+ "smallvec",
+ "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
@@ -2301,176 +2366,246 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
 
 [[package]]
+name = "planus"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
+dependencies = [
+ "array-init-cursor",
+]
+
+[[package]]
 name = "polars"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "112b33c016ec5949e414016b24d329a2188051e4f65d59a555986ecd7c7387ae"
+checksum = "b8f04742abbadbd348d73a803617e6df61464485a410361e9c6634e55a4bc01c"
 dependencies = [
+ "getrandom",
  "polars-core",
  "polars-io",
  "polars-lazy",
  "polars-ops",
  "polars-time",
+ "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7aac9a1d70c683cda8dd4958bd489d8c0206c5ab1435a656a14563c6415f5a64"
+checksum = "eacd179fe0cc7cf18e12a80cfda3e6d15ce907655203cc69277e883a925f9bd8"
 dependencies = [
  "arrow2",
- "hashbrown",
- "num",
+ "hashbrown 0.13.2",
+ "multiversion",
+ "num-traits",
+ "polars-error",
+ "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fda4c06062d5e22036e686762bd2da2cf2fc003728e123a99f9c2df7335afc10"
+checksum = "04145d95791f31a0df3b2d3d600cbb5d0d43ccc105d74e871ffe7351a5e70cbe"
 dependencies = [
  "ahash 0.8.3",
- "anyhow",
  "arrow2",
  "bitflags",
  "chrono",
  "comfy-table",
- "hashbrown",
+ "either",
+ "hashbrown 0.13.2",
  "indexmap",
  "ndarray",
- "num",
+ "num-traits",
  "once_cell",
  "polars-arrow",
+ "polars-error",
+ "polars-row",
  "polars-utils",
  "rand",
  "rand_distr",
  "rayon",
  "regex",
  "serde",
  "smartstring",
  "thiserror",
+ "wasm-timer",
+ "xxhash-rust",
+]
+
+[[package]]
+name = "polars-error"
+version = "0.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5fc2fb4ff74f7224b4096b3551b309c50bfd49bb0b66fb3948e70feffb1a8e51"
+dependencies = [
+ "arrow2",
+ "regex",
+ "thiserror",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "125fd8302050f3b6be46f7a9a92a4ac62dcab738c4e32cd2af7b9be5f4cdf709"
+checksum = "d4d186157d427b39085f812e74eefb04608b7bd033ef3a7f848b93a5939c396d"
 dependencies = [
  "ahash 0.8.3",
- "anyhow",
  "arrow2",
- "csv-core",
+ "async-trait",
+ "bytes",
+ "chrono",
  "dirs",
+ "fast-float",
+ "futures",
  "lexical",
  "lexical-core",
  "memchr",
  "memmap2",
- "num",
+ "num-traits",
  "once_cell",
  "polars-arrow",
  "polars-core",
+ "polars-error",
  "polars-time",
  "polars-utils",
  "rayon",
  "regex",
+ "serde",
  "simdutf8",
+ "tokio",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55376a76c7bd050bb42fd124c290e1908e7ebf8f4c6cce6c4c41e56402f10a33"
+checksum = "385b1beb0ae4f1c8fbe6aef9769b8e0a22a8b56ba494e382f17de82ce653702f"
 dependencies = [
  "ahash 0.8.3",
  "bitflags",
  "glob",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-pipe",
  "polars-plan",
  "polars-time",
  "polars-utils",
  "rayon",
+ "smartstring",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfd3f6552b3e9539634c35047f372db331b6227f75c36fcbe4670ab58bbcbeb3"
+checksum = "b8beae89044ad6f5a2237103852d2650c7a52e7b339e356c1d707b9427b48ba7"
 dependencies = [
  "arrow2",
+ "either",
+ "memchr",
  "polars-arrow",
  "polars-core",
  "polars-utils",
+ "serde",
+ "smartstring",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa865a4fc6dcfb9967505c4714c29277898e21dd29ea7633a3f9d1abbe879a7d"
+checksum = "59c7fbda6ff77db1ae1a0d8f210b9729b2c0cb7c584345504a8282e3bd38e97d"
 dependencies = [
+ "crossbeam-channel",
  "enum_dispatch",
- "hashbrown",
- "num",
+ "hashbrown 0.13.2",
+ "num-traits",
+ "polars-arrow",
  "polars-core",
  "polars-io",
+ "polars-ops",
  "polars-plan",
+ "polars-row",
  "polars-utils",
  "rayon",
+ "smartstring",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "673480b0ee55b0abb5be247862bfe1f3b623897f504006a10adbc25c878bf531"
+checksum = "11b788cb03c651c9b92c2293b0adc07cb89ae64d7f187310cb7d62d688ccd9d8"
 dependencies = [
  "ahash 0.8.3",
+ "arrow2",
+ "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-time",
  "polars-utils",
  "rayon",
+ "serde",
+ "smartstring",
+]
+
+[[package]]
+name = "polars-row"
+version = "0.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bfcd216b7953321a6946c38d352fdfa67260a4d2125cbb4a1c3b46f03d0bebb"
+dependencies = [
+ "arrow2",
+ "polars-error",
+ "polars-utils",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "783e53abda73c226807e850d91de67ab376d91866f378306d3e7f6b9844c17de"
+checksum = "5384945cc104ba99683455760dcfe1048e4025bfaf78043e14450cc8c988a745"
 dependencies = [
+ "arrow2",
+ "atoi",
  "chrono",
- "lexical",
+ "now",
+ "once_cell",
  "polars-arrow",
  "polars-core",
+ "polars-ops",
  "polars-utils",
+ "regex",
+ "serde",
+ "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.25.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2d5b6ec3c45989c1fbaf0e13a3832f4b5e418e776518d7a24d62672e5366364"
+checksum = "7c1823141ed08322d17e9717ddf652c42df92f0d9b0c52cc5a242c96bc845144"
 dependencies = [
+ "once_cell",
  "rayon",
+ "smartstring",
+ "sysinfo",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
@@ -2507,86 +2642,87 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
- "parking_lot",
+ "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyultima"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "frtb_engine",
+ "once_cell",
  "polars",
  "polars-arrow",
  "pyo3",
  "serde_json",
  "thiserror",
  "ultibi",
 ]
@@ -2680,21 +2816,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
 version = "1.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2805,24 +2950,24 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.11"
+version = "0.37.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db4165c9963ab29e422d6c26fbc1d37f15bace6b2810221f9d925023480fcf0e"
+checksum = "722529a737f5a942fdbac3a46cee213053196737c5eaa3386d52e85b786f2659"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35edb675feee39aec9c99fa5ff985081995a06d594114ae14cbe797ad7b7a6d7"
@@ -2925,37 +3070,37 @@
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3064,14 +3209,15 @@
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
  "autocfg",
+ "serde",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "socket2"
 version = "0.4.9"
@@ -3148,45 +3294,65 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.11"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21e3787bb71465627110e7d87ed4faaa36c1f61042ee67badb9e2ef173accc40"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "sysinfo"
+version = "0.28.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4c2f3ca6693feb29a89724516f016488e9aafc7f37264f898593ee4b942f31b"
+dependencies = [
+ "cfg-if",
+ "core-foundation-sys",
+ "libc",
+ "ntapi",
+ "once_cell",
+ "winapi",
+]
+
+[[package]]
+name = "target-features"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24840de800c1707d75c800893dbd727a5e1501ce921944e602f0698167491e36"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "template_drivers"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "actix-files",
  "actix-web",
  "actix-web-httpauth",
  "actix-web-static-files",
  "anyhow",
  "clap",
@@ -3230,15 +3396,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "thread-tree"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ffbd370cb847953a25954d9f63e14824a36113f8c72eecf6eccef5dc4b45d630"
@@ -3306,15 +3472,15 @@
 checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
- "parking_lot",
+ "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
  "windows-sys 0.45.0",
 ]
 
@@ -3322,15 +3488,15 @@
 name = "tokio-macros"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3480,23 +3646,23 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ultibi"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "ultibi_core",
  "ultibi_server",
 ]
 
 [[package]]
 name = "ultibi_core"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "aws-config",
  "aws-sdk-s3",
  "dashmap",
  "derivative",
  "futures",
  "once_cell",
@@ -3507,15 +3673,15 @@
  "tokio",
  "toml",
  "utoipa",
 ]
 
 [[package]]
 name = "ultibi_server"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "actix-web",
  "actix-web-static-files",
  "anyhow",
  "dotenv",
  "log",
  "mime",
@@ -3599,56 +3765,56 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "utoipa"
-version = "3.2.0"
-source = "git+https://github.com/juhaku/utoipa#dcb15d3b0634f0c2ba3b228917c566e29d1ebbf0"
+version = "3.3.0"
+source = "git+https://github.com/juhaku/utoipa#489ddd663051a578e9285f5f4b5d87c0f626d6c0"
 dependencies = [
  "indexmap",
  "serde",
  "serde_json",
  "utoipa-gen",
 ]
 
 [[package]]
 name = "utoipa-gen"
-version = "3.2.0"
-source = "git+https://github.com/juhaku/utoipa#dcb15d3b0634f0c2ba3b228917c566e29d1ebbf0"
+version = "3.3.0"
+source = "git+https://github.com/juhaku/utoipa#489ddd663051a578e9285f5f4b5d87c0f626d6c0"
 dependencies = [
  "lazy_static",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "utoipa-swagger-ui"
-version = "3.1.1"
-source = "git+https://github.com/juhaku/utoipa#dcb15d3b0634f0c2ba3b228917c566e29d1ebbf0"
+version = "3.1.3"
+source = "git+https://github.com/juhaku/utoipa#489ddd663051a578e9285f5f4b5d87c0f626d6c0"
 dependencies = [
  "actix-web",
  "mime_guess",
  "regex",
  "rust-embed",
  "serde",
  "serde_json",
  "utoipa",
  "zip",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "5b55a3fef2a1e3b3a00ce878640918820d3c51081576ac657d23af9fc7928fdb"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
@@ -3756,14 +3922,29 @@
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
 
 [[package]]
+name = "wasm-timer"
+version = "0.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "be0ecb0db480561e9a7642b5d3e4187c128914e58aa84330b9493e3eb68c5e7f"
+dependencies = [
+ "futures",
+ "js-sys",
+ "parking_lot 0.11.2",
+ "pin-utils",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
 name = "web-sys"
 version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
@@ -3808,103 +3989,169 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.46.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winnow"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
 dependencies = [
  "memchr",
 ]
@@ -3921,14 +4168,20 @@
 [[package]]
 name = "xmlparser"
 version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "114ba2b24d2167ef6d67d7d04c8cc86522b87f490025f39f0303b7db5bf5e3d8"
 
 [[package]]
+name = "xxhash-rust"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "735a71d46c4d68d71d4b24d03fdc2b98e38cea81730595801db779c04fe80d70"
+
+[[package]]
 name = "yearfrac"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73ba657166ee46d227598eb47c3c7d121eceea28aa43a03fbf76657ac8b4fea7"
 dependencies = [
  "chrono",
  "serde",
@@ -3960,25 +4213,25 @@
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.4+zstd.1.5.4"
+version = "6.0.5+zstd.1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7afb4b54b8910cf5447638cb54bf4e8a65cbedd783af98b98c62ffe91f185543"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.7+zstd.1.5.4"
+version = "2.0.8+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94509c3ba2fe55294d752b79842c530ccfab760192521df74a081a78d2b3c7f5"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
```

