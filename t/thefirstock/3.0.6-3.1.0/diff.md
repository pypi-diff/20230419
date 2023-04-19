# Comparing `tmp/thefirstock-3.0.6.tar.gz` & `tmp/thefirstock-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thefirstock-3.0.6.tar", last modified: Sun Mar 19 14:36:44 2023, max compression
+gzip compressed data, was "thefirstock-3.1.0.tar", last modified: Wed Apr 19 12:42:54 2023, max compression
```

## Comparing `thefirstock-3.0.6.tar` & `thefirstock-3.1.0.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.568957 thefirstock-3.0.6/
--rw-rw-rw-   0        0        0     1084 2022-04-12 18:40:30.000000 thefirstock-3.0.6/LICENSE
--rw-rw-rw-   0        0        0     3210 2023-03-19 14:36:44.568957 thefirstock-3.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2682 2023-02-27 19:53:45.000000 thefirstock-3.0.6/README.md
--rw-rw-rw-   0        0        0       86 2022-04-18 19:26:35.000000 thefirstock-3.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      715 2023-03-19 14:36:44.574960 thefirstock-3.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.291175 thefirstock-3.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.327174 thefirstock-3.0.6/src/thefirstock/
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.358175 thefirstock-3.0.6/src/thefirstock/Variables/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:54.000000 thefirstock-3.0.6/src/thefirstock/Variables/__init__.py
--rw-rw-rw-   0        0        0     2414 2023-03-19 14:08:42.000000 thefirstock-3.0.6/src/thefirstock/Variables/enums.py
--rw-rw-rw-   0        0        0       91 2023-02-28 04:28:54.000000 thefirstock-3.0.6/src/thefirstock/Variables/fixedParams.py
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:54.000000 thefirstock-3.0.6/src/thefirstock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.360174 thefirstock-3.0.6/src/thefirstock/firstockModules/
--rw-rw-rw-   0        0        0        0 2023-03-14 16:36:13.000000 thefirstock-3.0.6/src/thefirstock/firstockModules/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/firstockModules/firstockWebSockets.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.364172 thefirstock-3.0.6/src/thefirstock/loginNProfile/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/__init__.py
--rw-rw-rw-   0        0        0      423 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/loginFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.369177 thefirstock-3.0.6/src/thefirstock/loginNProfile/loginFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/loginFunctionality/__init__.py
--rw-rw-rw-   0        0        0      196 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/loginFunctionality/base.py
--rw-rw-rw-   0        0        0      473 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/loginFunctionality/execution.py
--rw-rw-rw-   0        0        0     1197 2023-03-09 05:55:14.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/loginFunctionality/functions.py
--rw-rw-rw-   0        0        0      222 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/logoutFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.375179 thefirstock-3.0.6/src/thefirstock/loginNProfile/logoutFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/logoutFunctionality/__init__.py
--rw-rw-rw-   0        0        0      166 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/logoutFunctionality/base.py
--rw-rw-rw-   0        0        0      267 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/logoutFunctionality/execution.py
--rw-rw-rw-   0        0        0      673 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/logoutFunctionality/functions.py
--rw-rw-rw-   0        0        0      253 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/userDetailsFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.379687 thefirstock-3.0.6/src/thefirstock/loginNProfile/userDetailsFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/userDetailsFunctionality/__init__.py
--rw-rw-rw-   0        0        0      171 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/userDetailsFunctionality/base.py
--rw-rw-rw-   0        0        0      283 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/userDetailsFunctionality/execution.py
--rw-rw-rw-   0        0        0      706 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/loginNProfile/userDetailsFunctionality/functions.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.393694 thefirstock-3.0.6/src/thefirstock/marketConnect/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/__init__.py
--rw-rw-rw-   0        0        0      326 2023-02-28 04:28:55.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getIndexListFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.397694 thefirstock-3.0.6/src/thefirstock/marketConnect/getIndexListFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getIndexListFunctionality/__init__.py
--rw-rw-rw-   0        0        0      178 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getIndexListFunctionality/base.py
--rw-rw-rw-   0        0        0      329 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getIndexListFunctionality/execution.py
--rw-rw-rw-   0        0        0      865 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getIndexListFunctionality/functions.py
--rw-rw-rw-   0        0        0      320 2023-03-19 14:32:03.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.401694 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteFunctionality/
--rw-rw-rw-   0        0        0        0 2023-03-19 14:08:27.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteFunctionality/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-19 14:28:46.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteFunctionality/base.py
--rw-rw-rw-   0        0        0      348 2023-03-19 14:29:40.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteFunctionality/execution.py
--rw-rw-rw-   0        0        0      858 2023-03-19 14:30:03.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteFunctionality/functions.py
--rw-rw-rw-   0        0        0      331 2023-03-19 14:26:33.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteLTPFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.406698 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/
--rw-rw-rw-   0        0        0        0 2023-03-19 14:06:00.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/__init__.py
--rw-rw-rw-   0        0        0      187 2023-03-19 14:26:21.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/base.py
--rw-rw-rw-   0        0        0      359 2023-03-19 14:26:33.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/execution.py
--rw-rw-rw-   0        0        0      866 2023-03-19 14:26:18.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/functions.py
--rw-rw-rw-   0        0        0      427 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getOptionChainFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.411695 thefirstock-3.0.6/src/thefirstock/marketConnect/getOptionChainFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getOptionChainFunctionality/__init__.py
--rw-rw-rw-   0        0        0      199 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getOptionChainFunctionality/base.py
--rw-rw-rw-   0        0        0      472 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getOptionChainFunctionality/execution.py
--rw-rw-rw-   0        0        0      848 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getOptionChainFunctionality/functions.py
--rw-rw-rw-   0        0        0      335 2023-03-19 14:12:06.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuoteLTPFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.415694 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuoteLTPFuntionality/
--rw-rw-rw-   0        0        0        0 2023-03-19 14:05:19.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuoteLTPFuntionality/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-19 14:10:50.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuoteLTPFuntionality/base.py
--rw-rw-rw-   0        0        0      363 2023-03-19 14:11:37.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuoteLTPFuntionality/execution.py
--rw-rw-rw-   0        0        0      883 2023-03-19 14:11:37.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuoteLTPFuntionality/functions.py
--rw-rw-rw-   0        0        0      315 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuotesFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.419695 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuotesFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuotesFunctionality/__init__.py
--rw-rw-rw-   0        0        0      182 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuotesFunctionality/base.py
--rw-rw-rw-   0        0        0      358 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuotesFunctionality/execution.py
--rw-rw-rw-   0        0        0      878 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getQuotesFunctionality/functions.py
--rw-rw-rw-   0        0        0      347 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getSecurityInfoFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.424693 thefirstock-3.0.6/src/thefirstock/marketConnect/getSecurityInfoFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getSecurityInfoFunctionality/__init__.py
--rw-rw-rw-   0        0        0      188 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getSecurityInfoFunctionality/base.py
--rw-rw-rw-   0        0        0      393 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getSecurityInfoFunctionality/execution.py
--rw-rw-rw-   0        0        0      897 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/getSecurityInfoFunctionality/functions.py
--rw-rw-rw-   0        0        0      560 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.428215 thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFunctionality/__init__.py
--rw-rw-rw-   0        0        0      241 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFunctionality/base.py
--rw-rw-rw-   0        0        0      778 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFunctionality/execution.py
--rw-rw-rw-   0        0        0     1217 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFunctionality/functions.py
--rw-rw-rw-   0        0        0      298 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/searchScripsFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.432752 thefirstock-3.0.6/src/thefirstock/marketConnect/searchScripsFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/searchScripsFunctionality/__init__.py
--rw-rw-rw-   0        0        0      179 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/searchScripsFunctionality/base.py
--rw-rw-rw-   0        0        0      333 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/searchScripsFunctionality/execution.py
--rw-rw-rw-   0        0        0      853 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/searchScripsFunctionality/functions.py
--rw-rw-rw-   0        0        0      319 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/spanCalculatorFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.437282 thefirstock-3.0.6/src/thefirstock/marketConnect/spanCalculatorFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/spanCalculatorFunctionality/__init__.py
--rw-rw-rw-   0        0        0      184 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/spanCalculatorFunctionality/base.py
--rw-rw-rw-   0        0        0      359 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/spanCalculatorFunctionality/execution.py
--rw-rw-rw-   0        0        0      737 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/spanCalculatorFunctionality/functions.py
--rw-rw-rw-   0        0        0      449 2023-02-28 04:28:56.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/timePriceSeriesFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.441282 thefirstock-3.0.6/src/thefirstock/marketConnect/timePriceSeriesFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/timePriceSeriesFunctionality/__init__.py
--rw-rw-rw-   0        0        0      203 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/timePriceSeriesFunctionality/base.py
--rw-rw-rw-   0        0        0      508 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/timePriceSeriesFunctionality/execution.py
--rw-rw-rw-   0        0        0      872 2023-02-28 04:28:57.000000 thefirstock-3.0.6/src/thefirstock/marketConnect/timePriceSeriesFunctionality/functions.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.455282 thefirstock-3.0.6/src/thefirstock/ordersNReport/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/__init__.py
--rw-rw-rw-   0        0        0      321 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/basketMarginFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.459282 thefirstock-3.0.6/src/thefirstock/ordersNReport/basketMarginFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/basketMarginFunctionality/__init__.py
--rw-rw-rw-   0        0        0      180 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/basketMarginFunctionality/base.py
--rw-rw-rw-   0        0        0      337 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/basketMarginFunctionality/execution.py
--rw-rw-rw-   0        0        0      878 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/basketMarginFunctionality/functions.py
--rw-rw-rw-   0        0        0      309 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/cancelOrderFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.463287 thefirstock-3.0.6/src/thefirstock/ordersNReport/cancelOrderFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/cancelOrderFunctionality/__init__.py
--rw-rw-rw-   0        0        0      184 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/cancelOrderFunctionality/base.py
--rw-rw-rw-   0        0        0      352 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/cancelOrderFunctionality/execution.py
--rw-rw-rw-   0        0        0      862 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/cancelOrderFunctionality/functions.py
--rw-rw-rw-   0        0        0      234 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/holdingFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.467292 thefirstock-3.0.6/src/thefirstock/ordersNReport/holdingsFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/holdingsFunctionality/__init__.py
--rw-rw-rw-   0        0        0      168 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/holdingsFunctionality/base.py
--rw-rw-rw-   0        0        0      265 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/holdingsFunctionality/execution.py
--rw-rw-rw-   0        0        0      859 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/holdingsFunctionality/functions.py
--rw-rw-rw-   0        0        0      223 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/limitFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.471292 thefirstock-3.0.6/src/thefirstock/ordersNReport/limitFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/limitFunctionality/__init__.py
--rw-rw-rw-   0        0        0      165 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/limitFunctionality/base.py
--rw-rw-rw-   0        0        0      252 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/limitFunctionality/execution.py
--rw-rw-rw-   0        0        0      820 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/limitFunctionality/functions.py
--rw-rw-rw-   0        0        0      564 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.475292 thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFunctionality/__init__.py
--rw-rw-rw-   0        0        0      238 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFunctionality/base.py
--rw-rw-rw-   0        0        0      729 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFunctionality/execution.py
--rw-rw-rw-   0        0        0     1146 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFunctionality/functions.py
--rw-rw-rw-   0        0        0      241 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderBookFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.481434 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderBookFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderBookFunctionality/__init__.py
--rw-rw-rw-   0        0        0      169 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderBookFunctionality/base.py
--rw-rw-rw-   0        0        0      272 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderBookFunctionality/execution.py
--rw-rw-rw-   0        0        0      800 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderBookFunctionality/functions.py
--rw-rw-rw-   0        0        0      546 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.485428 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:28:59.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFunctionality/__init__.py
--rw-rw-rw-   0        0        0      219 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFunctionality/base.py
--rw-rw-rw-   0        0        0      663 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFunctionality/execution.py
--rw-rw-rw-   0        0        0     1134 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFunctionality/functions.py
--rw-rw-rw-   0        0        0      679 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.490430 thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFunctionality/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFunctionality/base.py
--rw-rw-rw-   0        0        0      775 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFunctionality/execution.py
--rw-rw-rw-   0        0        0     1072 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFunctionality/functions.py
--rw-rw-rw-   0        0        0      259 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/positionBookFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.495434 thefirstock-3.0.6/src/thefirstock/ordersNReport/positionBookFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/positionBookFunctionality/__init__.py
--rw-rw-rw-   0        0        0      172 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/positionBookFunctionality/base.py
--rw-rw-rw-   0        0        0      289 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/positionBookFunctionality/execution.py
--rw-rw-rw-   0        0        0      840 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/positionBookFunctionality/functions.py
--rw-rw-rw-   0        0        0      592 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.499430 thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFunctionality/__init__.py
--rw-rw-rw-   0        0        0      224 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFunctionality/base.py
--rw-rw-rw-   0        0        0      689 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFunctionality/execution.py
--rw-rw-rw-   0        0        0     1169 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFunctionality/functions.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.503433 thefirstock-3.0.6/src/thefirstock/ordersNReport/singleOrderHistory/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/singleOrderHistory/__init__.py
--rw-rw-rw-   0        0        0      191 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/singleOrderHistory/base.py
--rw-rw-rw-   0        0        0      381 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/singleOrderHistory/execution.py
--rw-rw-rw-   0        0        0      870 2023-02-28 04:29:00.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/singleOrderHistory/functions.py
--rw-rw-rw-   0        0        0      338 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/singleOrderHistoryFirstock.py
--rw-rw-rw-   0        0        0      242 2023-02-28 04:28:58.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/tradeBookFirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.508428 thefirstock-3.0.6/src/thefirstock/ordersNReport/tradeBookFunctionality/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/tradeBookFunctionality/__init__.py
--rw-rw-rw-   0        0        0      169 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/tradeBookFunctionality/base.py
--rw-rw-rw-   0        0        0      271 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/tradeBookFunctionality/execution.py
--rw-rw-rw-   0        0        0      829 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/ordersNReport/tradeBookFunctionality/functions.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.511430 thefirstock-3.0.6/src/thefirstock/pyClient/
--rw-rw-rw-   0        0        0     1034 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/__init__.py
--rw-rw-rw-   0        0        0     1481 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/client.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.516434 thefirstock-3.0.6/src/thefirstock/pyClient/common/
--rw-rw-rw-   0        0        0      132 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/common/__init__.py
--rw-rw-rw-   0        0        0      789 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/common/enums.py
--rw-rw-rw-   0        0        0     2536 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/common/exceptions.py
--rw-rw-rw-   0        0        0     2569 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/common/models.py
--rw-rw-rw-   0        0        0      286 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/models.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.517430 thefirstock-3.0.6/src/thefirstock/pyClient/modules/
--rw-rw-rw-   0        0        0       62 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.521433 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/
--rw-rw-rw-   0        0        0      502 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/datasource.py
--rw-rw-rw-   0        0        0      366 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/endpoints.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.525429 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/models/
--rw-rw-rw-   0        0        0       89 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/models/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/models/login.py
--rw-rw-rw-   0        0        0      962 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/models/save_fcm_token.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.530427 thefirstock-3.0.6/src/thefirstock/pyClient/utils/
--rw-rw-rw-   0        0        0      150 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.531431 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/
--rw-rw-rw-   0        0        0       94 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.534430 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/noren/
--rw-rw-rw-   0        0        0       25 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/noren/__init__.py
--rw-rw-rw-   0        0        0      684 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/noren/datasource.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.538051 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/rest/
--rw-rw-rw-   0        0        0       26 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/rest/__init__.py
--rw-rw-rw-   0        0        0      480 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/rest/context.py
--rw-rw-rw-   0        0        0     3998 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/rest/datasource.py
--rw-rw-rw-   0        0        0     2726 2023-02-28 04:29:01.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/decoders.py
--rw-rw-rw-   0        0        0     3103 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/encoders.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.541539 thefirstock-3.0.6/src/thefirstock/pyClient/utils/interceptors/
--rw-rw-rw-   0        0        0       27 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/interceptors/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/interceptors/http_error.py
--rw-rw-rw-   0        0        0      814 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/interceptors/interceptor.py
--rw-rw-rw-   0        0        0     1151 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/utils/stateful.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.544874 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/
--rw-rw-rw-   0        0        0     1482 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/__init__.py
--rw-rw-rw-   0        0        0     5581 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/client.py
--rw-rw-rw-   0        0        0      626 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/enums.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.549935 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/
--rw-rw-rw-   0        0        0       71 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/__init__.py
--rw-rw-rw-   0        0        0      582 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/connection.py
--rw-rw-rw-   0        0        0      932 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/depth.py
--rw-rw-rw-   0        0        0      810 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/order.py
--rw-rw-rw-   0        0        0     1031 2023-02-28 04:29:02.000000 thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/touchline.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.567953 thefirstock-3.0.6/src/thefirstock/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/bearPutSpread.py
--rw-rw-rw-   0        0        0      592 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/bearPutSpreadFirstock.py
--rw-rw-rw-   0        0        0      881 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/bullCallSpread.py
--rw-rw-rw-   0        0        0      602 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/bullCallSpreadFirstock.py
--rw-rw-rw-   0        0        0      748 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/longStraddle.py
--rw-rw-rw-   0        0        0      493 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/longStraddleFirstock.py
--rw-rw-rw-   0        0        0      823 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/longStrangle.py
--rw-rw-rw-   0        0        0      569 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/longStrangleFirstock.py
--rw-rw-rw-   0        0        0      535 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/multiPlaceOrder.py
--rw-rw-rw-   0        0        0      256 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/multiPlaceOrderFirstock.py
--rw-rw-rw-   0        0        0      866 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/shortStraddle.py
--rw-rw-rw-   0        0        0      585 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/shortStraddleFirstock.py
--rw-rw-rw-   0        0        0      942 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/shortStrangle.py
--rw-rw-rw-   0        0        0      661 2023-02-28 04:29:03.000000 thefirstock-3.0.6/src/thefirstock/strategies/shortStrangleFirstock.py
--rw-rw-rw-   0        0        0     4413 2023-03-19 14:32:42.000000 thefirstock-3.0.6/src/thefirstock/thefirstock.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:36:44.354175 thefirstock-3.0.6/src/thefirstock.egg-info/
--rw-rw-rw-   0        0        0     3210 2023-03-19 14:36:44.000000 thefirstock-3.0.6/src/thefirstock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11400 2023-03-19 14:36:44.000000 thefirstock-3.0.6/src/thefirstock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 14:36:44.000000 thefirstock-3.0.6/src/thefirstock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-19 14:36:44.000000 thefirstock-3.0.6/src/thefirstock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-19 14:36:44.000000 thefirstock-3.0.6/src/thefirstock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.935769 thefirstock-3.1.0/
+-rw-rw-rw-   0        0        0     1084 2022-04-12 18:40:32.000000 thefirstock-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3210 2023-04-19 12:42:54.936766 thefirstock-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2682 2023-03-20 06:17:40.000000 thefirstock-3.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-18 19:26:36.000000 thefirstock-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      715 2023-04-19 12:42:54.937768 thefirstock-3.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.742628 thefirstock-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.766525 thefirstock-3.1.0/src/thefirstock/
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.804169 thefirstock-3.1.0/src/thefirstock/Variables/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/Variables/__init__.py
+-rw-rw-rw-   0        0        0     2414 2023-03-19 14:08:44.000000 thefirstock-3.1.0/src/thefirstock/Variables/enums.py
+-rw-rw-rw-   0        0        0       91 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/Variables/fixedParams.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.805966 thefirstock-3.1.0/src/thefirstock/firstockModules/
+-rw-rw-rw-   0        0        0        0 2023-03-14 16:36:14.000000 thefirstock-3.1.0/src/thefirstock/firstockModules/__init__.py
+-rw-rw-rw-   0        0        0     2460 2023-04-19 12:26:49.000000 thefirstock-3.1.0/src/thefirstock/firstockModules/firstockWebSockets.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.810750 thefirstock-3.1.0/src/thefirstock/loginNProfile/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/loginFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.813747 thefirstock-3.1.0/src/thefirstock/loginNProfile/loginFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/loginFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/loginFunctionality/base.py
+-rw-rw-rw-   0        0        0      473 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/loginFunctionality/execution.py
+-rw-rw-rw-   0        0        0     1197 2023-04-12 11:34:46.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/loginFunctionality/functions.py
+-rw-rw-rw-   0        0        0      222 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/logoutFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.816259 thefirstock-3.1.0/src/thefirstock/loginNProfile/logoutFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/logoutFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/logoutFunctionality/base.py
+-rw-rw-rw-   0        0        0      267 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/logoutFunctionality/execution.py
+-rw-rw-rw-   0        0        0      673 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/logoutFunctionality/functions.py
+-rw-rw-rw-   0        0        0      253 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/userDetailsFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.819271 thefirstock-3.1.0/src/thefirstock/loginNProfile/userDetailsFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/userDetailsFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      171 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/userDetailsFunctionality/base.py
+-rw-rw-rw-   0        0        0      283 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/userDetailsFunctionality/execution.py
+-rw-rw-rw-   0        0        0      706 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/loginNProfile/userDetailsFunctionality/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.829172 thefirstock-3.1.0/src/thefirstock/marketConnect/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-02-28 04:28:56.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getIndexListFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.832176 thefirstock-3.1.0/src/thefirstock/marketConnect/getIndexListFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getIndexListFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      178 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getIndexListFunctionality/base.py
+-rw-rw-rw-   0        0        0      329 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getIndexListFunctionality/execution.py
+-rw-rw-rw-   0        0        0      865 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getIndexListFunctionality/functions.py
+-rw-rw-rw-   0        0        0      320 2023-03-19 14:32:04.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.835177 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-03-19 14:08:28.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-19 14:28:48.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteFunctionality/base.py
+-rw-rw-rw-   0        0        0      348 2023-03-19 14:29:42.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteFunctionality/execution.py
+-rw-rw-rw-   0        0        0      858 2023-03-19 14:30:04.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteFunctionality/functions.py
+-rw-rw-rw-   0        0        0      331 2023-03-19 14:26:34.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteLTPFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.838216 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/
+-rw-rw-rw-   0        0        0        0 2023-03-19 14:06:02.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-03-19 14:26:22.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/base.py
+-rw-rw-rw-   0        0        0      359 2023-03-19 14:26:34.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/execution.py
+-rw-rw-rw-   0        0        0      866 2023-03-19 14:26:20.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/functions.py
+-rw-rw-rw-   0        0        0      427 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getOptionChainFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.841210 thefirstock-3.1.0/src/thefirstock/marketConnect/getOptionChainFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getOptionChainFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      199 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getOptionChainFunctionality/base.py
+-rw-rw-rw-   0        0        0      472 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getOptionChainFunctionality/execution.py
+-rw-rw-rw-   0        0        0      848 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getOptionChainFunctionality/functions.py
+-rw-rw-rw-   0        0        0      335 2023-03-19 14:12:08.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuoteLTPFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.844220 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuoteLTPFuntionality/
+-rw-rw-rw-   0        0        0        0 2023-03-19 14:05:20.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuoteLTPFuntionality/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-19 14:10:52.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuoteLTPFuntionality/base.py
+-rw-rw-rw-   0        0        0      363 2023-03-19 14:11:38.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuoteLTPFuntionality/execution.py
+-rw-rw-rw-   0        0        0      883 2023-03-19 14:11:38.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuoteLTPFuntionality/functions.py
+-rw-rw-rw-   0        0        0      315 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuotesFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.846213 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuotesFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuotesFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      182 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuotesFunctionality/base.py
+-rw-rw-rw-   0        0        0      358 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuotesFunctionality/execution.py
+-rw-rw-rw-   0        0        0      878 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getQuotesFunctionality/functions.py
+-rw-rw-rw-   0        0        0      347 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getSecurityInfoFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.849743 thefirstock-3.1.0/src/thefirstock/marketConnect/getSecurityInfoFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getSecurityInfoFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      188 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getSecurityInfoFunctionality/base.py
+-rw-rw-rw-   0        0        0      393 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getSecurityInfoFunctionality/execution.py
+-rw-rw-rw-   0        0        0      897 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/getSecurityInfoFunctionality/functions.py
+-rw-rw-rw-   0        0        0      560 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.853743 thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFunctionality/base.py
+-rw-rw-rw-   0        0        0      778 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFunctionality/execution.py
+-rw-rw-rw-   0        0        0     1217 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFunctionality/functions.py
+-rw-rw-rw-   0        0        0      298 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/searchScripsFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.856740 thefirstock-3.1.0/src/thefirstock/marketConnect/searchScripsFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/searchScripsFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/searchScripsFunctionality/base.py
+-rw-rw-rw-   0        0        0      333 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/searchScripsFunctionality/execution.py
+-rw-rw-rw-   0        0        0      853 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/searchScripsFunctionality/functions.py
+-rw-rw-rw-   0        0        0      319 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/spanCalculatorFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.859270 thefirstock-3.1.0/src/thefirstock/marketConnect/spanCalculatorFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/spanCalculatorFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/spanCalculatorFunctionality/base.py
+-rw-rw-rw-   0        0        0      359 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/spanCalculatorFunctionality/execution.py
+-rw-rw-rw-   0        0        0      737 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/spanCalculatorFunctionality/functions.py
+-rw-rw-rw-   0        0        0      449 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/timePriceSeriesFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.862270 thefirstock-3.1.0/src/thefirstock/marketConnect/timePriceSeriesFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/timePriceSeriesFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/timePriceSeriesFunctionality/base.py
+-rw-rw-rw-   0        0        0      508 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/timePriceSeriesFunctionality/execution.py
+-rw-rw-rw-   0        0        0      872 2023-02-28 04:28:58.000000 thefirstock-3.1.0/src/thefirstock/marketConnect/timePriceSeriesFunctionality/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.872794 thefirstock-3.1.0/src/thefirstock/ordersNReport/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/basketMarginFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.875797 thefirstock-3.1.0/src/thefirstock/ordersNReport/basketMarginFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/basketMarginFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/basketMarginFunctionality/base.py
+-rw-rw-rw-   0        0        0      337 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/basketMarginFunctionality/execution.py
+-rw-rw-rw-   0        0        0      878 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/basketMarginFunctionality/functions.py
+-rw-rw-rw-   0        0        0      309 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/cancelOrderFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.877799 thefirstock-3.1.0/src/thefirstock/ordersNReport/cancelOrderFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/cancelOrderFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/cancelOrderFunctionality/base.py
+-rw-rw-rw-   0        0        0      352 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/cancelOrderFunctionality/execution.py
+-rw-rw-rw-   0        0        0      862 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/cancelOrderFunctionality/functions.py
+-rw-rw-rw-   0        0        0      234 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/holdingFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.880320 thefirstock-3.1.0/src/thefirstock/ordersNReport/holdingsFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/holdingsFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/holdingsFunctionality/base.py
+-rw-rw-rw-   0        0        0      265 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/holdingsFunctionality/execution.py
+-rw-rw-rw-   0        0        0      859 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/holdingsFunctionality/functions.py
+-rw-rw-rw-   0        0        0      223 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/limitFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.883321 thefirstock-3.1.0/src/thefirstock/ordersNReport/limitFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/limitFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/limitFunctionality/base.py
+-rw-rw-rw-   0        0        0      252 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/limitFunctionality/execution.py
+-rw-rw-rw-   0        0        0      820 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/limitFunctionality/functions.py
+-rw-rw-rw-   0        0        0      564 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.886325 thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      238 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFunctionality/base.py
+-rw-rw-rw-   0        0        0      729 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFunctionality/execution.py
+-rw-rw-rw-   0        0        0     1146 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFunctionality/functions.py
+-rw-rw-rw-   0        0        0      241 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderBookFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.888324 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderBookFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderBookFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      169 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderBookFunctionality/base.py
+-rw-rw-rw-   0        0        0      272 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderBookFunctionality/execution.py
+-rw-rw-rw-   0        0        0      800 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderBookFunctionality/functions.py
+-rw-rw-rw-   0        0        0      546 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.890855 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFunctionality/base.py
+-rw-rw-rw-   0        0        0      663 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFunctionality/execution.py
+-rw-rw-rw-   0        0        0     1134 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFunctionality/functions.py
+-rw-rw-rw-   0        0        0      679 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.893855 thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFunctionality/base.py
+-rw-rw-rw-   0        0        0      775 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFunctionality/execution.py
+-rw-rw-rw-   0        0        0     1072 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFunctionality/functions.py
+-rw-rw-rw-   0        0        0      259 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/positionBookFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.895854 thefirstock-3.1.0/src/thefirstock/ordersNReport/positionBookFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/positionBookFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      172 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/positionBookFunctionality/base.py
+-rw-rw-rw-   0        0        0      289 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/positionBookFunctionality/execution.py
+-rw-rw-rw-   0        0        0      840 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/positionBookFunctionality/functions.py
+-rw-rw-rw-   0        0        0      592 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.897854 thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      224 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFunctionality/base.py
+-rw-rw-rw-   0        0        0      689 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFunctionality/execution.py
+-rw-rw-rw-   0        0        0     1169 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFunctionality/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.900492 thefirstock-3.1.0/src/thefirstock/ordersNReport/singleOrderHistory/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/singleOrderHistory/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/singleOrderHistory/base.py
+-rw-rw-rw-   0        0        0      381 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/singleOrderHistory/execution.py
+-rw-rw-rw-   0        0        0      870 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/singleOrderHistory/functions.py
+-rw-rw-rw-   0        0        0      338 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/singleOrderHistoryFirstock.py
+-rw-rw-rw-   0        0        0      242 2023-02-28 04:29:00.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/tradeBookFirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.903386 thefirstock-3.1.0/src/thefirstock/ordersNReport/tradeBookFunctionality/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/tradeBookFunctionality/__init__.py
+-rw-rw-rw-   0        0        0      169 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/tradeBookFunctionality/base.py
+-rw-rw-rw-   0        0        0      271 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/tradeBookFunctionality/execution.py
+-rw-rw-rw-   0        0        0      829 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/ordersNReport/tradeBookFunctionality/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.906411 thefirstock-3.1.0/src/thefirstock/pyClient/
+-rw-rw-rw-   0        0        0     1034 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/__init__.py
+-rw-rw-rw-   0        0        0     1481 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/client.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.908380 thefirstock-3.1.0/src/thefirstock/pyClient/common/
+-rw-rw-rw-   0        0        0      132 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/common/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/common/enums.py
+-rw-rw-rw-   0        0        0     2536 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/common/exceptions.py
+-rw-rw-rw-   0        0        0     2569 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/common/models.py
+-rw-rw-rw-   0        0        0      286 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/models.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.909380 thefirstock-3.1.0/src/thefirstock/pyClient/modules/
+-rw-rw-rw-   0        0        0       62 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.910888 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/
+-rw-rw-rw-   0        0        0      502 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/datasource.py
+-rw-rw-rw-   0        0        0      366 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/endpoints.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.912898 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/models/
+-rw-rw-rw-   0        0        0       89 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/models/__init__.py
+-rw-rw-rw-   0        0        0     3277 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/models/login.py
+-rw-rw-rw-   0        0        0      962 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/models/save_fcm_token.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.915897 thefirstock-3.1.0/src/thefirstock/pyClient/utils/
+-rw-rw-rw-   0        0        0      150 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.916898 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/
+-rw-rw-rw-   0        0        0       94 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.917897 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/noren/
+-rw-rw-rw-   0        0        0       25 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/noren/__init__.py
+-rw-rw-rw-   0        0        0      684 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/noren/datasource.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.919899 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/rest/
+-rw-rw-rw-   0        0        0       26 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/rest/__init__.py
+-rw-rw-rw-   0        0        0      480 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/rest/context.py
+-rw-rw-rw-   0        0        0     3998 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/rest/datasource.py
+-rw-rw-rw-   0        0        0     2726 2023-02-28 04:29:02.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/decoders.py
+-rw-rw-rw-   0        0        0     3103 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/encoders.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.921508 thefirstock-3.1.0/src/thefirstock/pyClient/utils/interceptors/
+-rw-rw-rw-   0        0        0       27 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/interceptors/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/interceptors/http_error.py
+-rw-rw-rw-   0        0        0      814 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/interceptors/interceptor.py
+-rw-rw-rw-   0        0        0     1151 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/utils/stateful.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.922420 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/
+-rw-rw-rw-   0        0        0     1482 2023-04-18 10:12:00.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/__init__.py
+-rw-rw-rw-   0        0        0     5581 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/client.py
+-rw-rw-rw-   0        0        0      626 2023-04-19 06:11:36.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/enums.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.925422 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/
+-rw-rw-rw-   0        0        0       72 2023-04-18 09:39:26.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/connection.py
+-rw-rw-rw-   0        0        0      994 2023-04-18 08:00:34.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/depth.py
+-rw-rw-rw-   0        0        0      809 2023-04-18 09:30:48.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/order.py
+-rw-rw-rw-   0        0        0     1031 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/touchline.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.935769 thefirstock-3.1.0/src/thefirstock/strategies/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/bearPutSpread.py
+-rw-rw-rw-   0        0        0      592 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/bearPutSpreadFirstock.py
+-rw-rw-rw-   0        0        0      881 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/bullCallSpread.py
+-rw-rw-rw-   0        0        0      602 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/bullCallSpreadFirstock.py
+-rw-rw-rw-   0        0        0      748 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/longStraddle.py
+-rw-rw-rw-   0        0        0      493 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/longStraddleFirstock.py
+-rw-rw-rw-   0        0        0      823 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/longStrangle.py
+-rw-rw-rw-   0        0        0      569 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/longStrangleFirstock.py
+-rw-rw-rw-   0        0        0      535 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/multiPlaceOrder.py
+-rw-rw-rw-   0        0        0      256 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/multiPlaceOrderFirstock.py
+-rw-rw-rw-   0        0        0      866 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/shortStraddle.py
+-rw-rw-rw-   0        0        0      585 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/shortStraddleFirstock.py
+-rw-rw-rw-   0        0        0      942 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/shortStrangle.py
+-rw-rw-rw-   0        0        0      661 2023-02-28 04:29:04.000000 thefirstock-3.1.0/src/thefirstock/strategies/shortStrangleFirstock.py
+-rw-rw-rw-   0        0        0     4413 2023-03-19 14:32:44.000000 thefirstock-3.1.0/src/thefirstock/thefirstock.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:54.802173 thefirstock-3.1.0/src/thefirstock.egg-info/
+-rw-rw-rw-   0        0        0     3210 2023-04-19 12:42:54.000000 thefirstock-3.1.0/src/thefirstock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11400 2023-04-19 12:42:54.000000 thefirstock-3.1.0/src/thefirstock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:42:54.000000 thefirstock-3.1.0/src/thefirstock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-19 12:42:54.000000 thefirstock-3.1.0/src/thefirstock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 12:42:54.000000 thefirstock-3.1.0/src/thefirstock.egg-info/top_level.txt
```

### Comparing `thefirstock-3.0.6/LICENSE` & `thefirstock-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/PKG-INFO` & `thefirstock-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thefirstock
-Version: 3.0.6
+Version: 3.1.0
 Author: Firstock
 Author-email: technology@thefirstock.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `thefirstock-3.0.6/README.md` & `thefirstock-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/setup.cfg` & `thefirstock-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6865 6669 7273 746f 636b 0d0a   = thefirstock..
-00000020: 7665 7273 696f 6e20 3d20 332e 302e 360d  version = 3.0.6.
+00000020: 7665 7273 696f 6e20 3d20 332e 312e 300d  version = 3.1.0.
 00000030: 0a61 7574 686f 7220 3d20 4669 7273 746f  .author = Firsto
 00000040: 636b 0d0a 6175 7468 6f72 5f65 6d61 696c  ck..author_email
 00000050: 203d 2074 6563 686e 6f6c 6f67 7940 7468   = technology@th
 00000060: 6566 6972 7374 6f63 6b2e 636f 6d0d 0a6c  efirstock.com..l
 00000070: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000080: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 00000090: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

### Comparing `thefirstock-3.0.6/src/thefirstock/Variables/enums.py` & `thefirstock-3.1.0/src/thefirstock/Variables/enums.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/firstockModules/firstockWebSockets.py` & `thefirstock-3.1.0/src/thefirstock/firstockModules/firstockWebSockets.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,20 +8,28 @@
 from thefirstock.pyClient import Client
 from thefirstock.pyClient.utils.encoders import date_encoder
 from thefirstock.pyClient.utils.encoders import password_hash_encoder
 from pydantic import BaseModel, IPvAnyAddress, EmailStr, SecretStr, root_validator
 from thefirstock.pyClient.utils.decoders import build_loader, timestamp_decoder, datetime_decoder
 
 
