# Comparing `tmp/zipline-tej-0.0.8.tar.gz` & `tmp/zipline-tej-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline-tej-0.0.8.tar", last modified: Mon Jun  5 03:06:09 2023, max compression
+gzip compressed data, was "zipline-tej-0.0.9.tar", last modified: Mon Jun  5 03:53:12 2023, max compression
```

## Comparing `zipline-tej-0.0.8.tar` & `zipline-tej-0.0.9.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:09.056148 zipline-tej-0.0.8/
--rw-rw-rw-   0        0        0    13262 2023-06-05 03:06:09.056148 zipline-tej-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    12877 2023-06-02 09:13:48.000000 zipline-tej-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 03:06:09.056148 zipline-tej-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3671 2023-06-05 03:05:55.000000 zipline-tej-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.539157 zipline-tej-0.0.8/zipline-tej/
--rw-rw-rw-   0        0        0     3674 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/__init__.py
--rw-rw-rw-   0        0        0    12296 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/__main__.py
--rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/_version.py
--rw-rw-rw-   0        0        0    89973 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/algorithm.py
--rw-rw-rw-   0        0        0     1678 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/api.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.570413 zipline-tej-0.0.8/zipline-tej/assets/
--rw-rw-rw-   0        0        0     1188 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/__init__.py
--rw-rw-rw-   0        0        0    17577 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/asset_db_migrations.py
--rw-rw-rw-   0        0        0     4943 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/asset_db_schema.py
--rw-rw-rw-   0        0        0    35430 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/asset_writer.py
--rw-rw-rw-   0        0        0    54555 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/assets.py
--rw-rw-rw-   0        0        0     2078 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/exchange_info.py
--rw-rw-rw-   0        0        0      767 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/futures.py
--rw-rw-rw-   0        0        0    11295 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/roll_finder.py
--rw-rw-rw-   0        0        0    10815 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/assets/synthetic.py
--rw-rw-rw-   0        0        0     1799 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/country.py
--rw-rw-rw-   0        0        0     1819 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/currency.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.608183 zipline-tej-0.0.8/zipline-tej/data/
--rw-rw-rw-   0        0        0      209 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/__init__.py
--rw-rw-rw-   0        0        0    26366 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/adjustments.py
--rw-rw-rw-   0        0        0     4181 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/bar_reader.py
--rw-rw-rw-   0        0        0    25147 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/bcolz_daily_bars.py
--rw-rw-rw-   0        0        0     1652 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/benchmarks.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.623808 zipline-tej-0.0.8/zipline-tej/data/bundles/
--rw-rw-rw-   0        0        0      627 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/bundles/__init__.py
--rw-rw-rw-   0        0        0    21102 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/bundles/core.py
--rw-rw-rw-   0        0        0     8742 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/bundles/csvdir.py
--rw-rw-rw-   0        0        0     9059 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/bundles/quandl.py
--rw-rw-rw-   0        0        0    12516 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/bundles/tquant.py
--rw-rw-rw-   0        0        0    12351 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/continuous_future_reader.py
--rw-rw-rw-   0        0        0    59712 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/data_portal.py
--rw-rw-rw-   0        0        0     4947 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/dispatch_bar_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.639433 zipline-tej-0.0.8/zipline-tej/data/fx/
--rw-rw-rw-   0        0        0      366 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/fx/__init__.py
--rw-rw-rw-   0        0        0     5495 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/fx/base.py
--rw-rw-rw-   0        0        0      394 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/fx/exploding.py
--rw-rw-rw-   0        0        0    11540 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/fx/hdf5.py
--rw-rw-rw-   0        0        0     1843 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/fx/in_memory.py
--rw-rw-rw-   0        0        0      355 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/fx/utils.py
--rw-rw-rw-   0        0        0    34276 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/hdf5_daily_bars.py
--rw-rw-rw-   0        0        0    21993 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/history_loader.py
--rw-rw-rw-   0        0        0     5382 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/in_memory_daily_bars.py
--rw-rw-rw-   0        0        0     1272 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/loader.py
--rw-rw-rw-   0        0        0    48513 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/minute_bars.py
--rw-rw-rw-   0        0        0    27729 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/resample.py
--rw-rw-rw-   0        0        0     1817 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/session_bars.py
--rw-rw-rw-   0        0        0     1700 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/data/treasury.py
--rw-rw-rw-   0        0        0      285 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/dispatch.py
--rw-rw-rw-   0        0        0    26888 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.655056 zipline-tej-0.0.8/zipline-tej/examples/
--rw-rw-rw-   0        0        0     2378 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/__init__.py
--rw-rw-rw-   0        0        0     1612 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/buy_and_hold.py
--rw-rw-rw-   0        0        0     2034 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/buyapple.py
--rw-rw-rw-   0        0        0     2439 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/buyapple_ide.py
--rw-rw-rw-   0        0        0     4470 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/dual_ema_talib.py
--rw-rw-rw-   0        0        0     4165 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/dual_moving_average.py
--rw-rw-rw-   0        0        0     3162 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/momentum_pipeline.py
--rw-rw-rw-   0        0        0     4878 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/examples/olmar.py
--rw-rw-rw-   0        0        0     7312 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/extensions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.692823 zipline-tej-0.0.8/zipline-tej/finance/
--rw-rw-rw-   0        0        0      670 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/__init__.py
--rw-rw-rw-   0        0        0     7089 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/asset_restrictions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.692823 zipline-tej-0.0.8/zipline-tej/finance/blotter/
--rw-rw-rw-   0        0        0      739 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/blotter/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/blotter/blotter.py
--rw-rw-rw-   0        0        0    17341 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/blotter/simulation_blotter.py
--rw-rw-rw-   0        0        0     2096 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/cancel_policy.py
--rw-rw-rw-   0        0        0    13935 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/commission.py
--rw-rw-rw-   0        0        0     6879 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/constants.py
--rw-rw-rw-   0        0        0    14273 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/controls.py
--rw-rw-rw-   0        0        0     7533 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/execution.py
--rw-rw-rw-   0        0        0    28436 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/ledger.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.692823 zipline-tej-0.0.8/zipline-tej/finance/metrics/
--rw-rw-rw-   0        0        0     3720 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/metrics/__init__.py
--rw-rw-rw-   0        0        0     3095 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/metrics/core.py
--rw-rw-rw-   0        0        0    29630 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/metrics/metric.py
--rw-rw-rw-   0        0        0    11837 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/metrics/tracker.py
--rw-rw-rw-   0        0        0     8621 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/order.py
--rw-rw-rw-   0        0        0     8147 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/position.py
--rw-rw-rw-   0        0        0     1647 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/shared.py
--rw-rw-rw-   0        0        0    22666 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/slippage.py
--rw-rw-rw-   0        0        0     5556 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/trading.py
--rw-rw-rw-   0        0        0     2473 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/finance/transaction.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.708458 zipline-tej-0.0.8/zipline-tej/gens/
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/gens/__init__.py
--rw-rw-rw-   0        0        0     1063 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/gens/composites.py
--rw-rw-rw-   0        0        0    12006 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/gens/tradesimulation.py
--rw-rw-rw-   0        0        0     1999 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/gens/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.724080 zipline-tej-0.0.8/zipline-tej/lib/
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/lib/__init__.py
--rw-rw-rw-   0        0        0    13462 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/lib/adjusted_array.py
--rw-rw-rw-   0        0        0    28546 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/lib/labelarray.py
--rw-rw-rw-   0        0        0     1813 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/lib/normalize.py
--rw-rw-rw-   0        0        0      389 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/lib/quantiles.py
--rw-rw-rw-   0        0        0     8376 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/master.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.755328 zipline-tej-0.0.8/zipline-tej/pipeline/
--rw-rw-rw-   0        0        0      734 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1707 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/api_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.770952 zipline-tej-0.0.8/zipline-tej/pipeline/classifiers/
--rw-rw-rw-   0        0        0      230 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/classifiers/__init__.py
--rw-rw-rw-   0        0        0    19647 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/classifiers/classifier.py
--rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/common.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.770952 zipline-tej-0.0.8/zipline-tej/pipeline/data/
--rw-rw-rw-   0        0        0      382 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/data/__init__.py
--rw-rw-rw-   0        0        0    33755 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/data/dataset.py
--rw-rw-rw-   0        0        0      827 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/data/equity_pricing.py
--rw-rw-rw-   0        0        0    19447 2023-06-02 09:04:44.000000 zipline-tej-0.0.8/zipline-tej/pipeline/data/tejquant.py
--rw-rw-rw-   0        0        0     1006 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/data/testing.py
--rw-rw-rw-   0        0        0    14783 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/domain.py
--rw-rw-rw-   0        0        0     1903 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/downsample_helpers.py
--rw-rw-rw-   0        0        0      323 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/dtypes.py
--rw-rw-rw-   0        0        0    36374 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/engine.py
--rw-rw-rw-   0        0        0    10639 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/expression.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.793094 zipline-tej-0.0.8/zipline-tej/pipeline/factors/
--rw-rw-rw-   0        0        0     1907 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/factors/__init__.py
--rw-rw-rw-   0        0        0    16252 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/factors/basic.py
--rw-rw-rw-   0        0        0     3614 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/factors/events.py
--rw-rw-rw-   0        0        0    65638 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/factors/factor.py
--rw-rw-rw-   0        0        0    26905 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/factors/statistical.py
--rw-rw-rw-   0        0        0    12277 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/factors/technical.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.793094 zipline-tej-0.0.8/zipline-tej/pipeline/filters/
--rw-rw-rw-   0        0        0      628 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/filters/__init__.py
--rw-rw-rw-   0        0        0    25761 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/filters/filter.py
--rw-rw-rw-   0        0        0     1180 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/filters/smoothing.py
--rw-rw-rw-   0        0        0    17933 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/graph.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.808727 zipline-tej-0.0.8/zipline-tej/pipeline/hooks/
--rw-rw-rw-   0        0        0      295 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/hooks/__init__.py
--rw-rw-rw-   0        0        0     2245 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/hooks/delegate.py
--rw-rw-rw-   0        0        0     2834 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/hooks/iface.py
--rw-rw-rw-   0        0        0      599 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/hooks/no.py
--rw-rw-rw-   0        0        0    16278 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/hooks/progress.py
--rw-rw-rw-   0        0        0     1901 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/hooks/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.839975 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/
--rw-rw-rw-   0        0        0      171 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/__init__.py
--rw-rw-rw-   0        0        0     1599 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/base.py
--rw-rw-rw-   0        0        0    61161 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/earnings_estimates.py
--rw-rw-rw-   0        0        0     7578 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/equity_pricing_loader.py
--rw-rw-rw-   0        0        0     8556 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/events.py
--rw-rw-rw-   0        0        0     6844 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/frame.py
--rw-rw-rw-   0        0        0    13063 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/synthetic.py
--rw-rw-rw-   0        0        0      651 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/testing.py
--rw-rw-rw-   0        0        0    13306 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/loaders/utils.py
--rw-rw-rw-   0        0        0    24184 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/mixins.py
--rw-rw-rw-   0        0        0    11318 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/pipeline.py
--rw-rw-rw-   0        0        0      197 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/sentinels.py
--rw-rw-rw-   0        0        0    33623 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/term.py
--rw-rw-rw-   0        0        0     6068 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/pipeline/visualize.py
--rw-rw-rw-   0        0        0     8182 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/protocol.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.839975 zipline-tej-0.0.8/zipline-tej/resources/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.839975 zipline-tej-0.0.8/zipline-tej/resources/market_data/
--rw-rw-rw-   0        0        0   251155 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/market_data/SPY_benchmark.csv
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/market_data/__init__.py
--rw-rw-rw-   0        0        0   671941 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/market_data/treasury_curves.csv
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.855599 zipline-tej-0.0.8/zipline-tej/resources/security_lists/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.855599 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.492279 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.855599 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/__init__.py
--rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.871224 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/__init__.py
--rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.871224 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/__init__.py
--rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.886851 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/__init__.py
--rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.893367 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/__init__.py
--rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.893367 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/__init__.py
--rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.893367 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/__init__.py
--rw-rw-rw-   0        0        0        5 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.909000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/__init__.py
--rw-rw-rw-   0        0        0       20 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.909000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/__init__.py
--rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.909000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/__init__.py
--rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.924625 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/__init__.py
--rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.924625 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/__init__.py
--rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.940249 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/__init__.py
--rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.940249 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/delete
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.940249 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/__init__.py
--rw-rw-rw-   0        0        0      208 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/add
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/delete
--rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/__init__.py
--rw-rw-rw-   0        0        0    18936 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/test_algorithms.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:08.971498 zipline-tej-0.0.8/zipline-tej/testing/
--rw-rw-rw-   0        0        0     1404 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/testing/__init__.py
--rw-rw-rw-   0        0        0    55119 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/testing/core.py
--rw-rw-rw-   0        0        0     2683 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/testing/debug.py
--rw-rw-rw-   0        0        0    82068 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/testing/fixtures.py
--rw-rw-rw-   0        0        0     3306 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/testing/pipeline_terms.py
--rw-rw-rw-   0        0        0    17906 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/testing/predicates.py
--rw-rw-rw-   0        0        0     1066 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/testing/slippage.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:09.040524 zipline-tej-0.0.8/zipline-tej/utils/
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/__init__.py
--rw-rw-rw-   0        0        0      787 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/algo_instance.py
--rw-rw-rw-   0        0        0     4268 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/api_support.py
--rw-rw-rw-   0        0        0    10164 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/argcheck.py
--rw-rw-rw-   0        0        0    11721 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/cache.py
--rw-rw-rw-   0        0        0     4063 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/calendar_utils.py
--rw-rw-rw-   0        0        0      191 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/classproperty.py
--rw-rw-rw-   0        0        0     3319 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/cli.py
--rw-rw-rw-   0        0        0      854 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/compat.py
--rw-rw-rw-   0        0        0     2244 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/context_tricks.py
--rw-rw-rw-   0        0        0     7689 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/data.py
--rw-rw-rw-   0        0        0     1774 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/date_utils.py
--rw-rw-rw-   0        0        0     1572 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/deprecate.py
--rw-rw-rw-   0        0        0      248 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/dummy.py
--rw-rw-rw-   0        0        0    25153 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/events.py
--rw-rw-rw-   0        0        0     1226 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/exploding_object.py
--rw-rw-rw-   0        0        0     5023 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/factory.py
--rw-rw-rw-   0        0        0     3902 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/final.py
--rw-rw-rw-   0        0        0     1651 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/formatting.py
--rw-rw-rw-   0        0        0    10662 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/functional.py
--rw-rw-rw-   0        0        0      665 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/idbox.py
--rw-rw-rw-   0        0        0    26914 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/input_validation.py
--rw-rw-rw-   0        0        0     2668 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/math_utils.py
--rw-rw-rw-   0        0        0     7957 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/memoize.py
--rw-rw-rw-   0        0        0    13647 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/numpy_utils.py
--rw-rw-rw-   0        0        0     9268 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/pandas_utils.py
--rw-rw-rw-   0        0        0     5983 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/paths.py
--rw-rw-rw-   0        0        0     7429 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/preprocess.py
--rw-rw-rw-   0        0        0     5025 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/range.py
--rw-rw-rw-   0        0        0    38036 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/run_algo.py
--rw-rw-rw-   0        0        0     5408 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/security_list.py
--rw-rw-rw-   0        0        0     2380 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/sentinel.py
--rw-rw-rw-   0        0        0     3610 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/sharedoc.py
--rw-rw-rw-   0        0        0     1760 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/sqlite_utils.py
--rw-rw-rw-   0        0        0      402 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/utils/string_formatting.py
--rw-rw-rw-   0        0        0      664 2023-06-02 08:45:48.000000 zipline-tej-0.0.8/zipline-tej/zipline_warnings.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:06:09.056148 zipline-tej-0.0.8/zipline_tej.egg-info/
--rw-rw-rw-   0        0        0    13262 2023-06-05 03:06:08.000000 zipline-tej-0.0.8/zipline_tej.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10063 2023-06-05 03:06:08.000000 zipline-tej-0.0.8/zipline_tej.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 03:06:08.000000 zipline-tej-0.0.8/zipline_tej.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-06-05 03:06:08.000000 zipline-tej-0.0.8/zipline_tej.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-05 03:06:08.000000 zipline-tej-0.0.8/zipline_tej.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.530144 zipline-tej-0.0.9/
+-rw-rw-rw-   0        0        0    13262 2023-06-05 03:53:12.530144 zipline-tej-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12877 2023-06-02 09:13:48.000000 zipline-tej-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 03:53:12.530144 zipline-tej-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     4148 2023-06-05 03:50:44.000000 zipline-tej-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.091316 zipline-tej-0.0.9/zipline-tej/
+-rw-rw-rw-   0        0        0     3674 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/__init__.py
+-rw-rw-rw-   0        0        0    12296 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/__main__.py
+-rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/_version.py
+-rw-rw-rw-   0        0        0    89973 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/algorithm.py
+-rw-rw-rw-   0        0        0     1678 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/api.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.113451 zipline-tej-0.0.9/zipline-tej/assets/
+-rw-rw-rw-   0        0        0     1188 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/__init__.py
+-rw-rw-rw-   0        0        0    17577 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/asset_db_migrations.py
+-rw-rw-rw-   0        0        0     4943 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/asset_db_schema.py
+-rw-rw-rw-   0        0        0    35430 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/asset_writer.py
+-rw-rw-rw-   0        0        0    54555 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/assets.py
+-rw-rw-rw-   0        0        0     2078 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/exchange_info.py
+-rw-rw-rw-   0        0        0      767 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/futures.py
+-rw-rw-rw-   0        0        0    11295 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/roll_finder.py
+-rw-rw-rw-   0        0        0    10815 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/assets/synthetic.py
+-rw-rw-rw-   0        0        0     1799 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/country.py
+-rw-rw-rw-   0        0        0     1819 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/currency.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.144711 zipline-tej-0.0.9/zipline-tej/data/
+-rw-rw-rw-   0        0        0      209 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/__init__.py
+-rw-rw-rw-   0        0        0    26366 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/adjustments.py
+-rw-rw-rw-   0        0        0     4181 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/bar_reader.py
+-rw-rw-rw-   0        0        0    25147 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/bcolz_daily_bars.py
+-rw-rw-rw-   0        0        0     1652 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/benchmarks.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.144711 zipline-tej-0.0.9/zipline-tej/data/bundles/
+-rw-rw-rw-   0        0        0      627 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/bundles/__init__.py
+-rw-rw-rw-   0        0        0    21102 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/bundles/core.py
+-rw-rw-rw-   0        0        0     8742 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/bundles/csvdir.py
+-rw-rw-rw-   0        0        0     9059 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/bundles/quandl.py
+-rw-rw-rw-   0        0        0    12516 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/bundles/tquant.py
+-rw-rw-rw-   0        0        0    12351 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/continuous_future_reader.py
+-rw-rw-rw-   0        0        0    59712 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/data_portal.py
+-rw-rw-rw-   0        0        0     4947 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/dispatch_bar_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.160334 zipline-tej-0.0.9/zipline-tej/data/fx/
+-rw-rw-rw-   0        0        0      366 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/fx/__init__.py
+-rw-rw-rw-   0        0        0     5495 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/fx/base.py
+-rw-rw-rw-   0        0        0      394 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/fx/exploding.py
+-rw-rw-rw-   0        0        0    11540 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/fx/hdf5.py
+-rw-rw-rw-   0        0        0     1843 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/fx/in_memory.py
+-rw-rw-rw-   0        0        0      355 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/fx/utils.py
+-rw-rw-rw-   0        0        0    34276 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/hdf5_daily_bars.py
+-rw-rw-rw-   0        0        0    21993 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/history_loader.py
+-rw-rw-rw-   0        0        0     5382 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/in_memory_daily_bars.py
+-rw-rw-rw-   0        0        0     1272 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/loader.py
+-rw-rw-rw-   0        0        0    48513 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/minute_bars.py
+-rw-rw-rw-   0        0        0    27729 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/resample.py
+-rw-rw-rw-   0        0        0     1817 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/session_bars.py
+-rw-rw-rw-   0        0        0     1700 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/data/treasury.py
+-rw-rw-rw-   0        0        0      285 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/dispatch.py
+-rw-rw-rw-   0        0        0    26888 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.175957 zipline-tej-0.0.9/zipline-tej/examples/
+-rw-rw-rw-   0        0        0     2378 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/__init__.py
+-rw-rw-rw-   0        0        0     1612 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/buy_and_hold.py
+-rw-rw-rw-   0        0        0     2034 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/buyapple.py
+-rw-rw-rw-   0        0        0     2439 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/buyapple_ide.py
+-rw-rw-rw-   0        0        0     4470 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/dual_ema_talib.py
+-rw-rw-rw-   0        0        0     4165 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/dual_moving_average.py
+-rw-rw-rw-   0        0        0     3162 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/momentum_pipeline.py
+-rw-rw-rw-   0        0        0     4878 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/examples/olmar.py
+-rw-rw-rw-   0        0        0     7312 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/extensions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.207205 zipline-tej-0.0.9/zipline-tej/finance/
+-rw-rw-rw-   0        0        0      670 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/__init__.py
+-rw-rw-rw-   0        0        0     7089 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/asset_restrictions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.213715 zipline-tej-0.0.9/zipline-tej/finance/blotter/
+-rw-rw-rw-   0        0        0      739 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/blotter/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/blotter/blotter.py
+-rw-rw-rw-   0        0        0    17341 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/blotter/simulation_blotter.py
+-rw-rw-rw-   0        0        0     2096 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/cancel_policy.py
+-rw-rw-rw-   0        0        0    13935 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/commission.py
+-rw-rw-rw-   0        0        0     6879 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/constants.py
+-rw-rw-rw-   0        0        0    14273 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/controls.py
+-rw-rw-rw-   0        0        0     7533 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/execution.py
+-rw-rw-rw-   0        0        0    28436 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/ledger.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.213715 zipline-tej-0.0.9/zipline-tej/finance/metrics/
+-rw-rw-rw-   0        0        0     3720 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3095 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/metrics/core.py
+-rw-rw-rw-   0        0        0    29630 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/metrics/metric.py
+-rw-rw-rw-   0        0        0    11837 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/metrics/tracker.py
+-rw-rw-rw-   0        0        0     8621 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/order.py
+-rw-rw-rw-   0        0        0     8147 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/position.py
+-rw-rw-rw-   0        0        0     1647 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/shared.py
+-rw-rw-rw-   0        0        0    22666 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/slippage.py
+-rw-rw-rw-   0        0        0     5556 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/trading.py
+-rw-rw-rw-   0        0        0     2473 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/finance/transaction.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.213715 zipline-tej-0.0.9/zipline-tej/gens/
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/gens/__init__.py
+-rw-rw-rw-   0        0        0     1063 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/gens/composites.py
+-rw-rw-rw-   0        0        0    12006 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/gens/tradesimulation.py
+-rw-rw-rw-   0        0        0     1999 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/gens/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.229347 zipline-tej-0.0.9/zipline-tej/lib/
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/lib/__init__.py
+-rw-rw-rw-   0        0        0    13462 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/lib/adjusted_array.py
+-rw-rw-rw-   0        0        0    28546 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/lib/labelarray.py
+-rw-rw-rw-   0        0        0     1813 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/lib/normalize.py
+-rw-rw-rw-   0        0        0      389 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/lib/quantiles.py
+-rw-rw-rw-   0        0        0     8376 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/master.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.260595 zipline-tej-0.0.9/zipline-tej/pipeline/
+-rw-rw-rw-   0        0        0      734 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1707 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/api_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.260595 zipline-tej-0.0.9/zipline-tej/pipeline/classifiers/
+-rw-rw-rw-   0        0        0      230 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/classifiers/__init__.py
+-rw-rw-rw-   0        0        0    19647 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/classifiers/classifier.py
+-rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/common.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.276220 zipline-tej-0.0.9/zipline-tej/pipeline/data/
+-rw-rw-rw-   0        0        0      382 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/data/__init__.py
+-rw-rw-rw-   0        0        0    33755 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/data/dataset.py
+-rw-rw-rw-   0        0        0      827 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/data/equity_pricing.py
+-rw-rw-rw-   0        0        0    19447 2023-06-02 09:04:44.000000 zipline-tej-0.0.9/zipline-tej/pipeline/data/tejquant.py
+-rw-rw-rw-   0        0        0     1006 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/data/testing.py
+-rw-rw-rw-   0        0        0    14783 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/domain.py
+-rw-rw-rw-   0        0        0     1903 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/downsample_helpers.py
+-rw-rw-rw-   0        0        0      323 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/dtypes.py
+-rw-rw-rw-   0        0        0    36374 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/engine.py
+-rw-rw-rw-   0        0        0    10639 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/expression.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.291844 zipline-tej-0.0.9/zipline-tej/pipeline/factors/
+-rw-rw-rw-   0        0        0     1907 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/factors/__init__.py
+-rw-rw-rw-   0        0        0    16252 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/factors/basic.py
+-rw-rw-rw-   0        0        0     3614 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/factors/events.py
+-rw-rw-rw-   0        0        0    65638 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/factors/factor.py
+-rw-rw-rw-   0        0        0    26905 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/factors/statistical.py
+-rw-rw-rw-   0        0        0    12277 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/factors/technical.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.291844 zipline-tej-0.0.9/zipline-tej/pipeline/filters/
+-rw-rw-rw-   0        0        0      628 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/filters/__init__.py
+-rw-rw-rw-   0        0        0    25761 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/filters/filter.py
+-rw-rw-rw-   0        0        0     1180 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/filters/smoothing.py
+-rw-rw-rw-   0        0        0    17933 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/graph.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.313975 zipline-tej-0.0.9/zipline-tej/pipeline/hooks/
+-rw-rw-rw-   0        0        0      295 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/hooks/__init__.py
+-rw-rw-rw-   0        0        0     2245 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/hooks/delegate.py
+-rw-rw-rw-   0        0        0     2834 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/hooks/iface.py
+-rw-rw-rw-   0        0        0      599 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/hooks/no.py
+-rw-rw-rw-   0        0        0    16278 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/hooks/progress.py
+-rw-rw-rw-   0        0        0     1901 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/hooks/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.329609 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/
+-rw-rw-rw-   0        0        0      171 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/__init__.py
+-rw-rw-rw-   0        0        0     1599 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/base.py
+-rw-rw-rw-   0        0        0    61161 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/earnings_estimates.py
+-rw-rw-rw-   0        0        0     7578 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/equity_pricing_loader.py
+-rw-rw-rw-   0        0        0     8556 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/events.py
+-rw-rw-rw-   0        0        0     6844 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/frame.py
+-rw-rw-rw-   0        0        0    13063 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/synthetic.py
+-rw-rw-rw-   0        0        0      651 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/testing.py
+-rw-rw-rw-   0        0        0    13306 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/loaders/utils.py
+-rw-rw-rw-   0        0        0    24184 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/mixins.py
+-rw-rw-rw-   0        0        0    11318 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/pipeline.py
+-rw-rw-rw-   0        0        0      197 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/sentinels.py
+-rw-rw-rw-   0        0        0    33623 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/term.py
+-rw-rw-rw-   0        0        0     6068 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/pipeline/visualize.py
+-rw-rw-rw-   0        0        0     8182 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/protocol.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.329609 zipline-tej-0.0.9/zipline-tej/resources/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.329609 zipline-tej-0.0.9/zipline-tej/resources/market_data/
+-rw-rw-rw-   0        0        0   251155 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/market_data/SPY_benchmark.csv
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/market_data/__init__.py
+-rw-rw-rw-   0        0        0   671941 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/market_data/treasury_curves.csv
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.329609 zipline-tej-0.0.9/zipline-tej/resources/security_lists/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.329609 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.044443 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.345229 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120913/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.345229 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20120919/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.360853 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20121012/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.360853 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130605/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.360853 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20130916/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.360853 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131002/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.376495 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/__init__.py
+-rw-rw-rw-   0        0        0        5 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131009/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.376495 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131121/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.376495 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20131227/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.397601 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140410/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.397601 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20140923/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.397601 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141119/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.414243 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20141226/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.414243 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/delete
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.414243 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/__init__.py
+-rw-rw-rw-   0        0        0      208 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/add
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20160826/delete
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:12:54.000000 zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/__init__.py
+-rw-rw-rw-   0        0        0    18936 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/test_algorithms.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.429884 zipline-tej-0.0.9/zipline-tej/testing/
+-rw-rw-rw-   0        0        0     1404 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/testing/__init__.py
+-rw-rw-rw-   0        0        0    55119 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/testing/core.py
+-rw-rw-rw-   0        0        0     2683 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/testing/debug.py
+-rw-rw-rw-   0        0        0    82068 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/testing/fixtures.py
+-rw-rw-rw-   0        0        0     3306 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/testing/pipeline_terms.py
+-rw-rw-rw-   0        0        0    17906 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/testing/predicates.py
+-rw-rw-rw-   0        0        0     1066 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/testing/slippage.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.514509 zipline-tej-0.0.9/zipline-tej/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/algo_instance.py
+-rw-rw-rw-   0        0        0     4268 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/api_support.py
+-rw-rw-rw-   0        0        0    10164 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/argcheck.py
+-rw-rw-rw-   0        0        0    11721 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/cache.py
+-rw-rw-rw-   0        0        0     4063 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/calendar_utils.py
+-rw-rw-rw-   0        0        0      191 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/classproperty.py
+-rw-rw-rw-   0        0        0     3319 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/cli.py
+-rw-rw-rw-   0        0        0      854 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/compat.py
+-rw-rw-rw-   0        0        0     2244 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/context_tricks.py
+-rw-rw-rw-   0        0        0     7689 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/data.py
+-rw-rw-rw-   0        0        0     1774 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/date_utils.py
+-rw-rw-rw-   0        0        0     1572 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/deprecate.py
+-rw-rw-rw-   0        0        0      248 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/dummy.py
+-rw-rw-rw-   0        0        0    25153 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/events.py
+-rw-rw-rw-   0        0        0     1226 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/exploding_object.py
+-rw-rw-rw-   0        0        0     5023 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/factory.py
+-rw-rw-rw-   0        0        0     3902 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/final.py
+-rw-rw-rw-   0        0        0     1651 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/formatting.py
+-rw-rw-rw-   0        0        0    10662 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/functional.py
+-rw-rw-rw-   0        0        0      665 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/idbox.py
+-rw-rw-rw-   0        0        0    26914 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/input_validation.py
+-rw-rw-rw-   0        0        0     2668 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/math_utils.py
+-rw-rw-rw-   0        0        0     7957 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/memoize.py
+-rw-rw-rw-   0        0        0    13647 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/numpy_utils.py
+-rw-rw-rw-   0        0        0     9268 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/pandas_utils.py
+-rw-rw-rw-   0        0        0     5983 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/paths.py
+-rw-rw-rw-   0        0        0     7429 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/preprocess.py
+-rw-rw-rw-   0        0        0     5025 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/range.py
+-rw-rw-rw-   0        0        0    38036 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/run_algo.py
+-rw-rw-rw-   0        0        0     5408 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/security_list.py
+-rw-rw-rw-   0        0        0     2380 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/sentinel.py
+-rw-rw-rw-   0        0        0     3610 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/sharedoc.py
+-rw-rw-rw-   0        0        0     1760 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/sqlite_utils.py
+-rw-rw-rw-   0        0        0      402 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/utils/string_formatting.py
+-rw-rw-rw-   0        0        0      664 2023-06-02 08:45:48.000000 zipline-tej-0.0.9/zipline-tej/zipline_warnings.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:53:12.530144 zipline-tej-0.0.9/zipline_tej.egg-info/
+-rw-rw-rw-   0        0        0    13262 2023-06-05 03:53:11.000000 zipline-tej-0.0.9/zipline_tej.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10063 2023-06-05 03:53:11.000000 zipline-tej-0.0.9/zipline_tej.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 03:53:11.000000 zipline-tej-0.0.9/zipline_tej.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      442 2023-06-05 03:53:11.000000 zipline-tej-0.0.9/zipline_tej.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-05 03:53:11.000000 zipline-tej-0.0.9/zipline_tej.egg-info/top_level.txt
```

### Comparing `zipline-tej-0.0.8/PKG-INFO` & `zipline-tej-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-tej
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for stock backtesting modified by TEJ.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