-SOCKET_URL = r'wss://norenapi.thefirstock.com/NorenWSTP/'
+SOCKET_URL1 = r'wss://norenapi.thefirstock.com/NorenWSTP/'
+SOCKET_URL2 = r'ws://norenapi.thefirstock.com:5810/NorenWSTP/'
 
-try:
-    client = Client(socket_url=SOCKET_URL)
-except Exception as e:
-    print(e)
+
+def webSocketSelection(parameter):
+    try:
+        if parameter == 1:
+            client = Client(socket_url=SOCKET_URL1)
+            return client
+        elif parameter == 2:
+            client = Client(socket_url=SOCKET_URL2)
+            return client
+    except Exception as e:
+        print(e)
 
 
 class ResponseStatus(str, Enum):
     OK = 'Ok'
     NOT_OK = 'Not_Ok'
 
 
@@ -86,14 +94,15 @@
     class Config:
         json_loads = build_loader({
             "lastaccesstime": timestamp_decoder(),
             "request_time": datetime_decoder()
         })
 
 
-def webSocketLogin():
+def webSocketLogin(params=1):
     with open("config.json") as file:
         data = json.load(file)
 
+    client = webSocketSelection(params)
     client.login(data)
 
     return client
```

### Comparing `thefirstock-3.0.6/src/thefirstock/loginNProfile/loginFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/loginNProfile/loginFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/loginNProfile/logoutFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/loginNProfile/logoutFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/loginNProfile/userDetailsFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/loginNProfile/userDetailsFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/getIndexListFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/getIndexListFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/getMultiQuoteLTPFuntionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/getOptionChainFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/getOptionChainFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/getQuoteLTPFuntionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/getQuoteLTPFuntionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/getQuotesFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/getQuotesFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/getSecurityInfoFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/getSecurityInfoFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFirstock.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFunctionality/execution.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFunctionality/execution.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/optionGreekFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/optionGreekFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/searchScripsFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/searchScripsFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/spanCalculatorFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/spanCalculatorFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/marketConnect/timePriceSeriesFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/marketConnect/timePriceSeriesFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/basketMarginFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/basketMarginFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/cancelOrderFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/cancelOrderFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/holdingsFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/holdingsFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/limitFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/limitFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFirstock.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFunctionality/execution.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFunctionality/execution.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/modifyOrderFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/modifyOrderFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/orderBookFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/orderBookFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFirstock.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFunctionality/execution.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFunctionality/execution.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/orderMarginFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/orderMarginFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFirstock.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFunctionality/execution.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFunctionality/execution.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/placeOrderFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/placeOrderFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/positionBookFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/positionBookFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFirstock.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFunctionality/execution.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFunctionality/execution.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/productConversionFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/productConversionFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/singleOrderHistory/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/singleOrderHistory/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/ordersNReport/tradeBookFunctionality/functions.py` & `thefirstock-3.1.0/src/thefirstock/ordersNReport/tradeBookFunctionality/functions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/__init__.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/__init__.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/client.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/client.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/common/enums.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/common/enums.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/common/exceptions.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/common/models.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/common/models.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/datasource.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/datasource.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/models/login.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/models/login.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/modules/users/models/save_fcm_token.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/modules/users/models/save_fcm_token.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/noren/datasource.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/noren/datasource.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/utils/datasources/rest/datasource.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/utils/datasources/rest/datasource.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/utils/decoders.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/utils/decoders.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/utils/encoders.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/utils/interceptors/interceptor.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/utils/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/utils/stateful.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/utils/stateful.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/websocket/__init__.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/websocket/client.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/websocket/client.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/websocket/enums.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/websocket/enums.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/connection.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/connection.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/depth.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/order.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 """
-The model for sending depth subscription & unsubscription request
+The model for sending order subscription & unsubscription request
 """
 
 from typing import List
 from pydantic import BaseModel
 
 from ..enums import MessageTopic
 from ...utils.encoders import build_dumber, list_encoder
 