### Comparing `zipline-tej-0.0.8/README.md` & `zipline-tej-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/setup.py` & `zipline-tej-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,36 @@
     'requests >= 2.7.0',
     'inflection >= 0.3.1',
     'python-dateutil',
     'six',
     'more-itertools',
     'tejapi',
     'matplotlib',
+    'babel',
+    'Jinja2',
+    'ipython',
+    'matplotlib-inline',
+    'pyzmq',
+    'tornado',
+    'psutil',
+    'pyyaml',
+    'snowballstemmer',
+    'sphinxcontrib-applehelp',
+    'sphinxcontrib-devhelp',
+    'sphinxcontrib-htmlhelp',
+    'sphinxcontrib-jsmath',
+    'sphinxcontrib-qthelp',
+    'sphinxcontrib-serializinghtml',
+    'tinycss2',
+    'pywin32-ctypes',
+    'nest-asyncio',
+    'traitlets',
+    'python-slugify',
+    'click',
+    'Pygments',
 ]
 
 installs_for_two = [
     'pyOpenSSL',
     'ndg-httpsclient',
     'pyasn1'
 ]
@@ -78,15 +100,15 @@
 long_description = (this_directionary/"README.md").read_text(encoding='utf-8')
 setup(
     name='zipline-tej',
     description='Package for stock backtesting modified by TEJ.',
     keywords=['tej', 'zipline', 'data', 'financial', 'economic','stock','backtest','TEJ',],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.8',
+    version='0.0.9',
     author='tej',
     author_email='tej@tej.com.tw',
     maintainer='tej api Development Team',
     maintainer_email='tej@tej.com',
     url='https://api.tej.com.tw',
     license='MIT',
     install_requires=install_requires,
```

### Comparing `zipline-tej-0.0.8/zipline-tej/__init__.py` & `zipline-tej-0.0.9/zipline-tej/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/__main__.py` & `zipline-tej-0.0.9/zipline-tej/__main__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/_version.py` & `zipline-tej-0.0.9/zipline-tej/_version.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/algorithm.py` & `zipline-tej-0.0.9/zipline-tej/algorithm.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/api.py` & `zipline-tej-0.0.9/zipline-tej/api.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/__init__.py` & `zipline-tej-0.0.9/zipline-tej/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/asset_db_migrations.py` & `zipline-tej-0.0.9/zipline-tej/assets/asset_db_migrations.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/asset_db_schema.py` & `zipline-tej-0.0.9/zipline-tej/assets/asset_db_schema.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/asset_writer.py` & `zipline-tej-0.0.9/zipline-tej/assets/asset_writer.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/assets.py` & `zipline-tej-0.0.9/zipline-tej/assets/assets.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/exchange_info.py` & `zipline-tej-0.0.9/zipline-tej/assets/exchange_info.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/futures.py` & `zipline-tej-0.0.9/zipline-tej/assets/futures.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/roll_finder.py` & `zipline-tej-0.0.9/zipline-tej/assets/roll_finder.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/assets/synthetic.py` & `zipline-tej-0.0.9/zipline-tej/assets/synthetic.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/country.py` & `zipline-tej-0.0.9/zipline-tej/country.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/currency.py` & `zipline-tej-0.0.9/zipline-tej/currency.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/adjustments.py` & `zipline-tej-0.0.9/zipline-tej/data/adjustments.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/bar_reader.py` & `zipline-tej-0.0.9/zipline-tej/data/bar_reader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/bcolz_daily_bars.py` & `zipline-tej-0.0.9/zipline-tej/data/bcolz_daily_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/benchmarks.py` & `zipline-tej-0.0.9/zipline-tej/data/benchmarks.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/bundles/__init__.py` & `zipline-tej-0.0.9/zipline-tej/data/bundles/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/bundles/core.py` & `zipline-tej-0.0.9/zipline-tej/data/bundles/core.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/bundles/csvdir.py` & `zipline-tej-0.0.9/zipline-tej/data/bundles/csvdir.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/bundles/quandl.py` & `zipline-tej-0.0.9/zipline-tej/data/bundles/quandl.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/bundles/tquant.py` & `zipline-tej-0.0.9/zipline-tej/data/bundles/tquant.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/continuous_future_reader.py` & `zipline-tej-0.0.9/zipline-tej/data/continuous_future_reader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/data_portal.py` & `zipline-tej-0.0.9/zipline-tej/data/data_portal.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/dispatch_bar_reader.py` & `zipline-tej-0.0.9/zipline-tej/data/dispatch_bar_reader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/fx/base.py` & `zipline-tej-0.0.9/zipline-tej/data/fx/base.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/fx/hdf5.py` & `zipline-tej-0.0.9/zipline-tej/data/fx/hdf5.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/fx/in_memory.py` & `zipline-tej-0.0.9/zipline-tej/data/fx/in_memory.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/hdf5_daily_bars.py` & `zipline-tej-0.0.9/zipline-tej/data/hdf5_daily_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/history_loader.py` & `zipline-tej-0.0.9/zipline-tej/data/history_loader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/in_memory_daily_bars.py` & `zipline-tej-0.0.9/zipline-tej/data/in_memory_daily_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/loader.py` & `zipline-tej-0.0.9/zipline-tej/data/loader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/minute_bars.py` & `zipline-tej-0.0.9/zipline-tej/data/minute_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/resample.py` & `zipline-tej-0.0.9/zipline-tej/data/resample.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/session_bars.py` & `zipline-tej-0.0.9/zipline-tej/data/session_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/data/treasury.py` & `zipline-tej-0.0.9/zipline-tej/data/treasury.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/errors.py` & `zipline-tej-0.0.9/zipline-tej/errors.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/__init__.py` & `zipline-tej-0.0.9/zipline-tej/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/buy_and_hold.py` & `zipline-tej-0.0.9/zipline-tej/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/buyapple.py` & `zipline-tej-0.0.9/zipline-tej/examples/buyapple.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/buyapple_ide.py` & `zipline-tej-0.0.9/zipline-tej/examples/buyapple_ide.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/dual_ema_talib.py` & `zipline-tej-0.0.9/zipline-tej/examples/dual_ema_talib.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/dual_moving_average.py` & `zipline-tej-0.0.9/zipline-tej/examples/dual_moving_average.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/momentum_pipeline.py` & `zipline-tej-0.0.9/zipline-tej/examples/momentum_pipeline.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/examples/olmar.py` & `zipline-tej-0.0.9/zipline-tej/examples/olmar.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/extensions.py` & `zipline-tej-0.0.9/zipline-tej/extensions.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/__init__.py` & `zipline-tej-0.0.9/zipline-tej/finance/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/asset_restrictions.py` & `zipline-tej-0.0.9/zipline-tej/finance/asset_restrictions.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/blotter/__init__.py` & `zipline-tej-0.0.9/zipline-tej/finance/blotter/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/blotter/blotter.py` & `zipline-tej-0.0.9/zipline-tej/finance/blotter/blotter.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/blotter/simulation_blotter.py` & `zipline-tej-0.0.9/zipline-tej/finance/blotter/simulation_blotter.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/cancel_policy.py` & `zipline-tej-0.0.9/zipline-tej/finance/cancel_policy.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/commission.py` & `zipline-tej-0.0.9/zipline-tej/finance/commission.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/constants.py` & `zipline-tej-0.0.9/zipline-tej/finance/constants.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/controls.py` & `zipline-tej-0.0.9/zipline-tej/finance/controls.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/execution.py` & `zipline-tej-0.0.9/zipline-tej/finance/execution.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/ledger.py` & `zipline-tej-0.0.9/zipline-tej/finance/ledger.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/metrics/__init__.py` & `zipline-tej-0.0.9/zipline-tej/finance/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/metrics/core.py` & `zipline-tej-0.0.9/zipline-tej/finance/metrics/core.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/metrics/metric.py` & `zipline-tej-0.0.9/zipline-tej/finance/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/metrics/tracker.py` & `zipline-tej-0.0.9/zipline-tej/finance/metrics/tracker.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/order.py` & `zipline-tej-0.0.9/zipline-tej/finance/order.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/position.py` & `zipline-tej-0.0.9/zipline-tej/finance/position.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/shared.py` & `zipline-tej-0.0.9/zipline-tej/finance/shared.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/slippage.py` & `zipline-tej-0.0.9/zipline-tej/finance/slippage.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/trading.py` & `zipline-tej-0.0.9/zipline-tej/finance/trading.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/finance/transaction.py` & `zipline-tej-0.0.9/zipline-tej/finance/transaction.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/gens/composites.py` & `zipline-tej-0.0.9/zipline-tej/gens/composites.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/gens/tradesimulation.py` & `zipline-tej-0.0.9/zipline-tej/gens/tradesimulation.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/gens/utils.py` & `zipline-tej-0.0.9/zipline-tej/gens/utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/lib/adjusted_array.py` & `zipline-tej-0.0.9/zipline-tej/lib/adjusted_array.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/lib/labelarray.py` & `zipline-tej-0.0.9/zipline-tej/lib/labelarray.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/lib/normalize.py` & `zipline-tej-0.0.9/zipline-tej/lib/normalize.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/master.py` & `zipline-tej-0.0.9/zipline-tej/master.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/__init__.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/api_utils.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/api_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/classifiers/classifier.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/classifiers/classifier.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/common.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/common.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/data/dataset.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/data/dataset.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/data/equity_pricing.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/data/equity_pricing.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/data/tejquant.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/data/tejquant.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/data/testing.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/data/testing.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/domain.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/domain.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/downsample_helpers.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/downsample_helpers.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/engine.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/engine.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/expression.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/expression.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/factors/__init__.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/factors/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/factors/basic.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/factors/basic.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/factors/events.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/factors/events.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/factors/factor.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/factors/factor.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/factors/statistical.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/factors/statistical.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/factors/technical.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/factors/technical.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/filters/__init__.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/filters/filter.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/filters/filter.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/filters/smoothing.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/filters/smoothing.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/graph.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/graph.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/hooks/delegate.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/hooks/delegate.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/hooks/iface.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/hooks/iface.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/hooks/no.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/hooks/no.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/hooks/progress.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/hooks/progress.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/hooks/testing.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/hooks/testing.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/base.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/base.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/earnings_estimates.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/earnings_estimates.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/equity_pricing_loader.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/equity_pricing_loader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/events.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/events.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/frame.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/frame.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/synthetic.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/synthetic.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/testing.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/testing.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/loaders/utils.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/loaders/utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/mixins.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/mixins.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/pipeline.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/term.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/term.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/pipeline/visualize.py` & `zipline-tej-0.0.9/zipline-tej/pipeline/visualize.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/protocol.py` & `zipline-tej-0.0.9/zipline-tej/protocol.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/resources/market_data/SPY_benchmark.csv` & `zipline-tej-0.0.9/zipline-tej/resources/market_data/SPY_benchmark.csv`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/resources/market_data/treasury_curves.csv` & `zipline-tej-0.0.9/zipline-tej/resources/market_data/treasury_curves.csv`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/add` & `zipline-tej-0.0.9/zipline-tej/resources/security_lists/leveraged_etf_list/20020103/20150123/add`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/test_algorithms.py` & `zipline-tej-0.0.9/zipline-tej/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/testing/__init__.py` & `zipline-tej-0.0.9/zipline-tej/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/testing/core.py` & `zipline-tej-0.0.9/zipline-tej/testing/core.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/testing/debug.py` & `zipline-tej-0.0.9/zipline-tej/testing/debug.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/testing/fixtures.py` & `zipline-tej-0.0.9/zipline-tej/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/testing/pipeline_terms.py` & `zipline-tej-0.0.9/zipline-tej/testing/pipeline_terms.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/testing/predicates.py` & `zipline-tej-0.0.9/zipline-tej/testing/predicates.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/testing/slippage.py` & `zipline-tej-0.0.9/zipline-tej/testing/slippage.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/algo_instance.py` & `zipline-tej-0.0.9/zipline-tej/utils/algo_instance.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/api_support.py` & `zipline-tej-0.0.9/zipline-tej/utils/api_support.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/argcheck.py` & `zipline-tej-0.0.9/zipline-tej/utils/argcheck.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/cache.py` & `zipline-tej-0.0.9/zipline-tej/utils/cache.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/calendar_utils.py` & `zipline-tej-0.0.9/zipline-tej/utils/calendar_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/cli.py` & `zipline-tej-0.0.9/zipline-tej/utils/cli.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/compat.py` & `zipline-tej-0.0.9/zipline-tej/utils/compat.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/context_tricks.py` & `zipline-tej-0.0.9/zipline-tej/utils/context_tricks.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/data.py` & `zipline-tej-0.0.9/zipline-tej/utils/data.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/date_utils.py` & `zipline-tej-0.0.9/zipline-tej/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/deprecate.py` & `zipline-tej-0.0.9/zipline-tej/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/events.py` & `zipline-tej-0.0.9/zipline-tej/utils/events.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/exploding_object.py` & `zipline-tej-0.0.9/zipline-tej/utils/exploding_object.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/factory.py` & `zipline-tej-0.0.9/zipline-tej/utils/factory.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/final.py` & `zipline-tej-0.0.9/zipline-tej/utils/final.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/formatting.py` & `zipline-tej-0.0.9/zipline-tej/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/functional.py` & `zipline-tej-0.0.9/zipline-tej/utils/functional.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/idbox.py` & `zipline-tej-0.0.9/zipline-tej/utils/idbox.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/input_validation.py` & `zipline-tej-0.0.9/zipline-tej/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/math_utils.py` & `zipline-tej-0.0.9/zipline-tej/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/memoize.py` & `zipline-tej-0.0.9/zipline-tej/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/numpy_utils.py` & `zipline-tej-0.0.9/zipline-tej/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/pandas_utils.py` & `zipline-tej-0.0.9/zipline-tej/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/paths.py` & `zipline-tej-0.0.9/zipline-tej/utils/paths.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/preprocess.py` & `zipline-tej-0.0.9/zipline-tej/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/range.py` & `zipline-tej-0.0.9/zipline-tej/utils/range.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/run_algo.py` & `zipline-tej-0.0.9/zipline-tej/utils/run_algo.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/security_list.py` & `zipline-tej-0.0.9/zipline-tej/utils/security_list.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/sentinel.py` & `zipline-tej-0.0.9/zipline-tej/utils/sentinel.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/sharedoc.py` & `zipline-tej-0.0.9/zipline-tej/utils/sharedoc.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/utils/sqlite_utils.py` & `zipline-tej-0.0.9/zipline-tej/utils/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline-tej/zipline_warnings.py` & `zipline-tej-0.0.9/zipline-tej/zipline_warnings.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.8/zipline_tej.egg-info/PKG-INFO` & `zipline-tej-0.0.9/zipline_tej.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-tej
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for stock backtesting modified by TEJ.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

### Comparing `zipline-tej-0.0.8/zipline_tej.egg-info/SOURCES.txt` & `zipline-tej-0.0.9/zipline_tej.egg-info/SOURCES.txt`

 * *Files identical despite different names*