-class DepthSubscribeModel(BaseModel):
-  """
-  The depth subscription request model
-  """
-  t: MessageTopic = MessageTopic.DEPTH_SUB
-  """Always 'd' for depth task"""
-  k: List[str] = []
-  """One or more scriplist for subscription"""
-
-  class Config:
-    """The model config"""
-    json_dumps = build_dumber({
-      "k": list_encoder("|")
-    })
 
-class DepthUnsubscribeModel(BaseModel):
+class OrderSubscribeModel(BaseModel):
+    """
+  The order subscription request model
   """
+    t: MessageTopic = MessageTopic.ORDER_SUB
+    """Always 'o' for order update task"""
+    actid: str
+    """Account id based on which order updated to be sent."""
+
+
+class OrderUnsubscribeModel(BaseModel):
+    """
   The depth subscription request model
   """
-  t: MessageTopic = MessageTopic.DEPTH_UNSUB
-  """Always 'ud' for unsubscribe depth task"""
-  k: List[str] = []
-  """One or more scriplist for unsubscription"""
-
-  class Config:
-    """The model config"""
-    json_dumps = build_dumber({
-      "k": list_encoder("|")
-    })
+    t: MessageTopic = MessageTopic.ORDER_UNSUB
+    """Always 'uo' for unsubscribe order update task"""
+
+    class Config:
+        """The model config"""
+        json_dumps = build_dumber({
+            "k": list_encoder("|")
+        })
```

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/order.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/depth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 """
-The model for sending order subscription & unsubscription request
+The model for sending depth subscription & unsubscription request
 """
 
 from typing import List
 from pydantic import BaseModel
 
 from ..enums import MessageTopic
 from ...utils.encoders import build_dumber, list_encoder
 
 
-class OrderSubscribeModel(BaseModel):
+class DepthSubscribeModel(BaseModel):
     """
-  The order subscription request model
+  The depth subscription request model
   """
-    t: MessageTopic = MessageTopic.ORDER_SUB
-    """Always 'o' for order update task"""
-    actid: str;
-    """Account id based on which order updated to be sent."""
+    t: MessageTopic = MessageTopic.DEPTH_SUB
+    """Always 'd' for depth task"""
+    k: List[str] = []
+    """One or more scriplist for subscription"""
+
+    class Config:
+        """The model config"""
+        json_dumps = build_dumber({
+            "k": list_encoder("|")
+        })
 
 
-class OrderUnsubscribeModel(BaseModel):
+class DepthUnsubscribeModel(BaseModel):
     """
   The depth subscription request model
   """
-    t: MessageTopic = MessageTopic.ORDER_UNSUB
-    """Always 'uo' for unsubscribe order update task"""
+    t: MessageTopic = MessageTopic.DEPTH_UNSUB
+    """Always 'ud' for unsubscribe depth task"""
+    k: List[str] = []
+    """One or more scriplist for unsubscription"""
 
     class Config:
         """The model config"""
         json_dumps = build_dumber({
             "k": list_encoder("|")
         })
```

### Comparing `thefirstock-3.0.6/src/thefirstock/pyClient/websocket/models/touchline.py` & `thefirstock-3.1.0/src/thefirstock/pyClient/websocket/models/touchline.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/bearPutSpread.py` & `thefirstock-3.1.0/src/thefirstock/strategies/bearPutSpread.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/bearPutSpreadFirstock.py` & `thefirstock-3.1.0/src/thefirstock/strategies/bearPutSpreadFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/bullCallSpread.py` & `thefirstock-3.1.0/src/thefirstock/strategies/bullCallSpread.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/bullCallSpreadFirstock.py` & `thefirstock-3.1.0/src/thefirstock/strategies/bullCallSpreadFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/longStraddle.py` & `thefirstock-3.1.0/src/thefirstock/strategies/longStraddle.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/longStrangle.py` & `thefirstock-3.1.0/src/thefirstock/strategies/longStrangle.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/longStrangleFirstock.py` & `thefirstock-3.1.0/src/thefirstock/strategies/longStrangleFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/multiPlaceOrder.py` & `thefirstock-3.1.0/src/thefirstock/strategies/multiPlaceOrder.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/shortStraddle.py` & `thefirstock-3.1.0/src/thefirstock/strategies/shortStraddle.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/shortStraddleFirstock.py` & `thefirstock-3.1.0/src/thefirstock/strategies/shortStraddleFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/shortStrangle.py` & `thefirstock-3.1.0/src/thefirstock/strategies/shortStrangle.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/strategies/shortStrangleFirstock.py` & `thefirstock-3.1.0/src/thefirstock/strategies/shortStrangleFirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock/thefirstock.py` & `thefirstock-3.1.0/src/thefirstock/thefirstock.py`

 * *Files identical despite different names*

### Comparing `thefirstock-3.0.6/src/thefirstock.egg-info/PKG-INFO` & `thefirstock-3.1.0/src/thefirstock.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thefirstock
-Version: 3.0.6
+Version: 3.1.0
 Author: Firstock
 Author-email: technology@thefirstock.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `thefirstock-3.0.6/src/thefirstock.egg-info/SOURCES.txt` & `thefirstock-3.1.0/src/thefirstock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

